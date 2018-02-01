```
Executed on ubu16chk4000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 44 9180k   44 4112k    0     0  5819k      0  0:00:01 --:--:--  0:00:01 5816k100 9180k  100 9180k    0     0  11.1M      0 --:--:-- --:--:-- --:--:-- 11.1M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  8  141M    8 12.0M    0     0  13.8M      0  0:00:10 --:--:--  0:00:10 13.8M 36  141M   36 52.0M    0     0  27.3M      0  0:00:05  0:00:01  0:00:04 27.3M 62  141M   62 88.0M    0     0  30.2M      0  0:00:04  0:00:02  0:00:02 30.2M 89  141M   89  127M    0     0  33.0M      0  0:00:04  0:00:03  0:00:01 33.0M100  141M  100  141M    0     0  33.6M      0  0:00:04  0:00:04 --:--:-- 33.6M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   e9b9c49..d8c169f  master     -> origin/master
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
] Testing  DEBUG_FLG1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```