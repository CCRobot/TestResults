```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 61 11.1M   61 6976k    0     0  4989k      0  0:00:02  0:00:01  0:00:01 4989k100 11.1M  100 11.1M    0     0  5784k      0  0:00:01  0:00:01 --:--:-- 5783k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  8  132M    8 10.8M    0     0  9632k      0  0:00:14  0:00:01  0:00:13 9630k 14  132M   14 18.8M    0     0  8962k      0  0:00:15  0:00:02  0:00:13 8961k 18  132M   18 24.7M    0     0  8033k      0  0:00:16  0:00:03  0:00:13 8032k 25  132M   25 34.0M    0     0  8393k      0  0:00:16  0:00:04  0:00:12 8392k 32  132M   32 42.4M    0     0  8440k      0  0:00:16  0:00:05  0:00:11 8788k 41  132M   41 55.2M    0     0  9200k      0  0:00:14  0:00:06  0:00:08 9102k 49  132M   49 64.8M    0     0  9280k      0  0:00:14  0:00:07  0:00:07 9417k 56  132M   56 74.7M    0     0  9378k      0  0:00:14  0:00:08  0:00:06  9.9M 63  132M   63 84.2M    0     0  9420k      0  0:00:14  0:00:09  0:00:05 10.0M 69  132M   69 91.9M    0     0  9202k      0  0:00:14  0:00:10  0:00:04 9975k 74  132M   74 98.9M    0     0  9083k      0  0:00:14  0:00:11  0:00:03 8940k 81  132M   81  108M    0     0  9130k      0  0:00:14  0:00:12  0:00:02 8915k 88  132M   88  117M    0     0  8977k      0  0:00:15  0:00:13  0:00:02 8346k 93  132M   93  124M    0     0  8980k      0  0:00:15  0:00:14  0:00:01 8177k100  132M  100  132M    0     0  9023k      0  0:00:15  0:00:15 --:--:-- 8641k
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
] Testing  RL18_PACK
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```