```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 41 11.1M   41 4768k    0     0  5740k      0  0:00:01 --:--:--  0:00:01 5737k100 11.1M  100 11.1M    0     0  9678k      0  0:00:01  0:00:01 --:--:-- 9686k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  138M    4 5808k    0     0  9198k      0  0:00:15 --:--:--  0:00:15 9189k 13  138M   13 18.0M    0     0  11.0M      0  0:00:12  0:00:01  0:00:11 11.0M 23  138M   23 32.2M    0     0  12.2M      0  0:00:11  0:00:02  0:00:09 12.2M 30  138M   30 42.0M    0     0  11.5M      0  0:00:11  0:00:03  0:00:08 11.5M 39  138M   39 55.1M    0     0  11.8M      0  0:00:11  0:00:04  0:00:07 11.8M 44  138M   44 62.2M    0     0  11.0M      0  0:00:12  0:00:05  0:00:07 11.3M 53  138M   53 73.7M    0     0  11.1M      0  0:00:12  0:00:06  0:00:06 11.1M 63  138M   63 87.3M    0     0  11.4M      0  0:00:12  0:00:07  0:00:05 11.0M 73  138M   73  101M    0     0  11.7M      0  0:00:11  0:00:08  0:00:03 11.9M 82  138M   82  113M    0     0  11.7M      0  0:00:11  0:00:09  0:00:02 11.7M 92  138M   92  127M    0     0  12.0M      0  0:00:11  0:00:10  0:00:01 13.1M100  138M  100  138M    0     0  12.0M      0  0:00:11  0:00:11 --:--:-- 13.2M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   9169de3..5127477  master      -> origin/master
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
] Testing  RL18_DBG_F2_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```