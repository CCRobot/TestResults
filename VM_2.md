```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 80 11.1M   80 9200k    0     0  8408k      0  0:00:01  0:00:01 --:--:-- 8401k100 11.1M  100 11.1M    0     0  8748k      0  0:00:01  0:00:01 --:--:-- 8748k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  153M    4 7808k    0     0   9.7M      0  0:00:15 --:--:--  0:00:15  9.7M 14  153M   14 22.8M    0     0  12.8M      0  0:00:11  0:00:01  0:00:10 12.8M 22  153M   22 34.2M    0     0  12.3M      0  0:00:12  0:00:02  0:00:10 12.3M 31  153M   31 48.0M    0     0  12.7M      0  0:00:12  0:00:03  0:00:09 12.7M 39  153M   39 60.2M    0     0  12.6M      0  0:00:12  0:00:04  0:00:08 12.6M 46  153M   46 72.1M    0     0  12.4M      0  0:00:12  0:00:05  0:00:07 12.9M 58  153M   58 90.4M    0     0  13.3M      0  0:00:11  0:00:06  0:00:05 13.5M 67  153M   67  104M    0     0  13.4M      0  0:00:11  0:00:07  0:00:04 14.0M 78  153M   78  120M    0     0  13.6M      0  0:00:11  0:00:08  0:00:03 14.3M 85  153M   85  131M    0     0  13.4M      0  0:00:11  0:00:09  0:00:02 14.2M 93  153M   93  143M    0     0  13.3M      0  0:00:11  0:00:10  0:00:01 14.3M100  153M  100  153M    0     0  13.2M      0  0:00:11  0:00:11 --:--:-- 13.1M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   6ea656a..8e5ec68  master     -> origin/master
Updating 6ea656a..8e5ec68
Fast-forward
 lib/Runtime/Base/FunctionBody.cpp           | 10 +--------
 lib/Runtime/Language/DynamicProfileInfo.cpp |  6 +++---
 test/bailout/inline_get_bailout.js          | 32 +++++++++++++++++++++++++++++
 test/bailout/inline_get_bailout_helper.js   | 18 ++++++++++++++++
 test/bailout/rlexe.xml                      |  6 ++++++
 5 files changed, 60 insertions(+), 12 deletions(-)
 create mode 100644 test/bailout/inline_get_bailout.js
 create mode 100644 test/bailout/inline_get_bailout_helper.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  obastemur_testmac.sh
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```