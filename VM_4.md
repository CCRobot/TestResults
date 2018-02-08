```
Executed on ubu16chk400001D
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1 9180k    1  143k    0     0   287k      0  0:00:31 --:--:--  0:00:31  287k100 9180k  100 9180k    0     0  9352k      0 --:--:-- --:--:-- --:--:-- 9349k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  152M    0  319k    0     0   632k      0  0:04:07 --:--:--  0:04:07  632k 18  152M   18 28.0M    0     0  18.5M      0  0:00:08  0:00:01  0:00:07 18.5M 46  152M   46 70.9M    0     0  28.4M      0  0:00:05  0:00:02  0:00:03 28.4M 74  152M   74  114M    0     0  32.6M      0  0:00:04  0:00:03  0:00:01 32.6M100  152M  100  152M    0     0  35.0M      0  0:00:04  0:00:04 --:--:-- 35.1M
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
] Testing  NODE_BUILD_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```