```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 79 11.1M   79 9104k    0     0  9563k      0  0:00:01 --:--:--  0:00:01 9563k100 11.1M  100 11.1M    0     0   9.9M      0  0:00:01  0:00:01 --:--:--  9.9M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  129M    5 7472k    0     0  9151k      0  0:00:14 --:--:--  0:00:14 9145k 13  129M   13 18.0M    0     0   9.9M      0  0:00:12  0:00:01  0:00:11  9.9M 22  129M   22 29.7M    0     0  10.5M      0  0:00:12  0:00:02  0:00:10 10.5M 31  129M   31 40.5M    0     0  10.6M      0  0:00:12  0:00:03  0:00:09 10.6M 36  129M   36 47.1M    0     0   9.7M      0  0:00:13  0:00:04  0:00:09  9.7M 43  129M   43 55.9M    0     0  9841k      0  0:00:13  0:00:05  0:00:08 9955k 53  129M   53 68.7M    0     0  10.0M      0  0:00:12  0:00:06  0:00:06 10.1M 61  129M   61 80.0M    0     0  10.2M      0  0:00:12  0:00:07  0:00:05 10.0M 70  129M   70 91.3M    0     0  10.3M      0  0:00:12  0:00:08  0:00:04 10.1M 78  129M   78  101M    0     0  10.3M      0  0:00:12  0:00:09  0:00:03 10.9M 86  129M   86  112M    0     0  10.3M      0  0:00:12  0:00:10  0:00:02 11.2M 95  129M   95  122M    0     0  10.3M      0  0:00:12  0:00:11  0:00:01 10.8M100  129M  100  129M    0     0  10.4M      0  0:00:12  0:00:12 --:--:-- 10.9M
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
] Testing  RLS18_TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```