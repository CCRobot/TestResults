```
Executed on ubu16chk4000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  12.2M      0 --:--:-- --:--:-- --:--:-- 12.2M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  138M    0 65113    0     0   163k      0  0:14:25 --:--:--  0:14:25  163k 16  138M   16 22.3M    0     0  16.1M      0  0:00:08  0:00:01  0:00:07 16.1M 33  138M   33 46.7M    0     0  19.5M      0  0:00:07  0:00:02  0:00:05 19.5M 51  138M   51 70.7M    0     0  20.9M      0  0:00:06  0:00:03  0:00:03 20.9M 69  138M   69 95.7M    0     0  21.7M      0  0:00:06  0:00:04  0:00:02 21.7M 86  138M   86  119M    0     0  22.1M      0  0:00:06  0:00:05  0:00:01 23.8M100  138M  100  138M    0     0  22.4M      0  0:00:06  0:00:06 --:--:-- 24.2M
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
] Testing  RLS18_TEST_ubuntu
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```