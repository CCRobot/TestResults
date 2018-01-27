```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 23 11.1M   23 2703k    0     0  5026k      0  0:00:02 --:--:--  0:00:02 5025k 94 11.1M   94 10.5M    0     0  7006k      0  0:00:01  0:00:01 --:--:-- 7004k100 11.1M  100 11.1M    0     0  7175k      0  0:00:01  0:00:01 --:--:-- 7171k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  139M    6 9360k    0     0   9.8M      0  0:00:14 --:--:--  0:00:14  9.8M 13  139M   13 18.4M    0     0  9793k      0  0:00:14  0:00:01  0:00:13 9790k 21  139M   21 30.6M    0     0  10.4M      0  0:00:13  0:00:02  0:00:11 10.4M 27  139M   27 38.9M    0     0   9.9M      0  0:00:14  0:00:03  0:00:11  9.9M 36  139M   36 50.3M    0     0  10.2M      0  0:00:13  0:00:04  0:00:09 10.2M 44  139M   44 62.2M    0     0  10.4M      0  0:00:13  0:00:05  0:00:08 10.6M 51  139M   51 71.8M    0     0  10.3M      0  0:00:13  0:00:06  0:00:07 10.6M 60  139M   60 84.0M    0     0  10.5M      0  0:00:13  0:00:07  0:00:06 10.6M 69  139M   69 96.4M    0     0  10.8M      0  0:00:12  0:00:08  0:00:04 11.4M 78  139M   78  108M    0     0  10.9M      0  0:00:12  0:00:09  0:00:03 11.6M 85  139M   85  119M    0     0  10.9M      0  0:00:12  0:00:10  0:00:02 11.5M 94  139M   94  131M    0     0  11.0M      0  0:00:12  0:00:11  0:00:01 12.0M100  139M  100  139M    0     0  10.9M      0  0:00:12  0:00:12 --:--:-- 11.6M
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
] Testing  TEST_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```