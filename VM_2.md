```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  4 11.1M    4  479k    0     0  1885k      0  0:00:06 --:--:--  0:00:06 1880k100 11.1M  100 11.1M    0     0  10.6M      0  0:00:01  0:00:01 --:--:-- 10.6M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  153M    6 10.5M    0     0  9082k      0  0:00:17  0:00:01  0:00:16 9079k 15  153M   15 23.4M    0     0  10.6M      0  0:00:14  0:00:02  0:00:12 10.6M 21  153M   21 33.6M    0     0   9.9M      0  0:00:15  0:00:03  0:00:12  9.9M 26  153M   26 41.0M    0     0   9.7M      0  0:00:15  0:00:04  0:00:11  9.7M 33  153M   33 52.0M    0     0  10.0M      0  0:00:15  0:00:05  0:00:10 10.4M 41  153M   41 64.2M    0     0  10.3M      0  0:00:14  0:00:06  0:00:08 10.7M 49  153M   49 75.9M    0     0  10.5M      0  0:00:14  0:00:07  0:00:07 10.4M 56  153M   56 86.8M    0     0  10.5M      0  0:00:14  0:00:08  0:00:06 11.0M 62  153M   62 96.0M    0     0  10.4M      0  0:00:14  0:00:09  0:00:05 11.0M 69  153M   69  107M    0     0  10.5M      0  0:00:14  0:00:10  0:00:04 11.0M 76  153M   76  118M    0     0  10.5M      0  0:00:14  0:00:11  0:00:03 10.7M 83  153M   83  128M    0     0  10.5M      0  0:00:14  0:00:12  0:00:02 10.4M 91  153M   91  140M    0     0  10.6M      0  0:00:14  0:00:13  0:00:01 10.6M 96  153M   96  148M    0     0  10.4M      0  0:00:14  0:00:14 --:--:-- 10.4M100  153M  100  153M    0     0  10.3M      0  0:00:14  0:00:14 --:--:--  9.8M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   6ea656a..e4e4805  master      -> origin/master
   30bef33..f255bd9  release/1.8 -> origin/release/1.8
   f1a6b10..8af539b  release/1.9 -> origin/release/1.9
Updating 6ea656a..e4e4805
Fast-forward
 lib/Parser/Parse.cpp                        |  1 -
 lib/Runtime/Base/FunctionBody.cpp           | 10 +---
 lib/Runtime/Language/DynamicProfileInfo.cpp |  6 +-
 lib/Runtime/Library/JavascriptArray.inl     |  2 +-
 test/bailout/inline_get_bailout.js          | 32 +++++++++++
 test/bailout/inline_get_bailout_helper.js   | 18 ++++++
 test/bailout/rlexe.xml                      |  6 ++
 test/es6module/exportBinding.js             | 88 +++++++++++++++++++++++++++++
 test/es6module/exportBindingLoader.js       |  6 ++
 test/es6module/rlexe.xml                    |  7 +++
 10 files changed, 162 insertions(+), 14 deletions(-)
 create mode 100644 test/bailout/inline_get_bailout.js
 create mode 100644 test/bailout/inline_get_bailout_helper.js
 create mode 100644 test/es6module/exportBinding.js
 create mode 100644 test/es6module/exportBindingLoader.js
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