```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 56 11.1M   56 6400k    0     0  7492k      0  0:00:01 --:--:--  0:00:01 7485k100 11.1M  100 11.1M    0     0  9817k      0  0:00:01  0:00:01 --:--:-- 9819k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  140M    4 6288k    0     0  9316k      0  0:00:15 --:--:--  0:00:15 9315k 13  140M   13 18.6M    0     0  11.1M      0  0:00:12  0:00:01  0:00:11 11.1M 22  140M   22 31.1M    0     0  11.6M      0  0:00:12  0:00:02  0:00:10 11.6M 30  140M   30 43.2M    0     0  11.7M      0  0:00:11  0:00:03  0:00:08 11.7M 39  140M   39 55.5M    0     0  11.8M      0  0:00:11  0:00:04  0:00:07 11.8M 48  140M   48 68.4M    0     0  12.0M      0  0:00:11  0:00:05  0:00:06 12.4M 56  140M   56 79.2M    0     0  11.8M      0  0:00:11  0:00:06  0:00:05 12.1M 66  140M   66 93.6M    0     0  12.2M      0  0:00:11  0:00:07  0:00:04 12.5M 75  140M   75  106M    0     0  12.2M      0  0:00:11  0:00:08  0:00:03 12.5M 82  140M   82  116M    0     0  11.9M      0  0:00:11  0:00:09  0:00:02 12.0M 89  140M   89  126M    0     0  11.8M      0  0:00:11  0:00:10  0:00:01 11.5M 98  140M   98  138M    0     0  11.8M      0  0:00:11  0:00:11 --:--:-- 11.9M100  140M  100  140M    0     0  11.9M      0  0:00:11  0:00:11 --:--:-- 11.3M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   9c435c9..4070f8d  master      -> origin/master
   3e52c09..17fcf4a  release/1.8 -> origin/release/1.8
   abd18d0..0615a51  release/1.9 -> origin/release/1.9
Updating 9c435c9..4070f8d
Fast-forward
 lib/Jsrt/Jsrt.cpp                                  |   22 +-
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
 18 files changed, 2855 insertions(+), 8353 deletions(-)
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
] Testing  NODE_BUILD_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```