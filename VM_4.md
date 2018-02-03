```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 49 11.1M   49 5616k    0     0  8373k      0  0:00:01 --:--:--  0:00:01 8369k100 11.1M  100 11.1M    0     0  10.4M      0  0:00:01  0:00:01 --:--:-- 10.4M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  143M    3 4448k    0     0  7544k      0  0:00:19 --:--:--  0:00:19 7538k 11  143M   11 16.7M    0     0  10.5M      0  0:00:13  0:00:01  0:00:12 10.5M 20  143M   20 30.2M    0     0  11.6M      0  0:00:12  0:00:02  0:00:10 11.6M 30  143M   30 43.6M    0     0  12.1M      0  0:00:11  0:00:03  0:00:08 12.1M 38  143M   38 56.0M    0     0  12.2M      0  0:00:11  0:00:04  0:00:07 12.2M 47  143M   47 67.8M    0     0  12.1M      0  0:00:11  0:00:05  0:00:06 12.7M 56  143M   56 81.9M    0     0  12.4M      0  0:00:11  0:00:06  0:00:05 13.0M 66  143M   66 95.7M    0     0  12.6M      0  0:00:11  0:00:07  0:00:04 13.1M 73  143M   73  106M    0     0  12.3M      0  0:00:11  0:00:08  0:00:03 12.5M 80  143M   80  116M    0     0  12.0M      0  0:00:11  0:00:09  0:00:02 11.9M 89  143M   89  128M    0     0  11.9M      0  0:00:12  0:00:10  0:00:02 11.6M 95  143M   95  137M    0     0  11.8M      0  0:00:12  0:00:11  0:00:01 11.1M100  143M  100  143M    0     0  11.9M      0  0:00:12  0:00:12 --:--:-- 10.7M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   6c93ac5..eac97b9  master      -> origin/master
   c4d03a6..006593e  release/1.8 -> origin/release/1.8
   1dd69bc..5c0bed5  release/1.9 -> origin/release/1.9
Updating 6c93ac5..eac97b9
Fast-forward
 lib/Parser/RegexParser.cpp              |  5 +++++
 lib/Parser/rterrors.h                   |  1 +
 pal/src/loader/module.cpp               |  2 +-
 test/Regex/rlexe.xml                    |  6 ++++++
 test/Regex/unicode_forbidden_escapes.js | 33 +++++++++++++++++++++++++++++++++
 5 files changed, 46 insertions(+), 1 deletion(-)
 create mode 100644 test/Regex/unicode_forbidden_escapes.js
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