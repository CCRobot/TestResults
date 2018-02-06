```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 14 11.1M   14 1631k    0     0  2142k      0  0:00:05 --:--:--  0:00:05 2141k 53 11.1M   53 6128k    0     0  3482k      0  0:00:03  0:00:01  0:00:02 3481k100 11.1M  100 11.1M    0     0  4149k      0  0:00:02  0:00:02 --:--:-- 4150k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  145M    2 3967k    0     0  3957k      0  0:00:37  0:00:01  0:00:36 3955k  5  145M    5 8560k    0     0  4272k      0  0:00:34  0:00:02  0:00:32 4271k  9  145M    9 13.5M    0     0  4622k      0  0:00:32  0:00:03  0:00:29 4621k 15  145M   15 22.3M    0     0  5703k      0  0:00:26  0:00:04  0:00:22 5702k 22  145M   22 32.1M    0     0  6584k      0  0:00:22  0:00:05  0:00:17 6590k 30  145M   30 44.0M    0     0  7513k      0  0:00:19  0:00:06  0:00:13 8227k 38  145M   38 56.2M    0     0  8228k      0  0:00:18  0:00:07  0:00:11 9813k 44  145M   44 64.0M    0     0  8198k      0  0:00:18  0:00:08  0:00:10 10.1M 52  145M   52 76.2M    0     0  8671k      0  0:00:17  0:00:09  0:00:08 10.7M 58  145M   58 85.4M    0     0  8749k      0  0:00:16  0:00:10  0:00:06 10.6M 66  145M   66 97.2M    0     0  9055k      0  0:00:16  0:00:11  0:00:05 10.6M 74  145M   74  108M    0     0  9259k      0  0:00:16  0:00:12  0:00:04 10.4M 84  145M   84  122M    0     0  9651k      0  0:00:15  0:00:13  0:00:02 11.6M 92  145M   92  134M    0     0  9816k      0  0:00:15  0:00:14  0:00:01 11.6M 98  145M   98  142M    0     0  9728k      0  0:00:15  0:00:15 --:--:-- 11.4M100  145M  100  145M    0     0  9728k      0  0:00:15  0:00:15 --:--:-- 11.1M
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
] Testing  RLS18_TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```