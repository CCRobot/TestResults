```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  10.8M      0  0:00:01  0:00:01 --:--:-- 10.8M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  7  120M    7 9312k    0     0  8115k      0  0:00:15  0:00:01  0:00:14 8111k 15  120M   15 19.0M    0     0  9086k      0  0:00:13  0:00:02  0:00:11 9083k 24  120M   24 29.1M    0     0  9473k      0  0:00:12  0:00:03  0:00:09 9470k 34  120M   34 41.1M    0     0   9.9M      0  0:00:12  0:00:04  0:00:08  9.9M 44  120M   44 52.8M    0     0  10.2M      0  0:00:11  0:00:05  0:00:06 10.6M 52  120M   52 62.7M    0     0  10.2M      0  0:00:11  0:00:06  0:00:05 10.7M 60  120M   60 72.9M    0     0  10.2M      0  0:00:11  0:00:07  0:00:04 10.7M 67  120M   67 81.6M    0     0  10.0M      0  0:00:11  0:00:08  0:00:03 10.5M 76  120M   76 91.9M    0     0  10.0M      0  0:00:11  0:00:09  0:00:02 10.1M 84  120M   84  101M    0     0   9.9M      0  0:00:12  0:00:10  0:00:02 9928k 91  120M   91  110M    0     0   9.9M      0  0:00:12  0:00:11  0:00:01 9753k100  120M  100  120M    0     0  10.1M      0  0:00:11  0:00:11 --:--:-- 10.0M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   39f7ce4..6ff574b  master      -> origin/master
   3e73938..0903451  release/1.7 -> origin/release/1.7
   fac40c6..11cdbc5  release/1.8 -> origin/release/1.8
Updating 39f7ce4..6ff574b
Fast-forward
 bin/ch/262.js                             |  10 +-
 bin/ch/HostConfigFlagsList.h              |   2 +-
 bin/ch/RuntimeThreadData.cpp              |  17 -
 bin/ch/WScriptJsrt.cpp                    |  21 +-
 lib/Common/Warnings.h                     |   4 +
 pal/src/CMakeLists.txt                    |   1 +
 pal/src/include/pal/semaphore.hpp         |  60 +++
 pal/src/synchobj/semaphore.cpp            | 604 ++++++++++++++++++++++++++++++
 test/$262/rlexe.xml                       |  10 -
 test/{$262/$262test.js => 262/262test.js} |  36 +-
 test/262/rlexe.xml                        |   9 +
 test/rlexedirs.xml                        |   2 +-
 12 files changed, 716 insertions(+), 60 deletions(-)
 create mode 100644 pal/src/include/pal/semaphore.hpp
 create mode 100644 pal/src/synchobj/semaphore.cpp
 delete mode 100644 test/$262/rlexe.xml
 rename test/{$262/$262test.js => 262/262test.js} (83%)
 create mode 100644 test/262/rlexe.xml
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```