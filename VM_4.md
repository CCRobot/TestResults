```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 66 11.1M   66 7600k    0     0  7835k      0  0:00:01 --:--:--  0:00:01 7835k100 11.1M  100 11.1M    0     0  8984k      0  0:00:01  0:00:01 --:--:-- 8990k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  139M    5 7376k    0     0  10.5M      0  0:00:13 --:--:--  0:00:13 10.5M 15  139M   15 21.2M    0     0  12.6M      0  0:00:11  0:00:01  0:00:10 12.6M 25  139M   25 34.8M    0     0  12.9M      0  0:00:10  0:00:02  0:00:08 12.9M 33  139M   33 47.0M    0     0  12.7M      0  0:00:10  0:00:03  0:00:07 12.7M 43  139M   43 60.7M    0     0  12.9M      0  0:00:10  0:00:04  0:00:06 12.9M 52  139M   52 72.5M    0     0  12.7M      0  0:00:10  0:00:05  0:00:05 13.0M 61  139M   61 85.4M    0     0  12.7M      0  0:00:10  0:00:06  0:00:04 12.8M 70  139M   70 98.2M    0     0  12.7M      0  0:00:10  0:00:07  0:00:03 12.6M 79  139M   79  111M    0     0  12.8M      0  0:00:10  0:00:08  0:00:02 12.8M 88  139M   88  123M    0     0  12.7M      0  0:00:10  0:00:09  0:00:01 12.5M 98  139M   98  137M    0     0  12.8M      0  0:00:10  0:00:10 --:--:-- 13.0M100  139M  100  139M    0     0  12.9M      0  0:00:10  0:00:10 --:--:-- 13.1M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   5127477..8384c14  master      -> origin/master
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
] Testing  NODE_BUILD_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```