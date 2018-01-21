```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 58 11.1M   58 6640k    0     0  8039k      0  0:00:01 --:--:--  0:00:01 8038k100 11.1M  100 11.1M    0     0  10.5M      0  0:00:01  0:00:01 --:--:-- 10.5M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  135M    5 8208k    0     0  10.3M      0  0:00:13 --:--:--  0:00:13 10.3M 15  135M   15 21.3M    0     0  12.2M      0  0:00:11  0:00:01  0:00:10 12.2M 24  135M   24 33.7M    0     0  12.2M      0  0:00:11  0:00:02  0:00:09 12.2M 35  135M   35 47.7M    0     0  12.7M      0  0:00:10  0:00:03  0:00:07 12.7M 46  135M   46 63.0M    0     0  13.2M      0  0:00:10  0:00:04  0:00:06 13.2M 56  135M   56 75.9M    0     0  13.2M      0  0:00:10  0:00:05  0:00:05 13.6M 64  135M   64 87.1M    0     0  12.9M      0  0:00:10  0:00:06  0:00:04 13.1M 71  135M   71 96.8M    0     0  12.5M      0  0:00:10  0:00:07  0:00:03 12.6M 82  135M   82  111M    0     0  12.7M      0  0:00:10  0:00:08  0:00:02 12.6M 92  135M   92  125M    0     0  12.8M      0  0:00:10  0:00:09  0:00:01 12.4M100  135M  100  135M    0     0  13.1M      0  0:00:10  0:00:10 --:--:-- 13.1M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   bbc4c2e..8ce2142  master      -> origin/master
   9833ad5..c3c7923  release/1.8 -> origin/release/1.8
   e488ebb..50e5667  release/1.9 -> origin/release/1.9
Updating bbc4c2e..8ce2142
Fast-forward
 bin/NativeTests/FileLoadHelpers.cpp             |  2 +-
 bin/ch/Helpers.cpp                              | 11 ++++++-----
 lib/Runtime/Language/SourceTextModuleRecord.cpp | 12 +++++++-----
 test/es6/module_4482_dep1.js                    |  9 ++++++---
 test/es6/module_4482_dep2.js                    |  4 ++--
 test/es6/module_4482_dep3.js                    |  7 +++++--
 6 files changed, 27 insertions(+), 18 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```