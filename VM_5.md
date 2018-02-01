```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 29 11.1M   29 3407k    0     0  6694k      0  0:00:01 --:--:--  0:00:01 6694k100 11.1M  100 11.1M    0     0   9.9M      0  0:00:01  0:00:01 --:--:--  9.9M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  141M    2 3375k    0     0  8995k      0  0:00:16 --:--:--  0:00:16 8977k 11  141M   11 16.0M    0     0  11.6M      0  0:00:12  0:00:01  0:00:11 11.6M 21  141M   21 30.3M    0     0  12.7M      0  0:00:11  0:00:02  0:00:09 12.7M 30  141M   30 42.9M    0     0  12.7M      0  0:00:11  0:00:03  0:00:08 12.7M 42  141M   42 60.0M    0     0  13.7M      0  0:00:10  0:00:04  0:00:06 13.7M 52  141M   52 74.2M    0     0  13.8M      0  0:00:10  0:00:05  0:00:05 14.1M 59  141M   59 83.8M    0     0  13.1M      0  0:00:10  0:00:06  0:00:04 13.5M 67  141M   67 96.2M    0     0  13.0M      0  0:00:10  0:00:07  0:00:03 13.1M 77  141M   77  109M    0     0  13.0M      0  0:00:10  0:00:08  0:00:02 13.3M 86  141M   86  122M    0     0  13.0M      0  0:00:10  0:00:09  0:00:01 12.5M 97  141M   97  137M    0     0  13.2M      0  0:00:10  0:00:10 --:--:-- 12.7M100  141M  100  141M    0     0  13.3M      0  0:00:10  0:00:10 --:--:-- 13.6M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   e9b9c49..d8c169f  master      -> origin/master
   480bec0..7443cf6  release/1.8 -> origin/release/1.8
   a231b21..24928c5  release/1.9 -> origin/release/1.9
Updating e9b9c49..d8c169f
Fast-forward
 lib/Parser/Parse.cpp                               |  4 ++
 lib/Runtime/ByteCode/ScopeInfo.cpp                 |  7 +++-
 lib/Runtime/ByteCode/ScopeInfo.h                   | 14 ++++++-
 lib/Runtime/Debug/DiagObjectModel.cpp              |  4 +-
 lib/Runtime/Debug/TTSnapObjects.cpp                |  2 +-
 lib/Runtime/Debug/TTSnapshotExtractor.cpp          |  2 +-
 lib/Runtime/Language/JavascriptOperators.cpp       | 10 ++---
 lib/Runtime/Language/JavascriptOperators.inl       |  5 +--
 .../Library/IntlEngineInterfaceExtensionObject.cpp | 14 +++++--
 lib/Runtime/Library/JavascriptObject.cpp           |  2 +-
 lib/Runtime/Types/RecyclableObject.cpp             |  6 ---
 lib/Runtime/Types/RecyclableObject.h               |  2 -
 lib/Runtime/Types/RecyclableObject.inl             |  8 ++--
 lib/Runtime/Types/Type.h                           | 15 +++++--
 test/Strings/rlexe.xml                             |  1 -
 test/es6/DeferParseLambda.js                       | 48 ++++++++++++++++++++++
 test/es6/rlexe.xml                                 |  7 ++++
 17 files changed, 113 insertions(+), 38 deletions(-)
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