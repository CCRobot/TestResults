```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 10 11.1M   10 1199k    0     0  3932k      0  0:00:02 --:--:--  0:00:02 3933k 72 11.1M   72 8208k    0     0  6271k      0  0:00:01  0:00:01 --:--:-- 6270k100 11.1M  100 11.1M    0     0  6563k      0  0:00:01  0:00:01 --:--:-- 6563k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  132M    1 2671k    0     0  3599k      0  0:00:37 --:--:--  0:00:37 3595k  5  132M    5 8096k    0     0  5219k      0  0:00:25  0:00:01  0:00:24 5216k 11  132M   11 15.1M    0     0  6089k      0  0:00:22  0:00:02  0:00:20 6087k 17  132M   17 23.7M    0     0  6839k      0  0:00:19  0:00:03  0:00:16 6837k 24  132M   24 32.7M    0     0  7365k      0  0:00:18  0:00:04  0:00:14 7365k 31  132M   31 41.9M    0     0  7744k      0  0:00:17  0:00:05  0:00:12 8382k 40  132M   40 53.2M    0     0  8316k      0  0:00:16  0:00:06  0:00:10 9277k 46  132M   46 61.8M    0     0  8258k      0  0:00:16  0:00:07  0:00:09 9340k 51  132M   51 67.7M    0     0  8108k      0  0:00:16  0:00:08  0:00:08 9008k 60  132M   60 79.3M    0     0  8509k      0  0:00:15  0:00:09  0:00:06 9550k 65  132M   65 86.4M    0     0  8327k      0  0:00:16  0:00:10  0:00:06 8963k 71  132M   71 94.7M    0     0  8400k      0  0:00:16  0:00:11  0:00:05 8508k 78  132M   78  103M    0     0  8428k      0  0:00:16  0:00:12  0:00:04 8694k 85  132M   85  113M    0     0  8581k      0  0:00:15  0:00:13  0:00:02 9391k 93  132M   93  123M    0     0  8662k      0  0:00:15  0:00:14  0:00:01 8953k100  132M  100  132M    0     0  8754k      0  0:00:15  0:00:15 --:--:-- 9694k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c6ae741..f0edaf7  master      -> origin/master
   b0a2395..75c64b4  release/1.8 -> origin/release/1.8
   c6ae741..98e7835  release/1.9 -> origin/release/1.9
Updating c6ae741..f0edaf7
Fast-forward
 bin/NativeTests/JsRTApiTest.cpp                 |  41 +++++
 lib/Backend/Lower.cpp                           |  23 ++-
 lib/Backend/LowerMDShared.cpp                   |   7 +-
 lib/Backend/LowerMDShared.h                     |   3 +-
 lib/Backend/amd64/LowererMDArch.cpp             | 102 ++++++++++++
 lib/Backend/amd64/LowererMDArch.h               |   3 +-
 lib/Backend/arm/LowerMD.cpp                     |   7 +-
 lib/Backend/arm/LowerMD.h                       |   1 +
 lib/Backend/arm64/LowerMD.cpp                   |   6 +-
 lib/Backend/arm64/LowerMD.h                     |   1 +
 lib/Backend/i386/LowererMDArch.cpp              |   5 +
 lib/Backend/i386/LowererMDArch.h                |   3 +-
 lib/Common/Common/NumberUtilities.h             |  56 +++++++
 lib/Jsrt/Core/JsrtCore.cpp                      |   6 +-
 lib/Runtime/Language/SourceTextModuleRecord.cpp |   1 -
 lib/Runtime/Library/JavascriptArray.inl         |  12 +-
 test/AsmJs/divByConstants.baseline              |   2 +
 test/AsmJs/divByConstants.js                    | 180 +++++++++++++++++++++
 test/AsmJs/rlexe.xml                            |   7 +
 test/wasm/divByConstants.js                     | 198 ++++++++++++++++++++++++
 test/wasm/rlexe.xml                             |   7 +
 21 files changed, 648 insertions(+), 23 deletions(-)
 create mode 100644 test/AsmJs/divByConstants.baseline
 create mode 100644 test/AsmJs/divByConstants.js
 create mode 100644 test/wasm/divByConstants.js
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