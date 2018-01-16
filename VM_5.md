```
Executed on ubu16chk4000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  12.8M      0 --:--:-- --:--:-- --:--:-- 12.9M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 15  132M   15 20.0M    0     0  15.7M      0  0:00:08  0:00:01  0:00:07 15.7M 42  132M   42 56.0M    0     0  24.1M      0  0:00:05  0:00:02  0:00:03 24.1M 68  132M   68 91.0M    0     0  27.9M      0  0:00:04  0:00:03  0:00:01 27.9M 94  132M   94  125M    0     0  29.4M      0  0:00:04  0:00:04 --:--:-- 29.4M100  132M  100  132M    0     0  30.0M      0  0:00:04  0:00:04 --:--:-- 32.5M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c6ae741..4bc99f6  master     -> origin/master
   b0a2395..eb19165  release/1.8 -> origin/release/1.8
   c6ae741..12a738b  release/1.9 -> origin/release/1.9
Updating c6ae741..4bc99f6
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
 test/wasm/rlexe.xml                             |   6 +
 21 files changed, 647 insertions(+), 23 deletions(-)
 create mode 100644 test/AsmJs/divByConstants.baseline
 create mode 100644 test/AsmJs/divByConstants.js
 create mode 100644 test/wasm/divByConstants.js
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