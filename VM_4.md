```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 65 11.1M   65 7504k    0     0  7334k      0  0:00:01  0:00:01 --:--:-- 7335k100 11.1M  100 11.1M    0     0  7244k      0  0:00:01  0:00:01 --:--:-- 7244k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  126M    2 3743k    0     0  8590k      0  0:00:15 --:--:--  0:00:15 8586k  9  126M    9 12.2M    0     0  8705k      0  0:00:14  0:00:01  0:00:13 8701k 18  126M   18 23.8M    0     0   9.7M      0  0:00:12  0:00:02  0:00:10  9.7M 25  126M   25 32.3M    0     0  9648k      0  0:00:13  0:00:03  0:00:10 9645k 33  126M   33 42.7M    0     0  9881k      0  0:00:13  0:00:04  0:00:09 9879k 40  126M   40 51.5M    0     0  9720k      0  0:00:13  0:00:05  0:00:08 9818k 46  126M   46 59.0M    0     0  9389k      0  0:00:13  0:00:06  0:00:07 9584k 53  126M   53 67.7M    0     0  9329k      0  0:00:13  0:00:07  0:00:06 8987k 61  126M   61 77.7M    0     0  9441k      0  0:00:13  0:00:08  0:00:05 9298k 69  126M   69 88.0M    0     0  9539k      0  0:00:13  0:00:09  0:00:04 9238k 76  126M   76 96.9M    0     0  9512k      0  0:00:13  0:00:10  0:00:03 9286k 83  126M   83  105M    0     0  9484k      0  0:00:13  0:00:11  0:00:02 9605k 90  126M   90  113M    0     0  9375k      0  0:00:13  0:00:12  0:00:01 9443k 97  126M   97  122M    0     0  9338k      0  0:00:13  0:00:13 --:--:-- 9166k100  126M  100  126M    0     0  9373k      0  0:00:13  0:00:13 --:--:-- 9013k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   dee6b5f..d7bb357  master      -> origin/master
   0be1e74..23984b9  release/1.8 -> origin/release/1.8
Updating dee6b5f..d7bb357
Fast-forward
 lib/Backend/BailOut.cpp                            |   8 +-
 lib/Backend/EmitBuffer.cpp                         |  37 ++-
 lib/Backend/EmitBuffer.h                           |   2 +-
 lib/Backend/GlobOpt.cpp                            |  59 ++--
 lib/Backend/GlobOpt.h                              |  23 ++
 lib/Backend/GlobOptIntBounds.cpp                   |   2 +-
 lib/Backend/InlineeFrameInfo.cpp                   |  17 +-
 lib/Backend/InlineeFrameInfo.h                     |   6 +-
 lib/Backend/InterpreterThunkEmitter.cpp            |  14 +-
 lib/Backend/JITOutput.cpp                          |   8 +-
 lib/Backend/JITThunkEmitter.cpp                    |   4 +-
 lib/Backend/Lower.cpp                              |  35 ++-
 lib/Backend/Lower.h                                |   2 +
 lib/Common/ConfigFlagsList.h                       |   5 +-
 lib/Common/Core/SysInfo.h                          |   2 +
 lib/Common/Memory/CustomHeap.cpp                   |   2 +-
 lib/Common/Memory/CustomHeap.h                     |   2 +-
 lib/Common/Memory/HeapBlockMap.cpp                 |   2 +-
 lib/Common/Memory/HeapConstants.h                  |   2 +
 lib/Common/Memory/PageAllocator.cpp                |   7 +-
 lib/Common/Memory/PageAllocator.h                  |   1 +
 lib/Common/Memory/Recycler.cpp                     |  12 +
 lib/Common/Memory/SectionAllocWrapper.cpp          |  16 +-
 lib/Common/Memory/SectionAllocWrapper.h            |   4 +-
 lib/Common/Memory/VirtualAllocWrapper.cpp          |  16 +-
 lib/Common/Memory/VirtualAllocWrapper.h            |   4 +-
 lib/JITServer/JITServer.cpp                        |   6 +-
 lib/Parser/Parse.cpp                               |   2 +-
 lib/Runtime/Base/ThreadContextInfo.cpp             |   5 +
 lib/Runtime/ByteCode/ByteCodeEmitter.cpp           |   7 +-
 lib/Runtime/ByteCode/ByteCodeGenerator.cpp         |   5 +
 lib/Runtime/Debug/DiagObjectModel.h                |   2 +-
 lib/Runtime/Debug/DiagStackFrame.cpp               |   2 +-
 lib/Runtime/Debug/TTRuntmeInfoTracker.cpp          |   5 +
 lib/Runtime/Debug/TTSerializeEnum.h                |   3 +
 lib/Runtime/Debug/TTSnapObjects.cpp                | 345 ++++++++++++++++++++-
 lib/Runtime/Debug/TTSnapObjects.h                  |  73 +++++
 lib/Runtime/Debug/TTSnapshot.cpp                   |  33 +-
 lib/Runtime/Debug/TTSupport.h                      | 130 ++++----
 lib/Runtime/Language/AsmJsByteCodeGenerator.cpp    |   7 +-
 lib/Runtime/Language/AsmJsEncoder.cpp              |   8 +-
 lib/Runtime/Language/InterpreterStackFrame.cpp     |  77 +++--
 lib/Runtime/Language/InterpreterStackFrame.h       |   6 +-
 lib/Runtime/Language/JavascriptOperators.cpp       |  16 +-
 lib/Runtime/Language/JavascriptOperators.h         |   2 +-
 lib/Runtime/Language/JavascriptStackWalker.cpp     |  32 +-
 lib/Runtime/Language/JavascriptStackWalker.h       |   7 +-
 lib/Runtime/Language/SourceTextModuleRecord.cpp    |  19 +-
 lib/Runtime/Library/CustomExternalIterator.h       |  18 ++
 lib/Runtime/Library/JavascriptArray.cpp            | 314 ++++---------------
 lib/Runtime/Library/JavascriptArray.h              |  16 +-
 lib/Runtime/Library/JavascriptArray.inl            |  83 +++--
 lib/Runtime/Library/JavascriptFunction.cpp         |   5 +-
 lib/Runtime/Library/JavascriptGenerator.cpp        | 157 +++++++++-
 lib/Runtime/Library/JavascriptGenerator.h          |  34 +-
 .../Library/JavascriptGeneratorFunction.cpp        |  27 +-
 lib/Runtime/Library/JavascriptGeneratorFunction.h  |  13 +-
 lib/Runtime/Library/JavascriptLibrary.cpp          |  35 ++-
 lib/Runtime/Library/JavascriptLibrary.h            |  10 +
 lib/Runtime/Library/ScriptFunction.cpp             |  19 +-
 lib/Runtime/Library/ScriptFunction.h               |   1 +
 lib/Runtime/Library/WebAssemblyModule.cpp          |   6 +
 lib/Runtime/Types/DynamicObject.cpp                |   4 +
 test/Optimizer/bug41530.js                         |  26 ++
 test/Optimizer/bug42111.js                         |  28 ++
 test/Optimizer/rlexe.xml                           |  10 +
 test/TTBasic/generatorBasic.js                     |  62 ++++
 test/TTBasic/generatorBasicRecord.baseline         |   4 +
 test/TTBasic/generatorBasicReplay_1.baseline       |   6 +
 test/TTBasic/generatorBasicReplay_2.baseline       |   6 +
 test/TTBasic/generatorBasicReplay_3.baseline       |   5 +
 test/TTBasic/generatorBasicReplay_4.baseline       |   4 +
 test/TTBasic/generatorBasicReplay_5.baseline       |   3 +
 test/TTBasic/generatorClassMethod.js               |  69 +++++
 test/TTBasic/generatorClassMethodRecord.baseline   |   3 +
 test/TTBasic/generatorClassMethodReplay.baseline   |   3 +
 test/TTBasic/generatorIntParam.js                  |  63 ++++
 test/TTBasic/generatorIntParamRecord.baseline      |   3 +
 test/TTBasic/generatorIntParamReplay.baseline      |   3 +
 test/TTBasic/generatorNested.js                    |  75 +++++
 test/TTBasic/generatorNestedRecord.baseline        |   5 +
 test/TTBasic/generatorNestedReplay.baseline        |   5 +
 test/TTBasic/generatorObjectParam.js               |  70 +++++
 test/TTBasic/generatorObjectParamRecord.baseline   |   3 +
 test/TTBasic/generatorObjectParamReplay.baseline   |   3 +
 test/TTBasic/generatorRestoreCompletedGenerator.js |  70 +++++
 ...neratorRestoreCompletedGeneratorRecord.baseline |   4 +
 ...neratorRestoreCompletedGeneratorReplay.baseline |   2 +
 test/TTBasic/generatorReturnYieldResult.js         |  58 ++++
 .../generatorReturnYieldResultRecord.baseline      |   3 +
 .../generatorReturnYieldResultReplay_1.baseline    |   5 +
 .../generatorReturnYieldResultReplay_2.baseline    |   5 +
 .../generatorReturnYieldResultReplay_3.baseline    |   4 +
 .../generatorReturnYieldResultReplay_4.baseline    |   3 +
 .../generatorWriteLogDuringGeneratorExecution.js   |  70 +++++
 ...WriteLogDuringGeneratorExecutionRecord.baseline |   4 +
 ...iteLogDuringGeneratorExecutionReplay_1.baseline |   6 +
 ...iteLogDuringGeneratorExecutionReplay_2.baseline |   6 +
 ...iteLogDuringGeneratorExecutionReplay_3.baseline |   5 +
 ...iteLogDuringGeneratorExecutionReplay_4.baseline |   4 +
 ...iteLogDuringGeneratorExecutionReplay_5.baseline |   3 +
 ...iteLogDuringGeneratorExecutionReplay_6.baseline |   2 +
 test/TTBasic/rlexe.xml                             | 227 ++++++++++++++
 test/es6/ES6ArrayAPI.js                            | 232 +++++++++++++-
 test/es6/function-expr-capture.js                  |  13 +
 test/es6/function-expr-capture2.js                 |  16 +
 test/es6/module-functionality.js                   |  19 ++
 test/es6/rlexe.xml                                 |  12 +
 108 files changed, 2499 insertions(+), 559 deletions(-)
 create mode 100644 test/Optimizer/bug41530.js
 create mode 100644 test/Optimizer/bug42111.js
 create mode 100644 test/TTBasic/generatorBasic.js
 create mode 100644 test/TTBasic/generatorBasicRecord.baseline
 create mode 100644 test/TTBasic/generatorBasicReplay_1.baseline
 create mode 100644 test/TTBasic/generatorBasicReplay_2.baseline
 create mode 100644 test/TTBasic/generatorBasicReplay_3.baseline
 create mode 100644 test/TTBasic/generatorBasicReplay_4.baseline
 create mode 100644 test/TTBasic/generatorBasicReplay_5.baseline
 create mode 100644 test/TTBasic/generatorClassMethod.js
 create mode 100644 test/TTBasic/generatorClassMethodRecord.baseline
 create mode 100644 test/TTBasic/generatorClassMethodReplay.baseline
 create mode 100644 test/TTBasic/generatorIntParam.js
 create mode 100644 test/TTBasic/generatorIntParamRecord.baseline
 create mode 100644 test/TTBasic/generatorIntParamReplay.baseline
 create mode 100644 test/TTBasic/generatorNested.js
 create mode 100644 test/TTBasic/generatorNestedRecord.baseline
 create mode 100644 test/TTBasic/generatorNestedReplay.baseline
 create mode 100644 test/TTBasic/generatorObjectParam.js
 create mode 100644 test/TTBasic/generatorObjectParamRecord.baseline
 create mode 100644 test/TTBasic/generatorObjectParamReplay.baseline
 create mode 100644 test/TTBasic/generatorRestoreCompletedGenerator.js
 create mode 100644 test/TTBasic/generatorRestoreCompletedGeneratorRecord.baseline
 create mode 100644 test/TTBasic/generatorRestoreCompletedGeneratorReplay.baseline
 create mode 100644 test/TTBasic/generatorReturnYieldResult.js
 create mode 100644 test/TTBasic/generatorReturnYieldResultRecord.baseline
 create mode 100644 test/TTBasic/generatorReturnYieldResultReplay_1.baseline
 create mode 100644 test/TTBasic/generatorReturnYieldResultReplay_2.baseline
 create mode 100644 test/TTBasic/generatorReturnYieldResultReplay_3.baseline
 create mode 100644 test/TTBasic/generatorReturnYieldResultReplay_4.baseline
 create mode 100644 test/TTBasic/generatorWriteLogDuringGeneratorExecution.js
 create mode 100644 test/TTBasic/generatorWriteLogDuringGeneratorExecutionRecord.baseline
 create mode 100644 test/TTBasic/generatorWriteLogDuringGeneratorExecutionReplay_1.baseline
 create mode 100644 test/TTBasic/generatorWriteLogDuringGeneratorExecutionReplay_2.baseline
 create mode 100644 test/TTBasic/generatorWriteLogDuringGeneratorExecutionReplay_3.baseline
 create mode 100644 test/TTBasic/generatorWriteLogDuringGeneratorExecutionReplay_4.baseline
 create mode 100644 test/TTBasic/generatorWriteLogDuringGeneratorExecutionReplay_5.baseline
 create mode 100644 test/TTBasic/generatorWriteLogDuringGeneratorExecutionReplay_6.baseline
 create mode 100644 test/es6/function-expr-capture.js
 create mode 100644 test/es6/function-expr-capture2.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_F2_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```