```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 70 11.1M   70 7984k    0     0  10.7M      0  0:00:01 --:--:--  0:00:01 10.7M100 11.1M  100 11.1M    0     0  11.2M      0 --:--:-- --:--:-- --:--:-- 11.2M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  137M    2 4192k    0     0  6736k      0  0:00:20 --:--:--  0:00:20 6728k 11  137M   11 15.9M    0     0  9848k      0  0:00:14  0:00:01  0:00:13 9847k 17  137M   17 23.7M    0     0  9274k      0  0:00:15  0:00:02  0:00:13 9273k 24  137M   24 33.9M    0     0  9598k      0  0:00:14  0:00:03  0:00:11 9597k 33  137M   33 46.4M    0     0  10.0M      0  0:00:13  0:00:04  0:00:09 10.0M 44  137M   44 60.6M    0     0  10.7M      0  0:00:12  0:00:05  0:00:07 11.3M 53  137M   53 73.3M    0     0  11.0M      0  0:00:12  0:00:06  0:00:06 11.5M 63  137M   63 86.4M    0     0  11.3M      0  0:00:12  0:00:07  0:00:05 12.5M 72  137M   72 99.9M    0     0  11.5M      0  0:00:11  0:00:08  0:00:03 13.1M 84  137M   84  115M    0     0  11.9M      0  0:00:11  0:00:09  0:00:02 13.7M 94  137M   94  129M    0     0  12.2M      0  0:00:11  0:00:10  0:00:01 13.8M 99  137M   99  136M    0     0  11.7M      0  0:00:11  0:00:11 --:--:-- 12.7M100  137M  100  137M    0     0  11.7M      0  0:00:11  0:00:11 --:--:-- 12.6M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   1c0c67e..9169de3  master      -> origin/master
   c60cf51..e5e1c85  release/1.8 -> origin/release/1.8
   cfcbe3b..37993b9  release/1.9 -> origin/release/1.9
Updating 1c0c67e..9169de3
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
 lib/Runtime/Language/JavascriptOperators.cpp       |  24 +-
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
 39 files changed, 1062 insertions(+), 966 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_FLG1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```