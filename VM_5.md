```
Executed on w1604chak000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  12.3M      0 --:--:-- --:--:-- --:--:-- 12.3M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 13  120M   13 16.0M    0     0  14.9M      0  0:00:08  0:00:01  0:00:07 14.9M 43  120M   43 52.0M    0     0  25.3M      0  0:00:04  0:00:02  0:00:02 25.2M 73  120M   73 88.0M    0     0  28.5M      0  0:00:04  0:00:03  0:00:01 28.5M 91  120M   91  109M    0     0  27.1M      0  0:00:04  0:00:04 --:--:-- 27.1M100  120M  100  120M    0     0  27.0M      0  0:00:04  0:00:04 --:--:-- 27.5M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   39f7ce4..328ffa4  master     -> origin/master
   3e73938..c6d73ba  release/1.7 -> origin/release/1.7
   fac40c6..e2b3d45  release/1.8 -> origin/release/1.8
Updating 39f7ce4..328ffa4
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
] Testing  TEST_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```