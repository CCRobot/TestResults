```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  10.5M      0  0:00:01  0:00:01 --:--:-- 10.5M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 10  131M   10 14.0M    0     0  13.0M      0  0:00:10  0:00:01  0:00:09 13.0M 22  131M   22 29.1M    0     0  14.0M      0  0:00:09  0:00:02  0:00:07 14.0M 35  131M   35 46.5M    0     0  15.1M      0  0:00:08  0:00:03  0:00:05 15.1M 47  131M   47 62.6M    0     0  15.3M      0  0:00:08  0:00:04  0:00:04 15.3M 60  131M   60 79.8M    0     0  15.7M      0  0:00:08  0:00:05  0:00:03 16.0M 72  131M   72 95.5M    0     0  15.7M      0  0:00:08  0:00:06  0:00:02 16.3M 83  131M   83  109M    0     0  15.5M      0  0:00:08  0:00:07  0:00:01 16.1M 94  131M   94  124M    0     0  15.4M      0  0:00:08  0:00:08 --:--:-- 15.6M100  131M  100  131M    0     0  15.5M      0  0:00:08  0:00:08 --:--:-- 15.7M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   79df905..117c750  master      -> origin/master
   b5cf4ec..4ec28f9  release/1.8 -> origin/release/1.8
Updating 79df905..117c750
Fast-forward
 bin/ch/MessageQueue.h                              |   13 +-
 bin/ch/WScriptJsrt.cpp                             |    5 +-
 lib/Runtime/Base/PropertyRecord.h                  |   13 +-
 lib/Runtime/Language/JavascriptOperators.cpp       |   18 +-
 lib/Runtime/Library/InJavascript/Intl.js           |    4 +-
 lib/Runtime/Library/InJavascript/Intl.js.bc.32b.h  | 4125 ++++++++++----------
 lib/Runtime/Library/InJavascript/Intl.js.bc.64b.h  | 4125 ++++++++++----------
 .../Library/InJavascript/Intl.js.nojit.bc.32b.h    | 3721 +++++++++---------
 .../Library/InJavascript/Intl.js.nojit.bc.64b.h    | 3721 +++++++++---------
 lib/Runtime/Library/JavascriptError.cpp            |    1 +
 test/Intl/DateTimeFormatOptions.js                 |    5 +
 test/Object/rlexe.xml                              |    1 +
 test/es6/module-bugfixes.js                        |   12 +
 test/es6/rlexe.xml                                 |    2 +-
 test/wasm/rlexe.xml                                |    3 +-
 15 files changed, 7898 insertions(+), 7871 deletions(-)
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