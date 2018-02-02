```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 30 11.1M   30 3487k    0     0  2938k      0  0:00:03  0:00:01  0:00:02 2938k 59 11.1M   59 6736k    0     0  3081k      0  0:00:03  0:00:02  0:00:01 3081k100 11.1M  100 11.1M    0     0  3935k      0  0:00:02  0:00:02 --:--:-- 3935k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  142M    1 1647k    0     0  5887k      0  0:00:24 --:--:--  0:00:24 5884k 12  142M   12 17.7M    0     0  13.8M      0  0:00:10  0:00:01  0:00:09 13.8M 21  142M   21 30.3M    0     0  13.3M      0  0:00:10  0:00:02  0:00:08 13.3M 28  142M   28 41.1M    0     0  12.5M      0  0:00:11  0:00:03  0:00:08 12.5M 37  142M   37 54.1M    0     0  12.6M      0  0:00:11  0:00:04  0:00:07 12.6M 47  142M   47 67.6M    0     0  12.8M      0  0:00:11  0:00:05  0:00:06 13.2M 56  142M   56 80.2M    0     0  12.7M      0  0:00:11  0:00:06  0:00:05 12.5M 64  142M   64 91.9M    0     0  12.6M      0  0:00:11  0:00:07  0:00:04 12.3M 74  142M   74  106M    0     0  12.8M      0  0:00:11  0:00:08  0:00:03 13.0M 81  142M   81  116M    0     0  12.6M      0  0:00:11  0:00:09  0:00:02 12.5M 90  142M   90  129M    0     0  12.5M      0  0:00:11  0:00:10  0:00:01 12.3M 99  142M   99  142M    0     0  12.6M      0  0:00:11  0:00:11 --:--:-- 12.4M100  142M  100  142M    0     0  12.6M      0  0:00:11  0:00:11 --:--:-- 12.6M
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
] Testing  DEBUG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```