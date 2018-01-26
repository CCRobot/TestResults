```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 17 11.1M   17 2015k    0     0  5547k      0  0:00:02 --:--:--  0:00:02 5537k100 11.1M  100 11.1M    0     0   9.9M      0  0:00:01  0:00:01 --:--:--  9.9M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  139M    0  415k    0     0  1748k      0  0:01:21 --:--:--  0:01:21 1746k  7  139M    7 10.7M    0     0  8909k      0  0:00:16  0:00:01  0:00:15 8906k 14  139M   14 19.7M    0     0  9063k      0  0:00:15  0:00:02  0:00:13 9062k 21  139M   21 29.4M    0     0  9329k      0  0:00:15  0:00:03  0:00:12 9327k 27  139M   27 38.7M    0     0  9368k      0  0:00:15  0:00:04  0:00:11 9367k 33  139M   33 46.2M    0     0  8734k      0  0:00:16  0:00:05  0:00:11 9055k 36  139M   36 50.4M    0     0  8122k      0  0:00:17  0:00:06  0:00:11 7932k 40  139M   40 56.1M    0     0  7950k      0  0:00:17  0:00:07  0:00:10 7452k 48  139M   48 67.4M    0     0  8387k      0  0:00:17  0:00:08  0:00:09 7776k 56  139M   56 78.1M    0     0  8668k      0  0:00:16  0:00:09  0:00:07 8073k 63  139M   63 88.1M    0     0  8650k      0  0:00:16  0:00:10  0:00:06 8560k 67  139M   67 94.6M    0     0  8628k      0  0:00:16  0:00:11  0:00:05 9286k 75  139M   75  105M    0     0  8832k      0  0:00:16  0:00:12  0:00:04  9.8M 84  139M   84  117M    0     0  9065k      0  0:00:15  0:00:13  0:00:02  9.9M 91  139M   91  127M    0     0  9205k      0  0:00:15  0:00:14  0:00:01  9.9M100  139M  100  139M    0     0  9389k      0  0:00:15  0:00:15 --:--:-- 10.7M
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
] Testing  RL18_PACK
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```