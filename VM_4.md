```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  9675k      0  0:00:01  0:00:01 --:--:-- 9678k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  9  129M    9 12.3M    0     0  11.6M      0  0:00:11  0:00:01  0:00:10 11.6M 19  129M   19 24.5M    0     0  11.9M      0  0:00:10  0:00:02  0:00:08 11.9M 27  129M   27 35.9M    0     0  11.7M      0  0:00:11  0:00:03  0:00:08 11.7M 37  129M   37 48.0M    0     0  11.7M      0  0:00:10  0:00:04  0:00:06 11.7M 48  129M   48 62.8M    0     0  12.4M      0  0:00:10  0:00:05  0:00:05 12.6M 57  129M   57 74.0M    0     0  12.2M      0  0:00:10  0:00:06  0:00:04 12.3M 67  129M   67 86.8M    0     0  12.2M      0  0:00:10  0:00:07  0:00:03 12.4M 76  129M   76 98.3M    0     0  12.1M      0  0:00:10  0:00:08  0:00:02 12.4M 86  129M   86  111M    0     0  12.3M      0  0:00:10  0:00:09  0:00:01 12.8M 96  129M   96  124M    0     0  12.3M      0  0:00:10  0:00:10 --:--:-- 12.2M100  129M  100  129M    0     0  12.4M      0  0:00:10  0:00:10 --:--:-- 12.8M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c27adba..6311ef5  master      -> origin/master
   745ddf8..148c8af  intl-icu    -> origin/intl-icu
   3e68e46..0ce001c  release/1.8 -> origin/release/1.8
Updating c27adba..6311ef5
Fast-forward
 bin/ChakraCore/ChakraCore.def                      |   2 +
 bin/NativeTests/JsRTApiTest.cpp                    | 211 +++++++++++++++++++++
 bin/ch/ChakraRtInterface.h                         |   5 +-
 lib/Backend/BackwardPass.cpp                       |   8 +-
 lib/Backend/BailOut.cpp                            |   8 +-
 lib/Backend/BailOut.h                              |   5 +-
 lib/Backend/FlowGraph.cpp                          |   3 +
 lib/Backend/GlobOpt.cpp                            |  65 ++++---
 lib/Backend/GlobOpt.h                              |   1 +
 lib/Backend/GlobOptBailOut.cpp                     |  29 +--
 lib/Backend/GlobOptBlockData.cpp                   |  38 +++-
 lib/Backend/GlobOptBlockData.h                     |   1 +
 lib/Backend/IR.cpp                                 |  13 +-
 lib/Backend/IR.h                                   |  20 +-
 lib/Backend/amd64/LinearScanMD.cpp                 |   8 +-
 lib/Backend/i386/LinearScanMD.cpp                  |   8 +-
 lib/Jsrt/ChakraCore.h                              |  47 +++++
 lib/Jsrt/Jsrt.cpp                                  |  76 ++++++--
 lib/Runtime/Base/FunctionBody.cpp                  |   3 +
 lib/Runtime/ByteCode/ByteCodeEmitter.cpp           |  18 +-
 lib/Runtime/Language/JavascriptOperators.cpp       |   2 +-
 lib/Runtime/Library/JavascriptExternalFunction.cpp |  23 ++-
 lib/Runtime/Library/JavascriptExternalFunction.h   |  11 +-
 lib/Runtime/Library/JavascriptLibrary.h            |   1 +
 test/Optimizer/capturedValuesBugs.js               |  29 +++
 test/Optimizer/rlexe.xml                           |  12 ++
 test/Optimizer/test146.js                          |  52 +++++
 test/Optimizer/test147.js                          |  19 ++
 test/es6/bug_OS14562349.js                         |  24 +++
 test/es6/rlexe.xml                                 |   7 +
 30 files changed, 642 insertions(+), 107 deletions(-)
 create mode 100644 test/Optimizer/test146.js
 create mode 100644 test/Optimizer/test147.js
 create mode 100644 test/es6/bug_OS14562349.js
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