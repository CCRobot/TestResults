```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 59 11.1M   59 6800k    0     0  7690k      0  0:00:01 --:--:--  0:00:01 7683k100 11.1M  100 11.1M    0     0  8716k      0  0:00:01  0:00:01 --:--:-- 8721k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  137M    2 3823k    0     0  6831k      0  0:00:20 --:--:--  0:00:20 6827k 12  137M   12 17.5M    0     0  11.2M      0  0:00:12  0:00:01  0:00:11 11.2M 22  137M   22 30.8M    0     0  12.0M      0  0:00:11  0:00:02  0:00:09 12.0M 29  137M   29 40.5M    0     0  11.4M      0  0:00:12  0:00:03  0:00:09 11.4M 37  137M   37 51.6M    0     0  11.3M      0  0:00:12  0:00:04  0:00:08 11.3M 45  137M   45 62.5M    0     0  11.2M      0  0:00:12  0:00:05  0:00:07 11.7M 54  137M   54 74.1M    0     0  11.3M      0  0:00:12  0:00:06  0:00:06 11.3M 63  137M   63 86.6M    0     0  11.4M      0  0:00:11  0:00:07  0:00:04 11.1M 68  137M   68 94.0M    0     0  10.9M      0  0:00:12  0:00:08  0:00:04 10.6M 75  137M   75  103M    0     0  10.7M      0  0:00:12  0:00:09  0:00:03 10.2M 83  137M   83  114M    0     0  10.8M      0  0:00:12  0:00:10  0:00:02 10.4M 92  137M   92  126M    0     0  10.9M      0  0:00:12  0:00:11  0:00:01 10.4M100  137M  100  137M    0     0  11.0M      0  0:00:12  0:00:12 --:--:-- 10.4M
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
] Testing  RL18_PACK
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```