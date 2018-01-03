```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 14 11.1M   14 1663k    0     0  3577k      0  0:00:03 --:--:--  0:00:03 3577k100 11.1M  100 11.1M    0     0  8984k      0  0:00:01  0:00:01 --:--:-- 8990k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 13  120M   13 16.0M    0     0  13.6M      0  0:00:08  0:00:01  0:00:07 13.6M 21  120M   21 26.2M    0     0  12.0M      0  0:00:10  0:00:02  0:00:08 12.0M 33  120M   33 40.5M    0     0  12.7M      0  0:00:09  0:00:03  0:00:06 12.7M 46  120M   46 56.0M    0     0  13.3M      0  0:00:09  0:00:04  0:00:05 13.3M 56  120M   56 67.6M    0     0  13.0M      0  0:00:09  0:00:05  0:00:04 13.6M 66  120M   66 80.6M    0     0  13.0M      0  0:00:09  0:00:06  0:00:03 12.9M 71  120M   71 86.0M    0     0  11.9M      0  0:00:10  0:00:07  0:00:03 11.9M 80  120M   80 97.4M    0     0  11.9M      0  0:00:10  0:00:08  0:00:02 11.3M 89  120M   89  108M    0     0  11.7M      0  0:00:10  0:00:09  0:00:01 10.4M100  120M  100  120M    0     0  12.0M      0  0:00:10  0:00:10 --:--:-- 10.9M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   523c01d..fb8e257  master      -> origin/master
   03a8be9..745ddf8  intl-icu    -> origin/intl-icu
   bd3a178..ce599fa  release/1.8 -> origin/release/1.8
Updating 523c01d..fb8e257
Fast-forward
 lib/Runtime/Base/ScriptContext.cpp                 | 87 ++++++++++++----------
 lib/Runtime/Base/ScriptContext.h                   | 11 ++-
 .../Language/JavascriptExceptionOperators.cpp      | 41 ++++++----
 test/Debugger/empty.baseline                       |  1 +
 test/Debugger/failfast.js                          | 17 +++++
 test/Debugger/rlexe.xml                            |  6 ++
 6 files changed, 108 insertions(+), 55 deletions(-)
 create mode 100644 test/Debugger/empty.baseline
 create mode 100644 test/Debugger/failfast.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_F1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```