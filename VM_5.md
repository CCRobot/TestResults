```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 32 11.1M   32 3647k    0     0  3653k      0  0:00:03 --:--:--  0:00:03 3651k100 11.1M  100 11.1M    0     0  6472k      0  0:00:01  0:00:01 --:--:-- 6474k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  143M    0  143k    0     0   650k      0  0:03:46 --:--:--  0:03:46  649k 10  143M   10 15.4M    0     0  12.6M      0  0:00:11  0:00:01  0:00:10 12.6M 21  143M   21 31.1M    0     0  14.0M      0  0:00:10  0:00:02  0:00:08 14.0M 30  143M   30 44.0M    0     0  13.6M      0  0:00:10  0:00:03  0:00:07 13.6M 40  143M   40 58.2M    0     0  13.7M      0  0:00:10  0:00:04  0:00:06 13.7M 51  143M   51 73.9M    0     0  14.1M      0  0:00:10  0:00:05  0:00:05 14.7M 60  143M   60 86.9M    0     0  13.9M      0  0:00:10  0:00:06  0:00:04 14.3M 66  143M   66 95.3M    0     0  13.1M      0  0:00:10  0:00:07  0:00:03 12.8M 75  143M   75  109M    0     0  13.2M      0  0:00:10  0:00:08  0:00:02 12.9M 87  143M   87  125M    0     0  13.6M      0  0:00:10  0:00:09  0:00:01 13.4M 96  143M   96  138M    0     0  13.5M      0  0:00:10  0:00:10 --:--:-- 13.0M100  143M  100  143M    0     0  13.5M      0  0:00:10  0:00:10 --:--:-- 13.0M
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
] Testing  DEBUG_FLG2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```