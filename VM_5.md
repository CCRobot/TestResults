```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 35 11.1M   35 4063k    0     0  7215k      0  0:00:01 --:--:--  0:00:01 7204k100 11.1M  100 11.1M    0     0  10.2M      0  0:00:01  0:00:01 --:--:-- 10.2M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  155M    1 2655k    0     0  5828k      0  0:00:27 --:--:--  0:00:27 5823k  8  155M    8 13.6M    0     0  9620k      0  0:00:16  0:00:01  0:00:15 9619k 14  155M   14 22.8M    0     0  9529k      0  0:00:16  0:00:02  0:00:14 9528k 20  155M   20 32.1M    0     0  9541k      0  0:00:16  0:00:03  0:00:13 9539k 27  155M   27 43.2M    0     0  9944k      0  0:00:15  0:00:04  0:00:11 9942k 33  155M   33 52.6M    0     0  9880k      0  0:00:16  0:00:05  0:00:11 10.0M 39  155M   39 61.7M    0     0  9800k      0  0:00:16  0:00:06  0:00:10 9852k 47  155M   47 73.1M    0     0   9.8M      0  0:00:15  0:00:07  0:00:08 10.0M 56  155M   56 88.0M    0     0  10.3M      0  0:00:14  0:00:08  0:00:06 11.1M 65  155M   65  101M    0     0  10.7M      0  0:00:14  0:00:09  0:00:05 11.6M 74  155M   74  115M    0     0  11.0M      0  0:00:14  0:00:10  0:00:04 12.4M 83  155M   83  129M    0     0  11.3M      0  0:00:13  0:00:11  0:00:02 13.5M 92  155M   92  143M    0     0  11.5M      0  0:00:13  0:00:12  0:00:01 14.1M100  155M  100  155M    0     0  11.8M      0  0:00:13  0:00:13 --:--:-- 14.4M
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
] Testing  DEBUG_FLG1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```