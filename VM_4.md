```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 41 11.1M   41 4688k    0     0  7731k      0  0:00:01 --:--:--  0:00:01 7723k100 11.1M  100 11.1M    0     0  9416k      0  0:00:01  0:00:01 --:--:-- 9421k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  127M    1 1311k    0     0  3448k      0  0:00:37 --:--:--  0:00:37 3442k  6  127M    6 8944k    0     0  6476k      0  0:00:20  0:00:01  0:00:19 6476k 15  127M   15 20.2M    0     0  8687k      0  0:00:15  0:00:02  0:00:13 8685k 25  127M   25 32.8M    0     0  9795k      0  0:00:13  0:00:03  0:00:10 9793k 31  127M   31 40.7M    0     0  9134k      0  0:00:14  0:00:04  0:00:10 9133k 37  127M   37 48.2M    0     0  9172k      0  0:00:14  0:00:05  0:00:09 9609k 47  127M   47 61.2M    0     0  9823k      0  0:00:13  0:00:06  0:00:07 10.4M 57  127M   57 73.9M    0     0  10.0M      0  0:00:12  0:00:07  0:00:05 10.7M 69  127M   69 88.4M    0     0  10.5M      0  0:00:12  0:00:08  0:00:04 11.2M 80  127M   80  102M    0     0  10.9M      0  0:00:11  0:00:09  0:00:02 12.9M 90  127M   90  115M    0     0  11.1M      0  0:00:11  0:00:10  0:00:01 13.5M100  127M  100  127M    0     0  11.3M      0  0:00:11  0:00:11 --:--:-- 13.5M
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
] Testing  RL18_DBG_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```