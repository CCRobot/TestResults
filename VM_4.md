```
Executed on ubu16chk400000Z
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 14 9180k   14 1311k    0     0  1812k      0  0:00:05 --:--:--  0:00:05 1811k100 9180k  100 9180k    0     0  8836k      0  0:00:01  0:00:01 --:--:-- 8844k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  141M    0 1231k    0     0  1869k      0  0:01:17 --:--:--  0:01:17 1868k 22  141M   22 32.0M    0     0  18.9M      0  0:00:07  0:00:01  0:00:06 18.9M 50  141M   50 72.0M    0     0  26.7M      0  0:00:05  0:00:02  0:00:03 26.7M 79  141M   79  112M    0     0  30.2M      0  0:00:04  0:00:03  0:00:01 30.2M100  141M  100  141M    0     0  32.3M      0  0:00:04  0:00:04 --:--:-- 32.3M
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
] Testing  NODE_BUILD_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```