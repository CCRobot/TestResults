```
Executed on ubu16chk400000U
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  8999k      0  0:00:01  0:00:01 --:--:-- 9000k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  140M    0 32345    0     0  95182      0  0:25:45 --:--:--  0:25:45 95132 14  140M   14 20.1M    0     0  15.2M      0  0:00:09  0:00:01  0:00:08 15.2M 44  140M   44 62.9M    0     0  27.0M      0  0:00:05  0:00:02  0:00:03 27.0M 73  140M   73  103M    0     0  31.0M      0  0:00:04  0:00:03  0:00:01 31.0M100  140M  100  140M    0     0  33.2M      0  0:00:04  0:00:04 --:--:-- 33.2M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   9c435c9..4070f8d  master     -> origin/master
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
] Testing  NODE_BUILD_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```