```
Executed on ubu16chk4000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2 9180k    2  207k    0     0   399k      0  0:00:22 --:--:--  0:00:22  399k100 9180k  100 9180k    0     0  11.0M      0 --:--:-- --:--:-- --:--:-- 11.0M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  127M    4 6496k    0     0  9714k      0  0:00:13 --:--:--  0:00:13 9710k 34  127M   34 43.9M    0     0  26.3M      0  0:00:04  0:00:01  0:00:03 26.3M 58  127M   58 75.0M    0     0  28.1M      0  0:00:04  0:00:02  0:00:02 28.1M 81  127M   81  103M    0     0  28.2M      0  0:00:04  0:00:03  0:00:01 28.2M 93  127M   93  119M    0     0  25.6M      0  0:00:04  0:00:04 --:--:-- 25.6M100  127M  100  127M    0     0  24.8M      0  0:00:05  0:00:05 --:--:-- 27.2M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   d7bb357..e7012ab  master     -> origin/master
   d91fb1d..f6f84bb  release/1.7 -> origin/release/1.7
   23984b9..0dd3ff3  release/1.8 -> origin/release/1.8
Updating d7bb357..e7012ab
Fast-forward
 lib/Backend/GlobOpt.cpp                   | 15 +++++++----
 lib/Backend/GlobOpt.h                     |  2 ++
 lib/Backend/GlobOptBlockData.cpp          |  2 +-
 lib/Backend/SwitchIRBuilder.cpp           | 42 +++++++++++++------------------
 lib/Backend/SwitchIRBuilder.h             |  4 ++-
 lib/Runtime/Library/WebAssemblyModule.cpp |  7 ++++--
 test/AsmJs/rlexe.xml                      |  2 ++
 7 files changed, 40 insertions(+), 34 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```