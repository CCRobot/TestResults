```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 68 11.1M   68 7792k    0     0  8599k      0  0:00:01 --:--:--  0:00:01 8590k100 11.1M  100 11.1M    0     0  9914k      0  0:00:01  0:00:01 --:--:-- 9922k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  132M    3 4832k    0     0  6549k      0  0:00:20 --:--:--  0:00:20 6547k  9  132M    9 12.0M    0     0  6963k      0  0:00:19  0:00:01  0:00:18 6963k 15  132M   15 20.1M    0     0  7536k      0  0:00:18  0:00:02  0:00:16 7535k 22  132M   22 30.1M    0     0  8258k      0  0:00:16  0:00:03  0:00:13 8256k 28  132M   28 38.1M    0     0  8232k      0  0:00:16  0:00:04  0:00:12 8232k 33  132M   33 44.6M    0     0  7807k      0  0:00:17  0:00:05  0:00:12 7989k 38  132M   38 51.7M    0     0  7866k      0  0:00:17  0:00:06  0:00:11 8186k 46  132M   46 61.5M    0     0  8140k      0  0:00:16  0:00:07  0:00:09 8470k 52  132M   52 69.8M    0     0  8183k      0  0:00:16  0:00:08  0:00:08 8128k 59  132M   59 78.9M    0     0  8297k      0  0:00:16  0:00:09  0:00:07 8358k 68  132M   68 91.5M    0     0  8733k      0  0:00:15  0:00:10  0:00:05 9842k 75  132M   75  100M    0     0  8740k      0  0:00:15  0:00:11  0:00:04 9919k 81  132M   81  108M    0     0  8730k      0  0:00:15  0:00:12  0:00:03 9644k 86  132M   86  115M    0     0  8607k      0  0:00:15  0:00:13  0:00:02 9348k 90  132M   90  119M    0     0  8333k      0  0:00:16  0:00:14  0:00:02 8406k 97  132M   97  128M    0     0  8391k      0  0:00:16  0:00:15  0:00:01 7657k100  132M  100  132M    0     0  8402k      0  0:00:16  0:00:16 --:--:-- 7513k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   1a5b904..813f97e  master      -> origin/master
   6785a49..461e8c7  release/1.8 -> origin/release/1.8
   98e7835..7949441  release/1.9 -> origin/release/1.9
Updating 1a5b904..813f97e
Fast-forward
 lib/Common/ChakraCoreVersion.h                     |  4 +--
 .../Language/JavascriptExceptionOperators.cpp      | 28 ++++++++++++++++
 lib/Runtime/Language/ModuleRecordBase.h            |  7 ++--
 lib/Runtime/Language/SourceTextModuleRecord.cpp    | 39 ++++++++++++++++++----
 lib/Runtime/Language/SourceTextModuleRecord.h      |  8 +++--
 test/AsmJs/rlexe.xml                               |  2 +-
 test/EH/rlexe.xml                                  |  6 ++++
 test/EH/tryfinallyinlineswbug.js                   | 26 +++++++++++++++
 test/Error/rlexe.xml                               |  2 ++
 test/es6/module-bugfixes.js                        | 31 ++++++++++-------
 test/es6/module_4482_dep1.js                       | 23 +++++++++++++
 test/es6/module_4482_dep2.js                       | 13 ++++++++
 test/es6/module_4482_dep3.js                       | 10 ++++++
 13 files changed, 171 insertions(+), 28 deletions(-)
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
] Testing  DEBUG_FLG2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```