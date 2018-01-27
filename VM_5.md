```
Executed on ubu16chk400000P
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 26 9180k   26 2463k    0     0  3796k      0  0:00:02 --:--:--  0:00:02 3795k100 9180k  100 9180k    0     0  10.5M      0 --:--:-- --:--:-- --:--:-- 10.5M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  139M    2 3887k    0     0  4883k      0  0:00:29 --:--:--  0:00:29 4883k 28  139M   28 40.0M    0     0  22.2M      0  0:00:06  0:00:01  0:00:05 22.2M 60  139M   60 84.0M    0     0  29.7M      0  0:00:04  0:00:02  0:00:02 29.7M 90  139M   90  125M    0     0  33.2M      0  0:00:04  0:00:03  0:00:01 33.2M100  139M  100  139M    0     0  34.2M      0  0:00:04  0:00:04 --:--:-- 34.2M
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
] Testing  DEBUG_FLG1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```