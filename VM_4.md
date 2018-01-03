```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 61 11.1M   61 7024k    0     0  7491k      0  0:00:01 --:--:--  0:00:01 7488k100 11.1M  100 11.1M    0     0  7950k      0  0:00:01  0:00:01 --:--:-- 7953k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  120M    3 4192k    0     0  8551k      0  0:00:14 --:--:--  0:00:14 8537k 16  120M   16 20.1M    0     0  13.5M      0  0:00:08  0:00:01  0:00:07 13.5M 26  120M   26 32.0M    0     0  12.7M      0  0:00:09  0:00:02  0:00:07 12.7M 37  120M   37 45.0M    0     0  12.9M      0  0:00:09  0:00:03  0:00:06 12.9M 50  120M   50 61.0M    0     0  13.6M      0  0:00:08  0:00:04  0:00:04 13.6M 60  120M   60 72.3M    0     0  13.1M      0  0:00:09  0:00:05  0:00:04 13.6M 72  120M   72 87.0M    0     0  13.4M      0  0:00:08  0:00:06  0:00:02 13.3M 84  120M   84  101M    0     0  13.6M      0  0:00:08  0:00:07  0:00:01 14.0M 97  120M   97  117M    0     0  13.8M      0  0:00:08  0:00:08 --:--:-- 14.4M100  120M  100  120M    0     0  13.7M      0  0:00:08  0:00:08 --:--:-- 13.9M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   39f7ce4..328ffa4  master      -> origin/master
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
] Testing  NODE_BUILD_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```