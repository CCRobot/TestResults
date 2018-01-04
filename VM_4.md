```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 59 11.1M   59 6800k    0     0   9.9M      0  0:00:01 --:--:--  0:00:01  9.9M100 11.1M  100 11.1M    0     0  11.6M      0 --:--:-- --:--:-- --:--:-- 11.6M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4  120M    4 5600k    0     0  7894k      0  0:00:15 --:--:--  0:00:15 7887k 15  120M   15 18.3M    0     0  10.7M      0  0:00:11  0:00:01  0:00:10 10.7M 21  120M   21 25.8M    0     0  9794k      0  0:00:12  0:00:02  0:00:10 9793k 33  120M   33 40.7M    0     0  11.0M      0  0:00:10  0:00:03  0:00:07 10.9M 45  120M   45 54.5M    0     0  11.5M      0  0:00:10  0:00:04  0:00:06 11.5M 56  120M   56 68.0M    0     0  11.9M      0  0:00:10  0:00:05  0:00:05 12.5M 67  120M   67 81.2M    0     0  12.1M      0  0:00:09  0:00:06  0:00:03 12.5M 76  120M   76 92.0M    0     0  11.9M      0  0:00:10  0:00:07  0:00:03 13.1M 86  120M   86  104M    0     0  12.0M      0  0:00:10  0:00:08  0:00:02 12.8M 97  120M   97  117M    0     0  12.1M      0  0:00:09  0:00:09 --:--:-- 12.6M100  120M  100  120M    0     0  12.0M      0  0:00:10  0:00:10 --:--:-- 12.2M
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
] Testing  RL18_DBG_F2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```