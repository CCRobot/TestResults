### Error Output   
```
{
   killed : false,
   code : 1,
   signal : null,
   cmd :  /bin/sh -c git checkout release/1.8 
} - [ exec ]
```
### stderr Output   

```
error: The following untracked working tree files would be overwritten by checkout:
	lib/Runtime/PlatformAgnostic/EventTrace.h
	lib/Runtime/PlatformAgnostic/Platform/Linux/EventTrace.cpp
	lib/Runtime/PlatformAgnostic/Platform/Windows/EventTrace.cpp
	lib/wabt/src/binary-reader-interpreter.cc
	lib/wabt/src/binary-reader-interpreter.h
	lib/wabt/src/interpreter.cc
	lib/wabt/src/interpreter.h
	pal/inc/CCSpinLock.hpp
	pal/src/sync/CCSpinLock.cpp
	test/native-tests/test-c98/Platform.js
	test/native-tests/test-c98/sample.cpp
	test/native-tests/test-char/Platform.js
	test/native-tests/test-char/dummy-1.c
	test/native-tests/test-char/dummy-2.c
	test/native-tests/test-char/sample.cpp
	test/native-tests/test-char16/Platform.js
	test/native-tests/test-char16/sample.cpp
	test/native-tests/test-pal/Platform.js
	test/native-tests/test-pal/sample.cpp
	test/native-tests/test-property/Platform.js
	test/native-tests/test-property/sample.cpp
Please move or remove them before you can switch branches.
Aborting

```
### stdout Output   

```

```   
#### exitCode : 1
