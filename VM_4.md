```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  11.4M      0 --:--:-- --:--:-- --:--:-- 11.4M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  126M    0 1215k    0     0  4330k      0  0:00:29 --:--:--  0:00:29 4325k  9  126M    9 12.1M    0     0  9742k      0  0:00:13  0:00:01  0:00:12 9737k 19  126M   19 24.0M    0     0  10.4M      0  0:00:12  0:00:02  0:00:10 10.4M 30  126M   30 38.5M    0     0  11.7M      0  0:00:10  0:00:03  0:00:07 11.7M 41  126M   41 53.0M    0     0  12.3M      0  0:00:10  0:00:04  0:00:06 12.3M 50  126M   50 63.5M    0     0  12.0M      0  0:00:10  0:00:05  0:00:05 12.4M 58  126M   58 74.3M    0     0  11.8M      0  0:00:10  0:00:06  0:00:04 12.4M 69  126M   69 87.3M    0     0  11.9M      0  0:00:10  0:00:07  0:00:03 12.7M 78  126M   78 99.3M    0     0  12.0M      0  0:00:10  0:00:08  0:00:02 12.1M 88  126M   88  112M    0     0  12.0M      0  0:00:10  0:00:09  0:00:01 11.7M 98  126M   98  124M    0     0  12.1M      0  0:00:10  0:00:10 --:--:-- 12.2M100  126M  100  126M    0     0  12.2M      0  0:00:10  0:00:10 --:--:-- 12.7M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   dee6b5f..af8b2a8  master      -> origin/master
   0be1e74..23984b9  release/1.8 -> origin/release/1.8
Updating dee6b5f..af8b2a8
Fast-forward
 lib/Backend/BailOut.cpp                         |   8 +-
 lib/Backend/EmitBuffer.cpp                      |  37 ++-
 lib/Backend/EmitBuffer.h                        |   2 +-
 lib/Backend/GlobOpt.cpp                         |  59 +++--
 lib/Backend/GlobOpt.h                           |  23 ++
 lib/Backend/GlobOptIntBounds.cpp                |   2 +-
 lib/Backend/InlineeFrameInfo.cpp                |  17 +-
 lib/Backend/InlineeFrameInfo.h                  |   6 +-
 lib/Backend/InterpreterThunkEmitter.cpp         |  14 +-
 lib/Backend/JITOutput.cpp                       |   8 +-
 lib/Backend/JITThunkEmitter.cpp                 |   4 +-
 lib/Backend/Lower.cpp                           |  35 ++-
 lib/Backend/Lower.h                             |   2 +
 lib/Common/ConfigFlagsList.h                    |   5 +-
 lib/Common/Core/SysInfo.h                       |   2 +
 lib/Common/Memory/CustomHeap.cpp                |   2 +-
 lib/Common/Memory/CustomHeap.h                  |   2 +-
 lib/Common/Memory/HeapBlockMap.cpp              |   2 +-
 lib/Common/Memory/HeapConstants.h               |   2 +
 lib/Common/Memory/PageAllocator.cpp             |   7 +-
 lib/Common/Memory/PageAllocator.h               |   1 +
 lib/Common/Memory/Recycler.cpp                  |  12 +
 lib/Common/Memory/SectionAllocWrapper.cpp       |  16 +-
 lib/Common/Memory/SectionAllocWrapper.h         |   4 +-
 lib/Common/Memory/VirtualAllocWrapper.cpp       |  16 +-
 lib/Common/Memory/VirtualAllocWrapper.h         |   4 +-
 lib/JITServer/JITServer.cpp                     |   6 +-
 lib/Parser/Parse.cpp                            |   2 +-
 lib/Runtime/Base/ThreadContextInfo.cpp          |   5 +
 lib/Runtime/ByteCode/ByteCodeEmitter.cpp        |   7 +-
 lib/Runtime/ByteCode/ByteCodeGenerator.cpp      |   5 +
 lib/Runtime/Debug/DiagObjectModel.h             |   2 +-
 lib/Runtime/Debug/DiagStackFrame.cpp            |   2 +-
 lib/Runtime/Language/AsmJsByteCodeGenerator.cpp |   7 +-
 lib/Runtime/Language/AsmJsEncoder.cpp           |   8 +-
 lib/Runtime/Language/JavascriptOperators.cpp    |  16 +-
 lib/Runtime/Language/JavascriptOperators.h      |   2 +-
 lib/Runtime/Language/JavascriptStackWalker.cpp  |  32 ++-
 lib/Runtime/Language/JavascriptStackWalker.h    |   7 +-
 lib/Runtime/Language/SourceTextModuleRecord.cpp |  19 +-
 lib/Runtime/Library/JavascriptArray.cpp         | 314 +++++-------------------
 lib/Runtime/Library/JavascriptArray.h           |  16 +-
 lib/Runtime/Library/JavascriptArray.inl         |  83 +++----
 lib/Runtime/Library/JavascriptFunction.cpp      |   5 +-
 lib/Runtime/Library/WebAssemblyModule.cpp       |   6 +
 lib/Runtime/Types/DynamicObject.cpp             |   4 +
 test/Optimizer/bug41530.js                      |  26 ++
 test/Optimizer/bug42111.js                      |  28 +++
 test/Optimizer/rlexe.xml                        |  10 +
 test/es6/ES6ArrayAPI.js                         | 232 ++++++++++++++++-
 test/es6/function-expr-capture.js               |  13 +
 test/es6/function-expr-capture2.js              |  16 ++
 test/es6/module-functionality.js                |  19 ++
 test/es6/rlexe.xml                              |  12 +
 54 files changed, 786 insertions(+), 410 deletions(-)
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
] Testing  RLS18_TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```