```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 55 11.1M   55 6368k    0     0  8538k      0  0:00:01 --:--:--  0:00:01 8536k100 11.1M  100 11.1M    0     0  10.7M      0  0:00:01  0:00:01 --:--:-- 10.7M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  142M    3 5328k    0     0  7664k      0  0:00:19 --:--:--  0:00:19 7655k 11  142M   11 16.0M    0     0  9628k      0  0:00:15  0:00:01  0:00:14 9624k 19  142M   19 28.0M    0     0  10.3M      0  0:00:13  0:00:02  0:00:11 10.3M 27  142M   27 38.7M    0     0  10.3M      0  0:00:13  0:00:03  0:00:10 10.3M 35  142M   35 50.9M    0     0  10.8M      0  0:00:13  0:00:04  0:00:09 10.8M 44  142M   44 63.4M    0     0  11.1M      0  0:00:12  0:00:05  0:00:07 11.6M 47  142M   47 67.2M    0     0  10.0M      0  0:00:14  0:00:06  0:00:08 10.2M 56  142M   56 80.1M    0     0  10.4M      0  0:00:13  0:00:07  0:00:06 10.4M 63  142M   63 91.0M    0     0  10.4M      0  0:00:13  0:00:08  0:00:05 10.6M 73  142M   73  104M    0     0  10.7M      0  0:00:13  0:00:09  0:00:04 10.7M 80  142M   80  115M    0     0  10.7M      0  0:00:13  0:00:10  0:00:03 10.3M 87  142M   87  125M    0     0  10.7M      0  0:00:13  0:00:11  0:00:02 11.6M 95  142M   95  136M    0     0  10.7M      0  0:00:13  0:00:12  0:00:01 11.2M100  142M  100  142M    0     0  10.8M      0  0:00:13  0:00:13 --:--:-- 11.4M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   e3b9cd5..6c93ac5  master      -> origin/master
   78de4fc..c4d03a6  release/1.8 -> origin/release/1.8
   3962348..1dd69bc  release/1.9 -> origin/release/1.9
Updating e3b9cd5..6c93ac5
Fast-forward
 CMakeLists.txt                                 |  13 ++-
 bin/ChakraCore/ChakraCore.def                  |   2 +
 bin/ch/ChakraRtInterface.h                     |   4 +-
 lib/JITServer/JITServer.cpp                    |  14 +++
 lib/Jsrt/ChakraDebug.h                         |  15 +++
 lib/Jsrt/Jsrt.cpp                              |   9 +-
 lib/Jsrt/JsrtDiag.cpp                          |  25 ++++-
 lib/Runtime/Base/ScriptContext.cpp             |   4 +-
 lib/Runtime/Base/ScriptContext.h               |  13 ++-
 lib/Runtime/Base/ThreadContext.cpp             |  12 ++-
 lib/Runtime/Debug/DiagObjectModel.cpp          |   6 +-
 lib/Runtime/Debug/TTActionEvents.cpp           |   8 +-
 lib/Runtime/Debug/TTEventLog.cpp               |  65 +++++++++----
 lib/Runtime/Debug/TTEventLog.h                 |  10 +-
 lib/Runtime/Debug/TTEvents.cpp                 |  34 +++++++
 lib/Runtime/Debug/TTEvents.h                   |  21 +++++
 lib/Runtime/Debug/TTExecutionInfo.cpp          | 125 ++++++++++++++++++++++++-
 lib/Runtime/Debug/TTExecutionInfo.h            |  39 +++++++-
 lib/Runtime/Debug/TTSupport.h                  |   6 +-
 lib/Runtime/Language/InterpreterLoop.inl       |  33 +++++++
 lib/Runtime/Language/InterpreterStackFrame.cpp |   5 +-
 lib/Runtime/Language/JavascriptOperators.cpp   |   2 +-
 lib/Runtime/Library/GlobalObject.cpp           |   2 +-
 lib/Runtime/Library/JavascriptFunction.cpp     |   2 +-
 test/Bugs/bug_OS14326981.js                    |  27 ++++++
 test/Bugs/rlexe.xml                            |   7 ++
 26 files changed, 446 insertions(+), 57 deletions(-)
 create mode 100644 test/Bugs/bug_OS14326981.js
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