```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 31 11.1M   31 3551k    0     0  6137k      0  0:00:01 --:--:--  0:00:01 6134k100 11.1M  100 11.1M    0     0  9982k      0  0:00:01  0:00:01 --:--:-- 9983k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  131M    1 1903k    0     0  4505k      0  0:00:29 --:--:--  0:00:29 4500k 10  131M   10 14.1M    0     0   9.9M      0  0:00:13  0:00:01  0:00:12  9.9M 18  131M   18 23.7M    0     0   9.7M      0  0:00:13  0:00:02  0:00:11  9.7M 24  131M   24 32.0M    0     0  9539k      0  0:00:14  0:00:03  0:00:11 9538k 29  131M   29 38.9M    0     0  9023k      0  0:00:14  0:00:04  0:00:10 9023k 40  131M   40 53.1M    0     0   9.7M      0  0:00:13  0:00:05  0:00:08 10.2M 48  131M   48 63.2M    0     0   9.8M      0  0:00:13  0:00:06  0:00:07  9.8M 57  131M   57 75.7M    0     0  10.1M      0  0:00:12  0:00:07  0:00:05 10.3M 66  131M   66 87.4M    0     0  10.3M      0  0:00:12  0:00:08  0:00:04 11.1M 75  131M   75 99.8M    0     0  10.5M      0  0:00:12  0:00:09  0:00:03 12.1M 85  131M   85  112M    0     0  10.7M      0  0:00:12  0:00:10  0:00:02 11.7M 94  131M   94  124M    0     0  10.8M      0  0:00:12  0:00:11  0:00:01 12.1M 99  131M   99  130M    0     0  10.5M      0  0:00:12  0:00:12 --:--:-- 10.9M100  131M  100  131M    0     0  10.5M      0  0:00:12  0:00:12 --:--:-- 10.7M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   79df905..1bddcb4  master      -> origin/master
   b5cf4ec..59932fe  release/1.8 -> origin/release/1.8
Updating 79df905..1bddcb4
Fast-forward
 lib/Runtime/Language/JavascriptOperators.cpp       |   18 +-
 lib/Runtime/Library/InJavascript/Intl.js           |    4 +-
 lib/Runtime/Library/InJavascript/Intl.js.bc.32b.h  | 4125 ++++++++++----------
 lib/Runtime/Library/InJavascript/Intl.js.bc.64b.h  | 4125 ++++++++++----------
 .../Library/InJavascript/Intl.js.nojit.bc.32b.h    | 3721 +++++++++---------
 .../Library/InJavascript/Intl.js.nojit.bc.64b.h    | 3721 +++++++++---------
 test/Intl/DateTimeFormatOptions.js                 |    5 +
 7 files changed, 7865 insertions(+), 7854 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```