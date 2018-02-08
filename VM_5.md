```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 66 11.1M   66 7536k    0     0  8420k      0  0:00:01 --:--:--  0:00:01 8420k100 11.1M  100 11.1M    0     0  9695k      0  0:00:01  0:00:01 --:--:-- 9702k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  152M    5 8912k    0     0  12.3M      0  0:00:12 --:--:--  0:00:12 12.3M 12  152M   12 18.6M    0     0  10.9M      0  0:00:13  0:00:01  0:00:12 10.9M 20  152M   20 32.0M    0     0  11.8M      0  0:00:12  0:00:02  0:00:10 11.8M 28  152M   28 43.7M    0     0  11.7M      0  0:00:12  0:00:03  0:00:09 11.7M 36  152M   36 55.8M    0     0  11.8M      0  0:00:12  0:00:04  0:00:08 11.8M 45  152M   45 69.1M    0     0  12.1M      0  0:00:12  0:00:05  0:00:07 12.0M 51  152M   51 78.4M    0     0  11.7M      0  0:00:13  0:00:06  0:00:07 11.9M 57  152M   57 87.8M    0     0  11.3M      0  0:00:13  0:00:07  0:00:06 11.1M 63  152M   63 96.7M    0     0  11.1M      0  0:00:13  0:00:08  0:00:05 10.6M 69  152M   69  106M    0     0  10.9M      0  0:00:13  0:00:09  0:00:04 10.0M 75  152M   75  115M    0     0  10.7M      0  0:00:14  0:00:10  0:00:04 9477k 81  152M   81  125M    0     0  10.6M      0  0:00:14  0:00:11  0:00:03 9536k 87  152M   87  134M    0     0  10.5M      0  0:00:14  0:00:12  0:00:02 9555k 94  152M   94  144M    0     0  10.5M      0  0:00:14  0:00:13  0:00:01 9846k 99  152M   99  152M    0     0  10.3M      0  0:00:14  0:00:14 --:--:-- 9465k100  152M  100  152M    0     0  10.3M      0  0:00:14  0:00:14 --:--:-- 9465k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   215b215..c0c17cf  master      -> origin/master
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
] Testing  DEBUG_FLG1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```