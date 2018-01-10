```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 60 11.1M   60 6832k    0     0  6996k      0  0:00:01 --:--:--  0:00:01 6992k100 11.1M  100 11.1M    0     0  7609k      0  0:00:01  0:00:01 --:--:-- 7612k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  127M    2 3919k    0     0  8460k      0  0:00:15 --:--:--  0:00:15 8447k 11  127M   11 14.2M    0     0  9937k      0  0:00:13  0:00:01  0:00:12 9934k 19  127M   19 24.6M    0     0   9.9M      0  0:00:12  0:00:02  0:00:10  9.9M 28  127M   28 36.6M    0     0  10.5M      0  0:00:12  0:00:03  0:00:09 10.5M 38  127M   38 49.2M    0     0  10.3M      0  0:00:12  0:00:04  0:00:08 10.3M 43  127M   43 55.7M    0     0  10.1M      0  0:00:12  0:00:05  0:00:07 10.3M 53  127M   53 68.0M    0     0  10.4M      0  0:00:12  0:00:06  0:00:06 10.7M 62  127M   62 80.2M    0     0  10.7M      0  0:00:11  0:00:07  0:00:04 11.1M 69  127M   69 89.3M    0     0  10.5M      0  0:00:12  0:00:08  0:00:04 10.5M 78  127M   78  100M    0     0  10.5M      0  0:00:12  0:00:09  0:00:03 10.7M 87  127M   87  112M    0     0  10.6M      0  0:00:11  0:00:10  0:00:01 11.2M 97  127M   97  124M    0     0  10.8M      0  0:00:11  0:00:11 --:--:-- 11.2M100  127M  100  127M    0     0  10.8M      0  0:00:11  0:00:11 --:--:-- 11.0M
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
] Testing  RLS18_TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```