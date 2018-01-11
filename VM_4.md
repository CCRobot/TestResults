```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 52 11.1M   52 5968k    0     0  7280k      0  0:00:01 --:--:--  0:00:01 7278k100 11.1M  100 11.1M    0     0  9611k      0  0:00:01  0:00:01 --:--:-- 9612k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  127M    5 7088k    0     0  11.1M      0  0:00:11 --:--:--  0:00:11 11.1M 16  127M   16 20.7M    0     0  12.7M      0  0:00:10  0:00:01  0:00:09 12.7M 28  127M   28 36.0M    0     0  13.7M      0  0:00:09  0:00:02  0:00:07 13.6M 40  127M   40 51.6M    0     0  14.2M      0  0:00:08  0:00:03  0:00:05 14.2M 50  127M   50 64.9M    0     0  14.0M      0  0:00:09  0:00:04  0:00:05 14.0M 59  127M   59 76.5M    0     0  13.6M      0  0:00:09  0:00:05  0:00:04 13.9M 69  127M   69 89.3M    0     0  13.5M      0  0:00:09  0:00:06  0:00:03 13.7M 79  127M   79  102M    0     0  13.4M      0  0:00:09  0:00:07  0:00:02 13.2M 84  127M   84  108M    0     0  12.5M      0  0:00:10  0:00:08  0:00:02 11.2M 93  127M   93  119M    0     0  12.3M      0  0:00:10  0:00:09  0:00:01 10.8M100  127M  100  127M    0     0  12.5M      0  0:00:10  0:00:10 --:--:-- 11.2M
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
] Testing  NODE_BUILD_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```