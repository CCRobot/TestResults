```
Executed on ubu16chk400000W
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  9486k      0 --:--:-- --:--:-- --:--:-- 9484k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  140M    0 32345    0     0  91064      0  0:26:57 --:--:--  0:26:57 90856 14  140M   14 20.0M    0     0  14.9M      0  0:00:09  0:00:01  0:00:08 14.9M 42  140M   42 60.0M    0     0  25.3M      0  0:00:05  0:00:02  0:00:03 25.3M 68  140M   68 96.0M    0     0  28.4M      0  0:00:04  0:00:03  0:00:01 28.4M 91  140M   91  128M    0     0  29.3M      0  0:00:04  0:00:04 --:--:-- 29.3M100  140M  100  140M    0     0  29.9M      0  0:00:04  0:00:04 --:--:-- 32.4M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   ed21221..10170c4  master     -> origin/master
   17fcf4a..fdf00b8  release/1.8 -> origin/release/1.8
   172bac8..cc2aede  release/1.9 -> origin/release/1.9
Updating ed21221..10170c4
Fast-forward
 lib/Backend/EmitBuffer.cpp                         |  7 +++++
 lib/Backend/InterpreterThunkEmitter.cpp            |  8 ------
 lib/Backend/NativeCodeGenerator.cpp                | 10 +++----
 lib/Common/Common/Jobs.cpp                         | 14 ++++++++--
 lib/Common/Common/Jobs.h                           |  8 ++++++
 lib/Common/Core/ConfigParser.cpp                   |  3 +-
 lib/Common/Core/DelayLoadLibrary.cpp               |  7 +++--
 lib/Common/Memory/DelayDeletingFunctionTable.cpp   | 19 ++-----------
 lib/Common/Memory/XDataAllocator.h                 |  7 ++---
 lib/Common/Memory/amd64/XDataAllocator.cpp         |  8 +++++-
 lib/Jsrt/Core/JsrtCore.cpp                         |  4 ---
 lib/Runtime/Base/FunctionBody.cpp                  | 32 +++++++++++++---------
 lib/Runtime/Base/ScriptContext.cpp                 |  4 ++-
 .../Library/JavascriptRegExpConstructor.cpp        |  1 -
 14 files changed, 72 insertions(+), 60 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  TEST_ubuntu
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```