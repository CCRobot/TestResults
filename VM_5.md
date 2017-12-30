```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 44 11.1M   44 5088k    0     0  7036k      0  0:00:01 --:--:--  0:00:01 7027k100 11.1M  100 11.1M    0     0  10.4M      0  0:00:01  0:00:01 --:--:-- 10.4M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  119M    2 3135k    0     0  4939k      0  0:00:24 --:--:--  0:00:24 4937k 16  119M   16 19.5M    0     0  11.9M      0  0:00:10  0:00:01  0:00:09 11.9M 29  119M   29 35.7M    0     0  13.5M      0  0:00:08  0:00:02  0:00:06 13.5M 42  119M   42 50.4M    0     0  13.8M      0  0:00:08  0:00:03  0:00:05 13.8M 54  119M   54 64.6M    0     0  13.9M      0  0:00:08  0:00:04  0:00:04 13.9M 64  119M   64 77.1M    0     0  13.6M      0  0:00:08  0:00:05  0:00:03 14.8M 76  119M   76 91.6M    0     0  13.7M      0  0:00:08  0:00:06  0:00:02 14.4M 89  119M   89  106M    0     0  13.9M      0  0:00:08  0:00:07  0:00:01 14.1M100  119M  100  119M    0     0  14.0M      0  0:00:08  0:00:08 --:--:-- 14.2M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   69c203a..39f7ce4  master      -> origin/master
   10ad5ab..fac40c6  release/1.8 -> origin/release/1.8
Updating 69c203a..39f7ce4
Fast-forward
 lib/Backend/Security.cpp                           |    3 +-
 lib/wabt/CMakeLists.txt                            |    8 +-
 lib/wabt/README.md                                 |   10 +-
 lib/wabt/chakra/wabtapi.cc                         |   23 +-
 lib/wabt/chakra/wabtapi.h                          |    1 +
 lib/wabt/chakra/windows/config.h                   |  266 +-
 lib/wabt/src/apply-names.cc                        |   34 +-
 ...ader-interpreter.cc => binary-reader-interp.cc} |  505 +-
 ...reader-interpreter.h => binary-reader-interp.h} |   22 +-
 lib/wabt/src/binary-reader-ir.cc                   |   50 +-
 lib/wabt/src/binary-reader-linker.cc               |   14 +-
 lib/wabt/src/binary-reader-logging.cc              |   37 +-
 lib/wabt/src/binary-reader-logging.h               |   16 +-
 lib/wabt/src/binary-reader-nop.h                   |   18 +
 lib/wabt/src/binary-reader-objdump.cc              |  156 +-
 lib/wabt/src/binary-reader-opcnt.cc                |   12 +-
 lib/wabt/src/binary-reader.cc                      |   88 +-
 lib/wabt/src/binary-reader.h                       |   14 +
 lib/wabt/src/binary-writer-spec.cc                 |   61 +-
 lib/wabt/src/binary-writer.cc                      |  112 +-
 lib/wabt/src/binding-hash.cc                       |    9 +-
 lib/wabt/src/common.cc                             |   12 +-
 lib/wabt/src/common.h                              |   25 +-
 lib/wabt/src/config.cc                             |    6 +-
 lib/wabt/src/config.h.in                           |  155 +-
 lib/wabt/src/emscripten-exported.json              |   26 +-
 lib/wabt/src/emscripten-helpers.cc                 |   56 +-
 lib/wabt/src/error-handler.cc                      |    7 +-
 lib/wabt/src/expr-visitor.cc                       |    8 +
 lib/wabt/src/expr-visitor.h                        |    4 +
 lib/wabt/src/feature.def                           |    1 +
 lib/wabt/src/filenames.cc                          |   56 +
 lib/wabt/src/filenames.h                           |   51 +
 lib/wabt/src/generate-names.cc                     |   39 +-
 lib/wabt/src/{interpreter.cc => interp.cc}         |  539 +-
 lib/wabt/src/{interpreter.h => interp.h}           |  103 +-
 lib/wabt/src/intrusive-list.h                      |   15 +-
 lib/wabt/src/ir.cc                                 |   99 +-
 lib/wabt/src/ir.h                                  |  104 +-
 lib/wabt/src/leb128.cc                             |   16 +-
 lib/wabt/src/lexer-source-line-finder.cc           |   12 +-
 lib/wabt/src/lexer-source.cc                       |   25 +-
 lib/wabt/src/lexer-source.h                        |    2 +-
 lib/wabt/src/literal.cc                            |  100 +-
 lib/wabt/src/opcode.cc                             |   20 +-
 lib/wabt/src/opcode.def                            |   23 +-
 lib/wabt/src/opcode.h                              |    3 +-
 lib/wabt/src/option-parser.cc                      |   26 +-
 lib/wabt/src/prebuilt/wast-lexer-gen.cc            | 7116 +++++++++++---------
 lib/wabt/src/resolve-names.cc                      |   20 +-
 lib/wabt/src/result.h                              |    3 +-
 lib/wabt/src/stream.cc                             |   30 +-
 lib/wabt/src/stream.h                              |    9 +-
 lib/wabt/src/test-filenames.cc                     |   61 +
 lib/wabt/src/test-intrusive-list.cc                |    3 +-
 lib/wabt/src/test-utf8.cc                          |    3 +-
 lib/wabt/src/token.cc                              |    5 +-
 lib/wabt/src/token.h                               |    2 +
 lib/wabt/src/tools/spectest-interp.cc              | 1605 +++--
 lib/wabt/src/tools/wasm-interp.cc                  |   83 +-
 lib/wabt/src/tools/wasm-link.cc                    |   54 +-
 lib/wabt/src/tools/wasm-objdump.cc                 |    2 +-
 lib/wabt/src/tools/wasm-opcodecnt.cc               |    2 +-
 lib/wabt/src/tools/wasm-validate.cc                |   95 +
 lib/wabt/src/tools/wasm2wat.cc                     |   10 +-
 lib/wabt/src/tools/wast2json.cc                    |   10 +-
 lib/wabt/src/tools/wat-desugar.cc                  |   12 +-
 lib/wabt/src/tools/wat2wasm.cc                     |   38 +-
 lib/wabt/src/tracing.cc                            |    3 +-
 lib/wabt/src/type-checker.cc                       |  230 +-
 lib/wabt/src/type-checker.h                        |   22 +-
 lib/wabt/src/utf8.cc                               |    6 +-
 lib/wabt/src/validator.cc                          |  211 +-
 lib/wabt/src/validator.h                           |   23 +-
 lib/wabt/src/wabt.post.js                          |   70 +-
 lib/wabt/src/wast-lexer.cc                         |   29 +-
 lib/wabt/src/wast-lexer.h                          |    8 +-
 lib/wabt/src/wast-parser.cc                        |  272 +-
 lib/wabt/src/wast-parser.h                         |    4 +
 lib/wabt/src/wat-writer.cc                         |  131 +-
 lib/wabt/ubsan.blacklist                           |    9 +-
 lib/wabt/wabt.vcxproj                              |    2 +
 test/WasmSpec/baselines/call_indirect.baseline     |    2 +-
 test/WasmSpec/baselines/float_literals.baseline    |    2 +-
 test/WasmSpec/baselines/linking.baseline           |    2 +-
 test/WasmSpec/baselines/unreached-invalid.baseline |    2 +-
 .../baselines/utf8-invalid-encoding.baseline       |    1 +
 test/WasmSpec/rlexe.xml                            |   31 +-
 test/WasmSpec/testsuite.rev                        |    2 +-
 test/WasmSpec/testsuite/build.py                   |   16 +-
 test/WasmSpec/testsuite/core/br.wast               |    8 +-
 test/WasmSpec/testsuite/core/br_table.wast         |    8 +-
 test/WasmSpec/testsuite/core/call_indirect.wast    |  234 +-
 test/WasmSpec/testsuite/core/elem.wast             |   44 +-
 test/WasmSpec/testsuite/core/float_literals.wast   |   12 +
 test/WasmSpec/testsuite/core/func.wast             |   16 +-
 test/WasmSpec/testsuite/core/func_ptrs.wast        |    6 +-
 test/WasmSpec/testsuite/core/imports.wast          |  108 +-
 test/WasmSpec/testsuite/core/left-to-right.wast    |    8 +-
 test/WasmSpec/testsuite/core/linking.wast          |   18 +-
 test/WasmSpec/testsuite/core/memory.wast           |    2 +-
 test/WasmSpec/testsuite/core/return.wast           |   16 +-
 test/WasmSpec/testsuite/core/typecheck.wast        |    4 +-
 test/WasmSpec/testsuite/core/unreachable.wast      |   16 +-
 .../WasmSpec/testsuite/core/unreached-invalid.wast |   55 +
 .../testsuite/core/utf8-invalid-encoding.wast      |  176 +
 .../testsuite/harness/wasm-module-builder.js       |    4 +-
 test/wasm/basic.wast                               |    2 +-
 test/wasm/inlining.js                              |    2 +-
 test/wasm/table.wast                               |    2 +-
 test/wasm/wasts/api.wast                           |    4 +-
 test/wasm/wasts/table_imports.wast                 |    8 +-
 tools/create_package.sh                            |    2 +-
 113 files changed, 8166 insertions(+), 5822 deletions(-)
 rename lib/wabt/src/{binary-reader-interpreter.cc => binary-reader-interp.cc} (74%)
 rename lib/wabt/src/{binary-reader-interpreter.h => binary-reader-interp.h} (60%)
 create mode 100644 lib/wabt/src/filenames.cc
 create mode 100644 lib/wabt/src/filenames.h
 rename lib/wabt/src/{interpreter.cc => interp.cc} (90%)
 rename lib/wabt/src/{interpreter.h => interp.h} (92%)
 create mode 100644 lib/wabt/src/test-filenames.cc
 create mode 100644 lib/wabt/src/tools/wasm-validate.cc
 create mode 100644 test/WasmSpec/baselines/utf8-invalid-encoding.baseline
 create mode 100644 test/WasmSpec/testsuite/core/utf8-invalid-encoding.wast
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_FLG1_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```