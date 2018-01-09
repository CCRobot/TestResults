```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 38 11.1M   38 4384k    0     0  6167k      0  0:00:01 --:--:--  0:00:01 6165k100 11.1M  100 11.1M    0     0  8488k      0  0:00:01  0:00:01 --:--:-- 8493k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  1  126M    1 1791k    0     0  5025k      0  0:00:25 --:--:--  0:00:25 5018k  8  126M    8 10.1M    0     0  7672k      0  0:00:16  0:00:01  0:00:15 7669k 16  126M   16 20.2M    0     0  8812k      0  0:00:14  0:00:02  0:00:12 8811k 20  126M   20 25.6M    0     0  7708k      0  0:00:16  0:00:03  0:00:13 7707k 26  126M   26 33.2M    0     0  7821k      0  0:00:16  0:00:04  0:00:12 7820k 33  126M   33 42.6M    0     0  8154k      0  0:00:15  0:00:05  0:00:10 8377k 41  126M   41 52.0M    0     0  8364k      0  0:00:15  0:00:06  0:00:09 8552k 50  126M   50 64.1M    0     0  8925k      0  0:00:14  0:00:07  0:00:07 8977k 55  126M   55 70.5M    0     0  8645k      0  0:00:14  0:00:08  0:00:06 9290k 63  126M   63 80.5M    0     0  8816k      0  0:00:14  0:00:09  0:00:05 9681k 70  126M   70 88.7M    0     0  8768k      0  0:00:14  0:00:10  0:00:04 9426k 79  126M   79  100M    0     0  9024k      0  0:00:14  0:00:11  0:00:03 9865k 85  126M   85  108M    0     0  8977k      0  0:00:14  0:00:12  0:00:02 9052k 94  126M   94  119M    0     0  9151k      0  0:00:14  0:00:13  0:00:01 9996k100  126M  100  126M    0     0  9300k      0  0:00:13  0:00:13 --:--:-- 10.0M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   dee6b5f..866a382  master      -> origin/master
   0be1e74..66b6ba8  release/1.8 -> origin/release/1.8
Updating dee6b5f..866a382
Fast-forward
 lib/Backend/BailOut.cpp                         |  8 +--
 lib/Backend/EmitBuffer.cpp                      | 31 +++++++--
 lib/Backend/EmitBuffer.h                        |  2 +-
 lib/Backend/GlobOpt.cpp                         | 59 +++++++++++-------
 lib/Backend/GlobOpt.h                           | 23 +++++++
 lib/Backend/GlobOptIntBounds.cpp                |  2 +-
 lib/Backend/InlineeFrameInfo.cpp                | 17 ++---
 lib/Backend/InlineeFrameInfo.h                  |  6 +-
 lib/Backend/JITOutput.cpp                       |  2 +-
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
 lib/Runtime/ByteCode/ByteCodeEmitter.cpp        |  7 ++-
 lib/Runtime/ByteCode/ByteCodeGenerator.cpp      |  5 ++
 lib/Runtime/Debug/DiagObjectModel.h             |  2 +-
 lib/Runtime/Debug/DiagStackFrame.cpp            |  2 +-
 lib/Runtime/Language/AsmJsByteCodeGenerator.cpp |  7 ++-
 lib/Runtime/Language/AsmJsEncoder.cpp           |  2 +-
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
 test/es6/rlexe.xml                              | 12 ++++
 48 files changed, 491 insertions(+), 166 deletions(-)
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
] Testing  RL18_PACK
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```