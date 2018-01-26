```
Executed on ubu16chk400000M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 44 9180k   44 4095k    0     0  4503k      0  0:00:02 --:--:--  0:00:02 4500k100 9180k  100 9180k    0     0  8549k      0  0:00:01  0:00:01 --:--:-- 8556k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  138M    2 3759k    0     0  4615k      0  0:00:30 --:--:--  0:00:30 4612k 28  138M   28 40.0M    0     0  21.4M      0  0:00:06  0:00:01  0:00:05 21.4M 57  138M   57 80.0M    0     0  27.9M      0  0:00:04  0:00:02  0:00:02 27.9M 86  138M   86  119M    0     0  31.2M      0  0:00:04  0:00:03  0:00:01 31.2M100  138M  100  138M    0     0  32.2M      0  0:00:04  0:00:04 --:--:-- 32.2M
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
] Testing  RL18_DBG_F2_ubuntu
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```