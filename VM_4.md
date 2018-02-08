```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 98 11.1M   98 10.9M    0     0  8323k      0  0:00:01  0:00:01 --:--:-- 8321k100 11.1M  100 11.1M    0     0  7872k      0  0:00:01  0:00:01 --:--:-- 7870k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  153M    0  735k    0     0   968k      0  0:02:41 --:--:--  0:02:41  967k  6  153M    6 10.5M    0     0  5574k      0  0:00:28  0:00:01  0:00:27 5573k 10  153M   10 16.0M    0     0  5498k      0  0:00:28  0:00:02  0:00:26 5497k 15  153M   15 24.0M    0     0  6540k      0  0:00:23  0:00:03  0:00:20 6540k 19  153M   19 30.1M    0     0  6484k      0  0:00:24  0:00:04  0:00:20 6484k 27  153M   27 41.6M    0     0  7066k      0  0:00:22  0:00:06  0:00:16 7945k 30  153M   30 46.7M    0     0  6878k      0  0:00:22  0:00:06  0:00:16 7378k 32  153M   32 49.9M    0     0  6561k      0  0:00:23  0:00:07  0:00:16 7219k 34  153M   34 53.4M    0     0  6244k      0  0:00:25  0:00:08  0:00:17 6022k 41  153M   41 63.2M    0     0  6634k      0  0:00:23  0:00:09  0:00:14 6775k 47  153M   47 73.1M    0     0  6963k      0  0:00:22  0:00:10  0:00:12 6831k 51  153M   51 78.2M    0     0  6811k      0  0:00:23  0:00:11  0:00:12 6714k 59  153M   59 91.3M    0     0  7334k      0  0:00:21  0:00:12  0:00:09 8544k 65  153M   65  101M    0     0  7522k      0  0:00:20  0:00:13  0:00:07 9761k 71  153M   71  109M    0     0  7578k      0  0:00:20  0:00:14  0:00:06 9420k 78  153M   78  120M    0     0  7825k      0  0:00:20  0:00:15  0:00:05 9680k 84  153M   84  129M    0     0  7813k      0  0:00:20  0:00:16  0:00:04  9.8M 90  153M   90  138M    0     0  7995k      0  0:00:19  0:00:17  0:00:02 9681k 99  153M   99  152M    0     0  8350k      0  0:00:18  0:00:18 --:--:-- 10.3M100  153M  100  153M    0     0  8346k      0  0:00:18  0:00:18 --:--:-- 10.8M
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
] Testing  RLS18_TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```