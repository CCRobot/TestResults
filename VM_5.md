```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 11 11.1M   11 1343k    0     0  2563k      0  0:00:04 --:--:--  0:00:04 2564k100 11.1M  100 11.1M    0     0   9.8M      0  0:00:01  0:00:01 --:--:--  9.8M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  133M    0  431k    0     0  1439k      0  0:01:35 --:--:--  0:01:35 1438k  7  133M    7  9.8M    0     0  7784k      0  0:00:17  0:00:01  0:00:16 7784k 15  133M   15 21.2M    0     0  9451k      0  0:00:14  0:00:02  0:00:12 9448k 24  133M   24 33.2M    0     0  10.0M      0  0:00:13  0:00:03  0:00:10 10.0M 34  133M   34 46.0M    0     0  10.7M      0  0:00:12  0:00:04  0:00:08 10.7M 45  133M   45 61.1M    0     0  11.5M      0  0:00:11  0:00:05  0:00:06 12.1M 56  133M   56 76.2M    0     0  12.0M      0  0:00:11  0:00:06  0:00:05 13.2M 66  133M   66 89.2M    0     0  12.2M      0  0:00:10  0:00:07  0:00:03 13.6M 75  133M   75  101M    0     0  12.0M      0  0:00:11  0:00:08  0:00:03 13.3M 83  133M   83  111M    0     0  12.0M      0  0:00:11  0:00:09  0:00:02 13.1M 92  133M   92  124M    0     0  12.0M      0  0:00:11  0:00:10  0:00:01 12.5M100  133M  100  133M    0     0  12.2M      0  0:00:10  0:00:10 --:--:-- 12.5M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   756a67a..7c1e5c2  master      -> origin/master
   7fb608a..cb4a35c  release/1.8 -> origin/release/1.8
   99131a0..4e2496a  release/1.9 -> origin/release/1.9
Updating 756a67a..7c1e5c2
Fast-forward
 bin/ch/DbgController.js                         |   1 +
 bin/ch/WScriptJsrt.cpp                          | 119 ++++++++++++++++++++++++
 bin/ch/WScriptJsrt.h                            |   3 +-
 bin/ch/ch.cpp                                   |   2 +-
 lib/JITClient/JITManager.cpp                    |   2 +-
 lib/Runtime/Language/SourceTextModuleRecord.cpp |  38 +++++---
 lib/Runtime/Language/SourceTextModuleRecord.h   |   3 +-
 test/Date/parseISO.baseline                     |   8 +-
 test/LetConst/p.baseline                        |  10 --
 test/LetConst/p.js                              |   6 +-
 test/LetConst/q.baseline                        |   5 -
 test/LetConst/q.js                              |   4 +-
 test/UnitTestFramework/known_globals.js         |  20 ++++
 test/es6/bug_issue_3257_mod/mod0.js             |   4 +-
 test/es6/bug_issue_3257_mod2/mod2.js            |   2 +-
 test/es6/module-bugfixes.js                     |   7 ++
 test/es6/module_4570_dep1.js                    |  11 +++
 test/es6/module_4570_dep2.js                    |   6 ++
 test/typedarray/samethread.baseline             |  36 -------
 test/typedarray/samethread.js                   |   4 +-
 20 files changed, 211 insertions(+), 80 deletions(-)
 create mode 100644 test/UnitTestFramework/known_globals.js
 create mode 100644 test/es6/module_4570_dep1.js
 create mode 100644 test/es6/module_4570_dep2.js
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