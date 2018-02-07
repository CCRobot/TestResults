```
Executed on ubu16chk400001B
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1 9180k    1  175k    0     0   351k      0  0:00:26 --:--:--  0:00:26  351k100 9180k  100 9180k    0     0  9180k      0  0:00:01  0:00:01 --:--:-- 9180k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  145M    0  191k    0     0   401k      0  0:06:10 --:--:--  0:06:10  401k 16  145M   16 24.0M    0     0  16.2M      0  0:00:08  0:00:01  0:00:07 16.2M 43  145M   43 63.7M    0     0  25.7M      0  0:00:05  0:00:02  0:00:03 25.7M 69  145M   69  101M    0     0  29.3M      0  0:00:04  0:00:03  0:00:01 29.2M 82  145M   82  120M    0     0  26.4M      0  0:00:05  0:00:04  0:00:01 26.4M100  145M  100  145M    0     0  27.6M      0  0:00:05  0:00:05 --:--:-- 30.4M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   a48d5fc..215b215  master     -> origin/master
   c1970eb..7aef2f4  intl-icu   -> origin/intl-icu
   2106305..dbce2eb  release/1.8 -> origin/release/1.8
   86e6e5c..e4493a2  release/1.9 -> origin/release/1.9
Updating a48d5fc..215b215
Fast-forward
 lib/Common/Codex/Utf8Helper.h           |  36 +++++------
 lib/JITClient/JITManager.cpp            |  13 ++--
 lib/JITClient/JITManager.h              |   1 +
 lib/Jsrt/Jsrt.cpp                       |   2 +-
 lib/Parser/RegexParser.cpp              |  18 +++++-
 lib/Runtime/Library/ConcatString.cpp    |  10 +--
 lib/Runtime/Library/WabtInterface.cpp   |   8 +--
 test/Regex/unicode_forbidden_escapes.js | 111 +++++++++++++++++++++++++++-----
 8 files changed, 147 insertions(+), 52 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_F1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```