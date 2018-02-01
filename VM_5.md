```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 41 11.1M   41 4752k    0     0  10.5M      0  0:00:01 --:--:--  0:00:01 10.4M100 11.1M  100 11.1M    0     0  13.7M      0 --:--:-- --:--:-- --:--:-- 13.7M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  141M    6 8992k    0     0  14.4M      0  0:00:09 --:--:--  0:00:09 14.4M 15  141M   15 22.3M    0     0  13.9M      0  0:00:10  0:00:01  0:00:09 13.9M 26  141M   26 37.3M    0     0  14.3M      0  0:00:09  0:00:02  0:00:07 14.3M 37  141M   37 53.3M    0     0  14.7M      0  0:00:09  0:00:03  0:00:06 14.7M 47  141M   47 67.2M    0     0  14.6M      0  0:00:09  0:00:04  0:00:05 14.6M 58  141M   58 82.7M    0     0  14.7M      0  0:00:09  0:00:05  0:00:04 14.7M 67  141M   67 96.0M    0     0  14.5M      0  0:00:09  0:00:06  0:00:03 14.7M 78  141M   78  110M    0     0  14.5M      0  0:00:09  0:00:07  0:00:02 14.6M 87  141M   87  123M    0     0  14.3M      0  0:00:09  0:00:08  0:00:01 14.1M 94  141M   94  133M    0     0  13.9M      0  0:00:10  0:00:09  0:00:01 13.2M100  141M  100  141M    0     0  13.9M      0  0:00:10  0:00:10 --:--:-- 12.9M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   e9b9c49..1f58d47  master      -> origin/master
   480bec0..9a42550  release/1.8 -> origin/release/1.8
   a231b21..77a31ac  release/1.9 -> origin/release/1.9
Updating e9b9c49..1f58d47
Fast-forward
 lib/Runtime/Debug/DiagObjectModel.cpp                     |  4 ++--
 lib/Runtime/Debug/TTSnapObjects.cpp                       |  2 +-
 lib/Runtime/Debug/TTSnapshotExtractor.cpp                 |  2 +-
 lib/Runtime/Language/JavascriptOperators.cpp              | 10 +++++-----
 lib/Runtime/Language/JavascriptOperators.inl              |  5 +----
 .../Library/IntlEngineInterfaceExtensionObject.cpp        | 14 ++++++++++----
 lib/Runtime/Library/JavascriptObject.cpp                  |  2 +-
 lib/Runtime/Types/RecyclableObject.cpp                    |  6 ------
 lib/Runtime/Types/RecyclableObject.h                      |  2 --
 lib/Runtime/Types/RecyclableObject.inl                    |  8 +++-----
 lib/Runtime/Types/Type.h                                  | 15 +++++++++++----
 test/Strings/rlexe.xml                                    |  1 -
 12 files changed, 35 insertions(+), 36 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_FLG2_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```