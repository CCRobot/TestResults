```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 63 11.1M   63 7248k    0     0  7180k      0  0:00:01  0:00:01 --:--:-- 7176k100 11.1M  100 11.1M    0     0  8079k      0  0:00:01  0:00:01 --:--:-- 8077k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  145M    3 4976k    0     0  8577k      0  0:00:17 --:--:--  0:00:17 8564k 11  145M   11 16.7M    0     0  10.5M      0  0:00:13  0:00:01  0:00:12 10.5M 18  145M   18 27.3M    0     0  10.5M      0  0:00:13  0:00:02  0:00:11 10.5M 27  145M   27 40.4M    0     0  11.2M      0  0:00:12  0:00:03  0:00:09 11.2M 33  145M   33 48.7M    0     0  10.6M      0  0:00:13  0:00:04  0:00:09 10.6M 41  145M   41 60.0M    0     0  10.7M      0  0:00:13  0:00:05  0:00:08 11.0M 48  145M   48 69.8M    0     0  10.6M      0  0:00:13  0:00:06  0:00:07 10.6M 55  145M   55 79.9M    0     0  10.5M      0  0:00:13  0:00:07  0:00:06 10.5M 59  145M   59 87.0M    0     0  10.1M      0  0:00:14  0:00:08  0:00:06 9540k 68  145M   68 99.2M    0     0  10.3M      0  0:00:14  0:00:09  0:00:05 10.0M 78  145M   78  113M    0     0  10.7M      0  0:00:13  0:00:10  0:00:03 10.8M 88  145M   88  129M    0     0  11.1M      0  0:00:13  0:00:11  0:00:02 11.8M 98  145M   98  142M    0     0  11.3M      0  0:00:12  0:00:12 --:--:-- 12.6M100  145M  100  145M    0     0  11.4M      0  0:00:12  0:00:12 --:--:-- 14.0M
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
] Testing  RL18_PACK
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```