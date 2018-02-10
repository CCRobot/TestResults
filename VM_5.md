```
Executed on DDCHAKRA001.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 56 11.1M   56 6400k    0     0  9474k      0  0:00:01 --:--:--  0:00:01 9467k100 11.1M  100 11.1M    0     0  10.9M      0  0:00:01  0:00:01 --:--:-- 10.9M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  3  154M    3 5984k    0     0  9359k      0  0:00:16 --:--:--  0:00:16 9350k 11  154M   11 18.3M    0     0  11.2M      0  0:00:13  0:00:01  0:00:12 11.2M 20  154M   20 30.9M    0     0  11.6M      0  0:00:13  0:00:02  0:00:11 11.6M 28  154M   28 44.5M    0     0  12.2M      0  0:00:12  0:00:03  0:00:09 12.2M 37  154M   37 58.6M    0     0  12.6M      0  0:00:12  0:00:04  0:00:08 12.6M 47  154M   47 73.0M    0     0  12.9M      0  0:00:11  0:00:05  0:00:06 13.4M 57  154M   57 88.0M    0     0  13.2M      0  0:00:11  0:00:06  0:00:05 13.9M 65  154M   65  101M    0     0  13.3M      0  0:00:11  0:00:07  0:00:04 14.1M 75  154M   75  117M    0     0  13.5M      0  0:00:11  0:00:08  0:00:03 14.5M 84  154M   84  129M    0     0  13.4M      0  0:00:11  0:00:09  0:00:02 14.2M 93  154M   93  143M    0     0  13.4M      0  0:00:11  0:00:10  0:00:01 14.0M100  154M  100  154M    0     0  13.5M      0  0:00:11  0:00:11 --:--:-- 13.9M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   e4e4805..a603ec3  master      -> origin/master
   f255bd9..6067869  release/1.8 -> origin/release/1.8
   8af539b..5a1a799  release/1.9 -> origin/release/1.9
Updating e4e4805..a603ec3
Fast-forward
 test/AsmJs/MathBuiltinsCall.baseline |  3 --
 test/AsmJs/MathBuiltinsCall.js       | 72 +++++++++++++++++++++---------------
 test/AsmJs/rlexe.xml                 |  6 ---
 test/DebuggerCommon/rlexe.xml        |  5 +--
 test/es7/rlexe.xml                   |  1 -
 5 files changed, 44 insertions(+), 43 deletions(-)
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