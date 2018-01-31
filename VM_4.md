```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 39 11.1M   39 4496k    0     0  7973k      0  0:00:01 --:--:--  0:00:01 7971k100 11.1M  100 11.1M    0     0  11.3M      0 --:--:-- --:--:-- --:--:-- 11.3M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  140M    3 4464k    0     0  7853k      0  0:00:18 --:--:--  0:00:18 7845k 12  140M   12 17.8M    0     0  11.3M      0  0:00:12  0:00:01  0:00:11 11.3M 20  140M   20 28.6M    0     0  11.1M      0  0:00:12  0:00:02  0:00:10 11.1M 28  140M   28 40.0M    0     0  11.2M      0  0:00:12  0:00:03  0:00:09 11.2M 36  140M   36 50.6M    0     0  11.0M      0  0:00:12  0:00:04  0:00:08 11.0M 44  140M   44 62.2M    0     0  11.1M      0  0:00:12  0:00:05  0:00:07 11.5M 51  140M   51 72.8M    0     0  11.0M      0  0:00:12  0:00:06  0:00:06 11.0M 59  140M   59 83.9M    0     0  11.0M      0  0:00:12  0:00:07  0:00:05 11.0M 67  140M   67 94.6M    0     0  11.0M      0  0:00:12  0:00:08  0:00:04 10.9M 75  140M   75  106M    0     0  11.1M      0  0:00:12  0:00:09  0:00:03 11.1M 83  140M   83  117M    0     0  11.0M      0  0:00:12  0:00:10  0:00:02 11.0M 92  140M   92  129M    0     0  11.1M      0  0:00:12  0:00:11  0:00:01 11.3M100  140M  100  140M    0     0  11.3M      0  0:00:12  0:00:12 --:--:-- 11.8M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   ed21221..b8fdf20  master      -> origin/master
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
] Testing  NODE_BUILD_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```