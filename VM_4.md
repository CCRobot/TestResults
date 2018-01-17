```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 11 11.1M   11 1311k    0     0  2876k      0  0:00:03 --:--:--  0:00:03 2876k100 11.1M  100 11.1M    0     0  9124k      0  0:00:01  0:00:01 --:--:-- 9126k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  132M    6 8656k    0     0  7279k      0  0:00:18  0:00:01  0:00:17 7280k 16  132M   16 22.5M    0     0  10.3M      0  0:00:12  0:00:02  0:00:10 10.2M 27  132M   27 36.0M    0     0  11.2M      0  0:00:11  0:00:03  0:00:08 11.2M 37  132M   37 50.3M    0     0  12.0M      0  0:00:11  0:00:04  0:00:07 12.0M 42  132M   42 57.0M    0     0  11.0M      0  0:00:12  0:00:05  0:00:07 11.4M 51  132M   51 68.0M    0     0  10.9M      0  0:00:12  0:00:06  0:00:06 11.8M 58  132M   58 78.1M    0     0  10.8M      0  0:00:12  0:00:07  0:00:05 11.1M 67  132M   67 89.7M    0     0  10.9M      0  0:00:12  0:00:08  0:00:04 10.7M 74  132M   74 98.8M    0     0  10.7M      0  0:00:12  0:00:09  0:00:03 9925k 81  132M   81  108M    0     0  10.6M      0  0:00:12  0:00:10  0:00:02 10.2M 89  132M   89  119M    0     0  10.6M      0  0:00:12  0:00:11  0:00:01 10.3M 98  132M   98  131M    0     0  10.7M      0  0:00:12  0:00:12 --:--:-- 10.6M100  132M  100  132M    0     0  10.8M      0  0:00:12  0:00:12 --:--:-- 10.5M
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
] Testing  NODE_BUILD_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```