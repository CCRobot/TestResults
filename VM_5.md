```
Executed on ubu16chk4000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  8760k      0  0:00:01  0:00:01 --:--:-- 8768k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  137M    0 32345    0     0  86633      0  0:27:39 --:--:--  0:27:39 86483 23  137M   23 32.0M    0     0  23.1M      0  0:00:05  0:00:01  0:00:04 23.1M 53  137M   53 73.9M    0     0  31.2M      0  0:00:04  0:00:02  0:00:02 31.2M 84  137M   84  115M    0     0  34.3M      0  0:00:03  0:00:03 --:--:-- 34.3M100  137M  100  137M    0     0  35.0M      0  0:00:03  0:00:03 --:--:-- 35.0M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   1c0c67e..5484179  master     -> origin/master
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
] Testing  DEBUG_FLG2_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```