```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 14 11.1M   14 1663k    0     0  4010k      0  0:00:02 --:--:--  0:00:02 4008k 69 11.1M   69 7888k    0     0  5559k      0  0:00:02  0:00:01  0:00:01 5558k100 11.1M  100 11.1M    0     0  6713k      0  0:00:01  0:00:01 --:--:-- 6710k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  120M    4 5968k    0     0  8476k      0  0:00:14 --:--:--  0:00:14 8465k 16  120M   16 19.9M    0     0  11.7M      0  0:00:10  0:00:01  0:00:09 11.7M 26  120M   26 32.0M    0     0  11.7M      0  0:00:10  0:00:02  0:00:08 11.7M 31  120M   31 38.3M    0     0  10.3M      0  0:00:11  0:00:03  0:00:08 10.3M 42  120M   42 51.1M    0     0  10.8M      0  0:00:11  0:00:04  0:00:07 10.8M 54  120M   54 65.8M    0     0  11.5M      0  0:00:10  0:00:05  0:00:05 12.0M 64  120M   64 77.3M    0     0  11.5M      0  0:00:10  0:00:06  0:00:04 11.4M 66  120M   66 80.2M    0     0  10.3M      0  0:00:11  0:00:07  0:00:04 9872k 73  120M   73 89.1M    0     0  10.2M      0  0:00:11  0:00:08  0:00:03 10.1M 84  120M   84  102M    0     0  10.5M      0  0:00:11  0:00:09  0:00:02 10.1M 95  120M   95  115M    0     0  10.7M      0  0:00:11  0:00:10  0:00:01  9.9M100  120M  100  120M    0     0  10.8M      0  0:00:11  0:00:11 --:--:--  9.8M
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
] Testing  RL18_PACK
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```