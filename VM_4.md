```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 81 11.1M   81 9280k    0     0  9738k      0  0:00:01 --:--:--  0:00:01 9737k100 11.1M  100 11.1M    0     0  10.0M      0  0:00:01  0:00:01 --:--:-- 10.0M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  152M    4 6848k    0     0  8338k      0  0:00:18 --:--:--  0:00:18 8330k 12  152M   12 19.5M    0     0  10.7M      0  0:00:14  0:00:01  0:00:13 10.7M 22  152M   22 35.0M    0     0  12.4M      0  0:00:12  0:00:02  0:00:10 12.4M 32  152M   32 49.4M    0     0  12.9M      0  0:00:11  0:00:03  0:00:08 12.9M 43  152M   43 66.8M    0     0  13.8M      0  0:00:11  0:00:04  0:00:07 13.8M 53  152M   53 82.5M    0     0  14.1M      0  0:00:10  0:00:05  0:00:05 15.1M 63  152M   63 96.5M    0     0  14.1M      0  0:00:10  0:00:06  0:00:04 15.3M 71  152M   71  108M    0     0  13.9M      0  0:00:10  0:00:07  0:00:03 14.7M 80  152M   80  122M    0     0  13.9M      0  0:00:10  0:00:08  0:00:02 14.6M 88  152M   88  134M    0     0  13.6M      0  0:00:11  0:00:09  0:00:02 13.5M 96  152M   96  148M    0     0  13.6M      0  0:00:11  0:00:10  0:00:01 13.1M100  152M  100  152M    0     0  13.7M      0  0:00:11  0:00:11 --:--:-- 13.1M
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
] Testing  NODE_BUILD_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```