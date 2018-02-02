```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  10.6M      0  0:00:01  0:00:01 --:--:-- 10.6M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  142M    5 7664k    0     0  7068k      0  0:00:20  0:00:01  0:00:19 7063k 14  142M   14 21.1M    0     0  10.1M      0  0:00:14  0:00:02  0:00:12 10.1M 23  142M   23 33.1M    0     0   9.8M      0  0:00:14  0:00:03  0:00:11  9.8M 28  142M   28 41.2M    0     0  10.1M      0  0:00:14  0:00:04  0:00:10 10.1M 38  142M   38 54.8M    0     0  10.7M      0  0:00:13  0:00:05  0:00:08 11.0M 47  142M   47 68.0M    0     0  11.1M      0  0:00:12  0:00:06  0:00:06 12.1M 57  142M   57 82.6M    0     0  11.6M      0  0:00:12  0:00:07  0:00:05 12.3M 67  142M   67 97.1M    0     0  12.0M      0  0:00:11  0:00:08  0:00:03 13.5M 75  142M   75  107M    0     0  11.8M      0  0:00:12  0:00:09  0:00:03 13.2M 85  142M   85  121M    0     0  12.0M      0  0:00:11  0:00:10  0:00:01 13.4M 97  142M   97  139M    0     0  12.5M      0  0:00:11  0:00:11 --:--:-- 14.2M100  142M  100  142M    0     0  12.6M      0  0:00:11  0:00:11 --:--:-- 14.3M
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
] Testing  NODE_BUILD_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```