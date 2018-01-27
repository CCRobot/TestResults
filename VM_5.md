```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  10.4M      0  0:00:01  0:00:01 --:--:-- 10.4M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  9  139M    9 13.1M    0     0  11.9M      0  0:00:11  0:00:01  0:00:10 11.9M 19  139M   19 27.0M    0     0  12.8M      0  0:00:10  0:00:02  0:00:08 12.8M 30  139M   30 42.1M    0     0  13.3M      0  0:00:10  0:00:03  0:00:07 13.3M 39  139M   39 54.8M    0     0  13.3M      0  0:00:10  0:00:04  0:00:06 13.3M 49  139M   49 68.6M    0     0  13.4M      0  0:00:10  0:00:05  0:00:05 13.7M 58  139M   58 81.5M    0     0  13.3M      0  0:00:10  0:00:06  0:00:04 13.6M 67  139M   67 93.9M    0     0  13.2M      0  0:00:10  0:00:07  0:00:03 13.3M 76  139M   76  106M    0     0  13.1M      0  0:00:10  0:00:08  0:00:02 13.0M 86  139M   86  120M    0     0  13.1M      0  0:00:10  0:00:09  0:00:01 13.0M 95  139M   95  132M    0     0  13.1M      0  0:00:10  0:00:10 --:--:-- 12.7M100  139M  100  139M    0     0  13.0M      0  0:00:10  0:00:10 --:--:-- 12.5M
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
] Testing  DEBUG_FLG1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```