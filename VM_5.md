```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 14 11.1M   14 1631k    0     0  5285k      0  0:00:02 --:--:--  0:00:02 5280k 60 11.1M   60 6832k    0     0  5221k      0  0:00:02  0:00:01  0:00:01 5219k100 11.1M  100 11.1M    0     0  6634k      0  0:00:01  0:00:01 --:--:-- 6632k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  155M    3 6240k    0     0  10.5M      0  0:00:14 --:--:--  0:00:14 10.5M  6  155M    6 10.6M    0     0  6893k      0  0:00:23  0:00:01  0:00:22 6891k 11  155M   11 18.2M    0     0  7266k      0  0:00:21  0:00:02  0:00:19 7264k 17  155M   17 26.9M    0     0  7505k      0  0:00:21  0:00:03  0:00:18 7505k 25  155M   25 38.9M    0     0  8714k      0  0:00:18  0:00:04  0:00:14 8714k 34  155M   34 53.3M    0     0  9798k      0  0:00:16  0:00:05  0:00:11 9685k 43  155M   43 67.9M    0     0  10.3M      0  0:00:15  0:00:06  0:00:09 11.4M 52  155M   52 80.8M    0     0  10.6M      0  0:00:14  0:00:07  0:00:07 12.5M 59  155M   59 92.6M    0     0  10.8M      0  0:00:14  0:00:08  0:00:06 13.3M 67  155M   67  104M    0     0  10.9M      0  0:00:14  0:00:09  0:00:05 13.1M 77  155M   77  119M    0     0  11.3M      0  0:00:13  0:00:10  0:00:03 13.2M 86  155M   86  134M    0     0  11.5M      0  0:00:13  0:00:11  0:00:02 13.2M 92  155M   92  143M    0     0  11.4M      0  0:00:13  0:00:12  0:00:01 12.5M100  155M  100  155M    0     0  11.5M      0  0:00:13  0:00:13 --:--:-- 12.8M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   54caa27..7662f64  master      -> origin/master
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
] Testing  DEBUG_FLG2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```