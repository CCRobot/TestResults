```
Executed on ubu16chk4000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  11.9M      0 --:--:-- --:--:-- --:--:-- 11.9M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  132M    0 32345    0     0  89442      0  0:25:58 --:--:--  0:25:58 89350 21  132M   21 28.2M    0     0  20.8M      0  0:00:06  0:00:01  0:00:05 20.8M 40  132M   40 54.1M    0     0  22.8M      0  0:00:05  0:00:02  0:00:03 22.8M 55  132M   55 74.4M    0     0  22.1M      0  0:00:05  0:00:03  0:00:02 22.1M 70  132M   70 94.1M    0     0  21.5M      0  0:00:06  0:00:04  0:00:02 21.5M 84  132M   84  112M    0     0  20.7M      0  0:00:06  0:00:05  0:00:01 22.2M100  132M  100  132M    0     0  20.9M      0  0:00:06  0:00:06 --:--:-- 21.0M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   1a5b904..e0a8f50  master     -> origin/master
   6785a49..6c055d9  release/1.8 -> origin/release/1.8
   98e7835..d7d99e1  release/1.9 -> origin/release/1.9
Updating 1a5b904..e0a8f50
Fast-forward
 bin/NativeTests/JsRTApiTest.cpp                    | 48 +++++++++++++++++
 lib/Backend/BailOut.cpp                            | 11 ++++
 lib/Common/ChakraCoreVersion.h                     |  4 +-
 lib/Runtime/Base/ThreadContext.cpp                 |  1 +
 lib/Runtime/Base/ThreadContext.h                   | 11 ++++
 .../Language/JavascriptExceptionOperators.cpp      | 61 ++++++++++++++++++++--
 lib/Runtime/Language/ModuleRecordBase.h            |  7 +--
 lib/Runtime/Language/SourceTextModuleRecord.cpp    | 40 +++++++++++---
 lib/Runtime/Language/SourceTextModuleRecord.h      |  8 +--
 test/AsmJs/rlexe.xml                               |  2 +-
 test/EH/hasBailedOutBug.baseline                   |  1 +
 test/EH/hasBailedOutBug.js                         | 48 +++++++++++++++++
 test/EH/rlexe.xml                                  | 12 +++++
 test/EH/tryfinallyinlineswbug.js                   | 26 +++++++++
 test/Error/rlexe.xml                               |  2 +
 test/es6/module-bugfixes.js                        | 31 ++++++-----
 test/es6/module_4482_dep1.js                       | 23 ++++++++
 test/es6/module_4482_dep2.js                       | 13 +++++
 test/es6/module_4482_dep3.js                       | 10 ++++
 19 files changed, 325 insertions(+), 34 deletions(-)
 create mode 100644 test/EH/hasBailedOutBug.baseline
 create mode 100644 test/EH/hasBailedOutBug.js
 create mode 100644 test/EH/tryfinallyinlineswbug.js
 create mode 100644 test/es6/module_4482_dep1.js
 create mode 100644 test/es6/module_4482_dep2.js
 create mode 100644 test/es6/module_4482_dep3.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_F1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```