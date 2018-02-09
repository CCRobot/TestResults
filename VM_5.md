```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 19 11.1M   19 2239k    0     0  4099k      0  0:00:02 --:--:--  0:00:02 4094k100 11.1M  100 11.1M    0     0  9159k      0  0:00:01  0:00:01 --:--:-- 9163k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  153M    0 1151k    0     0  4063k      0  0:00:38 --:--:--  0:00:38 4054k 11  153M   11 17.3M    0     0  13.5M      0  0:00:11  0:00:01  0:00:10 13.4M 20  153M   20 31.4M    0     0  13.7M      0  0:00:11  0:00:02  0:00:09 13.7M 30  153M   30 46.9M    0     0  14.2M      0  0:00:10  0:00:03  0:00:07 14.2M 39  153M   39 60.2M    0     0  14.0M      0  0:00:10  0:00:04  0:00:06 14.0M 49  153M   49 76.0M    0     0  14.3M      0  0:00:10  0:00:05  0:00:05 14.9M 58  153M   58 89.8M    0     0  14.3M      0  0:00:10  0:00:06  0:00:04 14.5M 64  153M   64 98.6M    0     0  13.5M      0  0:00:11  0:00:07  0:00:04 13.4M 71  153M   71  110M    0     0  13.2M      0  0:00:11  0:00:08  0:00:03 12.6M 78  153M   78  120M    0     0  12.9M      0  0:00:11  0:00:09  0:00:02 11.9M 85  153M   85  131M    0     0  12.7M      0  0:00:12  0:00:10  0:00:02 11.0M 91  153M   91  140M    0     0  12.3M      0  0:00:12  0:00:11  0:00:01 10.0M 97  153M   97  149M    0     0  12.2M      0  0:00:12  0:00:12 --:--:-- 10.2M100  153M  100  153M    0     0  12.1M      0  0:00:12  0:00:12 --:--:-- 10.0M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c0c17cf..6ea656a  master      -> origin/master
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
] Testing  DEBUG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```