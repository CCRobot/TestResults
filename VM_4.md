```
Executed on ubu16chk4000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  11.3M      0 --:--:-- --:--:-- --:--:-- 11.3M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 13  143M   13 20.0M    0     0  18.0M      0  0:00:07  0:00:01  0:00:06 18.0M 41  143M   41 60.0M    0     0  28.6M      0  0:00:05  0:00:02  0:00:03 28.6M 69  143M   69  100M    0     0  32.3M      0  0:00:04  0:00:03  0:00:01 32.2M 97  143M   97  140M    0     0  34.3M      0  0:00:04  0:00:04 --:--:-- 34.3M100  143M  100  143M    0     0  35.0M      0  0:00:04  0:00:04 --:--:-- 35.8M
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
] Testing  RLS18_TEST_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```