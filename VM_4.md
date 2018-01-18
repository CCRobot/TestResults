```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 24 11.1M   24 2735k    0     0  4083k      0  0:00:02 --:--:--  0:00:02 4082k 37 11.1M   37 4288k    0     0  2351k      0  0:00:04  0:00:01  0:00:03 2350k 73 11.1M   73 8416k    0     0  3151k      0  0:00:03  0:00:02  0:00:01 3150k100 11.1M  100 11.1M    0     0  3209k      0  0:00:03  0:00:03 --:--:-- 3209k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  133M    3 4992k    0     0  4488k      0  0:00:30  0:00:01  0:00:29 4485k  5  133M    5 7088k    0     0  3159k      0  0:00:43  0:00:02  0:00:41 3160k  7  133M    7 9936k    0     0  3194k      0  0:00:42  0:00:03  0:00:39 3193k 11  133M   11 14.7M    0     0  3571k      0  0:00:38  0:00:04  0:00:34 3571k 15  133M   15 20.2M    0     0  4065k      0  0:00:33  0:00:05  0:00:28 4157k 17  133M   17 23.6M    0     0  3966k      0  0:00:34  0:00:06  0:00:28 3849k 22  133M   22 30.1M    0     0  4346k      0  0:00:31  0:00:07  0:00:24 4892k 29  133M   29 39.7M    0     0  5025k      0  0:00:27  0:00:08  0:00:19 6164k 36  133M   36 48.6M    0     0  5466k      0  0:00:24  0:00:09  0:00:15 7114k 43  133M   43 57.9M    0     0  5871k      0  0:00:23  0:00:10  0:00:13 7718k 51  133M   51 68.7M    0     0  6333k      0  0:00:21  0:00:11  0:00:10 9227k 58  133M   58 78.0M    0     0  6604k      0  0:00:20  0:00:12  0:00:08 9817k 66  133M   66 88.8M    0     0  6937k      0  0:00:19  0:00:13  0:00:06  9.8M 75  133M   75  100M    0     0  7280k      0  0:00:18  0:00:14  0:00:04 10.3M 82  133M   82  109M    0     0  7447k      0  0:00:18  0:00:15  0:00:03 10.3M 89  133M   89  118M    0     0  7540k      0  0:00:18  0:00:16  0:00:02  9.9M 95  133M   95  127M    0     0  7640k      0  0:00:17  0:00:17 --:--:--  9.9M100  133M  100  133M    0     0  7656k      0  0:00:17  0:00:17 --:--:-- 9656k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   e0a8f50..9dd0d9d  master      -> origin/master
   6c055d9..55e9c9d  release/1.8 -> origin/release/1.8
   d7d99e1..d1c4faf  release/1.9 -> origin/release/1.9
 * [new tag]         v1.8.0      -> v1.8.0
Updating e0a8f50..9dd0d9d
Fast-forward
 lib/Common/ChakraCoreVersion.h                     |  4 +-
 lib/Runtime/Library/DateImplementation.cpp         | 28 ++++++++---
 test/Date/DateParse2.js                            |  9 ++--
 test/Date/DateParse2.v5.baseline                   | 56 ++++++++++++++++++++--
 test/Date/parseToStringResults.js                  | 41 ++++++++++++++++
 test/Date/parseToUTCStringAndToISOStringResults.js | 41 ++++++++++++++++
 test/Date/rlexe.xml                                | 14 ++++++
 7 files changed, 178 insertions(+), 15 deletions(-)
 create mode 100644 test/Date/parseToStringResults.js
 create mode 100644 test/Date/parseToUTCStringAndToISOStringResults.js
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