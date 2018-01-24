```
Executed on ubu16chk400000I
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 51 9180k   51 4768k    0     0  5156k      0  0:00:01 --:--:--  0:00:01 5154k100 9180k  100 9180k    0     0  8734k      0  0:00:01  0:00:01 --:--:-- 8743k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  137M    2 4112k    0     0  4605k      0  0:00:30 --:--:--  0:00:30 4604k 29  137M   29 40.0M    0     0  21.0M      0  0:00:06  0:00:01  0:00:05 21.0M 58  137M   58 80.0M    0     0  27.3M      0  0:00:05  0:00:02  0:00:03 27.3M 84  137M   84  116M    0     0  30.2M      0  0:00:04  0:00:03  0:00:01 30.2M100  137M  100  137M    0     0  31.7M      0  0:00:04  0:00:04 --:--:-- 31.7M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   1c0c67e..bdae93e  master     -> origin/master
   c60cf51..a5a6b65  release/1.8 -> origin/release/1.8
   cfcbe3b..2abdaab  release/1.9 -> origin/release/1.9
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
] Testing  RL18_DBG_F1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```