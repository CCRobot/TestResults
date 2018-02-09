```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 26 11.1M   26 2991k    0     0  6006k      0  0:00:01 --:--:--  0:00:01 6007k100 11.1M  100 11.1M    0     0  9917k      0  0:00:01  0:00:01 --:--:-- 9922k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  153M    1 2431k    0     0  7306k      0  0:00:21 --:--:--  0:00:21 7302k  8  153M    8 13.7M    0     0  10.3M      0  0:00:14  0:00:01  0:00:13 10.3M 15  153M   15 24.0M    0     0  10.3M      0  0:00:14  0:00:02  0:00:12 10.3M 25  153M   25 38.9M    0     0  11.6M      0  0:00:13  0:00:03  0:00:10 11.6M 32  153M   32 50.5M    0     0  11.6M      0  0:00:13  0:00:04  0:00:09 11.6M 41  153M   41 62.8M    0     0  11.7M      0  0:00:12  0:00:05  0:00:07 12.0M 48  153M   48 74.5M    0     0  11.7M      0  0:00:13  0:00:06  0:00:07 12.1M 56  153M   56 86.7M    0     0  11.8M      0  0:00:12  0:00:07  0:00:05 12.5M 65  153M   65  100M    0     0  12.0M      0  0:00:12  0:00:08  0:00:04 12.3M 73  153M   73  112M    0     0  12.0M      0  0:00:12  0:00:09  0:00:03 12.4M 82  153M   82  126M    0     0  12.2M      0  0:00:12  0:00:10  0:00:02 12.6M 89  153M   89  137M    0     0  12.1M      0  0:00:12  0:00:11  0:00:01 12.6M 99  153M   99  152M    0     0  12.3M      0  0:00:12  0:00:12 --:--:-- 13.0M100  153M  100  153M    0     0  12.3M      0  0:00:12  0:00:12 --:--:-- 12.8M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c0c17cf..8734707  master      -> origin/master
   05f4157..befded1  release/1.8 -> origin/release/1.8
   91ec1ef..aec9a9c  release/1.9 -> origin/release/1.9
Updating c0c17cf..8734707
Fast-forward
 lib/Backend/Func.cpp                               |   5 +-
 lib/Backend/IRBuilder.cpp                          |   2 +-
 lib/Runtime/Library/JavascriptFunction.cpp         |   6 +-
 lib/Runtime/Library/JavascriptLibrary.cpp          |   5 +
 .../JsBuiltInEngineInterfaceExtensionObject.cpp    |   2 -
 test/Bugs/bug14057294.js                           |  22 +
 test/Bugs/rlexe.xml                                |   5 +
 .../ES6_intl_simple_attach.js.dbg.baseline         | 140 ++----
 .../ES6_proto_invalidation.js.dbg.baseline         | 492 ++++++---------------
 .../ES6_proto_userDefinedObject.js.dbg.baseline    |  58 +--
 test/DebuggerCommon/TempStrExpr.js.dbg.baseline    |  16 +-
 test/DebuggerCommon/TypedArray.js.dbg.baseline     |  30 +-
 .../DebuggerCommon/array_prototest.js.dbg.baseline |  20 +-
 .../blockScopeBasicLetConstTest.js.dbg.baseline    |   4 +-
 test/DebuggerCommon/bug_543550.js.dbg.baseline     |  44 +-
 test/DebuggerCommon/bug_os_2946365.js.dbg.baseline |  36 +-
 .../frames_values_mapES6.js.dbg.baseline           | 178 ++------
 test/DebuggerCommon/indexprop.js.dbg.baseline      |  12 +-
 ...rom_interpreted_function_attach.js.dbg.baseline |  12 +-
 .../stringkeyedtypehandler.js.dbg.baseline         |  10 +-
 test/DebuggerCommon/symbols.js.dbg.baseline        |  68 +--
 test/DebuggerCommon/targeted.js.dbg.baseline       |  48 +-
 .../builtinFuncHasOwnPropCallerArguments.js        |  96 ++++
 test/Function/rlexe.xml                            |   6 +
 test/Function/typeErrorAccessor.baseline           |  26 +-
 test/Function/typeErrorAccessor.js                 |   8 +-
 test/es6/ES6RestrictedProperties.js                |  73 ++-
 test/es6/function.name.js                          |   2 +-
 28 files changed, 552 insertions(+), 874 deletions(-)
 create mode 100644 test/Bugs/bug14057294.js
 create mode 100644 test/Function/builtinFuncHasOwnPropCallerArguments.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```