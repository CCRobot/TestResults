```
Executed on w1604chak000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 37 9180k   37 3439k    0     0  5484k      0  0:00:01 --:--:--  0:00:01 5477k100 9180k  100 9180k    0     0  11.5M      0 --:--:-- --:--:-- --:--:-- 11.5M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  7  120M    7 8816k    0     0  10.2M      0  0:00:11 --:--:--  0:00:11 10.2M 36  120M   36 44.0M    0     0  23.8M      0  0:00:05  0:00:01  0:00:04 23.8M 62  120M   62 76.0M    0     0  26.5M      0  0:00:04  0:00:02  0:00:02 26.5M 89  120M   89  108M    0     0  27.7M      0  0:00:04  0:00:03  0:00:01 27.7M100  120M  100  120M    0     0  28.6M      0  0:00:04  0:00:04 --:--:-- 28.6M
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
] Testing  RLS18_TEST_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```