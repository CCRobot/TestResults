```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4 11.1M    4  543k    0     0  1744k      0  0:00:06 --:--:--  0:00:06 1742k100 11.1M  100 11.1M    0     0  9569k      0  0:00:01  0:00:01 --:--:-- 9572k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  124M    5 6416k    0     0  5793k      0  0:00:22  0:00:01  0:00:21 5790k 11  124M   11 13.7M    0     0  6692k      0  0:00:19  0:00:02  0:00:17 6690k 17  124M   17 21.8M    0     0  7189k      0  0:00:17  0:00:03  0:00:14 7188k 25  124M   25 31.2M    0     0  7801k      0  0:00:16  0:00:04  0:00:12 7801k 30  124M   30 38.5M    0     0  7721k      0  0:00:16  0:00:05  0:00:11 7900k 37  124M   37 46.6M    0     0  7820k      0  0:00:16  0:00:06  0:00:10 8268k 43  124M   43 53.6M    0     0  7731k      0  0:00:16  0:00:07  0:00:09 8169k 46  124M   46 58.2M    0     0  7360k      0  0:00:17  0:00:08  0:00:09 7467k 54  124M   54 68.2M    0     0  7670k      0  0:00:16  0:00:09  0:00:07 7565k 62  124M   62 78.4M    0     0  7946k      0  0:00:16  0:00:10  0:00:06 8174k 70  124M   70 87.6M    0     0  8079k      0  0:00:15  0:00:11  0:00:04 8393k 77  124M   77 96.5M    0     0  8167k      0  0:00:15  0:00:12  0:00:03 8787k 85  124M   85  106M    0     0  8286k      0  0:00:15  0:00:13  0:00:02 9786k 92  124M   92  115M    0     0  8393k      0  0:00:15  0:00:14  0:00:01 9711k100  124M  100  124M    0     0  8644k      0  0:00:14  0:00:14 --:--:--  9.9M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   fa3aeda..c47185f  master     -> origin/master
Updating fa3aeda..c47185f
Fast-forward
 Build/Chakra.Core.sln                              |  4 ++
 lib/Backend/CodeGenWorkItem.cpp                    |  2 +-
 lib/Backend/EmitBuffer.cpp                         | 10 ++-
 lib/Backend/EmitBuffer.h                           |  2 +-
 lib/Backend/InterpreterThunkEmitter.cpp            |  8 +++
 lib/Backend/NativeCodeGenerator.cpp                | 39 +++++++---
 lib/Backend/NativeCodeGenerator.h                  | 13 ++--
 lib/Backend/PDataManager.cpp                       |  1 +
 lib/Common/BackendApi.h                            |  2 +-
 lib/Common/Common/Jobs.cpp                         | 31 +++++++-
 lib/Common/Common/Jobs.h                           |  9 +++
 lib/Common/Core/DelayLoadLibrary.cpp               |  2 +
 lib/Common/Memory/CMakeLists.txt                   |  1 +
 lib/Common/Memory/Chakra.Common.Memory.vcxproj     |  3 +-
 .../Memory/Chakra.Common.Memory.vcxproj.filters    |  3 +-
 lib/Common/Memory/CustomHeap.cpp                   | 13 ++--
 lib/Common/Memory/DelayDeletingFunctionTable.cpp   | 82 ++++++++++++++++++++++
 lib/Common/Memory/XDataAllocator.h                 | 22 ++++++
 lib/Common/Memory/amd64/XDataAllocator.cpp         |  7 +-
 lib/Common/Memory/amd64/XDataAllocator.h           |  3 +
 lib/Common/Memory/arm/XDataAllocator.cpp           |  4 +-
 lib/Common/Memory/arm64/XDataAllocator.cpp         |  5 +-
 lib/Common/Memory/arm64/XDataAllocator.h           |  3 +
 lib/JITServer/JITServer.cpp                        |  2 +-
 lib/Runtime/Base/FunctionBody.cpp                  | 78 +++++++++-----------
 lib/Runtime/Base/FunctionBody.h                    |  6 +-
 lib/Runtime/Base/ScriptContext.cpp                 | 22 +++++-
 lib/Runtime/Base/ScriptContext.h                   |  2 +-
 lib/Runtime/Base/ThreadContext.cpp                 |  1 -
 lib/Runtime/Language/Arguments.h                   |  3 +-
 lib/Runtime/Library/JavascriptFunction.cpp         |  2 +
 31 files changed, 291 insertions(+), 94 deletions(-)
 create mode 100644 lib/Common/Memory/DelayDeletingFunctionTable.cpp
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_PACK
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```