```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 99 11.1M   99 11.1M    0     0  10.3M      0  0:00:01  0:00:01 --:--:-- 10.3M100 11.1M  100 11.1M    0     0  10.3M      0  0:00:01  0:00:01 --:--:-- 10.3M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  9  138M    9 12.6M    0     0  12.8M      0  0:00:10 --:--:--  0:00:10 12.8M 21  138M   21 29.5M    0     0  14.9M      0  0:00:09  0:00:01  0:00:08 14.9M 29  138M   29 40.9M    0     0  13.7M      0  0:00:10  0:00:02  0:00:08 13.7M 38  138M   38 52.9M    0     0  13.2M      0  0:00:10  0:00:03  0:00:07 13.2M 46  138M   46 64.4M    0     0  12.9M      0  0:00:10  0:00:04  0:00:06 12.9M 52  138M   52 73.0M    0     0  11.8M      0  0:00:11  0:00:06  0:00:05 11.6M 55  138M   55 77.3M    0     0  11.0M      0  0:00:12  0:00:06  0:00:06 9788k 60  138M   60 84.4M    0     0  10.5M      0  0:00:13  0:00:07  0:00:06 8887k 64  138M   64 89.7M    0     0   9.9M      0  0:00:13  0:00:08  0:00:05 7529k 69  138M   69 95.6M    0     0  9811k      0  0:00:14  0:00:09  0:00:05 6394k 73  138M   73  101M    0     0  9443k      0  0:00:15  0:00:10  0:00:05 6027k 77  138M   77  107M    0     0  9187k      0  0:00:15  0:00:11  0:00:04 6176k 86  138M   86  120M    0     0  9458k      0  0:00:15  0:00:12  0:00:03 7282k 94  138M   94  131M    0     0  9635k      0  0:00:14  0:00:13  0:00:01 8579k100  138M  100  138M    0     0  9747k      0  0:00:14  0:00:14 --:--:-- 9607k
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
] Testing  RL18_DBG_F1_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```