```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 10 11.1M   10 1183k    0     0  2507k      0  0:00:04 --:--:--  0:00:04 2507k100 11.1M  100 11.1M    0     0  8943k      0  0:00:01  0:00:01 --:--:-- 8947k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 12  126M   12 15.6M    0     0  13.1M      0  0:00:09  0:00:01  0:00:08 13.1M 24  126M   24 30.7M    0     0  14.0M      0  0:00:08  0:00:02  0:00:06 14.0M 37  126M   37 47.5M    0     0  14.9M      0  0:00:08  0:00:03  0:00:05 14.9M 49  126M   49 62.4M    0     0  14.9M      0  0:00:08  0:00:04  0:00:04 14.9M 61  126M   61 77.9M    0     0  15.0M      0  0:00:08  0:00:05  0:00:03 15.6M 74  126M   74 93.8M    0     0  15.1M      0  0:00:08  0:00:06  0:00:02 15.6M 85  126M   85  108M    0     0  15.0M      0  0:00:08  0:00:07  0:00:01 15.5M 97  126M   97  122M    0     0  15.0M      0  0:00:08  0:00:08 --:--:-- 15.0M100  126M  100  126M    0     0  15.0M      0  0:00:08  0:00:08 --:--:-- 15.1M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   dee6b5f..1e117b5  master      -> origin/master
   0be1e74..23984b9  release/1.8 -> origin/release/1.8
Updating dee6b5f..1e117b5
Fast-forward
 lib/Backend/BailOut.cpp                         |  8 +--
 lib/Backend/EmitBuffer.cpp                      | 37 ++++++++---
 lib/Backend/EmitBuffer.h                        |  2 +-
 lib/Backend/GlobOpt.cpp                         | 59 +++++++++++-------
 lib/Backend/GlobOpt.h                           | 23 +++++++
 lib/Backend/GlobOptIntBounds.cpp                |  2 +-
 lib/Backend/InlineeFrameInfo.cpp                | 17 ++---
 lib/Backend/InlineeFrameInfo.h                  |  6 +-
 lib/Backend/InterpreterThunkEmitter.cpp         | 14 ++++-
 lib/Backend/JITOutput.cpp                       |  8 ++-
 lib/Backend/JITThunkEmitter.cpp                 |  4 +-
 lib/Backend/Lower.cpp                           | 35 ++++++++++-
 lib/Backend/Lower.h                             |  2 +
 lib/Common/ConfigFlagsList.h                    |  5 +-
 lib/Common/Core/SysInfo.h                       |  2 +
 lib/Common/Memory/CustomHeap.cpp                |  2 +-
 lib/Common/Memory/CustomHeap.h                  |  2 +-
 lib/Common/Memory/HeapBlockMap.cpp              |  2 +-
 lib/Common/Memory/HeapConstants.h               |  2 +
 lib/Common/Memory/PageAllocator.cpp             |  7 +--
 lib/Common/Memory/PageAllocator.h               |  1 +
 lib/Common/Memory/Recycler.cpp                  | 12 ++++
 lib/Common/Memory/SectionAllocWrapper.cpp       | 16 ++++-
 lib/Common/Memory/SectionAllocWrapper.h         |  4 +-
 lib/Common/Memory/VirtualAllocWrapper.cpp       | 16 ++++-
 lib/Common/Memory/VirtualAllocWrapper.h         |  4 +-
 lib/JITServer/JITServer.cpp                     |  6 +-
 lib/Parser/Parse.cpp                            |  2 +-
 lib/Runtime/Base/ThreadContextInfo.cpp          |  5 ++
 lib/Runtime/ByteCode/ByteCodeEmitter.cpp        |  7 ++-
 lib/Runtime/ByteCode/ByteCodeGenerator.cpp      |  5 ++
 lib/Runtime/Debug/DiagObjectModel.h             |  2 +-
 lib/Runtime/Debug/DiagStackFrame.cpp            |  2 +-
 lib/Runtime/Language/AsmJsByteCodeGenerator.cpp |  7 ++-
 lib/Runtime/Language/AsmJsEncoder.cpp           |  8 ++-
 lib/Runtime/Language/JavascriptOperators.cpp    | 16 +++--
 lib/Runtime/Language/JavascriptOperators.h      |  2 +-
 lib/Runtime/Language/JavascriptStackWalker.cpp  | 32 +++++++---
 lib/Runtime/Language/JavascriptStackWalker.h    |  7 ++-
 lib/Runtime/Language/SourceTextModuleRecord.cpp | 19 +++++-
 lib/Runtime/Library/JavascriptArray.cpp         | 71 +++++++++++++++------
 lib/Runtime/Library/JavascriptArray.h           | 16 ++---
 lib/Runtime/Library/JavascriptArray.inl         | 83 +++++++++++--------------
 lib/Runtime/Library/JavascriptFunction.cpp      |  5 +-
 lib/Runtime/Library/WebAssemblyModule.cpp       |  6 ++
 lib/Runtime/Types/DynamicObject.cpp             |  4 ++
 test/Optimizer/bug41530.js                      | 26 ++++++++
 test/Optimizer/bug42111.js                      | 28 +++++++++
 test/Optimizer/rlexe.xml                        | 10 +++
 test/es6/function-expr-capture.js               | 13 ++++
 test/es6/function-expr-capture2.js              | 16 +++++
 test/es6/module-functionality.js                | 19 ++++++
 test/es6/rlexe.xml                              | 12 ++++
 53 files changed, 548 insertions(+), 173 deletions(-)
 create mode 100644 test/Optimizer/bug41530.js
 create mode 100644 test/Optimizer/bug42111.js
 create mode 100644 test/es6/function-expr-capture.js
 create mode 100644 test/es6/function-expr-capture2.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_F1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```