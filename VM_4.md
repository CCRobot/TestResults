```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 72 11.1M   72 8208k    0     0  8005k      0  0:00:01  0:00:01 --:--:-- 8000k100 11.1M  100 11.1M    0     0  8870k      0  0:00:01  0:00:01 --:--:-- 8870k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  137M    4 5952k    0     0  8290k      0  0:00:16 --:--:--  0:00:16 8289k 13  137M   13 18.4M    0     0  10.7M      0  0:00:12  0:00:01  0:00:11 10.7M 22  137M   22 31.1M    0     0  11.4M      0  0:00:11  0:00:02  0:00:09 11.4M 29  137M   29 39.8M    0     0  10.7M      0  0:00:12  0:00:03  0:00:09 10.7M 39  137M   39 54.8M    0     0  11.6M      0  0:00:11  0:00:04  0:00:07 11.6M 50  137M   50 68.8M    0     0  12.0M      0  0:00:11  0:00:05  0:00:06 12.6M 59  137M   59 81.5M    0     0  12.1M      0  0:00:11  0:00:06  0:00:05 12.6M 66  137M   66 91.4M    0     0  11.8M      0  0:00:11  0:00:07  0:00:04 12.0M 74  137M   74  101M    0     0  11.6M      0  0:00:11  0:00:08  0:00:03 12.4M 82  137M   82  112M    0     0  11.6M      0  0:00:11  0:00:09  0:00:02 11.5M 91  137M   91  124M    0     0  11.6M      0  0:00:11  0:00:10  0:00:01 11.2M100  137M  100  137M    0     0  11.7M      0  0:00:11  0:00:11 --:--:-- 11.1M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   1c0c67e..9243fbc  master      -> origin/master
   c60cf51..a5a6b65  release/1.8 -> origin/release/1.8
   cfcbe3b..b244840  release/1.9 -> origin/release/1.9
Updating 1c0c67e..9243fbc
Fast-forward
 lib/Common/Exceptions/ReportError.h                |   1 +
 lib/Common/Exceptions/Throw.cpp                    |   8 +
 lib/Common/Exceptions/Throw.h                      |   4 +-
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
 15 files changed, 896 insertions(+), 838 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```