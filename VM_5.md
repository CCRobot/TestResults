```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 70 11.1M   70 7984k    0     0  5956k      0  0:00:01  0:00:01 --:--:-- 5953k100 11.1M  100 11.1M    0     0  6432k      0  0:00:01  0:00:01 --:--:-- 6430k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  129M    3 4592k    0     0  5955k      0  0:00:22 --:--:--  0:00:22 5948k 10  129M   10 14.2M    0     0  8202k      0  0:00:16  0:00:01  0:00:15 8198k 18  129M   18 23.2M    0     0  8617k      0  0:00:15  0:00:02  0:00:13 8615k 25  129M   25 32.8M    0     0  8935k      0  0:00:14  0:00:03  0:00:11 8933k 34  129M   34 44.3M    0     0  9513k      0  0:00:13  0:00:04  0:00:09 9512k 44  129M   44 56.8M    0     0   9.8M      0  0:00:13  0:00:05  0:00:08 10.4M 50  129M   50 65.7M    0     0  9947k      0  0:00:13  0:00:06  0:00:07 10.3M 58  129M   58 75.9M    0     0   9.7M      0  0:00:13  0:00:07  0:00:06 10.5M 63  129M   63 82.1M    0     0  9589k      0  0:00:13  0:00:08  0:00:05  9.8M 68  129M   68 88.0M    0     0  9158k      0  0:00:14  0:00:09  0:00:05 8826k 72  129M   72 93.3M    0     0  8873k      0  0:00:14  0:00:10  0:00:04 7462k 77  129M   77  100M    0     0  8709k      0  0:00:15  0:00:11  0:00:04 7033k 82  129M   82  106M    0     0  8559k      0  0:00:15  0:00:12  0:00:03 6307k 89  129M   89  115M    0     0  8588k      0  0:00:15  0:00:13  0:00:02 6831k 96  129M   96  124M    0     0  8638k      0  0:00:15  0:00:14  0:00:01 7598k100  129M  100  129M    0     0  8600k      0  0:00:15  0:00:15 --:--:-- 7964k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c27adba..45cd410  master      -> origin/master
   745ddf8..148c8af  intl-icu    -> origin/intl-icu
   cf780ac..e20d5c6  release/1.7 -> origin/release/1.7
   3e68e46..6b6a96b  release/1.8 -> origin/release/1.8
Updating c27adba..45cd410
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
 lib/Runtime/ByteCode/ByteCodeGenerator.cpp         |   2 +-
 lib/Runtime/Debug/TTEventLog.cpp                   |   3 +-
 lib/Runtime/Debug/TTRuntmeInfoTracker.cpp          |   1 +
 lib/Runtime/Debug/TTSerializeEnum.h                |   4 +
 lib/Runtime/Debug/TTSnapObjects.cpp                | 189 +++++++++++++++---
 lib/Runtime/Debug/TTSnapObjects.h                  |  37 +++-
 lib/Runtime/Debug/TTSnapshot.cpp                   |  17 +-
 lib/Runtime/Debug/TTSupport.h                      |   2 +
 lib/Runtime/Language/JavascriptOperators.cpp       |   2 +-
 lib/Runtime/Library/JavascriptExternalFunction.cpp |  23 ++-
 lib/Runtime/Library/JavascriptExternalFunction.h   |  11 +-
 lib/Runtime/Library/JavascriptGenerator.cpp        |  18 +-
 .../Library/JavascriptGeneratorFunction.cpp        |  62 +++++-
 lib/Runtime/Library/JavascriptGeneratorFunction.h  |   2 +
 lib/Runtime/Library/JavascriptLibrary.cpp          |  10 +-
 lib/Runtime/Library/JavascriptLibrary.h            |   3 +-
 lib/Runtime/Library/JavascriptPromise.cpp          | 113 ++++++++++-
 pal/src/map/virtual.cpp                            |   7 +-
 pal/src/memory/heap.cpp                            |   8 +-
 test/Bugs/rlexe.xml                                |   7 +-
 test/Optimizer/capturedValuesBugs.js               |  29 +++
 test/Optimizer/rlexe.xml                           |  12 ++
 test/Optimizer/test146.js                          |  52 +++++
 test/Optimizer/test147.js                          |  19 ++
 test/TTBasic/asyncAwaitBasic.js                    |  75 ++++++++
 test/TTBasic/asyncAwaitBasicRecord.baseline        |   5 +
 test/TTBasic/asyncAwaitBasicReplay_1.baseline      |   7 +
 test/TTBasic/asyncAwaitBasicReplay_2.baseline      |   7 +
 test/TTBasic/asyncAwaitBasicReplay_3.baseline      |   4 +
 test/TTBasic/asyncAwaitBasicReplay_4.baseline      |   4 +
 test/TTBasic/asyncAwaitBasicReplay_5.baseline      |   3 +
 test/TTBasic/rlexe.xml                             |  51 ++++-
 test/es6/bug_OS14562349.js                         |  24 +++
 test/es6/rlexe.xml                                 |   7 +
 tools/compile_clang.sh                             |  34 +++-
 55 files changed, 1238 insertions(+), 185 deletions(-)
 create mode 100644 test/Optimizer/test146.js
 create mode 100644 test/Optimizer/test147.js
 create mode 100644 test/TTBasic/asyncAwaitBasic.js
 create mode 100644 test/TTBasic/asyncAwaitBasicRecord.baseline
 create mode 100644 test/TTBasic/asyncAwaitBasicReplay_1.baseline
 create mode 100644 test/TTBasic/asyncAwaitBasicReplay_2.baseline
 create mode 100644 test/TTBasic/asyncAwaitBasicReplay_3.baseline
 create mode 100644 test/TTBasic/asyncAwaitBasicReplay_4.baseline
 create mode 100644 test/TTBasic/asyncAwaitBasicReplay_5.baseline
 create mode 100644 test/es6/bug_OS14562349.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_FLG2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```