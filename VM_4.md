```
Executed on w1604chak000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  11.6M      0 --:--:-- --:--:-- --:--:-- 11.6M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  120M    0  543k    0     0  1110k      0  0:01:51 --:--:--  0:01:51 1109k 28  120M   28 34.7M    0     0  23.5M      0  0:00:05  0:00:01  0:00:04 23.5M 59  120M   59 72.0M    0     0  28.5M      0  0:00:04  0:00:02  0:00:02 28.5M 89  120M   89  108M    0     0  30.9M      0  0:00:03  0:00:03 --:--:-- 30.8M100  120M  100  120M    0     0  31.5M      0  0:00:03  0:00:03 --:--:-- 31.5M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   523c01d..763576b  master     -> origin/master
   03a8be9..745ddf8  intl-icu   -> origin/intl-icu
Updating 523c01d..763576b
Fast-forward
 lib/Runtime/Base/ScriptContext.cpp | 87 +++++++++++++++++++++-----------------
 lib/Runtime/Base/ScriptContext.h   | 11 +++--
 test/Debugger/empty.baseline       |  1 +
 test/Debugger/failfast.js          | 17 ++++++++
 test/Debugger/rlexe.xml            |  6 +++
 5 files changed, 80 insertions(+), 42 deletions(-)
 create mode 100644 test/Debugger/empty.baseline
 create mode 100644 test/Debugger/failfast.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```