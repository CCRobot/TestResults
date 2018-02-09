```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 67 11.1M   67 7664k    0     0  10.2M      0  0:00:01 --:--:--  0:00:01 10.2M100 11.1M  100 11.1M    0     0  10.2M      0  0:00:01  0:00:01 --:--:-- 10.2M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  2  153M    2 3407k    0     0  5330k      0  0:00:29 --:--:--  0:00:29 5324k 12  153M   12 18.9M    0     0  11.5M      0  0:00:13  0:00:01  0:00:12 11.5M 19  153M   19 29.7M    0     0  11.2M      0  0:00:13  0:00:02  0:00:11 11.2M 22  153M   22 35.0M    0     0  9869k      0  0:00:15  0:00:03  0:00:12 9868k 32  153M   32 49.2M    0     0  10.6M      0  0:00:14  0:00:04  0:00:10 10.6M 38  153M   38 59.5M    0     0  10.5M      0  0:00:14  0:00:05  0:00:09 11.2M 46  153M   46 70.9M    0     0  10.6M      0  0:00:14  0:00:06  0:00:08 10.3M 52  153M   52 80.3M    0     0  10.5M      0  0:00:14  0:00:07  0:00:07 10.1M 58  153M   58 89.7M    0     0  10.3M      0  0:00:14  0:00:08  0:00:06 10.9M 65  153M   65  100M    0     0  10.4M      0  0:00:14  0:00:09  0:00:05 10.3M 72  153M   72  111M    0     0  10.4M      0  0:00:14  0:00:10  0:00:04 10.3M 78  153M   78  120M    0     0  10.3M      0  0:00:14  0:00:11  0:00:03  9.8M 85  153M   85  131M    0     0  10.3M      0  0:00:14  0:00:12  0:00:02 10.1M 90  153M   90  138M    0     0  10.1M      0  0:00:15  0:00:13  0:00:02 9954k 94  153M   94  145M    0     0   9.9M      0  0:00:15  0:00:14  0:00:01 9155k 99  153M   99  153M    0     0   9.7M      0  0:00:15  0:00:15 --:--:-- 8556k100  153M  100  153M    0     0   9.8M      0  0:00:15  0:00:15 --:--:-- 8455k
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
] Testing  RL18_DBG_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```