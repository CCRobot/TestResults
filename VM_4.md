```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 45 11.1M   45 5184k    0     0  9061k      0  0:00:01 --:--:--  0:00:01 9047k100 11.1M  100 11.1M    0     0  11.4M      0 --:--:-- --:--:-- --:--:-- 11.3M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  131M    3 5216k    0     0  8906k      0  0:00:15 --:--:--  0:00:15 8901k 12  131M   12 16.2M    0     0  10.2M      0  0:00:12  0:00:01  0:00:11 10.2M 20  131M   20 27.2M    0     0  10.5M      0  0:00:12  0:00:02  0:00:10 10.5M 28  131M   28 37.4M    0     0  10.4M      0  0:00:12  0:00:03  0:00:09 10.4M 38  131M   38 50.3M    0     0  10.9M      0  0:00:11  0:00:04  0:00:07 10.9M 48  131M   48 64.0M    0     0  11.4M      0  0:00:11  0:00:05  0:00:06 11.7M 59  131M   59 78.3M    0     0  11.9M      0  0:00:11  0:00:06  0:00:05 12.4M 69  131M   69 91.5M    0     0  12.0M      0  0:00:10  0:00:07  0:00:03 12.8M 78  131M   78  103M    0     0  12.0M      0  0:00:10  0:00:08  0:00:02 13.2M 90  131M   90  119M    0     0  12.4M      0  0:00:10  0:00:09  0:00:01 13.7M 93  131M   93  122M    0     0  11.5M      0  0:00:11  0:00:10  0:00:01 11.7M 97  131M   97  127M    0     0  11.0M      0  0:00:11  0:00:11 --:--:--  9.8M100  131M  100  131M    0     0  10.7M      0  0:00:12  0:00:12 --:--:-- 8793k
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
] Testing  RL18_DBG_F2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```