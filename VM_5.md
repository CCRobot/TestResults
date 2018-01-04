```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  11.2M      0 --:--:-- --:--:-- --:--:-- 11.2M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  120M    0  895k    0     0  3908k      0  0:00:31 --:--:--  0:00:31 3893k  8  120M    8 10.7M    0     0  8984k      0  0:00:13  0:00:01  0:00:12 8982k 21  120M   21 26.5M    0     0  11.9M      0  0:00:10  0:00:02  0:00:08 11.9M 29  120M   29 36.2M    0     0  11.2M      0  0:00:10  0:00:03  0:00:07 11.2M 36  120M   36 43.7M    0     0  10.3M      0  0:00:11  0:00:04  0:00:07 10.3M 42  120M   42 51.2M    0     0   9.7M      0  0:00:12  0:00:05  0:00:07 10.0M 46  120M   46 56.7M    0     0  9330k      0  0:00:13  0:00:06  0:00:07 9414k 51  120M   51 62.3M    0     0  8834k      0  0:00:13  0:00:07  0:00:06 7333k 56  120M   56 68.7M    0     0  8551k      0  0:00:14  0:00:08  0:00:06 6661k 65  120M   65 79.4M    0     0  8813k      0  0:00:14  0:00:09  0:00:05 7297k 74  120M   74 89.5M    0     0  8968k      0  0:00:13  0:00:10  0:00:03 7852k 83  120M   83  101M    0     0  9244k      0  0:00:13  0:00:11  0:00:02 9136k 93  120M   93  113M    0     0  9481k      0  0:00:13  0:00:12  0:00:01 10.1M100  120M  100  120M    0     0  9811k      0  0:00:12  0:00:12 --:--:-- 11.8M
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
] Testing  DEBUG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```