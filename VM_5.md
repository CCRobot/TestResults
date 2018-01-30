```
Executed on ddchakra004.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 91 11.1M   91 10.1M    0     0  10.5M      0  0:00:01 --:--:--  0:00:01 10.5M100 11.1M  100 11.1M    0     0  9870k      0  0:00:01  0:00:01 --:--:-- 9871k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  140M    6 9728k    0     0  11.8M      0  0:00:11 --:--:--  0:00:11 11.8M 17  140M   17 24.0M    0     0  13.2M      0  0:00:10  0:00:01  0:00:09 13.2M 22  140M   22 30.8M    0     0  11.0M      0  0:00:12  0:00:02  0:00:10 11.0M 31  140M   31 43.6M    0     0  11.4M      0  0:00:12  0:00:03  0:00:09 11.4M 39  140M   39 55.8M    0     0  11.6M      0  0:00:12  0:00:04  0:00:08 11.6M 48  140M   48 67.9M    0     0  11.7M      0  0:00:11  0:00:05  0:00:06 11.6M 59  140M   59 83.5M    0     0  12.2M      0  0:00:11  0:00:06  0:00:05 11.9M 68  140M   68 95.9M    0     0  12.2M      0  0:00:11  0:00:07  0:00:04 13.0M 79  140M   79  111M    0     0  12.6M      0  0:00:11  0:00:08  0:00:03 13.5M 87  140M   87  122M    0     0  12.5M      0  0:00:11  0:00:09  0:00:02 13.4M 96  140M   96  135M    0     0  12.5M      0  0:00:11  0:00:10  0:00:01 13.5M100  140M  100  140M    0     0  12.6M      0  0:00:11  0:00:11 --:--:-- 13.1M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   9c435c9..59b0b53  master      -> origin/master
   3e52c09..17fcf4a  release/1.8 -> origin/release/1.8
   abd18d0..0615a51  release/1.9 -> origin/release/1.9
Updating 9c435c9..59b0b53
Fast-forward
 lib/Jsrt/Jsrt.cpp                        | 22 ++++++++++++++++------
 lib/Jsrt/JsrtDiag.cpp                    | 10 +++++++---
 test/Debugger/emptyJson.dbg.baseline     |  1 +
 test/Debugger/loadscript_after_detach.js | 17 +++++++++++++++++
 test/Debugger/rlexe.xml                  |  6 ++++++
 5 files changed, 47 insertions(+), 9 deletions(-)
 create mode 100644 test/Debugger/emptyJson.dbg.baseline
 create mode 100644 test/Debugger/loadscript_after_detach.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_FLG2_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```