```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 98 11.1M   98 11.0M    0     0  9051k      0  0:00:01  0:00:01 --:--:-- 9047k100 11.1M  100 11.1M    0     0  9104k      0  0:00:01  0:00:01 --:--:-- 9097k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 10  120M   10 12.7M    0     0  13.0M      0  0:00:09 --:--:--  0:00:09 13.0M 23  120M   23 28.0M    0     0  14.0M      0  0:00:08  0:00:02  0:00:06 14.0M 33  120M   33 40.0M    0     0  13.2M      0  0:00:09  0:00:03  0:00:06 13.2M 43  120M   43 52.2M    0     0  13.1M      0  0:00:09  0:00:03  0:00:06 13.1M 54  120M   54 65.8M    0     0  13.2M      0  0:00:09  0:00:04  0:00:05 13.2M 63  120M   63 76.7M    0     0  12.8M      0  0:00:09  0:00:05  0:00:04 12.7M 74  120M   74 89.1M    0     0  12.7M      0  0:00:09  0:00:06  0:00:03 12.2M 84  120M   84  101M    0     0  12.7M      0  0:00:09  0:00:07  0:00:02 12.4M 93  120M   93  112M    0     0  12.5M      0  0:00:09  0:00:08  0:00:01 12.0M100  120M  100  120M    0     0  12.6M      0  0:00:09  0:00:09 --:--:-- 11.9M
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
] Testing  DEBUG_FLG1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```