```
Executed on ubu16chk400001A
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 10 9180k   10  975k    0     0  1380k      0  0:00:06 --:--:--  0:00:06 1379k100 9180k  100 9180k    0     0  8692k      0  0:00:01  0:00:01 --:--:-- 8694k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  145M    0  847k    0     0  1344k      0  0:01:50 --:--:--  0:01:50 1343k 22  145M   22 32.0M    0     0  19.3M      0  0:00:07  0:00:01  0:00:06 19.3M 52  145M   52 75.6M    0     0  28.7M      0  0:00:05  0:00:02  0:00:03 28.7M 79  145M   79  116M    0     0  31.8M      0  0:00:04  0:00:03  0:00:01 31.8M100  145M  100  145M    0     0  33.8M      0  0:00:04  0:00:04 --:--:-- 33.8M
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
] Testing  RL18_DBG_F2_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```