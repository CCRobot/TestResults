```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 56 11.1M   56 6384k    0     0  7897k      0  0:00:01 --:--:--  0:00:01 7891k100 11.1M  100 11.1M    0     0  8297k      0  0:00:01  0:00:01 --:--:-- 8301k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  153M    1 1631k    0     0  5083k      0  0:00:30 --:--:--  0:00:30 5082k  7  153M    7 12.0M    0     0  9378k      0  0:00:16  0:00:01  0:00:15 9378k 15  153M   15 22.9M    0     0   9.9M      0  0:00:15  0:00:02  0:00:13  9.9M 21  153M   21 33.2M    0     0   9.8M      0  0:00:15  0:00:03  0:00:12  9.8M 27  153M   27 41.5M    0     0  9852k      0  0:00:15  0:00:04  0:00:11 9851k 34  153M   34 53.1M    0     0  10.0M      0  0:00:15  0:00:05  0:00:10 10.3M 41  153M   41 62.9M    0     0   9.9M      0  0:00:15  0:00:06  0:00:09 10.1M 48  153M   48 74.1M    0     0  10.1M      0  0:00:15  0:00:07  0:00:08 10.2M 56  153M   56 85.8M    0     0  10.3M      0  0:00:14  0:00:08  0:00:06 10.6M 62  153M   62 95.7M    0     0  10.2M      0  0:00:14  0:00:09  0:00:05 10.8M 70  153M   70  108M    0     0  10.4M      0  0:00:14  0:00:10  0:00:04 10.9M 77  153M   77  118M    0     0  10.4M      0  0:00:14  0:00:11  0:00:03 11.1M 83  153M   83  128M    0     0  10.4M      0  0:00:14  0:00:12  0:00:02 10.8M 91  153M   91  140M    0     0  10.5M      0  0:00:14  0:00:13  0:00:01 10.9M100  153M  100  153M    0     0  10.7M      0  0:00:14  0:00:14 --:--:-- 11.5M
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
] Testing  DEBUG_FLG1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```