```
Executed on ubu16chk4000012
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 44 9180k   44 4096k    0     0  3425k      0  0:00:02  0:00:01  0:00:01 3424k100 9180k  100 9180k    0     0  6903k      0  0:00:01  0:00:01 --:--:-- 6902k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  143M    2 3871k    0     0  4711k      0  0:00:31 --:--:--  0:00:31 4709k 22  143M   22 32.0M    0     0  17.5M      0  0:00:08  0:00:01  0:00:07 17.5M 47  143M   47 68.0M    0     0  23.4M      0  0:00:06  0:00:02  0:00:04 23.4M 71  143M   71  102M    0     0  26.7M      0  0:00:05  0:00:03  0:00:02 26.7M 95  143M   95  137M    0     0  28.5M      0  0:00:05  0:00:04  0:00:01 28.5M100  143M  100  143M    0     0  29.1M      0  0:00:04  0:00:04 --:--:-- 34.0M
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
] Testing  NODE_BUILD_ubuntu
Executed on ubu16chk4000012
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6 9180k    6  623k    0     0   800k      0  0:00:11 --:--:--  0:00:11  800k100 9180k  100 9180k    0     0  7759k      0  0:00:01  0:00:01 --:--:-- 7760k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  143M    0  671k    0     0  1180k      0  0:02:04 --:--:--  0:02:04 1180k 19  143M   19 28.0M    0     0  17.5M      0  0:00:08  0:00:01  0:00:07 17.4M 47  143M   47 68.0M    0     0  26.4M      0  0:00:05  0:00:02  0:00:03 26.4M 75  143M   75  109M    0     0  30.6M      0  0:00:04  0:00:03  0:00:01 30.6M100  143M  100  143M    0     0  32.9M      0  0:00:04  0:00:04 --:--:-- 32.9M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   eac97b9..97d5c20  master     -> origin/master
   006593e..7cdfaf0  release/1.8 -> origin/release/1.8
   5c0bed5..45a175d  release/1.9 -> origin/release/1.9
error: The following untracked working tree files would be overwritten by merge:
	test/es6/bug_OS13976524.js
Please move or remove them before you can merge.
Aborting
Updating eac97b9..97d5c20
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  NODE_BUILD_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```