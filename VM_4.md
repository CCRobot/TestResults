```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 56 11.1M   56 6448k    0     0  8829k      0  0:00:01 --:--:--  0:00:01 8820k100 11.1M  100 11.1M    0     0  10.4M      0  0:00:01  0:00:01 --:--:-- 10.4M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  153M    2 4576k    0     0  7039k      0  0:00:22 --:--:--  0:00:22 7040k 11  153M   11 17.3M    0     0  10.5M      0  0:00:14  0:00:01  0:00:13 10.5M 17  153M   17 27.4M    0     0  10.3M      0  0:00:14  0:00:02  0:00:12 10.3M 25  153M   25 38.3M    0     0  10.4M      0  0:00:14  0:00:03  0:00:11 10.4M 31  153M   31 48.3M    0     0  10.4M      0  0:00:14  0:00:04  0:00:10 10.4M 40  153M   40 61.6M    0     0  10.9M      0  0:00:14  0:00:05  0:00:09 11.4M 48  153M   48 73.7M    0     0  11.0M      0  0:00:13  0:00:06  0:00:07 11.2M 56  153M   56 86.3M    0     0  11.2M      0  0:00:13  0:00:07  0:00:06 11.7M 63  153M   63 97.3M    0     0  11.2M      0  0:00:13  0:00:08  0:00:05 11.8M 71  153M   71  109M    0     0  11.3M      0  0:00:13  0:00:09  0:00:04 12.1M 78  153M   78  119M    0     0  11.2M      0  0:00:13  0:00:10  0:00:03 11.5M 85  153M   85  131M    0     0  11.2M      0  0:00:13  0:00:11  0:00:02 11.5M 93  153M   93  142M    0     0  11.2M      0  0:00:13  0:00:12  0:00:01 11.2M100  153M  100  153M    0     0  11.2M      0  0:00:13  0:00:13 --:--:-- 11.1M
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
] Testing  NODE_BUILD_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```