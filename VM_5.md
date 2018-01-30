```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 35 11.1M   35 4047k    0     0  8761k      0  0:00:01 --:--:--  0:00:01 8761k100 11.1M  100 11.1M    0     0  10.8M      0  0:00:01  0:00:01 --:--:-- 10.8M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  140M    1 2383k    0     0  5931k      0  0:00:24 --:--:--  0:00:24 5929k 11  140M   11 16.1M    0     0  11.5M      0  0:00:12  0:00:01  0:00:11 11.5M 23  140M   23 32.2M    0     0  13.4M      0  0:00:10  0:00:02  0:00:08 13.4M 32  140M   32 45.6M    0     0  13.4M      0  0:00:10  0:00:03  0:00:07 13.4M 43  140M   43 60.6M    0     0  13.7M      0  0:00:10  0:00:04  0:00:06 13.7M 52  140M   52 74.2M    0     0  13.7M      0  0:00:10  0:00:05  0:00:05 14.3M 64  140M   64 90.5M    0     0  14.1M      0  0:00:09  0:00:06  0:00:03 14.8M 74  140M   74  105M    0     0  14.1M      0  0:00:09  0:00:07  0:00:02 14.5M 84  140M   84  118M    0     0  14.0M      0  0:00:09  0:00:08  0:00:01 14.4M 93  140M   93  131M    0     0  14.0M      0  0:00:10  0:00:09  0:00:01 14.2M100  140M  100  140M    0     0  14.0M      0  0:00:09  0:00:09 --:--:-- 14.5M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   9c435c9..ed21221  master      -> origin/master
   3e52c09..17fcf4a  release/1.8 -> origin/release/1.8
   abd18d0..172bac8  release/1.9 -> origin/release/1.9
Updating 9c435c9..ed21221
Fast-forward
 lib/Jsrt/Jsrt.cpp                                  |   57 +-
 lib/Jsrt/JsrtDiag.cpp                              |   10 +-
 .../Library/JavascriptRegExpConstructor.cpp        |   39 +-
 lib/Runtime/Library/JavascriptRegExpConstructor.h  |    2 +
 lib/Runtime/Library/RegexHelper.cpp                |   19 +-
 lib/Runtime/Library/RegexHelper.h                  |    2 +
 test/Date/parseISO.baseline                        | 7899 --------------------
 test/Date/parseISO.js                              |  432 --
 test/Date/parseInvalidISO.baseline                 |  329 +
 test/Date/parseInvalidISO.js                       |  231 +
 test/Date/parseValidISO.baseline                   | 1891 +++++
 test/Date/parseValidISO.js                         |  227 +
 test/Date/rlexe.xml                                |   28 +-
 test/Debugger/emptyJson.dbg.baseline               |    1 +
 test/Debugger/loadscript_after_detach.js           |   17 +
 test/Debugger/rlexe.xml                            |    6 +
 test/Regex/bug_OS14763260.js                       |   47 +
 test/Regex/rlexe.xml                               |    6 +
 18 files changed, 2882 insertions(+), 8361 deletions(-)
 delete mode 100644 test/Date/parseISO.baseline
 delete mode 100644 test/Date/parseISO.js
 create mode 100644 test/Date/parseInvalidISO.baseline
 create mode 100644 test/Date/parseInvalidISO.js
 create mode 100644 test/Date/parseValidISO.baseline
 create mode 100644 test/Date/parseValidISO.js
 create mode 100644 test/Debugger/emptyJson.dbg.baseline
 create mode 100644 test/Debugger/loadscript_after_detach.js
 create mode 100644 test/Regex/bug_OS14763260.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```