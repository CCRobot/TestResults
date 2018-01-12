```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 32 11.1M   32 3711k    0     0  5207k      0  0:00:02 --:--:--  0:00:02 5205k100 11.1M  100 11.1M    0     0  9103k      0  0:00:01  0:00:01 --:--:-- 9105k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  131M    1 1583k    0     0  4381k      0  0:00:30 --:--:--  0:00:30 4374k 11  131M   11 15.0M    0     0  11.0M      0  0:00:11  0:00:01  0:00:10 11.0M 20  131M   20 27.5M    0     0  11.6M      0  0:00:11  0:00:02  0:00:09 11.6M 30  131M   30 39.6M    0     0  11.8M      0  0:00:11  0:00:03  0:00:08 11.8M 37  131M   37 49.3M    0     0  11.3M      0  0:00:11  0:00:04  0:00:07 11.3M 45  131M   45 59.5M    0     0  11.1M      0  0:00:11  0:00:05  0:00:06 11.6M 52  131M   52 68.5M    0     0  10.7M      0  0:00:12  0:00:06  0:00:06 10.7M 58  131M   58 76.6M    0     0  10.3M      0  0:00:12  0:00:07  0:00:05  9.7M 64  131M   64 84.7M    0     0  10.1M      0  0:00:12  0:00:08  0:00:04 9223k 70  131M   70 92.7M    0     0   9.9M      0  0:00:13  0:00:09  0:00:04 8893k 81  131M   81  106M    0     0  10.2M      0  0:00:12  0:00:10  0:00:02 9630k 89  131M   89  117M    0     0  10.3M      0  0:00:12  0:00:11  0:00:01  9.7M 99  131M   99  130M    0     0  10.5M      0  0:00:12  0:00:12 --:--:-- 10.7M100  131M  100  131M    0     0  10.5M      0  0:00:12  0:00:12 --:--:-- 11.4M
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
] Testing  RLS18_TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```