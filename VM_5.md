```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 72 11.1M   72 8208k    0     0  11.7M      0 --:--:-- --:--:-- --:--:-- 11.7M100 11.1M  100 11.1M    0     0  12.8M      0 --:--:-- --:--:-- --:--:-- 12.8M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  153M    4 7712k    0     0  9766k      0  0:00:16 --:--:--  0:00:16 9762k 13  153M   13 20.9M    0     0  11.7M      0  0:00:13  0:00:01  0:00:12 11.6M 23  153M   23 35.5M    0     0  12.7M      0  0:00:12  0:00:02  0:00:10 12.7M 33  153M   33 51.8M    0     0  13.6M      0  0:00:11  0:00:03  0:00:08 13.6M 42  153M   42 65.6M    0     0  13.7M      0  0:00:11  0:00:04  0:00:07 13.7M 47  153M   47 72.0M    0     0  12.4M      0  0:00:12  0:00:05  0:00:07 12.8M 52  153M   52 80.2M    0     0  11.3M      0  0:00:13  0:00:07  0:00:06 11.2M 55  153M   55 85.3M    0     0  10.9M      0  0:00:13  0:00:07  0:00:06  9.9M 59  153M   59 90.9M    0     0  10.3M      0  0:00:14  0:00:08  0:00:06 7993k 62  153M   62 95.3M    0     0  9968k      0  0:00:15  0:00:09  0:00:06 6075k 67  153M   67  103M    0     0  9787k      0  0:00:16  0:00:10  0:00:06 6376k 75  153M   75  116M    0     0   9.8M      0  0:00:15  0:00:11  0:00:04 7712k 81  153M   81  125M    0     0   9.7M      0  0:00:15  0:00:12  0:00:03 8137k 87  153M   87  134M    0     0  9997k      0  0:00:15  0:00:13  0:00:02 8955k 94  153M   94  144M    0     0   9.7M      0  0:00:15  0:00:14  0:00:01  9.8M100  153M  100  153M    0     0   9.8M      0  0:00:15  0:00:15 --:--:-- 10.3M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c0c17cf..48c73e5  master      -> origin/master
   05f4157..30bef33  release/1.8 -> origin/release/1.8
   91ec1ef..c50dfa8  release/1.9 -> origin/release/1.9
Updating c0c17cf..48c73e5
Fast-forward
 lib/Backend/Func.cpp                               |   2 +-
 lib/Backend/IRBuilder.cpp                          |   2 +-
 lib/Common/Memory/SectionAllocWrapper.cpp          |   2 +-
 lib/Common/Memory/VirtualAllocWrapper.cpp          |   2 +-
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
 30 files changed, 552 insertions(+), 875 deletions(-)
 create mode 100644 test/Bugs/bug14057294.js
 create mode 100644 test/Function/builtinFuncHasOwnPropCallerArguments.js
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