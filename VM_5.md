```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 26 11.1M   26 3023k    0     0  4482k      0  0:00:02 --:--:--  0:00:02 4479k100 11.1M  100 11.1M    0     0  8052k      0  0:00:01  0:00:01 --:--:-- 8054k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  9  140M    9 13.4M    0     0  10.8M      0  0:00:13  0:00:01  0:00:12 10.8M 17  140M   17 24.2M    0     0  10.7M      0  0:00:13  0:00:02  0:00:11 10.7M 26  140M   26 36.9M    0     0  11.3M      0  0:00:12  0:00:03  0:00:09 11.3M 35  140M   35 49.3M    0     0  11.6M      0  0:00:12  0:00:04  0:00:08 11.6M 44  140M   44 62.2M    0     0  11.6M      0  0:00:12  0:00:05  0:00:07 12.3M 52  140M   52 73.4M    0     0  11.7M      0  0:00:11  0:00:06  0:00:05 12.0M 62  140M   62 87.9M    0     0  12.1M      0  0:00:11  0:00:07  0:00:04 12.7M 71  140M   71  100M    0     0  12.1M      0  0:00:11  0:00:08  0:00:03 12.6M 79  140M   79  111M    0     0  12.0M      0  0:00:11  0:00:09  0:00:02 12.4M 87  140M   87  123M    0     0  12.0M      0  0:00:11  0:00:10  0:00:01 12.4M 96  140M   96  135M    0     0  12.0M      0  0:00:11  0:00:11 --:--:-- 12.4M100  140M  100  140M    0     0  12.1M      0  0:00:11  0:00:11 --:--:-- 12.0M
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
] Testing  DEBUG_FLG1_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```