```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  8 11.1M    8  975k    0     0  2532k      0  0:00:04 --:--:--  0:00:04 2527k 39 11.1M   39 4544k    0     0  3278k      0  0:00:03  0:00:01  0:00:02 3276k 81 11.1M   81 9248k    0     0  3880k      0  0:00:02  0:00:02 --:--:-- 3879k100 11.1M  100 11.1M    0     0  3571k      0  0:00:03  0:00:03 --:--:-- 3571k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  153M    6 9920k    0     0  8408k      0  0:00:18  0:00:01  0:00:17 8406k 11  153M   11 16.8M    0     0  7923k      0  0:00:19  0:00:02  0:00:17 7922k 17  153M   17 27.2M    0     0  8708k      0  0:00:18  0:00:03  0:00:15 8707k 24  153M   24 37.1M    0     0  9096k      0  0:00:17  0:00:04  0:00:13 9095k 29  153M   29 45.7M    0     0  9055k      0  0:00:17  0:00:05  0:00:12 9426k 35  153M   35 54.0M    0     0  8963k      0  0:00:17  0:00:06  0:00:11 9094k 40  153M   40 62.5M    0     0  8917k      0  0:00:17  0:00:07  0:00:10 9349k 45  153M   45 70.1M    0     0  8785k      0  0:00:17  0:00:08  0:00:09 8834k 50  153M   50 76.7M    0     0  8557k      0  0:00:18  0:00:09  0:00:09 8108k 54  153M   54 83.8M    0     0  8437k      0  0:00:18  0:00:10  0:00:08 7798k 57  153M   57 88.3M    0     0  8094k      0  0:00:19  0:00:11  0:00:08 7021k 60  153M   60 93.2M    0     0  7842k      0  0:00:19  0:00:12  0:00:07 6297k 64  153M   64 98.2M    0     0  7631k      0  0:00:20  0:00:13  0:00:07 5747k 68  153M   68  104M    0     0  7547k      0  0:00:20  0:00:14  0:00:06 5689k 72  153M   72  111M    0     0  7522k      0  0:00:20  0:00:15  0:00:05 5662k 77  153M   77  118M    0     0  7515k      0  0:00:20  0:00:16  0:00:04 6220k 81  153M   81  125M    0     0  7473k      0  0:00:20  0:00:17  0:00:03 6576k 86  153M   86  132M    0     0  7436k      0  0:00:21  0:00:18  0:00:03 6921k 90  153M   90  138M    0     0  7388k      0  0:00:21  0:00:19  0:00:02 6940k 94  153M   94  145M    0     0  7358k      0  0:00:21  0:00:20  0:00:01 6860k 97  153M   97  149M    0     0  7228k      0  0:00:21  0:00:21 --:--:-- 6297k100  153M  100  153M    0     0  7212k      0  0:00:21  0:00:21 --:--:-- 6229k
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
] Testing  RL18_DBG_F2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```