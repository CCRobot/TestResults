```
Executed on w1604chak000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  11.3M      0 --:--:-- --:--:-- --:--:-- 11.3M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  120M    0 15961    0     0  46181      0  0:45:41 --:--:--  0:45:41 46130 23  120M   23 28.0M    0     0  20.3M      0  0:00:05  0:00:01  0:00:04 20.3M 53  120M   53 64.1M    0     0  27.6M      0  0:00:04  0:00:02  0:00:02 27.5M 86  120M   86  104M    0     0  30.7M      0  0:00:03  0:00:03 --:--:-- 30.6M100  120M  100  120M    0     0  32.1M      0  0:00:03  0:00:03 --:--:-- 32.1M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   523c01d..a13c30b  master     -> origin/master
   03a8be9..745ddf8  intl-icu   -> origin/intl-icu
   bd3a178..1209352  release/1.8 -> origin/release/1.8
Updating 523c01d..a13c30b
Fast-forward
 lib/Common/Core/Output.cpp                         | 13 +++
 lib/Common/Core/Output.h                           |  2 +
 lib/Parser/Parse.cpp                               | 12 ++-
 lib/Parser/Parse.h                                 |  1 +
 lib/Parser/ptree.h                                 |  5 ++
 lib/Runtime/Base/ScriptContext.cpp                 | 87 ++++++++++---------
 lib/Runtime/Base/ScriptContext.h                   | 11 ++-
 .../Language/JavascriptExceptionOperators.cpp      | 41 ++++++---
 test/Debugger/empty.baseline                       |  1 +
 test/Debugger/failfast.js                          | 17 ++++
 test/Debugger/rlexe.xml                            |  6 ++
 test/es6/bug_OS14880030.js                         | 98 ++++++++++++++++++++++
 test/es6/rlexe.xml                                 | 14 ++++
 13 files changed, 251 insertions(+), 57 deletions(-)
 create mode 100644 test/Debugger/empty.baseline
 create mode 100644 test/Debugger/failfast.js
 create mode 100644 test/es6/bug_OS14880030.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  TEST_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```