```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 15 11.1M   15 1727k    0     0  4797k      0  0:00:02 --:--:--  0:00:02 4785k100 11.1M  100 11.1M    0     0  10.6M      0  0:00:01  0:00:01 --:--:-- 10.6M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  133M    1 1423k    0     0  4757k      0  0:00:28 --:--:--  0:00:28 4745k 11  133M   11 15.5M    0     0  11.9M      0  0:00:11  0:00:01  0:00:10 11.9M 17  133M   17 23.3M    0     0  10.1M      0  0:00:13  0:00:02  0:00:11 10.1M 26  133M   26 35.1M    0     0  10.6M      0  0:00:12  0:00:03  0:00:09 10.6M 35  133M   35 48.0M    0     0  11.1M      0  0:00:11  0:00:04  0:00:07 11.1M 45  133M   45 61.0M    0     0  11.5M      0  0:00:11  0:00:05  0:00:06 11.9M 55  133M   55 74.5M    0     0  11.8M      0  0:00:11  0:00:06  0:00:05 11.7M 64  133M   64 86.6M    0     0  11.8M      0  0:00:11  0:00:07  0:00:04 12.6M 75  133M   75  100M    0     0  12.1M      0  0:00:11  0:00:08  0:00:03 13.0M 84  133M   84  113M    0     0  12.2M      0  0:00:10  0:00:09  0:00:01 13.0M 95  133M   95  128M    0     0  12.4M      0  0:00:10  0:00:10 --:--:-- 13.4M100  133M  100  133M    0     0  12.6M      0  0:00:10  0:00:10 --:--:-- 13.8M
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
] Testing  NODE_BUILD_osx
done!
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```