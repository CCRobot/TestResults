```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 41 11.1M   41 4688k    0     0  8200k      0  0:00:01 --:--:--  0:00:01 8195k100 11.1M  100 11.1M    0     0  11.0M      0  0:00:01  0:00:01 --:--:-- 11.0M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  135M    3 4176k    0     0  7618k      0  0:00:18 --:--:--  0:00:18 7606k 11  135M   11 15.5M    0     0  10.0M      0  0:00:13  0:00:01  0:00:12 10.0M 17  135M   17 23.7M    0     0  9537k      0  0:00:14  0:00:02  0:00:12 9534k 28  135M   28 38.8M    0     0  10.9M      0  0:00:12  0:00:03  0:00:09 10.9M 37  135M   37 50.7M    0     0  11.1M      0  0:00:12  0:00:04  0:00:08 11.1M 48  135M   48 66.0M    0     0  11.9M      0  0:00:11  0:00:05  0:00:06 12.4M 56  135M   56 76.2M    0     0  11.6M      0  0:00:11  0:00:06  0:00:05 12.1M 61  135M   61 83.1M    0     0  11.0M      0  0:00:12  0:00:07  0:00:05 11.8M 70  135M   70 96.0M    0     0  11.2M      0  0:00:12  0:00:08  0:00:04 11.3M 80  135M   80  109M    0     0  11.4M      0  0:00:11  0:00:09  0:00:02 11.7M 90  135M   90  122M    0     0  11.5M      0  0:00:11  0:00:10  0:00:01 11.2M 99  135M   99  135M    0     0  11.7M      0  0:00:11  0:00:11 --:--:-- 11.7M100  135M  100  135M    0     0  11.7M      0  0:00:11  0:00:11 --:--:-- 13.0M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   8ce2142..065f718  master      -> origin/master
   c3c7923..c60cf51  release/1.8 -> origin/release/1.8
   50e5667..cfcbe3b  release/1.9 -> origin/release/1.9
Updating 8ce2142..065f718
Fast-forward
 bin/ch/WScriptJsrt.cpp                             |  129 +-
 bin/ch/WScriptJsrt.h                               |    1 +
 bin/ch/stdafx.h                                    |   51 +-
 lib/Backend/CodeGenWorkItem.cpp                    |   17 +-
 lib/Backend/EmitBuffer.cpp                         |   12 +-
 lib/Backend/EmitBuffer.h                           |    2 +-
 lib/Backend/NativeCodeGenerator.cpp                |   32 +-
 lib/Backend/NativeCodeGenerator.h                  |   13 +-
 lib/Backend/PDataManager.cpp                       |    2 +-
 lib/Common/BackendApi.h                            |    2 +-
 lib/Common/ConfigFlagsList.h                       |    1 +
 lib/Common/Core/DelayLoadLibrary.cpp               |    9 +-
 lib/Common/Memory/DelayDeletingFunctionTable.cpp   |    9 +-
 lib/Common/Memory/XDataAllocator.h                 |    1 +
 lib/Common/Memory/amd64/XDataAllocator.cpp         |    5 +-
 lib/JITServer/JITServer.cpp                        |    2 +-
 lib/Runtime/Base/FunctionBody.cpp                  |   47 +-
 lib/Runtime/Base/FunctionBody.h                    |    6 +-
 lib/Runtime/Base/ScriptContext.cpp                 |    4 +-
 lib/Runtime/Base/ScriptContext.h                   |    2 +-
 test/es6/rlexe.xml                                 |  112 -
 test/{es6 => es6module}/ModuleCircularBar.js       |    0
 test/{es6 => es6module}/ModuleCircularFoo.js       |    0
 test/{es6 => es6module}/ModuleComplexExports.js    |    0
 test/{es6 => es6module}/ModuleComplexReexports.js  |    0
 test/{es6 => es6module}/ModuleDefaultExport1.js    |    0
 test/{es6 => es6module}/ModuleDefaultExport2.js    |    0
 test/{es6 => es6module}/ModuleDefaultExport3.js    |    0
 test/{es6 => es6module}/ModuleDefaultExport4.js    |    0
 test/{es6 => es6module}/ModuleDefaultReexport.js   |    0
 test/{es6 => es6module}/ModuleReexportDefault.js   |    0
 test/{es6 => es6module}/ModuleSimpleExport.js      |    0
 test/{es6 => es6module}/ModuleSimpleReexport.js    |    0
 .../ValidExportDefaultStatement1.js                |    0
 .../ValidExportDefaultStatement2.js                |    0
 test/{es6 => es6module}/ValidExportStatements.js   |    0
 test/{es6 => es6module}/ValidExportStatements2.js  |    0
 test/{es6 => es6module}/ValidImportStatements.js   |    0
 test/{es6 => es6module}/ValidReExportStatements.js |    0
 test/{es6 => es6module}/bug_OS12095746.baseline    |    0
 test/{es6 => es6module}/bug_OS12095746.js          |    0
 test/{es6 => es6module}/bug_OS12095746_mod0.js     |    0
 test/{es6 => es6module}/bug_OS12095746_mod1.js     |    0
 test/{es6 => es6module}/bug_OS12095746_mod2.js     |    0
 test/{es6 => es6module}/bug_OS12095746_moddep.js   |    0
 test/{es6 => es6module}/bug_OS12113549_module1.js  |    0
 test/{es6 => es6module}/bug_OS14562349.js          |    0
 test/{es6 => es6module}/bug_issue_3076.js          |    0
 .../dynamic-module-functionality.js                |    0
 .../dynamic-module-import-specifier.js             |    0
 test/{es6 => es6module}/exportmodule.js            |    0
 test/{es6 => es6module}/module-3250-bug-dep.js     |    0
 test/{es6 => es6module}/module-3250-bug-dep2.js    |    0
 test/{es6 => es6module}/module-3250-ext-a.js       |    0
 test/{es6 => es6module}/module-3250-ext-b.js       |    0
 test/{es6 => es6module}/module-bugfixes.js         |    0
 test/{es6 => es6module}/module-functionality.js    |    0
 test/{es6 => es6module}/module-namespace.js        |    0
 test/{es6 => es6module}/module-syntax.js           |    0
 test/{es6 => es6module}/module-syntax1.js          |    0
 test/{es6 => es6module}/moduleExport1.js           |    0
 test/{es6 => es6module}/moduleImportTheError.js    |    0
 test/{es6 => es6module}/moduleThrowAnError.js      |    0
 test/{es6 => es6module}/moduleUrlInError.js        |    0
 test/{es6 => es6module}/module_1_2645.js           |    0
 test/{es6 => es6module}/module_2_2645.js           |    0
 test/{es6 => es6module}/module_4482_dep1.js        |    0
 test/{es6 => es6module}/module_4482_dep2.js        |    0
 test/{es6 => es6module}/module_4482_dep3.js        |    0
 test/{es6 => es6module}/module_4570_dep1.js        |    0
 test/{es6 => es6module}/module_4570_dep2.js        |    0
 test/{es6 => es6module}/moduletest1.js             |    0
 test/{es6 => es6module}/moduletest2.js             |    0
 test/{es6 => es6module}/moduletest2_mod0.js        |    0
 test/{es6 => es6module}/moduletest2_mod1a.js       |    0
 test/{es6 => es6module}/moduletest2_mod1b.js       |    0
 test/{es6 => es6module}/moduletest2_mod2a.js       |    0
 test/{es6 => es6module}/moduletest2_mod2b.js       |    0
 test/{es6 => es6module}/otherModule.js             |    0
 test/{es6 => es6module}/passmodule.js              |    0
 test/es6module/rlexe.xml                           |  129 ++
 test/es6module/test001.js                          | 1957 ++++++++++++++++++
 test/es6module/test002.js                          | 2159 ++++++++++++++++++++
 .../testDynamicImportfromModule.js                 |    0
 test/{es6 => es6module}/test_bug_2645.js           |    0
 test/rlexedirs.xml                                 |    5 +
 86 files changed, 4482 insertions(+), 227 deletions(-)
 rename test/{es6 => es6module}/ModuleCircularBar.js (100%)
 rename test/{es6 => es6module}/ModuleCircularFoo.js (100%)
 rename test/{es6 => es6module}/ModuleComplexExports.js (100%)
 rename test/{es6 => es6module}/ModuleComplexReexports.js (100%)
 rename test/{es6 => es6module}/ModuleDefaultExport1.js (100%)
 rename test/{es6 => es6module}/ModuleDefaultExport2.js (100%)
 rename test/{es6 => es6module}/ModuleDefaultExport3.js (100%)
 rename test/{es6 => es6module}/ModuleDefaultExport4.js (100%)
 rename test/{es6 => es6module}/ModuleDefaultReexport.js (100%)
 rename test/{es6 => es6module}/ModuleReexportDefault.js (100%)
 rename test/{es6 => es6module}/ModuleSimpleExport.js (100%)
 rename test/{es6 => es6module}/ModuleSimpleReexport.js (100%)
 rename test/{es6 => es6module}/ValidExportDefaultStatement1.js (100%)
 rename test/{es6 => es6module}/ValidExportDefaultStatement2.js (100%)
 rename test/{es6 => es6module}/ValidExportStatements.js (100%)
 rename test/{es6 => es6module}/ValidExportStatements2.js (100%)
 rename test/{es6 => es6module}/ValidImportStatements.js (100%)
 rename test/{es6 => es6module}/ValidReExportStatements.js (100%)
 rename test/{es6 => es6module}/bug_OS12095746.baseline (100%)
 rename test/{es6 => es6module}/bug_OS12095746.js (100%)
 rename test/{es6 => es6module}/bug_OS12095746_mod0.js (100%)
 rename test/{es6 => es6module}/bug_OS12095746_mod1.js (100%)
 rename test/{es6 => es6module}/bug_OS12095746_mod2.js (100%)
 rename test/{es6 => es6module}/bug_OS12095746_moddep.js (100%)
 rename test/{es6 => es6module}/bug_OS12113549_module1.js (100%)
 rename test/{es6 => es6module}/bug_OS14562349.js (100%)
 rename test/{es6 => es6module}/bug_issue_3076.js (100%)
 rename test/{es6 => es6module}/dynamic-module-functionality.js (100%)
 rename test/{es6 => es6module}/dynamic-module-import-specifier.js (100%)
 rename test/{es6 => es6module}/exportmodule.js (100%)
 rename test/{es6 => es6module}/module-3250-bug-dep.js (100%)
 rename test/{es6 => es6module}/module-3250-bug-dep2.js (100%)
 rename test/{es6 => es6module}/module-3250-ext-a.js (100%)
 rename test/{es6 => es6module}/module-3250-ext-b.js (100%)
 rename test/{es6 => es6module}/module-bugfixes.js (100%)
 rename test/{es6 => es6module}/module-functionality.js (100%)
 rename test/{es6 => es6module}/module-namespace.js (100%)
 rename test/{es6 => es6module}/module-syntax.js (100%)
 rename test/{es6 => es6module}/module-syntax1.js (100%)
 rename test/{es6 => es6module}/moduleExport1.js (100%)
 rename test/{es6 => es6module}/moduleImportTheError.js (100%)
 rename test/{es6 => es6module}/moduleThrowAnError.js (100%)
 rename test/{es6 => es6module}/moduleUrlInError.js (100%)
 rename test/{es6 => es6module}/module_1_2645.js (100%)
 rename test/{es6 => es6module}/module_2_2645.js (100%)
 rename test/{es6 => es6module}/module_4482_dep1.js (100%)
 rename test/{es6 => es6module}/module_4482_dep2.js (100%)
 rename test/{es6 => es6module}/module_4482_dep3.js (100%)
 rename test/{es6 => es6module}/module_4570_dep1.js (100%)
 rename test/{es6 => es6module}/module_4570_dep2.js (100%)
 rename test/{es6 => es6module}/moduletest1.js (100%)
 rename test/{es6 => es6module}/moduletest2.js (100%)
 rename test/{es6 => es6module}/moduletest2_mod0.js (100%)
 rename test/{es6 => es6module}/moduletest2_mod1a.js (100%)
 rename test/{es6 => es6module}/moduletest2_mod1b.js (100%)
 rename test/{es6 => es6module}/moduletest2_mod2a.js (100%)
 rename test/{es6 => es6module}/moduletest2_mod2b.js (100%)
 rename test/{es6 => es6module}/otherModule.js (100%)
 rename test/{es6 => es6module}/passmodule.js (100%)
 create mode 100644 test/es6module/rlexe.xml
 create mode 100755 test/es6module/test001.js
 create mode 100755 test/es6module/test002.js
 rename test/{es6 => es6module}/testDynamicImportfromModule.js (100%)
 rename test/{es6 => es6module}/test_bug_2645.js (100%)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  TEST_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```