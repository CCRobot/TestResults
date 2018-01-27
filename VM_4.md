```
Executed on ubu16chk400000P
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 19 9180k   19 1807k    0     0  2315k      0  0:00:03 --:--:--  0:00:03 2314k100 9180k  100 9180k    0     0  8517k      0  0:00:01  0:00:01 --:--:-- 8524k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  139M    1 1807k    0     0  2626k      0  0:00:54 --:--:--  0:00:54 2623k 25  139M   25 36.0M    0     0  20.8M      0  0:00:06  0:00:01  0:00:05 20.8M 54  139M   54 76.0M    0     0  27.8M      0  0:00:04  0:00:02  0:00:02 27.8M 83  139M   83  116M    0     0  31.3M      0  0:00:04  0:00:03  0:00:01 31.3M100  139M  100  139M    0     0  33.3M      0  0:00:04  0:00:04 --:--:-- 33.3M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   5127477..8384c14  master     -> origin/master
   37993b9..acd7454  release/1.9 -> origin/release/1.9
Updating 5127477..8384c14
Fast-forward
 CMakeLists.txt                                    |  19 ++-
 bin/ch/Helpers.cpp                                | 188 ++++++++++++----------
 bin/ch/stdafx.h                                   |   7 +-
 lib/Backend/BackwardPass.cpp                      |  40 ++---
 lib/Backend/Encoder.cpp                           |   2 +-
 lib/Backend/Lower.cpp                             |  36 +++--
 lib/Backend/LowerMDShared.cpp                     |   4 +-
 lib/Backend/LowerMDShared.h                       |   2 +-
 lib/Backend/amd64/LowererMDArch.cpp               | 159 +++++++++++++++---
 lib/Backend/amd64/LowererMDArch.h                 |   4 +-
 lib/Backend/arm/LowerMD.cpp                       |   2 +-
 lib/Backend/arm/LowerMD.h                         |   2 +-
 lib/Backend/arm64/LowerMD.cpp                     |   4 +-
 lib/Backend/arm64/LowerMD.h                       |   4 +-
 lib/Backend/i386/LowererMDArch.cpp                |   2 +-
 lib/Backend/i386/LowererMDArch.h                  |   2 +-
 lib/Common/Common/NumberUtilities.h               |  76 +++++++--
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
 test/AsmJs/divByConstants.js                      |  44 ++---
 test/AsmJs/divByConstants_Unsigned.js             | 158 ++++++++++++++++++
 test/AsmJs/rlexe.xml                              |   7 +
 test/es6/bug_issue_3257.js                        |   7 -
 test/es6/bug_issue_3257_mod/mod0.js               |   9 --
 test/es6/bug_issue_3257_mod1.js                   |   7 -
 test/es6/bug_issue_3257_mod2/mod2.js              |   7 -
 test/es6/bug_issue_3257_script/script0.js         |   8 -
 test/es6/rlexe.xml                                |  10 --
 test/{es6 => es6module}/bug_issue_3257.baseline   |   0
 test/es6module/bug_issue_3257.js                  |  30 ++++
 test/es6module/rlexe.xml                          |   8 +
 test/wasm/divByConstants_unsigned.js              | 172 ++++++++++++++++++++
 test/wasm/rlexe.xml                               |   7 +
 43 files changed, 795 insertions(+), 276 deletions(-)
 create mode 100644 test/AsmJs/divByConstants_Unsigned.js
 delete mode 100644 test/es6/bug_issue_3257.js
 delete mode 100644 test/es6/bug_issue_3257_mod/mod0.js
 delete mode 100644 test/es6/bug_issue_3257_mod1.js
 delete mode 100644 test/es6/bug_issue_3257_mod2/mod2.js
 delete mode 100644 test/es6/bug_issue_3257_script/script0.js
 rename test/{es6 => es6module}/bug_issue_3257.baseline (100%)
 create mode 100644 test/es6module/bug_issue_3257.js
 create mode 100644 test/wasm/divByConstants_unsigned.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  NODE_BUILD_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```