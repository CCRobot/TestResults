```
Executed on ubu16chk400000Z
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  8745k      0  0:00:01  0:00:01 --:--:-- 8752k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 11  141M   11 16.0M    0     0  13.1M      0  0:00:10  0:00:01  0:00:09 13.1M 37  141M   37 52.9M    0     0  24.2M      0  0:00:05  0:00:02  0:00:03 24.2M 65  141M   65 93.2M    0     0  29.3M      0  0:00:04  0:00:03  0:00:01 29.3M 93  141M   93  132M    0     0  31.5M      0  0:00:04  0:00:04 --:--:-- 31.5M100  141M  100  141M    0     0  32.4M      0  0:00:04  0:00:04 --:--:-- 34.0M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   e9b9c49..6802d82  master     -> origin/master
   480bec0..5ebaf10  release/1.8 -> origin/release/1.8
   a231b21..4115143  release/1.9 -> origin/release/1.9
Updating e9b9c49..6802d82
Fast-forward
 lib/Parser/Parse.cpp                               |  4 ++
 lib/Runtime/ByteCode/ByteCodeEmitter.cpp           | 51 +++++++++-------------
 lib/Runtime/ByteCode/ScopeInfo.cpp                 |  7 ++-
 lib/Runtime/ByteCode/ScopeInfo.h                   | 14 +++++-
 lib/Runtime/Debug/DiagObjectModel.cpp              |  5 ++-
 lib/Runtime/Debug/TTSnapObjects.cpp                |  2 +-
 lib/Runtime/Debug/TTSnapshotExtractor.cpp          |  2 +-
 lib/Runtime/Language/JavascriptOperators.cpp       | 15 +++----
 lib/Runtime/Language/JavascriptOperators.inl       |  5 +--
 .../Library/IntlEngineInterfaceExtensionObject.cpp | 14 ++++--
 lib/Runtime/Library/JavascriptObject.cpp           |  2 +-
 lib/Runtime/Types/RecyclableObject.cpp             |  6 ---
 lib/Runtime/Types/RecyclableObject.h               |  2 -
 lib/Runtime/Types/RecyclableObject.inl             |  8 ++--
 lib/Runtime/Types/Type.h                           | 15 +++++--
 test/Basics/SpecialSymbolCapture.js                | 25 -----------
 test/DebuggerCommon/promiseDisplay.js.dbg.baseline |  2 +-
 test/Strings/rlexe.xml                             |  1 -
 test/es6/DeferParseLambda.js                       | 48 ++++++++++++++++++++
 test/es6/ES6Class_BaseClassConstruction.js         | 40 ++++++++++-------
 test/es6/rlexe.xml                                 |  7 +++
 21 files changed, 160 insertions(+), 115 deletions(-)
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