```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 17 11.1M   17 1999k    0     0  5082k      0  0:00:02 --:--:--  0:00:02 5075k100 11.1M  100 11.1M    0     0  10.4M      0  0:00:01  0:00:01 --:--:-- 10.4M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  120M    0  879k    0     0  2318k      0  0:00:53 --:--:--  0:00:53 2314k  9  120M    9 12.0M    0     0  9321k      0  0:00:13  0:00:01  0:00:12 9317k 18  120M   18 22.6M    0     0   9.7M      0  0:00:12  0:00:02  0:00:10  9.7M 28  120M   28 33.9M    0     0  10.2M      0  0:00:11  0:00:03  0:00:08 10.2M 39  120M   39 47.2M    0     0  10.9M      0  0:00:11  0:00:04  0:00:07 10.9M 48  120M   48 58.6M    0     0  11.0M      0  0:00:10  0:00:05  0:00:05 11.6M 59  120M   59 72.4M    0     0  11.4M      0  0:00:10  0:00:06  0:00:04 12.0M 70  120M   70 84.5M    0     0  11.5M      0  0:00:10  0:00:07  0:00:03 12.3M 80  120M   80 96.8M    0     0  11.6M      0  0:00:10  0:00:08  0:00:02 12.5M 91  120M   91  109M    0     0  11.7M      0  0:00:10  0:00:09  0:00:01 12.5M100  120M  100  120M    0     0  11.8M      0  0:00:10  0:00:10 --:--:-- 12.6M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   523c01d..a13c30b  master      -> origin/master
   03a8be9..745ddf8  intl-icu    -> origin/intl-icu
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
] Testing  NODE_BUILD_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```