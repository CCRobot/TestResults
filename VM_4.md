```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 17 11.1M   17 2015k    0     0  1917k      0  0:00:05  0:00:01  0:00:04 1915k100 11.1M  100 11.1M    0     0  6479k      0  0:00:01  0:00:01 --:--:-- 6477k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  145M    0 1455k    0     0  5287k      0  0:00:28 --:--:--  0:00:28 5273k  8  145M    8 12.9M    0     0  10.1M      0  0:00:14  0:00:01  0:00:13 10.1M 15  145M   15 22.7M    0     0  10.0M      0  0:00:14  0:00:02  0:00:12 10.0M 22  145M   22 32.2M    0     0   9.8M      0  0:00:14  0:00:03  0:00:11  9.8M 28  145M   28 40.9M    0     0  9821k      0  0:00:15  0:00:04  0:00:11 9819k 35  145M   35 51.3M    0     0  9974k      0  0:00:14  0:00:05  0:00:09  9.9M 41  145M   41 60.4M    0     0  9855k      0  0:00:15  0:00:06  0:00:09 9722k 48  145M   48 69.9M    0     0  9854k      0  0:00:15  0:00:07  0:00:08 9671k 56  145M   56 81.6M    0     0   9.8M      0  0:00:14  0:00:08  0:00:06  9.8M 64  145M   64 94.2M    0     0  10.1M      0  0:00:14  0:00:09  0:00:05 10.6M 73  145M   73  106M    0     0  10.3M      0  0:00:14  0:00:10  0:00:04 10.9M 82  145M   82  119M    0     0  10.6M      0  0:00:13  0:00:11  0:00:02 11.9M 90  145M   90  132M    0     0  10.7M      0  0:00:13  0:00:12  0:00:01 12.4M 99  145M   99  144M    0     0  10.9M      0  0:00:13  0:00:13 --:--:-- 12.6M100  145M  100  145M    0     0  10.9M      0  0:00:13  0:00:13 --:--:-- 12.6M
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
] Testing  RL18_DBG_F2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```