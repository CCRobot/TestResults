```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 41 11.1M   41 4736k    0     0  5918k      0  0:00:01 --:--:--  0:00:01 5912k100 11.1M  100 11.1M    0     0  9757k      0  0:00:01  0:00:01 --:--:-- 9761k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  133M    5 8208k    0     0  12.6M      0  0:00:10 --:--:--  0:00:10 12.6M 14  133M   14 18.7M    0     0  11.6M      0  0:00:11  0:00:01  0:00:10 11.6M 20  133M   20 26.9M    0     0  10.3M      0  0:00:12  0:00:02  0:00:10 10.3M 29  133M   29 39.2M    0     0  10.8M      0  0:00:12  0:00:03  0:00:09 10.8M 38  133M   38 51.4M    0     0  11.1M      0  0:00:12  0:00:04  0:00:08 11.1M 49  133M   49 65.6M    0     0  11.6M      0  0:00:11  0:00:05  0:00:06 11.5M 59  133M   59 79.7M    0     0  12.0M      0  0:00:11  0:00:06  0:00:05 12.2M 68  133M   68 91.9M    0     0  12.0M      0  0:00:11  0:00:07  0:00:04 12.9M 78  133M   78  104M    0     0  12.1M      0  0:00:11  0:00:08  0:00:03 13.0M 87  133M   87  117M    0     0  12.2M      0  0:00:10  0:00:09  0:00:01 13.1M 97  133M   97  131M    0     0  12.3M      0  0:00:10  0:00:10 --:--:-- 13.0M100  133M  100  133M    0     0  12.2M      0  0:00:10  0:00:10 --:--:-- 12.5M
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
] Testing  DEBUG_FLG2_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```