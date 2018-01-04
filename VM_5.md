```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 28 11.1M   28 3199k    0     0  5494k      0  0:00:02 --:--:--  0:00:02 5488k100 11.1M  100 11.1M    0     0  8943k      0  0:00:01  0:00:01 --:--:-- 8947k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  120M    0  271k    0     0   938k      0  0:02:11 --:--:--  0:02:11  936k  9  120M    9 12.0M    0     0  9384k      0  0:00:13  0:00:01  0:00:12 9378k 17  120M   17 21.4M    0     0  9575k      0  0:00:12  0:00:02  0:00:10 9572k 26  120M   26 32.0M    0     0  9984k      0  0:00:12  0:00:03  0:00:09 9984k 36  120M   36 43.5M    0     0  10.1M      0  0:00:11  0:00:04  0:00:07 10.1M 43  120M   43 52.5M    0     0   9.9M      0  0:00:12  0:00:05  0:00:07 10.4M 52  120M   52 63.4M    0     0  10.0M      0  0:00:11  0:00:06  0:00:05 10.3M 62  120M   62 75.1M    0     0  10.3M      0  0:00:11  0:00:07  0:00:04 10.7M 71  120M   71 85.9M    0     0  10.3M      0  0:00:11  0:00:08  0:00:03 10.7M 79  120M   79 95.6M    0     0  10.2M      0  0:00:11  0:00:09  0:00:02 10.4M 88  120M   88  106M    0     0  10.3M      0  0:00:11  0:00:10  0:00:01 10.8M 96  120M   96  116M    0     0  10.3M      0  0:00:11  0:00:11 --:--:-- 10.6M100  120M  100  120M    0     0  10.3M      0  0:00:11  0:00:11 --:--:-- 10.5M
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
] Testing  DEBUG_FLG2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```