```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5 11.1M    5  575k    0     0  2081k      0  0:00:05 --:--:--  0:00:05 2077k100 11.1M  100 11.1M    0     0  11.2M      0 --:--:-- --:--:-- --:--:-- 11.2M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  155M    0  783k    0     0  2882k      0  0:00:55 --:--:--  0:00:55 2880k 10  155M   10 15.8M    0     0  12.4M      0  0:00:12  0:00:01  0:00:11 12.4M 19  155M   19 29.5M    0     0  13.0M      0  0:00:11  0:00:02  0:00:09 13.0M 29  155M   29 46.4M    0     0  14.1M      0  0:00:10  0:00:03  0:00:07 14.1M 40  155M   40 62.8M    0     0  14.7M      0  0:00:10  0:00:04  0:00:06 14.7M 49  155M   49 77.1M    0     0  14.6M      0  0:00:10  0:00:05  0:00:05 15.2M 59  155M   59 92.3M    0     0  14.7M      0  0:00:10  0:00:06  0:00:04 15.3M 71  155M   71  110M    0     0  15.2M      0  0:00:10  0:00:07  0:00:03 16.2M 81  155M   81  126M    0     0  15.2M      0  0:00:10  0:00:08  0:00:02 15.9M 89  155M   89  138M    0     0  14.9M      0  0:00:10  0:00:09  0:00:01 15.1M 96  155M   96  150M    0     0  14.6M      0  0:00:10  0:00:10 --:--:-- 14.6M100  155M  100  155M    0     0  14.7M      0  0:00:10  0:00:10 --:--:-- 14.7M
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
] Testing  DEBUG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```