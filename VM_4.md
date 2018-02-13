```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  11.4M      0 --:--:-- --:--:-- --:--:-- 11.4M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 10  155M   10 16.0M    0     0  13.8M      0  0:00:11  0:00:01  0:00:10 13.8M 17  155M   17 27.8M    0     0  12.9M      0  0:00:12  0:00:02  0:00:10 12.9M 27  155M   27 42.4M    0     0  13.4M      0  0:00:11  0:00:03  0:00:08 13.4M 37  155M   37 57.7M    0     0  13.9M      0  0:00:11  0:00:04  0:00:07 13.9M 46  155M   46 72.0M    0     0  13.9M      0  0:00:11  0:00:05  0:00:06 14.4M 54  155M   54 84.7M    0     0  13.7M      0  0:00:11  0:00:06  0:00:05 13.7M 61  155M   61 95.9M    0     0  13.4M      0  0:00:11  0:00:07  0:00:04 13.6M 69  155M   69  107M    0     0  13.1M      0  0:00:11  0:00:08  0:00:03 12.9M 80  155M   80  124M    0     0  13.5M      0  0:00:11  0:00:09  0:00:02 13.3M 89  155M   89  139M    0     0  13.7M      0  0:00:11  0:00:10  0:00:01 13.4M 98  155M   98  153M    0     0  13.7M      0  0:00:11  0:00:11 --:--:-- 13.7M100  155M  100  155M    0     0  13.7M      0  0:00:11  0:00:11 --:--:-- 14.4M
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
] Testing  NODE_BUILD_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```