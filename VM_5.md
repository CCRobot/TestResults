```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 30 11.1M   30 3455k    0     0  4628k      0  0:00:02 --:--:--  0:00:02 4625k 92 11.1M   92 10.2M    0     0  6019k      0  0:00:01  0:00:01 --:--:-- 6017k100 11.1M  100 11.1M    0     0  5694k      0  0:00:01  0:00:01 --:--:-- 5693k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  129M    2 2911k    0     0  4012k      0  0:00:32 --:--:--  0:00:32 4010k  6  129M    6 8416k    0     0  4872k      0  0:00:27  0:00:01  0:00:26 4870k  9  129M    9 12.5M    0     0  4715k      0  0:00:28  0:00:02  0:00:26 4715k 17  129M   17 22.7M    0     0  6235k      0  0:00:21  0:00:03  0:00:18 6234k 22  129M   22 29.6M    0     0  6427k      0  0:00:20  0:00:04  0:00:16 6426k 28  129M   28 36.8M    0     0  6593k      0  0:00:20  0:00:05  0:00:15 6967k 32  129M   32 41.5M    0     0  6322k      0  0:00:20  0:00:06  0:00:14 6822k 35  129M   35 45.3M    0     0  6012k      0  0:00:21  0:00:07  0:00:14 6720k 40  129M   40 52.0M    0     0  6096k      0  0:00:21  0:00:08  0:00:13 5992k 50  129M   50 64.8M    0     0  6829k      0  0:00:19  0:00:09  0:00:10 7209k 61  129M   61 79.7M    0     0  7613k      0  0:00:17  0:00:10  0:00:07 8782k 72  129M   72 93.5M    0     0  8164k      0  0:00:16  0:00:11  0:00:05 10.3M 83  129M   83  108M    0     0  8684k      0  0:00:15  0:00:12  0:00:03 12.5M 94  129M   94  122M    0     0  9150k      0  0:00:14  0:00:13  0:00:01 14.1M100  129M  100  129M    0     0  9350k      0  0:00:14  0:00:14 --:--:-- 14.5M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c27adba..5ba7663  master      -> origin/master
   745ddf8..148c8af  intl-icu    -> origin/intl-icu
   3e68e46..0ce001c  release/1.8 -> origin/release/1.8
Updating c27adba..5ba7663
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
 pal/src/map/virtual.cpp                            |   7 +-
 pal/src/memory/heap.cpp                            |   8 +-
 test/Bugs/rlexe.xml                                |   7 +-
 test/Optimizer/capturedValuesBugs.js               |  29 +++
 test/Optimizer/rlexe.xml                           |  12 ++
 test/Optimizer/test146.js                          |  52 +++++
 test/Optimizer/test147.js                          |  19 ++
 test/es6/bug_OS14562349.js                         |  24 +++
 test/es6/rlexe.xml                                 |   7 +
 33 files changed, 649 insertions(+), 122 deletions(-)
 create mode 100644 test/Optimizer/test146.js
 create mode 100644 test/Optimizer/test147.js
 create mode 100644 test/es6/bug_OS14562349.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```