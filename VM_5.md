```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 13 11.1M   13 1487k    0     0  4672k      0  0:00:02 --:--:--  0:00:02 4663k100 11.1M  100 11.1M    0     0  12.6M      0 --:--:-- --:--:-- --:--:-- 12.6M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  143M    1 2847k    0     0  6783k      0  0:00:21 --:--:--  0:00:21 6779k 13  143M   13 19.4M    0     0  13.6M      0  0:00:10  0:00:01  0:00:09 13.6M 23  143M   23 33.2M    0     0  13.7M      0  0:00:10  0:00:02  0:00:08 13.7M 35  143M   35 50.7M    0     0  14.8M      0  0:00:09  0:00:03  0:00:06 14.8M 46  143M   46 66.5M    0     0  15.0M      0  0:00:09  0:00:04  0:00:05 15.0M 57  143M   57 82.3M    0     0  15.2M      0  0:00:09  0:00:05  0:00:04 15.9M 68  143M   68 98.6M    0     0  15.3M      0  0:00:09  0:00:06  0:00:03 15.8M 80  143M   80  116M    0     0  15.7M      0  0:00:09  0:00:07  0:00:02 16.6M 91  143M   91  132M    0     0  15.6M      0  0:00:09  0:00:08  0:00:01 16.2M100  143M  100  143M    0     0  15.8M      0  0:00:09  0:00:09 --:--:-- 16.5M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   eac97b9..97d5c20  master      -> origin/master
   006593e..7cdfaf0  release/1.8 -> origin/release/1.8
   5c0bed5..45a175d  release/1.9 -> origin/release/1.9
Updating eac97b9..97d5c20
Fast-forward
 lib/Parser/Parse.cpp                | 30 +++++++++++-------------------
 lib/Parser/Parse.h                  |  2 +-
 test/Basics/SpecialSymbolCapture.js | 13 +++++++++++++
 test/es6/bug_OS13976524.js          | 18 ++++++++++++++++++
 test/es6/rlexe.xml                  |  7 +++++++
 5 files changed, 50 insertions(+), 20 deletions(-)
 create mode 100644 test/es6/bug_OS13976524.js
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