```
Executed on ubu16chk4000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  11.6M      0 --:--:-- --:--:-- --:--:-- 11.7M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 18  129M   18 24.0M    0     0  20.0M      0  0:00:06  0:00:01  0:00:05 20.0M 43  129M   43 56.0M    0     0  25.9M      0  0:00:04  0:00:02  0:00:02 25.9M 69  129M   69 90.2M    0     0  28.5M      0  0:00:04  0:00:03  0:00:01 28.5M 95  129M   95  123M    0     0  29.7M      0  0:00:04  0:00:04 --:--:-- 29.7M100  129M  100  129M    0     0  29.9M      0  0:00:04  0:00:04 --:--:-- 31.3M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c27adba..08cf55d  master     -> origin/master
   3e68e46..c0c7999  release/1.8 -> origin/release/1.8
Updating c27adba..08cf55d
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
 lib/Runtime/ByteCode/ByteCodeEmitter.cpp | 18 +++++++--
 test/Optimizer/capturedValuesBugs.js     | 29 ++++++++++++++
 test/Optimizer/rlexe.xml                 | 12 ++++++
 test/Optimizer/test146.js                | 52 +++++++++++++++++++++++++
 test/Optimizer/test147.js                | 19 ++++++++++
 test/es6/bug_OS14562349.js               | 24 ++++++++++++
 test/es6/rlexe.xml                       |  7 ++++
 20 files changed, 290 insertions(+), 78 deletions(-)
 create mode 100644 test/Optimizer/test146.js
 create mode 100644 test/Optimizer/test147.js
 create mode 100644 test/es6/bug_OS14562349.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```