```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 86 11.1M   86 9808k    0     0  11.7M      0 --:--:-- --:--:-- --:--:-- 11.7M100 11.1M  100 11.1M    0     0  10.6M      0  0:00:01  0:00:01 --:--:-- 10.6M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  153M    4 7120k    0     0  9441k      0  0:00:16 --:--:--  0:00:16 9430k  8  153M    8 12.8M    0     0  7478k      0  0:00:20  0:00:01  0:00:19 7476k 16  153M   16 25.7M    0     0  9565k      0  0:00:16  0:00:02  0:00:14 9564k 25  153M   25 38.4M    0     0  10.2M      0  0:00:14  0:00:03  0:00:11 10.2M 36  153M   36 55.8M    0     0  11.7M      0  0:00:13  0:00:04  0:00:09 11.7M 45  153M   45 69.5M    0     0  12.0M      0  0:00:12  0:00:05  0:00:07 12.5M 54  153M   54 83.3M    0     0  12.3M      0  0:00:12  0:00:06  0:00:06 14.1M 63  153M   63 96.7M    0     0  12.4M      0  0:00:12  0:00:07  0:00:05 14.2M 72  153M   72  111M    0     0  12.7M      0  0:00:12  0:00:08  0:00:04 14.6M 81  153M   81  124M    0     0  12.7M      0  0:00:12  0:00:09  0:00:03 13.7M 90  153M   90  138M    0     0  12.8M      0  0:00:11  0:00:10  0:00:01 13.7M 94  153M   94  143M    0     0  12.2M      0  0:00:12  0:00:11  0:00:01 12.1M100  153M  100  153M    0     0  12.2M      0  0:00:12  0:00:12 --:--:-- 11.9M
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
] Testing  RL18_DBG_F1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```