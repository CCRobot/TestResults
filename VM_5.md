```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  10.5M      0  0:00:01  0:00:01 --:--:-- 10.5M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 11  120M   11 13.5M    0     0  13.0M      0  0:00:09  0:00:01  0:00:08 13.0M 23  120M   23 28.5M    0     0  14.0M      0  0:00:08  0:00:02  0:00:06 14.0M 37  120M   37 45.6M    0     0  15.0M      0  0:00:08  0:00:03  0:00:05 15.0M 51  120M   51 62.5M    0     0  15.4M      0  0:00:07  0:00:04  0:00:03 15.4M 61  120M   61 74.2M    0     0  14.7M      0  0:00:08  0:00:05  0:00:03 14.8M 76  120M   76 92.0M    0     0  15.2M      0  0:00:07  0:00:06  0:00:01 15.6M 87  120M   87  106M    0     0  15.0M      0  0:00:08  0:00:07  0:00:01 15.5M100  120M  100  120M    0     0  15.0M      0  0:00:08  0:00:08 --:--:-- 15.0M
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
] Testing  TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```