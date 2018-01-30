```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 35 11.1M   35 4096k    0     0  6900k      0  0:00:01 --:--:--  0:00:01 6895k100 11.1M  100 11.1M    0     0  9592k      0  0:00:01  0:00:01 --:--:-- 9596k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  140M    2 3487k    0     0  9122k      0  0:00:15 --:--:--  0:00:15 9105k 14  140M   14 20.0M    0     0  14.5M      0  0:00:09  0:00:01  0:00:08 14.5M 24  140M   24 34.5M    0     0  14.4M      0  0:00:09  0:00:02  0:00:07 14.4M 32  140M   32 46.2M    0     0  13.6M      0  0:00:10  0:00:03  0:00:07 13.6M 41  140M   41 58.7M    0     0  13.4M      0  0:00:10  0:00:04  0:00:06 13.4M 48  140M   48 68.5M    0     0  12.7M      0  0:00:11  0:00:05  0:00:06 13.0M 59  140M   59 83.8M    0     0  13.1M      0  0:00:10  0:00:06  0:00:04 12.7M 71  140M   71  100M    0     0  13.5M      0  0:00:10  0:00:07  0:00:03 13.1M 82  140M   82  116M    0     0  13.8M      0  0:00:10  0:00:08  0:00:02 13.9M 94  140M   94  132M    0     0  14.0M      0  0:00:09  0:00:09 --:--:-- 14.6M100  140M  100  140M    0     0  14.2M      0  0:00:09  0:00:09 --:--:-- 16.0M
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
] Testing  DEBUG_FLG1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```