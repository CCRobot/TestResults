```
Executed on ubu16chk400000G
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  7554k      0  0:00:01  0:00:01 --:--:-- 7556k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5  135M    5 7568k    0     0  6771k      0  0:00:20  0:00:01  0:00:19 6769k 26  135M   26 36.0M    0     0  16.9M      0  0:00:08  0:00:02  0:00:06 16.9M 53  135M   53 72.0M    0     0  22.6M      0  0:00:05  0:00:03  0:00:02 22.6M 79  135M   79  108M    0     0  25.7M      0  0:00:05  0:00:04  0:00:01 25.7M100  135M  100  135M    0     0  27.9M      0  0:00:04  0:00:04 --:--:-- 28.6M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   8ce2142..065f718  master     -> origin/master
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
] Testing  RL18_DBG_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```