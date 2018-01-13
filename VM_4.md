```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 69 11.1M   69 7936k    0     0  10.1M      0  0:00:01 --:--:--  0:00:01 10.0M100 11.1M  100 11.1M    0     0  11.0M      0  0:00:01  0:00:01 --:--:-- 11.0M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  131M    5 6880k    0     0  9337k      0  0:00:14 --:--:--  0:00:14 9335k 16  131M   16 21.0M    0     0  12.1M      0  0:00:10  0:00:01  0:00:09 12.1M 27  131M   27 36.3M    0     0  13.2M      0  0:00:09  0:00:02  0:00:07 13.2M 37  131M   37 49.8M    0     0  13.3M      0  0:00:09  0:00:03  0:00:06 13.3M 49  131M   49 64.9M    0     0  13.7M      0  0:00:09  0:00:04  0:00:05 13.7M 60  131M   60 79.7M    0     0  13.9M      0  0:00:09  0:00:05  0:00:04 14.6M 71  131M   71 93.6M    0     0  13.8M      0  0:00:09  0:00:06  0:00:03 14.5M 82  131M   82  108M    0     0  13.9M      0  0:00:09  0:00:07  0:00:02 14.3M 94  131M   94  124M    0     0  14.1M      0  0:00:09  0:00:08  0:00:01 14.8M100  131M  100  131M    0     0  14.3M      0  0:00:09  0:00:09 --:--:-- 15.0M
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
] Testing  NODE_BUILD_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```