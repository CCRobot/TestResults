```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 83 11.1M   83 9456k    0     0  8228k      0  0:00:01  0:00:01 --:--:-- 8222k100 11.1M  100 11.1M    0     0  9008k      0  0:00:01  0:00:01 --:--:-- 9004k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  124M    6 8576k    0     0  9834k      0  0:00:13 --:--:--  0:00:13 9834k 14  124M   14 18.4M    0     0   9.8M      0  0:00:12  0:00:01  0:00:11  9.8M 22  124M   22 27.8M    0     0  9919k      0  0:00:12  0:00:02  0:00:10 9918k 30  124M   30 37.7M    0     0  9731k      0  0:00:13  0:00:03  0:00:10 9731k 38  124M   38 48.0M    0     0   9.8M      0  0:00:12  0:00:04  0:00:08  9.8M 46  124M   46 58.0M    0     0   9.8M      0  0:00:12  0:00:05  0:00:07  9.9M 56  124M   56 70.6M    0     0  10.2M      0  0:00:12  0:00:06  0:00:06 10.4M 64  124M   64 80.7M    0     0  10.2M      0  0:00:12  0:00:07  0:00:05 10.5M 72  124M   72 90.1M    0     0  10.1M      0  0:00:12  0:00:08  0:00:04 10.6M 79  124M   79 98.9M    0     0  10.0M      0  0:00:12  0:00:09  0:00:03 10.2M 86  124M   86  107M    0     0   9.9M      0  0:00:12  0:00:10  0:00:02  9.9M 94  124M   94  117M    0     0   9.8M      0  0:00:12  0:00:11  0:00:01 9602k100  124M  100  124M    0     0   9.9M      0  0:00:12  0:00:12 --:--:-- 9724k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c47185f..dee6b5f  master      -> origin/master
   e02b39a..d91fb1d  release/1.7 -> origin/release/1.7
   d00b341..cb70795  release/1.8 -> origin/release/1.8
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
] Testing  RL18_DBG_F2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```