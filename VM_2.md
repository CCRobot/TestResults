```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 92 11.1M   92 10.2M    0     0  11.1M      0 --:--:-- --:--:-- --:--:-- 11.1M100 11.1M  100 11.1M    0     0  11.4M      0 --:--:-- --:--:-- --:--:-- 11.3M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  153M    5 8896k    0     0  9569k      0  0:00:16 --:--:--  0:00:16 9565k 11  153M   11 17.9M    0     0  9515k      0  0:00:16  0:00:01  0:00:15 9513k 18  153M   18 27.9M    0     0  9776k      0  0:00:16  0:00:02  0:00:14 9775k 24  153M   24 36.8M    0     0  9622k      0  0:00:16  0:00:03  0:00:13 9622k 30  153M   30 46.6M    0     0  9691k      0  0:00:16  0:00:04  0:00:12 9690k 34  153M   34 52.9M    0     0  9136k      0  0:00:17  0:00:05  0:00:12 9056k 43  153M   43 66.8M    0     0  9882k      0  0:00:15  0:00:06  0:00:09  9.7M 49  153M   49 76.2M    0     0  9845k      0  0:00:15  0:00:07  0:00:08 9884k 58  153M   58 89.1M    0     0   9.9M      0  0:00:15  0:00:08  0:00:07 10.4M 65  153M   65  100M    0     0  10.1M      0  0:00:15  0:00:09  0:00:06 10.7M 71  153M   71  110M    0     0  10.0M      0  0:00:15  0:00:10  0:00:05 11.4M 80  153M   80  122M    0     0  10.2M      0  0:00:14  0:00:11  0:00:03 11.1M 84  153M   84  129M    0     0  10.0M      0  0:00:15  0:00:12  0:00:03 10.6M 93  153M   93  143M    0     0  10.3M      0  0:00:14  0:00:13  0:00:01 10.9M100  153M  100  153M    0     0  10.2M      0  0:00:14  0:00:14 --:--:-- 10.6M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c0c17cf..f0da1c6  master      -> origin/master
   05f4157..befded1  release/1.8 -> origin/release/1.8
   91ec1ef..aec9a9c  release/1.9 -> origin/release/1.9
Updating c0c17cf..f0da1c6
Fast-forward
 lib/Backend/Func.cpp      |  5 +++--
 lib/Backend/IRBuilder.cpp |  2 +-
 test/Bugs/bug14057294.js  | 22 ++++++++++++++++++++++
 test/Bugs/rlexe.xml       |  5 +++++
 4 files changed, 31 insertions(+), 3 deletions(-)
 create mode 100644 test/Bugs/bug14057294.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_PACK
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```