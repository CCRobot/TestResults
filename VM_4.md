```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 54 11.1M   54 6208k    0     0  6926k      0  0:00:01 --:--:--  0:00:01 6920k100 11.1M  100 11.1M    0     0  9560k      0  0:00:01  0:00:01 --:--:-- 9564k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  139M    4 5808k    0     0  8602k      0  0:00:16 --:--:--  0:00:16 8591k 11  139M   11 16.2M    0     0  9894k      0  0:00:14  0:00:01  0:00:13 9893k 22  139M   22 32.0M    0     0  11.9M      0  0:00:11  0:00:02  0:00:09 11.9M 32  139M   32 45.7M    0     0  12.4M      0  0:00:11  0:00:03  0:00:08 12.4M 37  139M   37 51.7M    0     0  11.0M      0  0:00:12  0:00:04  0:00:08 11.0M 45  139M   45 63.5M    0     0  11.1M      0  0:00:12  0:00:05  0:00:07 11.5M 51  139M   51 72.0M    0     0  10.7M      0  0:00:12  0:00:06  0:00:06 11.1M 60  139M   60 84.5M    0     0  11.0M      0  0:00:12  0:00:07  0:00:05 10.5M 71  139M   71 99.5M    0     0  11.4M      0  0:00:12  0:00:08  0:00:04 10.7M 80  139M   80  112M    0     0  11.6M      0  0:00:12  0:00:09  0:00:03 12.1M 92  139M   92  128M    0     0  12.0M      0  0:00:11  0:00:10  0:00:01 12.9M100  139M  100  139M    0     0  12.0M      0  0:00:11  0:00:11 --:--:-- 13.7M
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
] Testing  RL18_DBG_F2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```