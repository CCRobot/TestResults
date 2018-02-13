```
Executed on ubu16chk400001M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 49 9180k   49 4576k    0     0  4708k      0  0:00:01 --:--:--  0:00:01 4707k100 9180k  100 9180k    0     0  8266k      0  0:00:01  0:00:01 --:--:-- 8271k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  155M    2 4096k    0     0  4829k      0  0:00:32 --:--:--  0:00:32 4824k 28  155M   28 44.0M    0     0  23.1M      0  0:00:06  0:00:01  0:00:05 23.1M 54  155M   54 84.0M    0     0  29.1M      0  0:00:05  0:00:02  0:00:03 29.1M 81  155M   81  126M    0     0  32.8M      0  0:00:04  0:00:03  0:00:01 32.8M100  155M  100  155M    0     0  34.3M      0  0:00:04  0:00:04 --:--:-- 34.3M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   54caa27..7662f64  master     -> origin/master
   249b434..ee5ffb3  release/1.8 -> origin/release/1.8
   782cd43..db6afe6  release/1.9 -> origin/release/1.9
Updating 54caa27..7662f64
Fast-forward
 bin/ChakraCore/ChakraCore.def              |   2 +
 bin/ch/ChakraRtInterface.cpp               |   1 +
 bin/ch/ChakraRtInterface.h                 |   3 +
 bin/ch/HostConfigFlagsList.h               |   1 +
 bin/ch/WScriptJsrt.cpp                     |  29 ++++++
 bin/ch/WScriptJsrt.h                       |   1 +
 bin/ch/ch.cpp                              |   5 +
 lib/Jsrt/ChakraCore.h                      |  43 +++++++++
 lib/Jsrt/Jsrt.cpp                          |   9 ++
 lib/Runtime/ByteCode/ByteCodeEmitter.cpp   |  15 ++-
 lib/Runtime/Library/JavascriptLibrary.cpp  |  26 ++++++
 lib/Runtime/Library/JavascriptLibrary.h    |   6 ++
 lib/Runtime/Library/JavascriptPromise.cpp  |  11 +++
 lib/Runtime/Library/JavascriptPromise.h    |   3 +
 test/es6/ES6Super.js                       |  79 ++++++++++++++++
 test/es7/PromiseRejectionTracking.baseline |  43 +++++++++
 test/es7/PromiseRejectionTracking.js       | 145 +++++++++++++++++++++++++++++
 test/es7/rlexe.xml                         |   8 ++
 test/runtests.py                           |  17 +++-
 test/wasm/rlexe.xml                        |   4 +-
 20 files changed, 441 insertions(+), 10 deletions(-)
 create mode 100644 test/es7/PromiseRejectionTracking.baseline
 create mode 100644 test/es7/PromiseRejectionTracking.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_FLG1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```