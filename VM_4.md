```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 71 11.1M   71 8160k    0     0  8434k      0  0:00:01 --:--:--  0:00:01 8429k100 11.1M  100 11.1M    0     0  8759k      0  0:00:01  0:00:01 --:--:-- 8761k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  145M    3 4960k    0     0  7672k      0  0:00:19 --:--:--  0:00:19 7666k 11  145M   11 16.4M    0     0   9.9M      0  0:00:14  0:00:01  0:00:13  9.9M 19  145M   19 27.9M    0     0  10.5M      0  0:00:13  0:00:02  0:00:11 10.5M 24  145M   24 36.2M    0     0   9.9M      0  0:00:14  0:00:03  0:00:11  9.9M 33  145M   33 48.0M    0     0  10.3M      0  0:00:14  0:00:04  0:00:10 10.3M 40  145M   40 59.2M    0     0  10.5M      0  0:00:13  0:00:05  0:00:08 10.8M 50  145M   50 73.9M    0     0  11.1M      0  0:00:13  0:00:06  0:00:07 11.5M 60  145M   60 87.2M    0     0  11.4M      0  0:00:12  0:00:07  0:00:05 11.8M 68  145M   68  100M    0     0  11.5M      0  0:00:12  0:00:08  0:00:04 12.7M 77  145M   77  113M    0     0  11.7M      0  0:00:12  0:00:09  0:00:03 13.0M 88  145M   88  127M    0     0  12.0M      0  0:00:12  0:00:10  0:00:02 13.7M 96  145M   96  140M    0     0  12.0M      0  0:00:12  0:00:11  0:00:01 13.2M100  145M  100  145M    0     0  11.9M      0  0:00:12  0:00:12 --:--:-- 12.8M
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
] Testing  RL18_DBG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```