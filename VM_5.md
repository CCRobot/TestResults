```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 26 11.1M   26 3007k    0     0  6764k      0  0:00:01 --:--:--  0:00:01 6758k100 11.1M  100 11.1M    0     0  11.0M      0  0:00:01  0:00:01 --:--:-- 11.0M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  120M    2 2623k    0     0  6153k      0  0:00:20 --:--:--  0:00:20 6144k 11  120M   11 13.8M    0     0  9937k      0  0:00:12  0:00:01  0:00:11 9931k 20  120M   20 25.0M    0     0  10.3M      0  0:00:11  0:00:02  0:00:09 10.3M 30  120M   30 36.5M    0     0  10.6M      0  0:00:11  0:00:03  0:00:08 10.6M 38  120M   38 46.3M    0     0  10.4M      0  0:00:11  0:00:04  0:00:07 10.4M 49  120M   49 60.1M    0     0  11.0M      0  0:00:10  0:00:05  0:00:05 11.5M 60  120M   60 73.0M    0     0  11.3M      0  0:00:10  0:00:06  0:00:04 11.8M 68  120M   68 83.0M    0     0  11.1M      0  0:00:10  0:00:07  0:00:03 11.5M 77  120M   77 93.7M    0     0  11.1M      0  0:00:10  0:00:08  0:00:02 11.4M 84  120M   84  102M    0     0  10.8M      0  0:00:11  0:00:09  0:00:02 11.2M 98  120M   98  118M    0     0  11.3M      0  0:00:10  0:00:10 --:--:-- 11.6M100  120M  100  120M    0     0  11.4M      0  0:00:10  0:00:10 --:--:-- 11.4M
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
] Testing  DEBUG_FLG1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```