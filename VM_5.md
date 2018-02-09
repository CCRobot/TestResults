```
Executed on ubu16chk4000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  11.5M      0 --:--:-- --:--:-- --:--:-- 11.5M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 11  153M   11 17.9M    0     0  15.1M      0  0:00:10  0:00:01  0:00:09 15.1M 23  153M   23 36.6M    0     0  16.7M      0  0:00:09  0:00:02  0:00:07 16.7M 36  153M   36 56.0M    0     0  17.5M      0  0:00:08  0:00:03  0:00:05 17.5M 49  153M   49 75.8M    0     0  18.1M      0  0:00:08  0:00:04  0:00:04 18.1M 62  153M   62 95.3M    0     0  18.3M      0  0:00:08  0:00:05  0:00:03 19.1M 74  153M   74  113M    0     0  18.3M      0  0:00:08  0:00:06  0:00:02 19.1M 86  153M   86  133M    0     0  18.5M      0  0:00:08  0:00:07  0:00:01 19.2M100  153M  100  153M    0     0  18.7M      0  0:00:08  0:00:08 --:--:-- 19.5M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c0c17cf..6ea656a  master     -> origin/master
   05f4157..30bef33  release/1.8 -> origin/release/1.8
   91ec1ef..f1a6b10  release/1.9 -> origin/release/1.9
Updating c0c17cf..6ea656a
Fast-forward
 lib/Backend/Func.cpp                               |   2 +-
 lib/Backend/IRBuilder.cpp                          |   2 +-
 lib/Common/Memory/SectionAllocWrapper.cpp          |   2 +-
 lib/Common/Memory/VirtualAllocWrapper.cpp          |   2 +-
 lib/Runtime/Debug/TTEventLog.cpp                   |  24 +-
 lib/Runtime/Debug/TTEventLog.h                     |   4 +-
 lib/Runtime/Debug/TTEvents.cpp                     |  15 +-
 lib/Runtime/Debug/TTEvents.h                       |   5 +-
 lib/Runtime/Debug/TTExecutionInfo.cpp              |  39 +-
 lib/Runtime/Library/JavascriptExternalFunction.cpp |   8 +-
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
 36 files changed, 613 insertions(+), 909 deletions(-)
 create mode 100644 test/Bugs/bug14057294.js
 create mode 100644 test/Function/builtinFuncHasOwnPropCallerArguments.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```