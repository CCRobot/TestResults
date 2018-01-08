```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 41 11.1M   41 4672k    0     0  3473k      0  0:00:03  0:00:01  0:00:02 3473k100 11.1M  100 11.1M    0     0  4921k      0  0:00:02  0:00:02 --:--:-- 4922k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  7  124M    7 9856k    0     0  9739k      0  0:00:13  0:00:01  0:00:12 9739k 19  124M   19 24.0M    0     0  11.9M      0  0:00:10  0:00:02  0:00:08 11.9M 28  124M   28 35.0M    0     0  11.6M      0  0:00:10  0:00:03  0:00:07 11.6M 34  124M   34 43.2M    0     0  10.7M      0  0:00:11  0:00:04  0:00:07 10.7M 41  124M   41 52.0M    0     0  10.3M      0  0:00:11  0:00:05  0:00:06 10.4M 49  124M   49 61.4M    0     0  10.2M      0  0:00:12  0:00:06  0:00:06 10.3M 56  124M   56 70.6M    0     0  10.0M      0  0:00:12  0:00:07  0:00:05 9554k 63  124M   63 79.3M    0     0  9788k      0  0:00:13  0:00:08  0:00:05 8579k 67  124M   67 84.1M    0     0  9562k      0  0:00:13  0:00:09  0:00:04 8377k 74  124M   74 93.1M    0     0  9527k      0  0:00:13  0:00:10  0:00:03 8408k 81  124M   81  101M    0     0  9451k      0  0:00:13  0:00:11  0:00:02 8228k 91  124M   91  114M    0     0  9721k      0  0:00:13  0:00:12  0:00:01 8876k100  124M  100  124M    0     0  9948k      0  0:00:12  0:00:12 --:--:-- 10.0M
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
] Testing  RL18_DBG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```