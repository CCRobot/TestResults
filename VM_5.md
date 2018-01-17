```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 88 11.1M   88  9.7M    0     0  9427k      0  0:00:01  0:00:01 --:--:-- 9422k100 11.1M  100 11.1M    0     0  9721k      0  0:00:01  0:00:01 --:--:-- 9719k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  132M    5 7488k    0     0  8623k      0  0:00:15 --:--:--  0:00:15 8616k 15  132M   15 21.2M    0     0  11.3M      0  0:00:11  0:00:01  0:00:10 11.3M 27  132M   27 36.5M    0     0  12.7M      0  0:00:10  0:00:02  0:00:08 12.7M 37  132M   37 50.4M    0     0  13.0M      0  0:00:10  0:00:03  0:00:07 13.0M 44  132M   44 59.5M    0     0  12.2M      0  0:00:10  0:00:04  0:00:06 12.2M 53  132M   53 71.6M    0     0  12.2M      0  0:00:10  0:00:05  0:00:05 12.8M 63  132M   63 84.0M    0     0  12.2M      0  0:00:10  0:00:06  0:00:04 12.5M 71  132M   71 95.2M    0     0  12.1M      0  0:00:10  0:00:07  0:00:03 11.7M 77  132M   77  102M    0     0  11.5M      0  0:00:11  0:00:08  0:00:03 10.4M 84  132M   84  112M    0     0  11.3M      0  0:00:11  0:00:09  0:00:02 10.4M 90  132M   90  120M    0     0  11.1M      0  0:00:11  0:00:10  0:00:01  9.8M 98  132M   98  130M    0     0  11.0M      0  0:00:12  0:00:11  0:00:01 9602k100  132M  100  132M    0     0  11.0M      0  0:00:12  0:00:12 --:--:-- 9218k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   1a5b904..e0a8f50  master      -> origin/master
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
] Testing  DEBUG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```