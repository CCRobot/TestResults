```
Executed on ubu16chk4000013
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  5 9180k    5  463k    0     0   683k      0  0:00:13 --:--:--  0:00:13  683k100 9180k  100 9180k    0     0  7723k      0  0:00:01  0:00:01 --:--:-- 7728k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0  143M    0  143k    0     0   310k      0  0:07:54 --:--:--  0:07:54  310k 16  143M   16 24.0M    0     0  16.0M      0  0:00:08  0:00:01  0:00:07 16.0M 44  143M   44 64.0M    0     0  25.6M      0  0:00:05  0:00:02  0:00:03 25.6M 72  143M   72  104M    0     0  29.8M      0  0:00:04  0:00:03  0:00:01 29.8M100  143M  100  143M    0     0  32.7M      0  0:00:04  0:00:04 --:--:-- 32.7M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   6c93ac5..eac97b9  master     -> origin/master
   c4d03a6..006593e  release/1.8 -> origin/release/1.8
   1dd69bc..5c0bed5  release/1.9 -> origin/release/1.9
Updating 6c93ac5..eac97b9
Fast-forward
 lib/Parser/RegexParser.cpp              |  5 +++++
 lib/Parser/rterrors.h                   |  1 +
 pal/src/loader/module.cpp               |  2 +-
 test/Regex/rlexe.xml                    |  6 ++++++
 test/Regex/unicode_forbidden_escapes.js | 33 +++++++++++++++++++++++++++++++++
 5 files changed, 46 insertions(+), 1 deletion(-)
 create mode 100644 test/Regex/unicode_forbidden_escapes.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_DBG_F2_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```