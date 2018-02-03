```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 31 11.1M   31 3535k    0     0  5081k      0  0:00:02 --:--:--  0:00:02 5079k100 11.1M  100 11.1M    0     0  9480k      0  0:00:01  0:00:01 --:--:-- 9484k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  143M    3 4864k    0     0  10.0M      0  0:00:14 --:--:--  0:00:14 10.0M 12  143M   12 18.1M    0     0  12.3M      0  0:00:11  0:00:01  0:00:10 12.3M 21  143M   21 30.4M    0     0  12.2M      0  0:00:11  0:00:02  0:00:09 12.2M 30  143M   30 43.6M    0     0  12.5M      0  0:00:11  0:00:03  0:00:08 12.5M 39  143M   39 57.3M    0     0  12.8M      0  0:00:11  0:00:04  0:00:07 12.8M 49  143M   49 71.0M    0     0  12.9M      0  0:00:11  0:00:05  0:00:06 13.2M 59  143M   59 84.9M    0     0  13.1M      0  0:00:10  0:00:06  0:00:04 13.3M 68  143M   68 98.3M    0     0  13.1M      0  0:00:10  0:00:07  0:00:03 13.5M 77  143M   77  112M    0     0  12.8M      0  0:00:11  0:00:08  0:00:03 13.0M 81  143M   81  117M    0     0  12.4M      0  0:00:11  0:00:09  0:00:02 12.1M 92  143M   92  133M    0     0  12.7M      0  0:00:11  0:00:10  0:00:01 12.4M100  143M  100  143M    0     0  12.7M      0  0:00:11  0:00:11 --:--:-- 12.1M
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
] Testing  NODE_BUILD_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```