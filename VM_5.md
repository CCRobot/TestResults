```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 69 11.1M   69 7904k    0     0  6517k      0  0:00:01  0:00:01 --:--:-- 6516k100 11.1M  100 11.1M    0     0  7037k      0  0:00:01  0:00:01 --:--:-- 7034k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  137M    3 5312k    0     0  9171k      0  0:00:15 --:--:--  0:00:15 9158k 11  137M   11 16.0M    0     0  10.2M      0  0:00:13  0:00:01  0:00:12 10.2M 19  137M   19 26.9M    0     0  9670k      0  0:00:14  0:00:02  0:00:12 9668k 24  137M   24 34.2M    0     0  9790k      0  0:00:14  0:00:03  0:00:11 9788k 35  137M   35 48.4M    0     0  10.5M      0  0:00:12  0:00:04  0:00:08 10.5M 43  137M   43 60.2M    0     0  10.7M      0  0:00:12  0:00:05  0:00:07 11.0M 49  137M   49 68.5M    0     0  10.4M      0  0:00:13  0:00:06  0:00:07 10.4M 55  137M   55 75.5M    0     0   9.9M      0  0:00:13  0:00:07  0:00:06 10.2M 64  137M   64 87.9M    0     0  10.2M      0  0:00:13  0:00:08  0:00:05 10.7M 74  137M   74  101M    0     0  10.6M      0  0:00:12  0:00:09  0:00:03 10.6M 82  137M   82  112M    0     0  10.6M      0  0:00:12  0:00:10  0:00:02 10.4M 89  137M   89  123M    0     0  10.6M      0  0:00:12  0:00:11  0:00:01 10.9M 97  137M   97  133M    0     0  10.6M      0  0:00:12  0:00:12 --:--:-- 11.6M100  137M  100  137M    0     0  10.6M      0  0:00:12  0:00:12 --:--:-- 11.5M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   1c0c67e..d062b50  master      -> origin/master
   c60cf51..e5e1c85  release/1.8 -> origin/release/1.8
   cfcbe3b..14831da  release/1.9 -> origin/release/1.9
Updating 1c0c67e..d062b50
Fast-forward
 lib/Common/DataStructures/SparseBitVector.h        |  29 +-
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
 22 files changed, 993 insertions(+), 919 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  TEST_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```