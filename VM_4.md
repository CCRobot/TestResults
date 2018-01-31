```
Executed on ubu16chk400000X
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 34 9180k   34 3167k    0     0  3287k      0  0:00:02 --:--:--  0:00:02 3285k100 9180k  100 9180k    0     0  7744k      0  0:00:01  0:00:01 --:--:-- 7747k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  140M    1 2575k    0     0  3405k      0  0:00:42 --:--:--  0:00:42 3402k 22  140M   22 32.2M    0     0  18.3M      0  0:00:07  0:00:01  0:00:06 18.3M 51  140M   51 72.0M    0     0  25.9M      0  0:00:05  0:00:02  0:00:03 25.9M 79  140M   79  112M    0     0  29.6M      0  0:00:04  0:00:03  0:00:01 29.6M100  140M  100  140M    0     0  31.3M      0  0:00:04  0:00:04 --:--:-- 31.3M
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
] Testing  RL18_DBG_F2_ubuntu
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```