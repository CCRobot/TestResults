```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 83 11.1M   83 9488k    0     0  10.1M      0  0:00:01 --:--:--  0:00:01 10.1M100 11.1M  100 11.1M    0     0  10.6M      0  0:00:01  0:00:01 --:--:-- 10.6M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  120M    6 8208k    0     0  9457k      0  0:00:13 --:--:--  0:00:13 9456k 17  120M   17 21.2M    0     0  11.4M      0  0:00:10  0:00:01  0:00:09 11.4M 29  120M   29 35.1M    0     0  12.3M      0  0:00:09  0:00:02  0:00:07 12.3M 38  120M   38 46.5M    0     0  12.0M      0  0:00:10  0:00:03  0:00:07 12.0M 49  120M   49 59.3M    0     0  12.2M      0  0:00:09  0:00:04  0:00:05 12.2M 52  120M   52 64.0M    0     0  10.9M      0  0:00:11  0:00:05  0:00:06 11.2M 59  120M   59 72.0M    0     0  10.4M      0  0:00:11  0:00:06  0:00:05 10.1M 66  120M   66 80.5M    0     0  10.2M      0  0:00:11  0:00:07  0:00:04 9291k 71  120M   71 86.8M    0     0   9.8M      0  0:00:12  0:00:08  0:00:04 8257k 78  120M   78 95.0M    0     0  9878k      0  0:00:12  0:00:09  0:00:03 7320k 89  120M   89  108M    0     0   9.9M      0  0:00:12  0:00:10  0:00:02 9012k 98  120M   98  119M    0     0  10.0M      0  0:00:12  0:00:11  0:00:01 9704k100  120M  100  120M    0     0  10.0M      0  0:00:12  0:00:12 --:--:-- 9798k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   523c01d..8e0bd3c  master      -> origin/master
   03a8be9..745ddf8  intl-icu    -> origin/intl-icu
   bd3a178..ce599fa  release/1.8 -> origin/release/1.8
Updating 523c01d..8e0bd3c
Fast-forward
 lib/Common/Core/Output.cpp                         | 13 ++++
 lib/Common/Core/Output.h                           |  2 +
 lib/Runtime/Base/ScriptContext.cpp                 | 87 ++++++++++++----------
 lib/Runtime/Base/ScriptContext.h                   | 11 ++-
 .../Language/JavascriptExceptionOperators.cpp      | 41 ++++++----
 test/Debugger/empty.baseline                       |  1 +
 test/Debugger/failfast.js                          | 17 +++++
 test/Debugger/rlexe.xml                            |  6 ++
 8 files changed, 123 insertions(+), 55 deletions(-)
 create mode 100644 test/Debugger/empty.baseline
 create mode 100644 test/Debugger/failfast.js
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