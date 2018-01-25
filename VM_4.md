```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6 11.1M    6  751k    0     0  2773k      0  0:00:04 --:--:--  0:00:04 2773k100 11.1M  100 11.1M    0     0  9638k      0  0:00:01  0:00:01 --:--:-- 9645k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  8  138M    8 12.1M    0     0  11.4M      0  0:00:12  0:00:01  0:00:11 11.4M 18  138M   18 25.2M    0     0  12.2M      0  0:00:11  0:00:02  0:00:09 12.2M 27  138M   27 38.2M    0     0  12.4M      0  0:00:11  0:00:03  0:00:08 12.4M 36  138M   36 50.9M    0     0  12.5M      0  0:00:11  0:00:04  0:00:07 12.5M 43  138M   43 60.8M    0     0  12.0M      0  0:00:11  0:00:05  0:00:06 12.2M 56  138M   56 77.7M    0     0  12.8M      0  0:00:10  0:00:06  0:00:04 13.1M 66  138M   66 91.5M    0     0  12.9M      0  0:00:10  0:00:07  0:00:03 13.2M 75  138M   75  104M    0     0  12.8M      0  0:00:10  0:00:08  0:00:02 13.1M 85  138M   85  118M    0     0  13.1M      0  0:00:10  0:00:09  0:00:01 13.5M 94  138M   94  130M    0     0  12.9M      0  0:00:10  0:00:10 --:--:-- 13.9M100  138M  100  138M    0     0  13.0M      0  0:00:10  0:00:10 --:--:-- 13.4M
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
] Testing  RLS18_TEST_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```