```
Executed on ubu16chk4000011
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0 9180k    0 32348    0     0  90823      0  0:01:43 --:--:--  0:01:43 90610100 9180k  100 9180k    0     0  9795k      0 --:--:-- --:--:-- --:--:-- 9787k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  142M    0 81497    0     0   194k      0  0:12:33 --:--:--  0:12:33  194k 16  142M   16 24.0M    0     0  17.1M      0  0:00:08  0:00:01  0:00:07 17.1M 47  142M   47 68.0M    0     0  27.8M      0  0:00:05  0:00:02  0:00:03 27.8M 77  142M   77  110M    0     0  32.6M      0  0:00:04  0:00:03  0:00:01 32.6M100  142M  100  142M    0     0  34.6M      0  0:00:04  0:00:04 --:--:-- 34.6M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   e3b9cd5..6c93ac5  master     -> origin/master
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
] Testing  DEBUG_FLG1_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```