```
Executed on ubu16chk400001F
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0 9180k    0 81500    0     0   159k      0  0:00:57 --:--:--  0:00:57  159k100 9180k  100 9180k    0     0  8234k      0  0:00:01  0:00:01 --:--:-- 8241k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  153M    0 81497    0     0   209k      0  0:12:28 --:--:--  0:12:28  209k 15  153M   15 23.9M    0     0  17.5M      0  0:00:08  0:00:01  0:00:07 17.5M 43  153M   43 66.3M    0     0  28.0M      0  0:00:05  0:00:02  0:00:03 28.0M 72  153M   72  110M    0     0  32.7M      0  0:00:04  0:00:03  0:00:01 32.7M100  153M  100  153M    0     0  35.2M      0  0:00:04  0:00:04 --:--:-- 35.2M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c0c17cf..8734707  master     -> origin/master
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
] Testing  TEST_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```