```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 35 11.1M   35 4096k    0     0  6045k      0  0:00:01 --:--:--  0:00:01 6041k 89 11.1M   89  9.9M    0     0  6039k      0  0:00:01  0:00:01 --:--:-- 6038k100 11.1M  100 11.1M    0     0  6258k      0  0:00:01  0:00:01 --:--:-- 6256k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  7  127M    7 9456k    0     0  10.9M      0  0:00:11 --:--:--  0:00:11 10.9M 12  127M   12 16.4M    0     0  8892k      0  0:00:14  0:00:01  0:00:13 8891k 18  127M   18 23.8M    0     0  8595k      0  0:00:15  0:00:02  0:00:13 8593k 23  127M   23 30.4M    0     0  8123k      0  0:00:16  0:00:03  0:00:13 8122k 27  127M   27 34.9M    0     0  7401k      0  0:00:17  0:00:04  0:00:13 7401k 34  127M   34 44.7M    0     0  7835k      0  0:00:16  0:00:05  0:00:11 7267k 43  127M   43 55.8M    0     0  8367k      0  0:00:15  0:00:06  0:00:09 8164k 53  127M   53 68.5M    0     0  8942k      0  0:00:14  0:00:07  0:00:07 9140k 63  127M   63 81.1M    0     0  9399k      0  0:00:13  0:00:08  0:00:05 10.1M 71  127M   71 91.1M    0     0  9486k      0  0:00:13  0:00:09  0:00:04 11.2M 79  127M   79  101M    0     0  9599k      0  0:00:13  0:00:10  0:00:03 11.3M 87  127M   87  111M    0     0  9660k      0  0:00:13  0:00:11  0:00:02 11.1M 94  127M   94  121M    0     0  9671k      0  0:00:13  0:00:12  0:00:01 10.5M100  127M  100  127M    0     0  9730k      0  0:00:13  0:00:13 --:--:-- 10.1M
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
] Testing  RL18_DBG_F1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```