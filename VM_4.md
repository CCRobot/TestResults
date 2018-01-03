```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 82 11.1M   82 9408k    0     0  8889k      0  0:00:01  0:00:01 --:--:-- 8883k100 11.1M  100 11.1M    0     0  9299k      0  0:00:01  0:00:01 --:--:-- 9298k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  120M    6 8272k    0     0   9.8M      0  0:00:12 --:--:--  0:00:12  9.8M 17  120M   17 21.2M    0     0  11.6M      0  0:00:10  0:00:01  0:00:09 11.6M 27  120M   27 32.4M    0     0  11.4M      0  0:00:10  0:00:02  0:00:08 11.4M 35  120M   35 42.3M    0     0  11.0M      0  0:00:10  0:00:03  0:00:07 11.0M 44  120M   44 54.0M    0     0  11.2M      0  0:00:10  0:00:04  0:00:06 11.1M 56  120M   56 68.4M    0     0  11.7M      0  0:00:10  0:00:05  0:00:05 12.0M 65  120M   65 78.2M    0     0  11.4M      0  0:00:10  0:00:06  0:00:04 11.4M 75  120M   75 90.2M    0     0  11.5M      0  0:00:10  0:00:07  0:00:03 11.5M 82  120M   82 98.5M    0     0  11.1M      0  0:00:10  0:00:08  0:00:02 11.2M 91  120M   91  109M    0     0  11.1M      0  0:00:10  0:00:09  0:00:01 11.1M 98  120M   98  118M    0     0  10.9M      0  0:00:10  0:00:10 --:--:-- 10.0M100  120M  100  120M    0     0  10.8M      0  0:00:11  0:00:11 --:--:--  9.8M
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
] Testing  RL18_DBG_F2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```