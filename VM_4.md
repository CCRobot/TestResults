```
Executed on ubu16chk4000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 44 9180k   44 4096k    0     0  5722k      0  0:00:01 --:--:--  0:00:01 5720k100 9180k  100 9180k    0     0  11.2M      0 --:--:-- --:--:-- --:--:-- 11.2M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:--  0:00:01 --:--:--     0  8  140M    8 12.0M    0     0  6161k      0  0:00:23  0:00:01  0:00:22 6159k 29  140M   29 41.1M    0     0  14.4M      0  0:00:09  0:00:02  0:00:07 14.4M 48  140M   48 68.0M    0     0  17.5M      0  0:00:08  0:00:03  0:00:05 17.5M 67  140M   67 95.2M    0     0  19.5M      0  0:00:07  0:00:04  0:00:03 19.5M 80  140M   80  113M    0     0  19.4M      0  0:00:07  0:00:05  0:00:02 23.8M 94  140M   94  132M    0     0  19.3M      0  0:00:07  0:00:06  0:00:01 24.8M100  140M  100  140M    0     0  19.5M      0  0:00:07  0:00:07 --:--:-- 22.9M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   ed21221..b8fdf20  master     -> origin/master
   17fcf4a..bcdae20  release/1.8 -> origin/release/1.8
   172bac8..9d70c00  release/1.9 -> origin/release/1.9
Updating ed21221..b8fdf20
Fast-forward
 lib/Backend/EmitBuffer.cpp                         |   7 +
 lib/Backend/InterpreterThunkEmitter.cpp            |   8 -
 lib/Backend/NativeCodeGenerator.cpp                |  10 +-
 lib/Backend/PDataManager.cpp                       |   2 +-
 lib/Common/Common/Jobs.cpp                         |  14 +-
 lib/Common/Common/Jobs.h                           |   8 +
 lib/Common/Core/ConfigParser.cpp                   |   3 +-
 lib/Common/Core/DelayLoadLibrary.cpp               |  11 +-
 lib/Common/Core/DelayLoadLibrary.h                 |   2 +-
 lib/Common/Memory/DelayDeletingFunctionTable.cpp   |  19 +-
 lib/Common/Memory/XDataAllocator.h                 |   7 +-
 lib/Common/Memory/amd64/XDataAllocator.cpp         |  10 +-
 lib/Common/Memory/arm/XDataAllocator.cpp           |   2 +-
 lib/Common/Memory/arm64/XDataAllocator.cpp         |   2 +-
 lib/Jsrt/Core/JsrtCore.cpp                         |   4 -
 lib/Runtime/Base/FunctionBody.cpp                  |  34 +--
 lib/Runtime/Base/ScriptContext.cpp                 |   4 +-
 lib/Runtime/Language/JavascriptOperators.cpp       | 252 ++++++++++-----------
 lib/Runtime/Language/JavascriptOperators.h         |  12 +
 .../Library/JavascriptRegExpConstructor.cpp        |   1 -
 lib/Runtime/Library/RuntimeLibraryPch.h            |   1 +
 lib/Runtime/Types/WithScopeObject.h                |  83 ++++---
 test/es6/unscopablesWithScopeTest.js               |  24 ++
 23 files changed, 285 insertions(+), 235 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  NODE_BUILD_ubuntu
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```