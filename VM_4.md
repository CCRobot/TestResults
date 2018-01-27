```
Executed on ubu16chk400000O
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2 9180k    2  255k    0     0   442k      0  0:00:20 --:--:--  0:00:20  442k100 9180k  100 9180k    0     0  8523k      0  0:00:01  0:00:01 --:--:-- 8524k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  139M    0  191k    0     0   404k      0  0:05:52 --:--:--  0:05:52  404k 16  139M   16 23.1M    0     0  15.7M      0  0:00:08  0:00:01  0:00:07 15.7M 45  139M   45 63.1M    0     0  25.3M      0  0:00:05  0:00:02  0:00:03 25.3M 66  139M   66 92.0M    0     0  26.2M      0  0:00:05  0:00:03  0:00:02 26.2M 86  139M   86  120M    0     0  27.0M      0  0:00:05  0:00:04  0:00:01 27.0M100  139M  100  139M    0     0  27.6M      0  0:00:05  0:00:05 --:--:-- 30.5M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   5127477..61e9cba  master     -> origin/master
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
] Testing  RL18_DBG_F1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```