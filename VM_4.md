```
Executed on ubu16chk400000M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  8907k      0  0:00:01  0:00:01 --:--:-- 8913k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 11  138M   11 16.0M    0     0  13.1M      0  0:00:10  0:00:01  0:00:09 13.1M 40  138M   40 55.9M    0     0  25.5M      0  0:00:05  0:00:02  0:00:03 25.5M 68  138M   68 94.2M    0     0  29.5M      0  0:00:04  0:00:03  0:00:01 29.5M 95  138M   95  132M    0     0  31.3M      0  0:00:04  0:00:04 --:--:-- 31.3M100  138M  100  138M    0     0  32.1M      0  0:00:04  0:00:04 --:--:-- 33.7M
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
] Testing  RL18_DBG_ubuntu
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```