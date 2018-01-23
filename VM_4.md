```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 49 11.1M   49 5632k    0     0  5131k      0  0:00:02  0:00:01  0:00:01 5129k100 11.1M  100 11.1M    0     0  5501k      0  0:00:02  0:00:02 --:--:-- 5503k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  137M    2 2927k    0     0  2906k      0  0:00:48  0:00:01  0:00:47 2904k  4  137M    4 6480k    0     0  3227k      0  0:00:43  0:00:02  0:00:41 3227k 11  137M   11 16.1M    0     0  5497k      0  0:00:25  0:00:03  0:00:22 5496k 18  137M   18 24.9M    0     0  6358k      0  0:00:22  0:00:04  0:00:18 6358k 27  137M   27 37.3M    0     0  7641k      0  0:00:18  0:00:05  0:00:13 7655k 34  137M   34 47.1M    0     0  8037k      0  0:00:17  0:00:06  0:00:11 9072k 43  137M   43 58.9M    0     0  8615k      0  0:00:16  0:00:07  0:00:09 10.5M 54  137M   54 74.2M    0     0  9491k      0  0:00:14  0:00:08  0:00:06 11.6M 64  137M   64 89.0M    0     0   9.8M      0  0:00:13  0:00:09  0:00:04 12.8M 76  137M   76  104M    0     0  10.4M      0  0:00:13  0:00:10  0:00:03 13.4M 85  137M   85  117M    0     0  10.6M      0  0:00:12  0:00:11  0:00:01 14.1M 94  137M   94  129M    0     0  10.7M      0  0:00:12  0:00:12 --:--:-- 14.0M100  137M  100  137M    0     0  10.9M      0  0:00:12  0:00:12 --:--:-- 13.9M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   1c0c67e..bdae93e  master      -> origin/master
   c60cf51..a5a6b65  release/1.8 -> origin/release/1.8
   cfcbe3b..7318a88  release/1.9 -> origin/release/1.9
Updating 1c0c67e..bdae93e
Fast-forward
 lib/Common/Exceptions/ReportError.h                |   1 +
 lib/Common/Exceptions/Throw.cpp                    |   8 +
 lib/Common/Exceptions/Throw.h                      |   4 +-
 lib/Jsrt/Jsrt.cpp                                  |  91 ++---
 lib/Runtime/Base/FunctionBody.cpp                  |   6 +-
 lib/Runtime/Base/FunctionBody.h                    |   8 +
 lib/Runtime/Language/InterpreterStackFrame.cpp     |   1 +
 .../Library/EngineInterfaceObjectBuiltIns.h        |   1 +
 lib/Runtime/Library/JavascriptFunction.cpp         |  11 +-
 lib/Runtime/Library/JavascriptFunction.h           |   4 +-
 lib/Runtime/Library/JsBuiltIn/JsBuiltIn.js         |   1 +
 .../Library/JsBuiltIn/JsBuiltIn.js.bc.32b.h        | 428 +++++++++++----------
 .../Library/JsBuiltIn/JsBuiltIn.js.bc.64b.h        | 428 +++++++++++----------
 .../Library/JsBuiltIn/JsBuiltIn.js.nojit.bc.32b.h  | 406 +++++++++----------
 .../Library/JsBuiltIn/JsBuiltIn.js.nojit.bc.64b.h  | 406 +++++++++----------
 .../JsBuiltInEngineInterfaceExtensionObject.cpp    |  21 +-
 16 files changed, 943 insertions(+), 882 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RLS18_TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```