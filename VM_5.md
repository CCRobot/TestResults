```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  10.3M      0  0:00:01  0:00:01 --:--:-- 10.3M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  124M    6 8208k    0     0  7972k      0  0:00:16  0:00:01  0:00:15 7968k 16  124M   16 20.0M    0     0   9.8M      0  0:00:12  0:00:02  0:00:10  9.8M 22  124M   22 27.8M    0     0  9424k      0  0:00:13  0:00:03  0:00:10 9422k 28  124M   28 35.9M    0     0  9131k      0  0:00:14  0:00:04  0:00:10 9129k 32  124M   32 40.7M    0     0  8297k      0  0:00:15  0:00:05  0:00:10 8335k 36  124M   36 45.0M    0     0  7651k      0  0:00:16  0:00:06  0:00:10 7585k 40  124M   40 50.3M    0     0  7337k      0  0:00:17  0:00:07  0:00:10 6229k 44  124M   44 55.8M    0     0  7124k      0  0:00:17  0:00:08  0:00:09 5731k 56  124M   56 70.1M    0     0  7961k      0  0:00:16  0:00:09  0:00:07 7017k 64  124M   64 80.2M    0     0  8201k      0  0:00:15  0:00:10  0:00:05 8104k 73  124M   73 92.0M    0     0  8521k      0  0:00:15  0:00:11  0:00:04 9565k 83  124M   83  104M    0     0  8849k      0  0:00:14  0:00:12  0:00:02 10.7M 94  124M   94  118M    0     0  9285k      0  0:00:13  0:00:13 --:--:-- 12.4M100  124M  100  124M    0     0  9376k      0  0:00:13  0:00:13 --:--:-- 11.8M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c47185f..dee6b5f  master      -> origin/master
   e02b39a..d91fb1d  release/1.7 -> origin/release/1.7
   d00b341..0be1e74  release/1.8 -> origin/release/1.8
 * [new tag]         v1.7.6      -> v1.7.6
Updating c47185f..dee6b5f
Fast-forward
 lib/Backend/BailOut.cpp        |  8 +++++++-
 test/Bugs/bug13830477.baseline |  7 +++++++
 test/Bugs/bug13830477.js       | 28 ++++++++++++++++++++++++++++
 test/Bugs/rlexe.xml            |  6 ++++++
 4 files changed, 48 insertions(+), 1 deletion(-)
 create mode 100644 test/Bugs/bug13830477.baseline
 create mode 100644 test/Bugs/bug13830477.js
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