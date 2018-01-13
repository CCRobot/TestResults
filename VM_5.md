```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  9374k      0  0:00:01  0:00:01 --:--:-- 9375k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  8  131M    8 11.2M    0     0  10.8M      0  0:00:12  0:00:01  0:00:11 10.8M 20  131M   20 27.0M    0     0  13.2M      0  0:00:09  0:00:02  0:00:07 13.2M 31  131M   31 41.3M    0     0  13.6M      0  0:00:09  0:00:03  0:00:06 13.6M 44  131M   44 59.0M    0     0  14.6M      0  0:00:09  0:00:04  0:00:05 14.5M 56  131M   56 73.9M    0     0  14.6M      0  0:00:08  0:00:05  0:00:03 14.8M 66  131M   66 87.4M    0     0  14.4M      0  0:00:09  0:00:06  0:00:03 15.2M 75  131M   75 99.7M    0     0  14.1M      0  0:00:09  0:00:07  0:00:02 14.5M 87  131M   87  115M    0     0  14.3M      0  0:00:09  0:00:08  0:00:01 14.7M 97  131M   97  128M    0     0  14.1M      0  0:00:09  0:00:09 --:--:-- 13.8M100  131M  100  131M    0     0  14.2M      0  0:00:09  0:00:09 --:--:-- 13.8M
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
] Testing  DEBUG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```