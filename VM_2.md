```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:--  0:00:01 --:--:--     0 32 11.1M   32 3711k    0     0  1700k      0  0:00:06  0:00:02  0:00:04 1700k 72 11.1M   72 8208k    0     0  2576k      0  0:00:04  0:00:03  0:00:01 2576k100 11.1M  100 11.1M    0     0  2912k      0  0:00:03  0:00:03 --:--:-- 2912k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  153M    0 1103k    0     0  4246k      0  0:00:37 --:--:--  0:00:37 4244k  5  153M    5 8672k    0     0  6870k      0  0:00:22  0:00:01  0:00:21 6866k 13  153M   13 20.0M    0     0  9042k      0  0:00:17  0:00:02  0:00:15 9041k 19  153M   19 29.5M    0     0  9287k      0  0:00:16  0:00:03  0:00:13 9285k 23  153M   23 35.7M    0     0  8592k      0  0:00:18  0:00:04  0:00:14 8591k 29  153M   29 45.8M    0     0  8920k      0  0:00:17  0:00:05  0:00:12 9164k 37  153M   37 57.7M    0     0  9448k      0  0:00:16  0:00:06  0:00:10  9.8M 45  153M   45 69.9M    0     0  9860k      0  0:00:15  0:00:07  0:00:08  9.9M 52  153M   52 81.3M    0     0   9.8M      0  0:00:15  0:00:08  0:00:07 10.3M 61  153M   61 94.9M    0     0  10.2M      0  0:00:15  0:00:09  0:00:06 11.8M 70  153M   70  108M    0     0  10.6M      0  0:00:14  0:00:10  0:00:04 12.6M 77  153M   77  119M    0     0  10.6M      0  0:00:14  0:00:11  0:00:03 12.4M 85  153M   85  131M    0     0  10.7M      0  0:00:14  0:00:12  0:00:02 12.3M 93  153M   93  143M    0     0  10.8M      0  0:00:14  0:00:13  0:00:01 12.3M100  153M  100  153M    0     0  10.8M      0  0:00:14  0:00:14 --:--:-- 12.0M
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