```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 92 11.1M   92 10.2M    0     0  9584k      0  0:00:01  0:00:01 --:--:-- 9579k100 11.1M  100 11.1M    0     0  9868k      0  0:00:01  0:00:01 --:--:-- 9862k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  127M    6 9152k    0     0  9881k      0  0:00:13 --:--:--  0:00:13 9872k 14  127M   14 18.5M    0     0  9877k      0  0:00:13  0:00:01  0:00:12 9872k 24  127M   24 31.5M    0     0  10.7M      0  0:00:11  0:00:02  0:00:09 10.7M 30  127M   30 39.1M    0     0   9.9M      0  0:00:12  0:00:03  0:00:09  9.9M 37  127M   37 48.0M    0     0  9979k      0  0:00:13  0:00:04  0:00:09 9979k 44  127M   44 56.4M    0     0  9748k      0  0:00:13  0:00:05  0:00:08 9724k 49  127M   49 63.0M    0     0  9318k      0  0:00:14  0:00:06  0:00:08 9104k 55  127M   55 71.5M    0     0  9241k      0  0:00:14  0:00:07  0:00:07 8195k 62  127M   62 80.3M    0     0  9215k      0  0:00:14  0:00:08  0:00:06 8433k 71  127M   71 91.5M    0     0  9442k      0  0:00:13  0:00:09  0:00:04 8913k 75  127M   75 96.9M    0     0  9088k      0  0:00:14  0:00:10  0:00:04 8307k 80  127M   80  103M    0     0  8868k      0  0:00:14  0:00:11  0:00:03 8244k 84  127M   84  108M    0     0  8601k      0  0:00:15  0:00:12  0:00:03 7587k 92  127M   92  118M    0     0  8718k      0  0:00:15  0:00:13  0:00:02 7830k 98  127M   98  125M    0     0  8628k      0  0:00:15  0:00:14  0:00:01 7012k100  127M  100  127M    0     0  8629k      0  0:00:15  0:00:15 --:--:-- 7448k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   d7bb357..9d0069e  master      -> origin/master
   d91fb1d..f6f84bb  release/1.7 -> origin/release/1.7
   23984b9..0dd3ff3  release/1.8 -> origin/release/1.8
Updating d7bb357..9d0069e
Fast-forward
 bin/ch/ch.cpp                             | 93 ++++++++++++++++---------------
 bin/rl/rl.cpp                             | 92 +++++++++++++++++++++++++++++-
 bin/rl/rl.h                               |  3 +-
 bin/rl/rlregr.cpp                         |  4 +-
 bin/rl/rlrun.cpp                          |  4 +-
 lib/Backend/GlobOpt.cpp                   | 15 +++--
 lib/Backend/GlobOpt.h                     |  2 +
 lib/Backend/GlobOptBlockData.cpp          |  2 +-
 lib/Backend/SwitchIRBuilder.cpp           | 42 ++++++--------
 lib/Backend/SwitchIRBuilder.h             |  4 +-
 lib/Runtime/Library/WebAssemblyModule.cpp |  7 ++-
 test/AsmJs/rlexe.xml                      |  2 +
 test/Miscellaneous/rlexe.xml              | 74 ++++++++++++++++++++++++
 test/runtests.cmd                         |  2 +
 test/runtests.py                          |  6 +-
 15 files changed, 264 insertions(+), 88 deletions(-)
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