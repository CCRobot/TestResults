```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 63 11.1M   63 7184k    0     0  7768k      0  0:00:01 --:--:--  0:00:01 7766k100 11.1M  100 11.1M    0     0  9256k      0  0:00:01  0:00:01 --:--:-- 9260k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  140M    4 6880k    0     0   9.9M      0  0:00:14 --:--:--  0:00:14  9.9M 15  140M   15 22.0M    0     0  13.1M      0  0:00:10  0:00:01  0:00:09 13.1M 19  140M   19 27.0M    0     0  10.1M      0  0:00:13  0:00:02  0:00:11 10.1M 30  140M   30 42.7M    0     0  11.6M      0  0:00:12  0:00:03  0:00:09 11.6M 37  140M   37 53.3M    0     0  11.4M      0  0:00:12  0:00:04  0:00:08 11.4M 45  140M   45 64.2M    0     0  11.3M      0  0:00:12  0:00:05  0:00:07 11.5M 54  140M   54 77.2M    0     0  11.5M      0  0:00:12  0:00:06  0:00:06 11.0M 65  140M   65 91.9M    0     0  11.9M      0  0:00:11  0:00:07  0:00:04 12.9M 75  140M   75  106M    0     0  12.2M      0  0:00:11  0:00:08  0:00:03 12.6M 86  140M   86  121M    0     0  12.5M      0  0:00:11  0:00:09  0:00:02 13.6M 96  140M   96  135M    0     0  12.6M      0  0:00:11  0:00:10  0:00:01 14.2M100  140M  100  140M    0     0  12.7M      0  0:00:11  0:00:11 --:--:-- 14.6M
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
] Testing  DEBUG_FLG2_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```