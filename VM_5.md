```
Executed on ubu16chk400000X
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 68 9180k   68 6288k    0     0  6794k      0  0:00:01 --:--:--  0:00:01 6790k100 9180k  100 9180k    0     0  8935k      0  0:00:01  0:00:01 --:--:-- 8939k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  140M    2 3039k    0     0  3474k      0  0:00:41 --:--:--  0:00:41 3473k 25  140M   25 36.0M    0     0  18.9M      0  0:00:07  0:00:01  0:00:06 18.9M 54  140M   54 76.0M    0     0  25.9M      0  0:00:05  0:00:02  0:00:03 25.9M 79  140M   79  112M    0     0  28.9M      0  0:00:04  0:00:03  0:00:01 28.9M100  140M  100  140M    0     0  30.9M      0  0:00:04  0:00:04 --:--:-- 30.9M
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
] Testing  DEBUG_FLG1_ubuntu
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```