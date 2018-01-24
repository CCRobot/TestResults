```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 58 11.1M   58 6656k    0     0  8584k      0  0:00:01 --:--:--  0:00:01 8577k100 11.1M  100 11.1M    0     0   9.8M      0  0:00:01  0:00:01 --:--:--  9.8M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  137M    4 6544k    0     0  10.1M      0  0:00:13 --:--:--  0:00:13 10.1M 17  137M   17 24.0M    0     0  14.7M      0  0:00:09  0:00:01  0:00:08 14.7M 26  137M   26 35.8M    0     0  13.6M      0  0:00:10  0:00:02  0:00:08 13.6M 33  137M   33 45.6M    0     0  12.5M      0  0:00:10  0:00:03  0:00:07 12.5M 42  137M   42 57.9M    0     0  12.5M      0  0:00:10  0:00:04  0:00:06 12.5M 51  137M   51 69.9M    0     0  12.4M      0  0:00:11  0:00:05  0:00:06 12.7M 59  137M   59 81.9M    0     0  12.3M      0  0:00:11  0:00:06  0:00:05 11.5M 66  137M   66 91.7M    0     0  12.0M      0  0:00:11  0:00:07  0:00:04 11.1M 75  137M   75  103M    0     0  11.9M      0  0:00:11  0:00:08  0:00:03 11.5M 84  137M   84  116M    0     0  12.0M      0  0:00:11  0:00:09  0:00:02 11.6M 96  137M   96  131M    0     0  12.3M      0  0:00:11  0:00:10  0:00:01 12.3M100  137M  100  137M    0     0  12.5M      0  0:00:10  0:00:10 --:--:-- 12.7M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   1c0c67e..962346b  master      -> origin/master
   c60cf51..a5a6b65  release/1.8 -> origin/release/1.8
   cfcbe3b..fdd885b  release/1.9 -> origin/release/1.9
Updating 1c0c67e..962346b
Fast-forward
 lib/Common/Exceptions/ReportError.h                |   1 +
 lib/Common/Exceptions/Throw.cpp                    |   8 +
 lib/Common/Exceptions/Throw.h                      |   4 +-
 lib/Jsrt/Jsrt.cpp                                  |  99 ++---
 lib/Runtime/Base/FunctionBody.cpp                  |   6 +-
 lib/Runtime/Base/FunctionBody.h                    |   8 +
 lib/Runtime/Debug/TTActionEvents.cpp               |  30 +-
 lib/Runtime/Debug/TTEventLog.cpp                   |  11 +-
 lib/Runtime/Debug/TTEventLog.h                     |   2 +-
 lib/Runtime/Language/InterpreterStackFrame.cpp     |   1 +
 .../Library/EngineInterfaceObjectBuiltIns.h        |   1 +
 lib/Runtime/Library/JavascriptFunction.cpp         |  11 +-
 lib/Runtime/Library/JavascriptFunction.h           |   4 +-
 lib/Runtime/Library/JavascriptLibrary.cpp          |   6 -
 lib/Runtime/Library/JavascriptLibrary.h            |   1 -
 lib/Runtime/Library/JsBuiltIn/JsBuiltIn.js         |   1 +
 .../Library/JsBuiltIn/JsBuiltIn.js.bc.32b.h        | 428 +++++++++++----------
 .../Library/JsBuiltIn/JsBuiltIn.js.bc.64b.h        | 428 +++++++++++----------
 .../Library/JsBuiltIn/JsBuiltIn.js.nojit.bc.32b.h  | 406 +++++++++----------
 .../Library/JsBuiltIn/JsBuiltIn.js.nojit.bc.64b.h  | 406 +++++++++----------
 .../JsBuiltInEngineInterfaceExtensionObject.cpp    |  21 +-
 21 files changed, 966 insertions(+), 917 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_F2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```