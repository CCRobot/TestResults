```
Executed on ubu16chk4000013
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  8502k      0  0:00:01  0:00:01 --:--:-- 8508k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  143M    5 8208k    0     0  7900k      0  0:00:18  0:00:01  0:00:17 7899k 30  143M   30 44.0M    0     0  21.5M      0  0:00:06  0:00:02  0:00:04 21.5M 58  143M   58 84.0M    0     0  27.5M      0  0:00:05  0:00:03  0:00:02 27.5M 86  143M   86  124M    0     0  30.4M      0  0:00:04  0:00:04 --:--:-- 30.4M100  143M  100  143M    0     0  31.8M      0  0:00:04  0:00:04 --:--:-- 32.0M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   eac97b9..97d5c20  master     -> origin/master
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
] Testing  DEBUG_FLG1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```