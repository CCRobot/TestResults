```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  11.9M      0 --:--:-- --:--:-- --:--:-- 11.9M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  8  141M    8 12.3M    0     0  12.5M      0  0:00:11 --:--:--  0:00:11 12.5M 16  141M   16 23.9M    0     0  12.1M      0  0:00:11  0:00:01  0:00:10 12.1M 26  141M   26 37.8M    0     0  12.7M      0  0:00:11  0:00:02  0:00:09 12.7M 36  141M   36 51.5M    0     0  12.9M      0  0:00:10  0:00:03  0:00:07 12.9M 45  141M   45 63.9M    0     0  12.8M      0  0:00:11  0:00:04  0:00:07 12.8M 53  141M   53 76.1M    0     0  12.7M      0  0:00:11  0:00:05  0:00:06 12.7M 62  141M   62 88.0M    0     0  12.6M      0  0:00:11  0:00:06  0:00:05 12.8M 71  141M   71  101M    0     0  12.7M      0  0:00:11  0:00:07  0:00:04 12.7M 80  141M   80  114M    0     0  12.7M      0  0:00:11  0:00:08  0:00:03 12.5M 91  141M   91  129M    0     0  12.9M      0  0:00:10  0:00:09  0:00:01 13.0M100  141M  100  141M    0     0  12.9M      0  0:00:10  0:00:10 --:--:-- 13.2M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   e9b9c49..6802d82  master      -> origin/master
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
] Testing  DEBUG_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```