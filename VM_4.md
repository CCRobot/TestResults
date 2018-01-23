```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 56 11.1M   56 6432k    0     0  7535k      0  0:00:01 --:--:--  0:00:01 7531k100 11.1M  100 11.1M    0     0  9489k      0  0:00:01  0:00:01 --:--:-- 9492k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  137M    5 7616k    0     0  11.7M      0  0:00:11 --:--:--  0:00:11 11.7M 15  137M   15 21.1M    0     0  12.9M      0  0:00:10  0:00:01  0:00:09 12.9M 19  137M   19 26.1M    0     0   9.9M      0  0:00:13  0:00:02  0:00:11  9.9M 26  137M   26 36.3M    0     0   9.9M      0  0:00:13  0:00:03  0:00:10  9.9M 30  137M   30 41.8M    0     0  9242k      0  0:00:15  0:00:04  0:00:11 9242k 37  137M   37 51.6M    0     0  9381k      0  0:00:14  0:00:05  0:00:09 9048k 43  137M   43 59.9M    0     0  9253k      0  0:00:15  0:00:06  0:00:09 7956k 50  137M   50 69.2M    0     0  9287k      0  0:00:15  0:00:07  0:00:08 8830k 53  137M   53 73.9M    0     0  8771k      0  0:00:16  0:00:08  0:00:08 7705k 61  137M   61 84.0M    0     0  8928k      0  0:00:15  0:00:09  0:00:06 8635k 65  137M   65 90.1M    0     0  8678k      0  0:00:16  0:00:10  0:00:06 7884k 72  137M   72 99.5M    0     0  8759k      0  0:00:16  0:00:11  0:00:05 8105k 80  137M   80  109M    0     0  8890k      0  0:00:15  0:00:12  0:00:03 8281k 88  137M   88  121M    0     0  9062k      0  0:00:15  0:00:13  0:00:02 9561k 94  137M   94  129M    0     0  9078k      0  0:00:15  0:00:14  0:00:01 9370k 98  137M   98  134M    0     0  8821k      0  0:00:15  0:00:15 --:--:-- 9126k100  137M  100  137M    0     0  8859k      0  0:00:15  0:00:15 --:--:-- 9136k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   1c0c67e..bdae93e  master      -> origin/master
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
] Testing  RL18_DBG_F1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```