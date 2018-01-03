```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 62 11.1M   62 7088k    0     0  8494k      0  0:00:01 --:--:--  0:00:01 8488k100 11.1M  100 11.1M    0     0  10.0M      0  0:00:01  0:00:01 --:--:-- 10.0M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  120M    5 7152k    0     0   9.8M      0  0:00:12 --:--:--  0:00:12  9.8M 18  120M   18 22.5M    0     0  13.1M      0  0:00:09  0:00:01  0:00:08 13.1M 30  120M   30 36.3M    0     0  13.3M      0  0:00:08  0:00:02  0:00:06 13.3M 42  120M   42 51.0M    0     0  13.7M      0  0:00:08  0:00:03  0:00:05 13.7M 53  120M   53 64.6M    0     0  13.7M      0  0:00:08  0:00:04  0:00:04 13.7M 67  120M   67 81.6M    0     0  14.2M      0  0:00:08  0:00:05  0:00:03 14.9M 79  120M   79 95.7M    0     0  14.2M      0  0:00:08  0:00:06  0:00:02 14.6M 90  120M   90  108M    0     0  14.0M      0  0:00:08  0:00:07  0:00:01 14.4M100  120M  100  120M    0     0  14.1M      0  0:00:08  0:00:08 --:--:-- 14.4M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   39f7ce4..6ff574b  master      -> origin/master
   3e73938..c6d73ba  release/1.7 -> origin/release/1.7
   fac40c6..e2b3d45  release/1.8 -> origin/release/1.8
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
] Testing  DEBUG_FLG2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```