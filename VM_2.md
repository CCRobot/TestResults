```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 17 11.1M   17 2015k    0     0  5273k      0  0:00:02 --:--:--  0:00:02 5262k100 11.1M  100 11.1M    0     0  9881k      0  0:00:01  0:00:01 --:--:-- 9888k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  129M    0 65113    0     0   285k      0  0:07:43 --:--:--  0:07:43  285k  9  129M    9 12.7M    0     0  10.4M      0  0:00:12  0:00:01  0:00:11 10.4M 19  129M   19 25.7M    0     0  11.5M      0  0:00:11  0:00:02  0:00:09 11.5M 30  129M   30 39.9M    0     0  12.4M      0  0:00:10  0:00:03  0:00:07 12.4M 42  129M   42 54.5M    0     0  12.9M      0  0:00:09  0:00:04  0:00:05 12.9M 52  129M   52 68.0M    0     0  12.9M      0  0:00:09  0:00:05  0:00:04 13.5M 61  129M   61 79.6M    0     0  12.7M      0  0:00:10  0:00:06  0:00:04 13.3M 71  129M   71 92.5M    0     0  12.8M      0  0:00:10  0:00:07  0:00:03 13.3M 82  129M   82  106M    0     0  12.9M      0  0:00:09  0:00:08  0:00:01 13.3M 92  129M   92  119M    0     0  12.9M      0  0:00:09  0:00:09 --:--:-- 13.0M100  129M  100  129M    0     0  13.1M      0  0:00:09  0:00:09 --:--:-- 13.2M
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
] Testing  RL18_PACK
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```