```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 30 11.1M   30 3471k    0     0  6964k      0  0:00:01 --:--:--  0:00:01 6957k100 11.1M  100 11.1M    0     0  10.7M      0  0:00:01  0:00:01 --:--:-- 10.7M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  137M    2 3215k    0     0  7204k      0  0:00:19 --:--:--  0:00:19 7193k 12  137M   12 16.4M    0     0  11.3M      0  0:00:12  0:00:01  0:00:11 11.3M 19  137M   19 26.4M    0     0  10.8M      0  0:00:12  0:00:02  0:00:10 10.8M 27  137M   27 37.4M    0     0  10.8M      0  0:00:12  0:00:03  0:00:09 10.8M 35  137M   35 48.5M    0     0  10.9M      0  0:00:12  0:00:04  0:00:08 10.9M 43  137M   43 59.5M    0     0  10.9M      0  0:00:12  0:00:05  0:00:07 11.2M 51  137M   51 71.0M    0     0  11.0M      0  0:00:12  0:00:06  0:00:06 10.9M 59  137M   59 81.9M    0     0  11.0M      0  0:00:12  0:00:07  0:00:05 11.0M 68  137M   68 94.3M    0     0  11.1M      0  0:00:12  0:00:08  0:00:04 11.3M 77  137M   77  105M    0     0  11.1M      0  0:00:12  0:00:09  0:00:03 11.4M 86  137M   86  118M    0     0  11.3M      0  0:00:12  0:00:10  0:00:02 11.7M 94  137M   94  129M    0     0  11.3M      0  0:00:12  0:00:11  0:00:01 11.6M100  137M  100  137M    0     0  11.3M      0  0:00:12  0:00:12 --:--:-- 11.9M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   1c0c67e..5484179  master      -> origin/master
   c60cf51..e5e1c85  release/1.8 -> origin/release/1.8
   cfcbe3b..37993b9  release/1.9 -> origin/release/1.9
Updating 1c0c67e..5484179
Fast-forward
 lib/Common/DataStructures/SparseBitVector.h        |  29 +-
 lib/Common/Exceptions/ReportError.h                |   1 +
 lib/Common/Exceptions/Throw.cpp                    |   8 +
 lib/Common/Exceptions/Throw.h                      |   4 +-
 lib/Jsrt/Jsrt.cpp                                  |  99 ++---
 lib/Runtime/Base/FunctionBody.cpp                  |   6 +-
 lib/Runtime/Base/FunctionBody.h                    |   8 +
 lib/Runtime/Base/PropertyRecord.h                  |   3 +-
 lib/Runtime/Base/ScriptContext.cpp                 |   2 +-
 lib/Runtime/Base/ThreadContext.cpp                 |   5 +-
 lib/Runtime/Debug/TTActionEvents.cpp               |  30 +-
 lib/Runtime/Debug/TTEventLog.cpp                   |  11 +-
 lib/Runtime/Debug/TTEventLog.h                     |   2 +-
 lib/Runtime/Language/InterpreterStackFrame.cpp     |   1 +
 lib/Runtime/Language/JavascriptConversion.cpp      |   2 +-
 lib/Runtime/Language/JavascriptOperators.cpp       |  26 +-
 lib/Runtime/Library/ConcatString.cpp               |  29 +-
 lib/Runtime/Library/ConcatString.h                 |   3 +-
 .../Library/EngineInterfaceObjectBuiltIns.h        |   1 +
 lib/Runtime/Library/ForInObjectEnumerator.cpp      |   4 +-
 lib/Runtime/Library/JSONStringifier.cpp            |   2 +-
 lib/Runtime/Library/JavascriptFunction.cpp         |  11 +-
 lib/Runtime/Library/JavascriptFunction.h           |   4 +-
 lib/Runtime/Library/JavascriptLibrary.cpp          |   6 -
 lib/Runtime/Library/JavascriptLibrary.h            |   1 -
 lib/Runtime/Library/JavascriptObject.cpp           |   2 +-
 lib/Runtime/Library/JavascriptString.cpp           |  10 +-
 lib/Runtime/Library/JavascriptString.h             |   6 +-
 lib/Runtime/Library/JsBuiltIn/JsBuiltIn.js         |   1 +
 .../Library/JsBuiltIn/JsBuiltIn.js.bc.32b.h        | 428 +++++++++++----------
 .../Library/JsBuiltIn/JsBuiltIn.js.bc.64b.h        | 428 +++++++++++----------
 .../Library/JsBuiltIn/JsBuiltIn.js.nojit.bc.32b.h  | 406 +++++++++----------
 .../Library/JsBuiltIn/JsBuiltIn.js.nojit.bc.64b.h  | 406 +++++++++----------
 .../JsBuiltInEngineInterfaceExtensionObject.cpp    |  21 +-
 lib/Runtime/Library/LazyJSONString.cpp             |   6 +-
 lib/Runtime/Library/PropertyString.h               |   9 +-
 .../Platform/Common/HiResTimer.cpp                 |   2 +-
 .../Types/DynamicObjectPropertyEnumerator.cpp      |   2 +-
 lib/Runtime/Types/SimpleDictionaryTypeHandler.cpp  |   5 +-
 39 files changed, 1059 insertions(+), 971 deletions(-)
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