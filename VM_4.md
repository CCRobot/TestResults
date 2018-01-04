```
Executed on w1604chak000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  12.1M      0 --:--:-- --:--:-- --:--:-- 12.1M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 19  120M   19 24.0M    0     0  19.1M      0  0:00:06  0:00:01  0:00:05 19.1M 50  120M   50 61.1M    0     0  27.8M      0  0:00:04  0:00:02  0:00:02 27.8M 82  120M   82  100M    0     0  30.3M      0  0:00:03  0:00:03 --:--:-- 30.3M100  120M  100  120M    0     0  31.9M      0  0:00:03  0:00:03 --:--:-- 31.9M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   523c01d..8e0bd3c  master     -> origin/master
   03a8be9..745ddf8  intl-icu   -> origin/intl-icu
   bd3a178..ce599fa  release/1.8 -> origin/release/1.8
Updating 523c01d..8e0bd3c
Fast-forward
 lib/Common/Core/Output.cpp                         | 13 ++++
 lib/Common/Core/Output.h                           |  2 +
 lib/Runtime/Base/ScriptContext.cpp                 | 87 ++++++++++++----------
 lib/Runtime/Base/ScriptContext.h                   | 11 ++-
 .../Language/JavascriptExceptionOperators.cpp      | 41 ++++++----
 test/Debugger/empty.baseline                       |  1 +
 test/Debugger/failfast.js                          | 17 +++++
 test/Debugger/rlexe.xml                            |  6 ++
 8 files changed, 123 insertions(+), 55 deletions(-)
 create mode 100644 test/Debugger/empty.baseline
 create mode 100644 test/Debugger/failfast.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_F1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```