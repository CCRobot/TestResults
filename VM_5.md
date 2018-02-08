```
Executed on ubu16chk4000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1 9180k    1 97884    0     0   202k      0  0:00:45 --:--:--  0:00:45  202k100 9180k  100 9180k    0     0  10.3M      0 --:--:-- --:--:-- --:--:-- 10.3M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  152M    2 4112k    0     0  6313k      0  0:00:24 --:--:--  0:00:24 6306k 28  152M   28 44.0M    0     0  26.8M      0  0:00:05  0:00:01  0:00:04 26.8M 54  152M   54 84.0M    0     0  31.6M      0  0:00:04  0:00:02  0:00:02 31.6M 75  152M   75  116M    0     0  32.2M      0  0:00:04  0:00:03  0:00:01 32.1M 98  152M   98  149M    0     0  32.6M      0  0:00:04  0:00:04 --:--:-- 32.6M100  152M  100  152M    0     0  32.8M      0  0:00:04  0:00:04 --:--:-- 37.1M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   215b215..c0c17cf  master     -> origin/master
   dbce2eb..05f4157  release/1.8 -> origin/release/1.8
   e4493a2..91ec1ef  release/1.9 -> origin/release/1.9
Updating 215b215..c0c17cf
Fast-forward
 lib/Backend/Func.cpp                       |  5 ++---
 lib/Backend/InliningDecider.cpp            |  8 +++++++-
 lib/Backend/ObjTypeSpecFldInfo.h           |  5 +++--
 lib/Parser/RegexParser.h                   | 11 ++++-------
 lib/Parser/RegexPattern.cpp                |  2 +-
 lib/Parser/RegexPattern.h                  |  2 +-
 lib/Parser/RegexRuntime.h                  |  4 ++--
 lib/Runtime/Library/JavascriptFunction.cpp | 11 ++++++-----
 lib/Runtime/Library/RegexHelper.cpp        | 21 +++++++++------------
 test/AsmJs/manyargs.js                     | 28 ++++++++++++++++++++++++++++
 test/AsmJs/rlexe.xml                       |  5 +++++
 test/typedarray/builtin_from.js            | 10 ++++++++++
 test/typedarray/rlexe.xml                  |  6 ++++++
 13 files changed, 84 insertions(+), 34 deletions(-)
 create mode 100644 test/AsmJs/manyargs.js
 create mode 100644 test/typedarray/builtin_from.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_FLG1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```