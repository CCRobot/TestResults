```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 65 11.1M   65 7424k    0     0  7194k      0  0:00:01  0:00:01 --:--:-- 7193k100 11.1M  100 11.1M    0     0  8179k      0  0:00:01  0:00:01 --:--:-- 8176k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  145M    3 5872k    0     0  9390k      0  0:00:15 --:--:--  0:00:15 9380k 15  145M   15 21.9M    0     0  13.5M      0  0:00:10  0:00:01  0:00:09 13.5M 23  145M   23 33.6M    0     0  12.8M      0  0:00:11  0:00:02  0:00:09 12.8M 28  145M   28 41.8M    0     0  11.5M      0  0:00:12  0:00:03  0:00:09 11.5M 36  145M   36 53.5M    0     0  11.5M      0  0:00:12  0:00:04  0:00:08 11.5M 43  145M   43 63.7M    0     0  11.3M      0  0:00:12  0:00:05  0:00:07 11.6M 50  145M   50 73.9M    0     0  11.1M      0  0:00:13  0:00:06  0:00:07 10.3M 58  145M   58 84.9M    0     0  11.1M      0  0:00:13  0:00:07  0:00:06 10.2M 65  145M   65 95.3M    0     0  10.6M      0  0:00:13  0:00:08  0:00:05 10.0M 71  145M   71  104M    0     0  10.8M      0  0:00:13  0:00:09  0:00:04 10.1M 81  145M   81  117M    0     0  11.0M      0  0:00:13  0:00:10  0:00:03 10.8M 91  145M   91  132M    0     0  11.4M      0  0:00:12  0:00:11  0:00:01 11.7M 97  145M   97  140M    0     0  11.1M      0  0:00:13  0:00:12  0:00:01 11.2M100  145M  100  145M    0     0  11.0M      0  0:00:13  0:00:13 --:--:-- 11.9M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   a48d5fc..215b215  master      -> origin/master
   c1970eb..7aef2f4  intl-icu    -> origin/intl-icu
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
] Testing  RL18_DBG_F1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```