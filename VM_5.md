```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 49 11.1M   49 5584k    0     0  5115k      0  0:00:02  0:00:01  0:00:01 5113k100 11.1M  100 11.1M    0     0  6443k      0  0:00:01  0:00:01 --:--:-- 6441k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  140M    0  991k    0     0  3258k      0  0:00:44 --:--:--  0:00:44 3251k  7  140M    7 10.9M    0     0  8594k      0  0:00:16  0:00:01  0:00:15 8588k 13  140M   13 19.2M    0     0  8565k      0  0:00:16  0:00:02  0:00:14 8562k 18  140M   18 25.3M    0     0  7864k      0  0:00:18  0:00:03  0:00:15 7864k 21  140M   21 30.6M    0     0  7298k      0  0:00:19  0:00:04  0:00:15 7297k 26  140M   26 37.3M    0     0  7217k      0  0:00:19  0:00:05  0:00:14 7459k 31  140M   31 43.5M    0     0  7080k      0  0:00:20  0:00:06  0:00:14 6686k 37  140M   37 52.9M    0     0  7414k      0  0:00:19  0:00:07  0:00:12 6885k 42  140M   42 59.4M    0     0  7333k      0  0:00:19  0:00:08  0:00:11 6984k 47  140M   47 66.2M    0     0  7294k      0  0:00:19  0:00:09  0:00:10 7291k 51  140M   51 72.3M    0     0  7187k      0  0:00:20  0:00:10  0:00:10 7155k 56  140M   56 80.0M    0     0  7244k      0  0:00:19  0:00:11  0:00:08 7451k 62  140M   62 88.1M    0     0  7333k      0  0:00:19  0:00:12  0:00:07 7212k 68  140M   68 96.0M    0     0  7392k      0  0:00:19  0:00:13  0:00:06 7487k 74  140M   74  104M    0     0  7493k      0  0:00:19  0:00:14  0:00:05 7862k 80  140M   80  113M    0     0  7584k      0  0:00:18  0:00:15  0:00:03 8403k 86  140M   86  121M    0     0  7646k      0  0:00:18  0:00:16  0:00:02 8555k 93  140M   93  130M    0     0  7745k      0  0:00:18  0:00:17  0:00:01 8762k 98  140M   98  138M    0     0  7737k      0  0:00:18  0:00:18 --:--:-- 8656k100  140M  100  140M    0     0  7727k      0  0:00:18  0:00:18 --:--:-- 8509k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   ed21221..10170c4  master      -> origin/master
   17fcf4a..fdf00b8  release/1.8 -> origin/release/1.8
   172bac8..cc2aede  release/1.9 -> origin/release/1.9
Updating ed21221..10170c4
Fast-forward
 lib/Backend/EmitBuffer.cpp                         |  7 +++++
 lib/Backend/InterpreterThunkEmitter.cpp            |  8 ------
 lib/Backend/NativeCodeGenerator.cpp                | 10 +++----
 lib/Common/Common/Jobs.cpp                         | 14 ++++++++--
 lib/Common/Common/Jobs.h                           |  8 ++++++
 lib/Common/Core/ConfigParser.cpp                   |  3 +-
 lib/Common/Core/DelayLoadLibrary.cpp               |  7 +++--
 lib/Common/Memory/DelayDeletingFunctionTable.cpp   | 19 ++-----------
 lib/Common/Memory/XDataAllocator.h                 |  7 ++---
 lib/Common/Memory/amd64/XDataAllocator.cpp         |  8 +++++-
 lib/Jsrt/Core/JsrtCore.cpp                         |  4 ---
 lib/Runtime/Base/FunctionBody.cpp                  | 32 +++++++++++++---------
 lib/Runtime/Base/ScriptContext.cpp                 |  4 ++-
 .../Library/JavascriptRegExpConstructor.cpp        |  1 -
 14 files changed, 72 insertions(+), 60 deletions(-)
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  TEST_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```