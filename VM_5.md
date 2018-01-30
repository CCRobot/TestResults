```
Executed on ubu16chk400000V
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  9168k      0  0:00:01  0:00:01 --:--:-- 9171k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  8  140M    8 12.0M    0     0  11.0M      0  0:00:12  0:00:01  0:00:11 11.0M 37  140M   37 52.0M    0     0  24.6M      0  0:00:05  0:00:02  0:00:03 24.6M 62  140M   62 88.0M    0     0  28.2M      0  0:00:04  0:00:03  0:00:01 28.2M 91  140M   91  128M    0     0  31.3M      0  0:00:04  0:00:04 --:--:-- 31.3M100  140M  100  140M    0     0  32.3M      0  0:00:04  0:00:04 --:--:-- 32.9M
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
] Testing  DEBUG_FLG1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```