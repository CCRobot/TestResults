```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 24 11.1M   24 2751k    0     0  6647k      0  0:00:01 --:--:--  0:00:01 6646k100 11.1M  100 11.1M    0     0  10.1M      0  0:00:01  0:00:01 --:--:-- 10.1M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  129M    0 15961    0     0  52625      0  0:42:53 --:--:--  0:42:53 52503 10  129M   10 13.8M    0     0  10.6M      0  0:00:12  0:00:01  0:00:11 10.6M 22  129M   22 29.1M    0     0  12.6M      0  0:00:10  0:00:02  0:00:08 12.6M 32  129M   32 41.4M    0     0  12.5M      0  0:00:10  0:00:03  0:00:07 12.5M 41  129M   41 53.7M    0     0  12.4M      0  0:00:10  0:00:04  0:00:06 12.4M 51  129M   51 66.8M    0     0  12.6M      0  0:00:10  0:00:05  0:00:05 13.3M 60  129M   60 78.5M    0     0  12.4M      0  0:00:10  0:00:06  0:00:04 12.9M 70  129M   70 91.3M    0     0  12.5M      0  0:00:10  0:00:07  0:00:03 12.4M 79  129M   79  102M    0     0  12.4M      0  0:00:10  0:00:08  0:00:02 12.3M 88  129M   88  114M    0     0  12.2M      0  0:00:10  0:00:09  0:00:01 12.0M 99  129M   99  128M    0     0  12.4M      0  0:00:10  0:00:10 --:--:-- 12.2M100  129M  100  129M    0     0  12.4M      0  0:00:10  0:00:10 --:--:-- 12.3M
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
] Testing  RL18_DBG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```