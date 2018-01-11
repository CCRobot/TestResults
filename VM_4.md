```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  9 11.1M    9 1135k    0     0  3208k      0  0:00:03 --:--:--  0:00:03 3207k 82 11.1M   82 9424k    0     0  6971k      0  0:00:01  0:00:01 --:--:-- 6970k100 11.1M  100 11.1M    0     0  7630k      0  0:00:01  0:00:01 --:--:-- 7628k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  129M    4 5824k    0     0  6960k      0  0:00:18 --:--:--  0:00:18 6958k  7  129M    7 9584k    0     0  5217k      0  0:00:25  0:00:01  0:00:24 5217k 14  129M   14 18.4M    0     0  6649k      0  0:00:19  0:00:02  0:00:17 6648k 19  129M   19 25.7M    0     0  6876k      0  0:00:19  0:00:03  0:00:16 6875k 25  129M   25 33.2M    0     0  7049k      0  0:00:18  0:00:04  0:00:14 7048k 37  129M   37 47.9M    0     0  8401k      0  0:00:15  0:00:05  0:00:10 8642k 45  129M   45 58.6M    0     0  8780k      0  0:00:15  0:00:06  0:00:09  9.8M 55  129M   55 71.3M    0     0  9319k      0  0:00:14  0:00:07  0:00:07 10.5M 66  129M   66 85.4M    0     0  9906k      0  0:00:13  0:00:08  0:00:05 11.9M 75  129M   75 97.9M    0     0   9.9M      0  0:00:12  0:00:09  0:00:03 12.9M 85  129M   85  110M    0     0  10.1M      0  0:00:12  0:00:10  0:00:02 12.3M 90  129M   90  116M    0     0   9.8M      0  0:00:13  0:00:11  0:00:02 11.5M 96  129M   96  124M    0     0  9963k      0  0:00:13  0:00:12  0:00:01 10.7M100  129M  100  129M    0     0  9955k      0  0:00:13  0:00:13 --:--:--  9.8M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c27adba..b98eebf  master      -> origin/master
   3e68e46..0ce001c  release/1.8 -> origin/release/1.8
Updating c27adba..b98eebf
Fast-forward
 lib/Backend/BackwardPass.cpp             |  8 ++--
 lib/Backend/BailOut.cpp                  |  8 +++-
 lib/Backend/BailOut.h                    |  5 ++-
 lib/Backend/FlowGraph.cpp                |  3 ++
 lib/Backend/GlobOpt.cpp                  | 65 +++++++++++++++++---------------
 lib/Backend/GlobOpt.h                    |  1 +
 lib/Backend/GlobOptBailOut.cpp           | 29 ++++++++------
 lib/Backend/GlobOptBlockData.cpp         | 38 ++++++++++++++++---
 lib/Backend/GlobOptBlockData.h           |  1 +
 lib/Backend/IR.cpp                       | 13 ++-----
 lib/Backend/IR.h                         | 20 ++++++++--
 lib/Backend/amd64/LinearScanMD.cpp       |  8 ++--
 lib/Backend/i386/LinearScanMD.cpp        |  8 ++--
 lib/Runtime/Base/FunctionBody.cpp        |  3 ++
 lib/Runtime/ByteCode/ByteCodeEmitter.cpp | 18 +++++++--
 test/Optimizer/capturedValuesBugs.js     | 29 ++++++++++++++
 test/Optimizer/rlexe.xml                 | 12 ++++++
 test/Optimizer/test146.js                | 52 +++++++++++++++++++++++++
 test/Optimizer/test147.js                | 19 ++++++++++
 test/es6/bug_OS14562349.js               | 24 ++++++++++++
 test/es6/rlexe.xml                       |  7 ++++
 21 files changed, 293 insertions(+), 78 deletions(-)
 create mode 100644 test/Optimizer/test146.js
 create mode 100644 test/Optimizer/test147.js
 create mode 100644 test/es6/bug_OS14562349.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_F1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```