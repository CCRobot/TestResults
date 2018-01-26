```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 24 11.1M   24 2815k    0     0  5753k      0  0:00:01 --:--:--  0:00:01 5746k100 11.1M  100 11.1M    0     0  8093k      0  0:00:01  0:00:01 --:--:-- 8094k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  8  139M    8 12.1M    0     0  11.3M      0  0:00:12  0:00:01  0:00:11 11.3M 17  139M   17 24.3M    0     0  11.7M      0  0:00:11  0:00:02  0:00:09 11.7M 25  139M   25 35.9M    0     0  11.7M      0  0:00:11  0:00:03  0:00:08 11.7M 31  139M   31 44.4M    0     0  10.9M      0  0:00:12  0:00:04  0:00:08 10.9M 38  139M   38 53.8M    0     0  10.6M      0  0:00:13  0:00:05  0:00:08 10.8M 43  139M   43 60.6M    0     0  10.0M      0  0:00:13  0:00:06  0:00:07 9952k 51  139M   51 71.5M    0     0  10.1M      0  0:00:13  0:00:07  0:00:06 9684k 59  139M   59 82.2M    0     0  10.1M      0  0:00:13  0:00:08  0:00:05 9486k 66  139M   66 92.5M    0     0  10.2M      0  0:00:13  0:00:09  0:00:04 9840k 73  139M   73  102M    0     0  10.2M      0  0:00:13  0:00:10  0:00:03  9.8M 82  139M   82  114M    0     0  10.3M      0  0:00:13  0:00:11  0:00:02 10.7M 88  139M   88  122M    0     0  10.1M      0  0:00:13  0:00:12  0:00:01 10.2M 94  139M   94  132M    0     0  10.1M      0  0:00:13  0:00:13 --:--:--  9.9M100  139M  100  139M    0     0  10.0M      0  0:00:13  0:00:13 --:--:-- 9974k
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
] Testing  RL18_DBG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```