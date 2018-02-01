```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 97 11.1M   97 10.7M    0     0  9770k      0  0:00:01  0:00:01 --:--:-- 9769k100 11.1M  100 11.1M    0     0  9887k      0  0:00:01  0:00:01 --:--:-- 9879k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  8  141M    8 12.0M    0     0  12.4M      0  0:00:11 --:--:--  0:00:11 12.4M 16  141M   16 24.0M    0     0  12.1M      0  0:00:11  0:00:01  0:00:10 12.1M 24  141M   24 35.3M    0     0  11.9M      0  0:00:11  0:00:02  0:00:09 11.9M 33  141M   33 47.9M    0     0  12.1M      0  0:00:11  0:00:03  0:00:08 12.1M 43  141M   43 62.2M    0     0  12.5M      0  0:00:11  0:00:04  0:00:07 12.5M 52  141M   52 74.5M    0     0  12.5M      0  0:00:11  0:00:05  0:00:06 12.5M 62  141M   62 88.2M    0     0  12.6M      0  0:00:11  0:00:06  0:00:05 12.8M 72  141M   72  102M    0     0  12.9M      0  0:00:10  0:00:07  0:00:03 13.5M 81  141M   81  115M    0     0  12.8M      0  0:00:11  0:00:08  0:00:03 13.4M 91  141M   91  129M    0     0  12.9M      0  0:00:10  0:00:09  0:00:01 13.4M 99  141M   99  141M    0     0  12.8M      0  0:00:10  0:00:10 --:--:-- 13.3M100  141M  100  141M    0     0  12.8M      0  0:00:10  0:00:10 --:--:-- 13.1M
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
] Testing  NODE_BUILD_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```