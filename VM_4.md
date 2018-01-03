```
Executed on w1604chak000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 89 9180k   89 8208k    0     0  10.8M      0 --:--:-- --:--:-- --:--:-- 10.8M100 9180k  100 9180k    0     0  11.9M      0 --:--:-- --:--:-- --:--:-- 11.9M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 10  120M   10 12.9M    0     0  13.5M      0  0:00:08 --:--:--  0:00:08 13.5M 39  120M   39 48.0M    0     0  23.9M      0  0:00:05  0:00:02  0:00:03 23.9M 66  120M   66 80.0M    0     0  26.9M      0  0:00:04  0:00:02  0:00:02 26.9M 95  120M   95  114M    0     0  29.0M      0  0:00:04  0:00:03  0:00:01 29.0M100  120M  100  120M    0     0  29.3M      0  0:00:04  0:00:04 --:--:-- 29.3M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   39f7ce4..6ff574b  master     -> origin/master
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
] Testing  RL18_DBG_F2_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```