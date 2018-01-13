```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 11 11.1M   11 1295k    0     0  3382k      0  0:00:03 --:--:--  0:00:03 3382k 97 11.1M   97 10.8M    0     0  8007k      0  0:00:01  0:00:01 --:--:-- 8005k100 11.1M  100 11.1M    0     0  8132k      0  0:00:01  0:00:01 --:--:-- 8129k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  9  131M    9 12.7M    0     0  13.2M      0  0:00:09 --:--:--  0:00:09 13.2M 18  131M   18 24.2M    0     0  12.3M      0  0:00:10  0:00:01  0:00:09 12.3M 27  131M   27 35.8M    0     0  12.0M      0  0:00:10  0:00:02  0:00:08 12.0M 35  131M   35 46.9M    0     0  11.8M      0  0:00:11  0:00:03  0:00:08 11.8M 40  131M   40 53.2M    0     0  10.7M      0  0:00:12  0:00:04  0:00:08 10.7M 46  131M   46 61.4M    0     0  10.2M      0  0:00:12  0:00:05  0:00:07 9966k 54  131M   54 72.0M    0     0  10.3M      0  0:00:12  0:00:06  0:00:06 9788k 62  131M   62 81.9M    0     0  10.2M      0  0:00:12  0:00:07  0:00:05 9446k 68  131M   68 90.6M    0     0  10.1M      0  0:00:12  0:00:08  0:00:04 8952k 75  131M   75 99.7M    0     0  10.0M      0  0:00:13  0:00:09  0:00:04 9518k 82  131M   82  108M    0     0   9.8M      0  0:00:13  0:00:10  0:00:03 9532k 88  131M   88  116M    0     0   9.7M      0  0:00:13  0:00:11  0:00:02 9182k 94  131M   94  124M    0     0  9826k      0  0:00:13  0:00:12  0:00:01 8695k100  131M  100  131M    0     0  9871k      0  0:00:13  0:00:13 --:--:-- 8942k
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
] Testing  DEBUG_FLG2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```