### Test Results [`RL18_DBG_F2_ubuntu`]   
*Target* -> `ubuntu`   
`Test was FAILED`

### Alias [ CHECKOUT_RELEASE1_8 ]   
*Test Command* : `git checkout release/1.8`   
*Details*      : [CHECKOUT_RELEASE1_8](https://github.com/CCRobot/TestResults/blob/20180204T035003RL18_DBG_F2_ubuntu/CHECKOUT_RELEASE1_8_0.md)   
*Exit Code*    : 0   

   
### Alias [ BUILD_STEP_UBUNTU ]   
*Test Command* : `./build.sh --static --debug -j=3`   
*Details*      : [BUILD_STEP_UBUNTU](https://github.com/CCRobot/TestResults/blob/20180204T035003RL18_DBG_F2_ubuntu/BUILD_STEP_UBUNTU_1.md)   
*Exit Code*    : 0   

   
### Alias [ BUILD_STEP_OSX ]   
*Test Command* : `./build.sh --static --debug -j=3 --icu=~/homebrew/Cellar/icu4c/58.2/include`   
*Details*      : [BUILD_STEP_OSX] was not executed yet   

   
### Alias [ TEST_STEP ]   
*Test Command* : `test/runtests.py -d --timeout 300 --flags "-RecyclerVerifyMark -RecyclerConcurrentStress -VerifyBarrierBit -KeepRecyclerTrackData" --include-slow --not-tag exclude_ccrobot`   
*Details*      : [TEST_STEP](https://github.com/CCRobot/TestResults/blob/20180204T035003RL18_DBG_F2_ubuntu/TEST_STEP_3.md)   
*Exit Code*    : 1   

   
### Alias [ VM ]   
*Test Command* : `stdout && stderr`   
*Details*      : [VM](https://github.com/CCRobot/TestResults/blob/20180204T035003RL18_DBG_F2_ubuntu/VM_4.md)   
*Exit Code*    : 0   

   
