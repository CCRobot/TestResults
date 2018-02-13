```
Executed on ubu16chk400001N
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  8966k      0  0:00:01  0:00:01 --:--:-- 8974k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  155M    0 32345    0     0  93750      0  0:28:55 --:--:--  0:28:55 93753 14  155M   14 22.1M    0     0  16.3M      0  0:00:09  0:00:01  0:00:08 16.3M 38  155M   38 60.0M    0     0  25.5M      0  0:00:06  0:00:02  0:00:04 25.5M 64  155M   64  100M    0     0  29.6M      0  0:00:05  0:00:03  0:00:02 29.6M 87  155M   87  136M    0     0  31.3M      0  0:00:04  0:00:04 --:--:-- 31.3M100  155M  100  155M    0     0  32.7M      0  0:00:04  0:00:04 --:--:-- 35.2M
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
] Testing  DEBUG_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```