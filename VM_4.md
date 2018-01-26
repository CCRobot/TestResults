```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 16 11.1M   16 1855k    0     0  4113k      0  0:00:02 --:--:--  0:00:02 4114k100 11.1M  100 11.1M    0     0  8575k      0  0:00:01  0:00:01 --:--:-- 8576k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  139M    6 8784k    0     0  7900k      0  0:00:18  0:00:01  0:00:17 7899k 14  139M   14 20.0M    0     0  9719k      0  0:00:14  0:00:02  0:00:12 9715k 20  139M   20 28.9M    0     0  9503k      0  0:00:15  0:00:03  0:00:12 9502k 28  139M   28 39.8M    0     0  9925k      0  0:00:14  0:00:04  0:00:10 9923k 38  139M   38 53.3M    0     0  10.4M      0  0:00:13  0:00:05  0:00:08 10.6M 45  139M   45 63.3M    0     0  10.3M      0  0:00:13  0:00:06  0:00:07 10.9M 55  139M   55 77.0M    0     0  10.8M      0  0:00:12  0:00:07  0:00:05 11.4M 62  139M   62 87.5M    0     0  10.7M      0  0:00:12  0:00:08  0:00:04 11.7M 66  139M   66 92.4M    0     0  10.1M      0  0:00:13  0:00:09  0:00:04 10.5M 75  139M   75  105M    0     0  10.4M      0  0:00:13  0:00:10  0:00:03 10.3M 83  139M   83  116M    0     0  10.4M      0  0:00:13  0:00:11  0:00:02 10.6M 90  139M   90  126M    0     0  10.4M      0  0:00:13  0:00:12  0:00:01  9.9M 98  139M   98  137M    0     0  10.4M      0  0:00:13  0:00:13 --:--:-- 10.0M100  139M  100  139M    0     0  10.4M      0  0:00:13  0:00:13 --:--:-- 11.1M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   5127477..61e9cba  master      -> origin/master
   37993b9..acd7454  release/1.9 -> origin/release/1.9
Updating 5127477..61e9cba
Fast-forward
 CMakeLists.txt                                    |  19 ++-
 bin/ch/Helpers.cpp                                | 188 ++++++++++++----------
 bin/ch/stdafx.h                                   |   7 +-
 lib/Backend/BackwardPass.cpp                      |  40 ++---
 lib/Backend/Encoder.cpp                           |   2 +-
 lib/Common/CommonDefines.h                        |   2 +-
 lib/Common/CommonPal.h                            |   8 +-
 lib/Common/Core/SysInfo.h                         |   4 +-
 lib/Common/DataStructures/Comparer.h              |   2 +-
 lib/Common/Memory/MarkContext.inl                 |   2 +-
 lib/Common/Memory/RecyclerWriteBarrierManager.cpp |   6 +-
 lib/Parser/errstr.cpp                             |   4 +-
 lib/Parser/screrror.cpp                           |   4 +-
 lib/Runtime/Library/ArrayBuffer.h                 |   2 +-
 lib/Runtime/Library/SharedArrayBuffer.h           |   4 +-
 pal/src/CMakeLists.txt                            |   4 -
 pal/src/configure.cmake                           |   2 +-
 test/es6/bug_issue_3257.js                        |   7 -
 test/es6/bug_issue_3257_mod/mod0.js               |   9 --
 test/es6/bug_issue_3257_mod1.js                   |   7 -
 test/es6/bug_issue_3257_mod2/mod2.js              |   7 -
 test/es6/bug_issue_3257_script/script0.js         |   8 -
 test/es6/rlexe.xml                                |  10 --
 test/{es6 => es6module}/bug_issue_3257.baseline   |   0
 test/es6module/bug_issue_3257.js                  |  30 ++++
 test/es6module/rlexe.xml                          |   8 +
 26 files changed, 197 insertions(+), 189 deletions(-)
 delete mode 100644 test/es6/bug_issue_3257.js
 delete mode 100644 test/es6/bug_issue_3257_mod/mod0.js
 delete mode 100644 test/es6/bug_issue_3257_mod1.js
 delete mode 100644 test/es6/bug_issue_3257_mod2/mod2.js
 delete mode 100644 test/es6/bug_issue_3257_script/script0.js
 rename test/{es6 => es6module}/bug_issue_3257.baseline (100%)
 create mode 100644 test/es6module/bug_issue_3257.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_F1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```