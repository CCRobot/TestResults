```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 36 11.1M   36 4176k    0     0  6151k      0  0:00:01 --:--:--  0:00:01 6150k100 11.1M  100 11.1M    0     0  9613k      0  0:00:01  0:00:01 --:--:-- 9620k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  127M    2 3887k    0     0  8218k      0  0:00:15 --:--:--  0:00:15 8218k 12  127M   12 16.1M    0     0  10.9M      0  0:00:11  0:00:01  0:00:10 10.9M 23  127M   23 29.4M    0     0  11.9M      0  0:00:10  0:00:02  0:00:08 11.8M 32  127M   32 41.0M    0     0  11.8M      0  0:00:10  0:00:03  0:00:07 11.8M 40  127M   40 51.2M    0     0  11.4M      0  0:00:11  0:00:04  0:00:07 11.4M 49  127M   49 63.1M    0     0  11.5M      0  0:00:11  0:00:05  0:00:06 11.8M 58  127M   58 74.3M    0     0  11.4M      0  0:00:11  0:00:06  0:00:05 11.6M 66  127M   66 84.8M    0     0  11.3M      0  0:00:11  0:00:07  0:00:04 11.0M 76  127M   76 98.0M    0     0  11.5M      0  0:00:11  0:00:08  0:00:03 11.3M 84  127M   84  108M    0     0  11.4M      0  0:00:11  0:00:09  0:00:02 11.4M 95  127M   95  122M    0     0  11.6M      0  0:00:10  0:00:10 --:--:-- 11.8M100  127M  100  127M    0     0  11.4M      0  0:00:11  0:00:11 --:--:-- 11.4M
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
] Testing  RL18_PACK
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```