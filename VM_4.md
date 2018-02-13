```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 11.1M  100 11.1M    0     0  11.8M      0 --:--:-- --:--:-- --:--:-- 11.8M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  8  155M    8 12.7M    0     0  11.9M      0  0:00:12  0:00:01  0:00:11 11.9M 14  155M   14 22.8M    0     0  11.0M      0  0:00:14  0:00:02  0:00:12 11.0M 19  155M   19 29.7M    0     0  9916k      0  0:00:16  0:00:03  0:00:13 9913k 26  155M   26 41.0M    0     0  10.0M      0  0:00:15  0:00:04  0:00:11 10.0M 34  155M   34 53.0M    0     0  10.4M      0  0:00:14  0:00:05  0:00:09 10.7M 41  155M   41 65.1M    0     0  10.7M      0  0:00:14  0:00:06  0:00:08 10.4M 49  155M   49 77.2M    0     0  10.9M      0  0:00:14  0:00:07  0:00:07 10.8M 55  155M   55 86.8M    0     0  10.7M      0  0:00:14  0:00:08  0:00:06 11.4M 64  155M   64 99.8M    0     0  11.0M      0  0:00:14  0:00:09  0:00:05 11.7M 67  155M   67  104M    0     0  10.3M      0  0:00:14  0:00:10  0:00:04 10.2M 70  155M   70  108M    0     0   9.8M      0  0:00:15  0:00:11  0:00:04 8969k 75  155M   75  117M    0     0  9958k      0  0:00:15  0:00:12  0:00:03 8203k 83  155M   83  129M    0     0   9.9M      0  0:00:15  0:00:13  0:00:02 8748k 86  155M   86  134M    0     0  9585k      0  0:00:16  0:00:14  0:00:02 6681k 90  155M   90  141M    0     0  9591k      0  0:00:16  0:00:15  0:00:01 7510k 97  155M   97  151M    0     0  9628k      0  0:00:16  0:00:16 --:--:-- 8617k100  155M  100  155M    0     0  9701k      0  0:00:16  0:00:16 --:--:-- 8990k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   7662f64..9d58876  master      -> origin/master
   ee5ffb3..3b3e3f8  release/1.8 -> origin/release/1.8
   db6afe6..e81ec84  release/1.9 -> origin/release/1.9
 * [new tag]         v1.8.1      -> v1.8.1
Updating 7662f64..9d58876
Fast-forward
 lib/Backend/FlowGraph.cpp                          |   3 +
 lib/Backend/FunctionJITTimeInfo.cpp                |  13 +-
 lib/Backend/GlobOpt.cpp                            |  43 +-
 lib/Backend/IRBuilder.cpp                          |  56 +--
 lib/Backend/IRBuilder.h                            |   2 +-
 lib/Backend/IRBuilderAsmJs.cpp                     |  16 +-
 lib/Backend/IRBuilderAsmJs.h                       |   2 -
 lib/Backend/Inline.cpp                             |  11 +-
 lib/Backend/JITTimeFunctionBody.cpp                |  28 +-
 lib/Backend/JITTimeProfileInfo.cpp                 |  22 +-
 lib/Backend/Lower.cpp                              | 475 +++++++++++++++++++--
 lib/Backend/Lower.h                                |   6 +-
 lib/Backend/LowerMDShared.cpp                      | 223 ++--------
 lib/Backend/LowerMDShared.h                        |   3 +-
 lib/Backend/Opnd.h                                 |   1 +
 lib/Backend/ServerScriptContext.cpp                |   2 +-
 lib/Backend/arm/LowerMD.cpp                        | 185 --------
 lib/Backend/arm/LowerMD.h                          |   5 -
 lib/Backend/arm64/EncoderMD.cpp                    |   8 +
 lib/Backend/arm64/LowerMD.cpp                      | 217 ++--------
 lib/Backend/arm64/LowerMD.h                        |   6 +-
 lib/Backend/arm64/MdOpCodes.h                      |   4 +-
 lib/Common/ConfigFlagsList.h                       |  18 +
 lib/Common/Core/ConfigParser.cpp                   |  21 +
 lib/Common/Memory/Allocator.h                      |   2 +-
 lib/Common/Memory/HeapBlockMap.h                   |   4 +-
 lib/Common/Memory/HeapBlockMap.inl                 |  42 +-
 lib/Common/Memory/MarkContext.inl                  |   2 +-
 lib/Common/Memory/Recycler.cpp                     |  64 ++-
 lib/Common/Memory/Recycler.h                       |   2 +-
 lib/Common/Memory/Recycler.inl                     |   4 +-
 lib/Common/Memory/WriteBarrierMacros.h             |   8 +
 lib/Parser/Parse.cpp                               |  37 +-
 lib/Parser/Parse.h                                 |   4 +-
 lib/Runtime/Base/FunctionBody.h                    |   5 +-
 lib/Runtime/Base/ThreadContext.h                   |  50 ++-
 lib/Runtime/ByteCode/AsmJsByteCodeDumper.cpp       |   2 +-
 lib/Runtime/Debug/DiagObjectModel.cpp              |   2 +-
 lib/Runtime/Debug/DiagObjectModel.h                |   5 +-
 lib/Runtime/Debug/TTInflateMap.cpp                 |   4 +-
 lib/Runtime/Debug/TTInflateMap.h                   |   8 +-
 lib/Runtime/Debug/TTSnapObjects.cpp                |   2 +-
 lib/Runtime/Debug/TTSnapValues.cpp                 |   8 +-
 lib/Runtime/Debug/TTSnapValues.h                   |   2 +-
 lib/Runtime/Debug/TTSnapshot.cpp                   |   2 +-
 lib/Runtime/Debug/TTSnapshotExtractor.cpp          |   6 +-
 lib/Runtime/Debug/TTSnapshotExtractor.h            |   2 +-
 lib/Runtime/Language/AsmJsModule.cpp               |   2 +-
 lib/Runtime/Language/InterpreterStackFrame.cpp     |   7 +-
 lib/Runtime/Language/InterpreterStackFrame.h       |   2 +-
 lib/Runtime/Language/JavascriptOperators.cpp       |   4 +-
 lib/Runtime/Library/BoundFunction.cpp              |   7 +-
 lib/Runtime/Library/BoundFunction.h                |   3 +-
 lib/Runtime/Library/ConcatString.cpp               |   4 +-
 lib/Runtime/Library/JavascriptArray.cpp            |  56 +--
 lib/Runtime/Library/JavascriptArray.h              |   7 +-
 .../Library/JavascriptGeneratorFunction.cpp        |   4 +-
 lib/Runtime/Library/JavascriptLibrary.cpp          |   3 +-
 lib/Runtime/Library/JavascriptLibrary.h            |   3 +-
 lib/Runtime/Library/RegexHelper.cpp                |   8 +-
 lib/Runtime/Library/ScriptFunction.cpp             |  10 +-
 lib/Runtime/Library/SparseArraySegment.h           |   5 +
 lib/Runtime/Library/StackScriptFunction.cpp        |  32 +-
 lib/Runtime/Library/StackScriptFunction.h          |   2 +-
 lib/Runtime/Library/WebAssemblyEnvironment.cpp     |   2 +-
 lib/Runtime/Library/WebAssemblyEnvironment.h       |   2 +-
 lib/Runtime/Library/WebAssemblyInstance.cpp        |   4 +-
 lib/Runtime/Library/WebAssemblyTable.cpp           |   7 +-
 lib/Runtime/Library/WebAssemblyTable.h             |   3 +-
 .../Types/DynamicObjectPropertyEnumerator.cpp      |   2 +-
 test/Bugs/bug_OS14115684.js                        |  17 +
 test/Bugs/rlexe.xml                                |   7 +
 tools/RecyclerChecker/RecyclerChecker.cpp          | 112 ++++-
 tools/RecyclerChecker/RecyclerChecker.h            |  25 ++
 74 files changed, 1087 insertions(+), 890 deletions(-)
 create mode 100644 test/Bugs/bug_OS14115684.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```