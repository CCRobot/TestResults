```
Executed on ubu16chk400000N
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  8894k      0  0:00:01  0:00:01 --:--:-- 8896k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 11  138M   11 16.0M    0     0  12.9M      0  0:00:10  0:00:01  0:00:09 12.9M 41  138M   41 57.0M    0     0  25.5M      0  0:00:05  0:00:02  0:00:03 25.5M 72  138M   72  100M    0     0  30.3M      0  0:00:04  0:00:03  0:00:01 30.3M 96  138M   96  134M    0     0  31.7M      0  0:00:04  0:00:04 --:--:-- 31.7M100  138M  100  138M    0     0  32.1M      0  0:00:04  0:00:04 --:--:-- 34.6M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   9169de3..5127477  master     -> origin/master
   e5e1c85..ac5bc4d  release/1.8 -> origin/release/1.8
Updating 9169de3..5127477
Fast-forward
 lib/Jsrt/Jsrt.cpp                            |  6 +++++-
 lib/Parser/Parse.cpp                         | 11 ++++++-----
 lib/Parser/perrors.h                         |  2 +-
 lib/Runtime/Base/FunctionBody.cpp            |  7 +++++--
 lib/Runtime/Base/ThreadContext.cpp           |  7 ++++++-
 lib/Runtime/Base/ThreadContext.h             |  2 +-
 lib/Runtime/Language/JavascriptOperators.cpp | 10 +++++++---
 test/Function/argumentsLimits.baseline       |  6 +++---
 8 files changed, 34 insertions(+), 17 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_F1_ubuntu
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```