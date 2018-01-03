```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 34 11.1M   34 3967k    0     0  6445k      0  0:00:01 --:--:--  0:00:01 6440k100 11.1M  100 11.1M    0     0  10.0M      0  0:00:01  0:00:01 --:--:-- 10.0M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  120M    2 3103k    0     0  6226k      0  0:00:19 --:--:--  0:00:19 6219k 13  120M   13 16.3M    0     0  10.9M      0  0:00:11  0:00:01  0:00:10 10.9M 23  120M   23 28.3M    0     0  11.3M      0  0:00:10  0:00:02  0:00:08 11.3M 31  120M   31 38.0M    0     0  10.6M      0  0:00:11  0:00:03  0:00:08 10.6M 38  120M   38 46.4M    0     0  10.3M      0  0:00:11  0:00:04  0:00:07 10.3M 46  120M   46 56.2M    0     0  10.2M      0  0:00:11  0:00:05  0:00:06 10.6M 57  120M   57 69.9M    0     0  10.7M      0  0:00:11  0:00:06  0:00:05 10.7M 70  120M   70 84.7M    0     0  11.2M      0  0:00:10  0:00:07  0:00:03 11.2M 80  120M   80 96.7M    0     0  11.3M      0  0:00:10  0:00:08  0:00:02 11.9M 89  120M   89  108M    0     0  11.3M      0  0:00:10  0:00:09  0:00:01 12.3M100  120M  100  120M    0     0  11.6M      0  0:00:10  0:00:10 --:--:-- 13.2M
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
] Testing  RL18_DBG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```