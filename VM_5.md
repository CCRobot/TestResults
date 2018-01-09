```
Executed on ubu16chk4000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  12.2M      0 --:--:-- --:--:-- --:--:-- 12.2M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  124M    0 32345    0     0  89277      0  0:24:26 --:--:--  0:24:26 89104 19  124M   19 24.0M    0     0  17.3M      0  0:00:07  0:00:01  0:00:06 17.3M 44  124M   44 56.0M    0     0  23.4M      0  0:00:05  0:00:02  0:00:03 23.4M 67  124M   67 84.0M    0     0  24.5M      0  0:00:05  0:00:03  0:00:02 24.5M 89  124M   89  111M    0     0  25.5M      0  0:00:04  0:00:04 --:--:-- 25.5M100  124M  100  124M    0     0  26.0M      0  0:00:04  0:00:04 --:--:-- 28.2M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c47185f..dee6b5f  master     -> origin/master
   e02b39a..d91fb1d  release/1.7 -> origin/release/1.7
   d00b341..0be1e74  release/1.8 -> origin/release/1.8
 * [new tag]         v1.7.6     -> v1.7.6
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
] Testing  DEBUG_FLG1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```