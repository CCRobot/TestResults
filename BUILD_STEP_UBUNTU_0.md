### Error Output   
```
{
   killed : false,
   code : 2,
   signal : null,
   cmd :  /bin/sh -c ./build.sh --static --debug -j=3 
} - [ exec ]
```
### stderr Output   

```

```
### stdout Output   

```
Searching for Clang...
Clang++ found at /usr/bin/clang++
Build path: /home/helixbot/dotnetbuild/work/c6429152-019c-49b7-9ed0-c0c11fbd8422/Work/979a27a3-ccf0-41d4-9d01-f5a897aca242/Exec/ChakraCore/out/Debug
-- /home/helixbot/dotnetbuild/work/c6429152-019c-49b7-9ed0-c0c11fbd8422/Work/979a27a3-ccf0-41d4-9d01-f5a897aca242/Exec/ChakraCore/bin/ch/DbgController.js.h is created

Compile Target : System Default
Generating Debug makefiles

-- The C compiler identification is Clang 3.8.0
-- The CXX compiler identification is Clang 3.8.0
-- Check for working C compiler: /usr/bin/clang
-- Check for working C compiler: /usr/bin/clang -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Detecting C compile features
-- Detecting C compile features - done
-- Check for working CXX compiler: /usr/bin/clang++
-- Check for working CXX compiler: /usr/bin/clang++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Performing Test CLANG_HAS_DISABLE_TAIL_CALLS_CFG
-- Performing Test CLANG_HAS_DISABLE_TAIL_CALLS_CFG - Success
-- The ASM compiler identification is Clang
-- Found assembler: /usr/bin/clang
-- Looking for include file ieeefp.h
-- Looking for include file ieeefp.h - not found
-- Looking for include file alloca.h
-- Looking for include file alloca.h - found
-- Looking for include file sys/vmparam.h
-- Looking for include file sys/vmparam.h - not found
-- Looking for include file mach/vm_types.h
-- Looking for include file mach/vm_types.h - not found
-- Looking for include file mach/vm_param.h
-- Looking for include file mach/vm_param.h - not found
-- Looking for include file procfs.h
-- Looking for include file procfs.h - not found
-- Looking for include file crt_externs.h
-- Looking for include file crt_externs.h - not found
-- Looking for include file sys/time.h
-- Looking for include file sys/time.h - found
-- Looking for include file pthread_np.h
-- Looking for include file pthread_np.h - not found
-- Looking for include file sys/lwp.h
-- Looking for include file sys/lwp.h - not found
-- Looking for include file runetype.h
-- Looking for include file runetype.h - not found
-- Looking for include file unicode/uchar.h
-- Looking for include file unicode/uchar.h - found
-- Looking for kqueue
-- Looking for kqueue - not found
-- Looking for getpwuid_r
-- Looking for getpwuid_r - found
-- Looking for pthread_suspend in pthread
-- Looking for pthread_suspend in pthread - not found
-- Looking for pthread_suspend_np in pthread
-- Looking for pthread_suspend_np in pthread - not found
-- Looking for pthread_continue in pthread
-- Looking for pthread_continue in pthread - not found
-- Looking for pthread_continue_np in pthread
-- Looking for pthread_continue_np in pthread - not found
-- Looking for pthread_resume_np in pthread
-- Looking for pthread_resume_np in pthread - not found
-- Looking for pthread_attr_get_np in pthread
-- Looking for pthread_attr_get_np in pthread - not found
-- Looking for pthread_getattr_np in pthread
-- Looking for pthread_getattr_np in pthread - found
-- Looking for pthread_sigqueue in pthread
-- Looking for pthread_sigqueue in pthread - found
-- Looking for sigreturn
-- Looking for sigreturn - found
-- Looking for _thread_sys_sigreturn
-- Looking for _thread_sys_sigreturn - not found
-- Looking for copysign
-- Looking for copysign - found
-- Looking for fsync
-- Looking for fsync - found
-- Looking for futimes
-- Looking for futimes - found
-- Looking for utimes
-- Looking for utimes - found
-- Looking for sysctl
-- Looking for sysctl - found
-- Looking for sysconf
-- Looking for sysconf - found
-- Looking for localtime_r
-- Looking for localtime_r - found
-- Looking for gmtime_r
-- Looking for gmtime_r - found
-- Looking for timegm
-- Looking for timegm - found
-- Looking for _snwprintf
-- Looking for _snwprintf - not found
-- Looking for poll
-- Looking for poll - found
-- Looking for statvfs
-- Looking for statvfs - found
-- Looking for thread_self
-- Looking for thread_self - not found
-- Looking for _lwp_self
-- Looking for _lwp_self - not found
-- Looking for pthread_mach_thread_np
-- Looking for pthread_mach_thread_np - not found
-- Looking for thread_set_exception_ports
-- Looking for thread_set_exception_ports - not found
-- Looking for vm_allocate
-- Looking for vm_allocate - not found
-- Looking for vm_read
-- Looking for vm_read - not found
-- Looking for directio
-- Looking for directio - not found
-- Looking for semget
-- Looking for semget - found
-- Looking for pthread_mutex_init
-- Looking for pthread_mutex_init - found
-- Looking for ttrace
-- Looking for ttrace - not found
-- Performing Test HAVE_STAT_TIMESPEC
-- Performing Test HAVE_STAT_TIMESPEC - Failed
-- Performing Test HAVE_STAT_NSEC
-- Performing Test HAVE_STAT_NSEC - Failed
-- Performing Test HAVE_TM_GMTOFF
-- Performing Test HAVE_TM_GMTOFF - Success
-- Performing Test HAVE_GREGSET_T
-- Performing Test HAVE_GREGSET_T - Success
-- Looking for sys/types.h
-- Looking for sys/types.h - found
-- Looking for stdint.h
-- Looking for stdint.h - found
-- Looking for stddef.h
-- Looking for stddef.h - found
-- Check size of struct reg
-- Check size of struct reg - failed
-- Check size of struct pt_regs
-- Check size of struct pt_regs - done
-- Check size of siginfo_t
-- Check size of siginfo_t - done
-- Check size of ucontext_t
-- Check size of ucontext_t - done
-- Check size of pthread_rwlock_t
-- Check size of pthread_rwlock_t - done
-- Check size of prwatch_t
-- Check size of prwatch_t - failed
-- Check size of off_t
-- Check size of off_t - done
-- Looking for SYS_yield
-- Looking for SYS_yield - not found
-- Looking for INFTIM
-- Looking for INFTIM - not found
-- Looking for CHAR_BIT
-- Looking for CHAR_BIT - not found
-- Looking for _DEBUG
-- Looking for _DEBUG - not found
-- Looking for _SC_PHYS_PAGES
-- Looking for _SC_PHYS_PAGES - found
-- Looking for _SC_AVPHYS_PAGES
-- Looking for _SC_AVPHYS_PAGES - found
-- Performing Test PLATFORM_ACCEPTS_ABS_OVERLOAD
-- Performing Test PLATFORM_ACCEPTS_ABS_OVERLOAD - Success
-- Performing Test REALPATH_SUPPORTS_NONEXISTENT_FILES
-- Performing Test REALPATH_SUPPORTS_NONEXISTENT_FILES - Failed
-- Performing Test SSCANF_SUPPORT_ll
-- Performing Test SSCANF_SUPPORT_ll - Success
-- Performing Test SSCANF_CANNOT_HANDLE_MISSING_EXPONENT
-- Performing Test SSCANF_CANNOT_HANDLE_MISSING_EXPONENT - Failed
-- Performing Test HAVE_LARGE_SNPRINTF_SUPPORT
-- Performing Test HAVE_LARGE_SNPRINTF_SUPPORT - Success
-- Performing Test HAVE_BROKEN_FIFO_SELECT
-- Performing Test HAVE_BROKEN_FIFO_SELECT - Failed
-- Performing Test HAVE_BROKEN_FIFO_KEVENT
-- Performing Test HAVE_BROKEN_FIFO_KEVENT - Failed
-- Performing Test HAVE_SCHED_GET_PRIORITY
-- Performing Test HAVE_SCHED_GET_PRIORITY - Success
-- Performing Test HAVE_SCHED_GETCPU
-- Performing Test HAVE_SCHED_GETCPU - Success
-- Performing Test HAVE_WORKING_GETTIMEOFDAY
-- Performing Test HAVE_WORKING_GETTIMEOFDAY - Success
-- Performing Test HAVE_WORKING_CLOCK_GETTIME
-- Performing Test HAVE_WORKING_CLOCK_GETTIME - Success
-- Performing Test HAVE_CLOCK_MONOTONIC
-- Performing Test HAVE_CLOCK_MONOTONIC - Success
-- Performing Test HAVE_CLOCK_MONOTONIC_COARSE
-- Performing Test HAVE_CLOCK_MONOTONIC_COARSE - Success
-- Performing Test HAVE_MACH_ABSOLUTE_TIME
-- Performing Test HAVE_MACH_ABSOLUTE_TIME - Failed
-- Performing Test HAVE_CLOCK_THREAD_CPUTIME
-- Performing Test HAVE_CLOCK_THREAD_CPUTIME - Success
-- Performing Test HAVE_MMAP_DEV_ZERO
-- Performing Test HAVE_MMAP_DEV_ZERO - Success
-- Performing Test MMAP_IGNORES_HINT
-- Performing Test MMAP_IGNORES_HINT - Failed
-- Performing Test MMAP_ANON_IGNORES_PROTECTION
-- Performing Test MMAP_ANON_IGNORES_PROTECTION - Failed
-- Performing Test MMAP_DOESNOT_ALLOW_REMAP
-- Performing Test MMAP_DOESNOT_ALLOW_REMAP - Failed
-- Performing Test ONE_SHARED_MAPPING_PER_FILEREGION_PER_PROCESS
-- Performing Test ONE_SHARED_MAPPING_PER_FILEREGION_PER_PROCESS - Failed
-- Performing Test PTHREAD_CREATE_MODIFIES_ERRNO
-- Performing Test PTHREAD_CREATE_MODIFIES_ERRNO - Failed
-- Performing Test SEM_INIT_MODIFIES_ERRNO
-- Performing Test SEM_INIT_MODIFIES_ERRNO - Failed
-- Performing Test HAVE_PROCFS_CTL
-- Performing Test HAVE_PROCFS_CTL - Failed
-- Performing Test HAVE_COMPATIBLE_ACOS
-- Performing Test HAVE_COMPATIBLE_ACOS - Success
-- Performing Test HAVE_COMPATIBLE_ASIN
-- Performing Test HAVE_COMPATIBLE_ASIN - Success
-- Performing Test HAVE_COMPATIBLE_ATAN2
-- Performing Test HAVE_COMPATIBLE_ATAN2 - Success
-- Performing Test HAVE_COMPATIBLE_EXP
-- Performing Test HAVE_COMPATIBLE_EXP - Failed
-- Performing Test HAVE_COMPATIBLE_LOG
-- Performing Test HAVE_COMPATIBLE_LOG - Success
-- Performing Test HAVE_COMPATIBLE_LOG10
-- Performing Test HAVE_COMPATIBLE_LOG10 - Success
-- Performing Test UNGETC_NOT_RETURN_EOF
-- Performing Test UNGETC_NOT_RETURN_EOF - Success
-- Performing Test HAS_POSIX_SEMAPHORES
-- Performing Test HAS_POSIX_SEMAPHORES - Success
-- Performing Test GETPWUID_R_SETS_ERRNO
-- Performing Test GETPWUID_R_SETS_ERRNO - Success
-- Performing Test FILE_OPS_CHECK_FERROR_OF_PREVIOUS_CALL
-- Performing Test FILE_OPS_CHECK_FERROR_OF_PREVIOUS_CALL - Failed
-- Looking for unistd.h
-- Looking for unistd.h - found
-- Looking for snprintf
-- Looking for snprintf - found
-- Looking for strcasecmp
-- Looking for strcasecmp - found
-- Check size of ssize_t
-- Check size of ssize_t - done
-- Check size of size_t
-- Check size of size_t - done
-- Configuring done
-- Generating done
-- Build files have been written to: /home/helixbot/dotnetbuild/work/c6429152-019c-49b7-9ed0-c0c11fbd8422/Work/979a27a3-ccf0-41d4-9d01-f5a897aca242/Exec/ChakraCore/out/Debug
Scanning dependencies of target libwabt
[  0%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/token.cc.o
Scanning dependencies of target Chakra.Pal
[  0%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/file.cpp.o
[  0%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/filecrt.cpp.o
[  1%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/finite.cpp.o
[  1%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/lstr.cpp.o
[  1%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/opcode.cc.o
[  1%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/malloc.cpp.o
[  1%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/mbstring.cpp.o
[  1%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/misc.cpp.o
Scanning dependencies of target Chakra.Backend
[  1%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/misctls.cpp.o
[  1%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/path.cpp.o
[  1%] Building CXX object lib/Backend/CMakeFiles/Chakra.Backend.dir/AgenPeeps.cpp.o
[  2%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/printf.cpp.o
[  2%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/error-handler.cc.o
[  2%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/printfcpp.cpp.o
[  2%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/silent_printf.cpp.o
[  2%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/string.cpp.o
[  2%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/stringtls.cpp.o
[  2%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/hash-util.cc.o
[  2%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/thread.cpp.o
[  3%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/filenames.cc.o
[  3%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/wchar.cpp.o
[  4%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/wchartls.cpp.o
In file included from /home/helixbot/dotnetbuild/work/c6429152-019c-49b7-9ed0-c0c11fbd8422/Work/979a27a3-ccf0-41d4-9d01-f5a897aca242/Exec/ChakraCore/lib/Backend/AgenPeeps.cpp:5:
In file included from /home/helixbot/dotnetbuild/work/c6429152-019c-49b7-9ed0-c0c11fbd8422/Work/979a27a3-ccf0-41d4-9d01-f5a897aca242/Exec/ChakraCore/lib/Backend/Backend.h:12:
In file included from /home/helixbot/dotnetbuild/work/c6429152-019c-49b7-9ed0-c0c11fbd8422/Work/979a27a3-ccf0-41d4-9d01-f5a897aca242/Exec/ChakraCore/lib/Backend/../Runtime/Runtime.h:520:
[1m/home/helixbot/dotnetbuild/work/c6429152-019c-49b7-9ed0-c0c11fbd8422/Work/979a27a3-ccf0-41d4-9d01-f5a897aca242/Exec/ChakraCore/lib/Backend/../Runtime/Library/PropertyString.h:25:22: [0m[0;1;31merror: [0m[1mno member named  propertyRecord  in  Js::PropertyString [0m
        return this->propertyRecord->GetPropertyId();
[0;1;32m               ~~~~  ^
[0m[  4%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/cruntime/runtime_proxy.cpp.o
[  4%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/makepath_s.c.o
[  4%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/mbusafecrt.c.o
[  4%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/safecrt_input_s.c.o
[  4%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/string-view.cc.o
[  4%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/safecrt_output_s.c.o
[  4%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/safecrt_winput_s.c.o
[  5%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/safecrt_woutput_s.c.o
[  5%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/memcpy_s.c.o
[  5%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/memmove_s.c.o
[  5%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/sprintf.c.o
1 error generated.
[  5%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/sscanf.c.o
lib/Backend/CMakeFiles/Chakra.Backend.dir/build.make:62: recipe for target  lib/Backend/CMakeFiles/Chakra.Backend.dir/AgenPeeps.cpp.o  failed
make[2]: *** [lib/Backend/CMakeFiles/Chakra.Backend.dir/AgenPeeps.cpp.o] Error 1
CMakeFiles/Makefile2:254: recipe for target  lib/Backend/CMakeFiles/Chakra.Backend.dir/all  failed
make[1]: *** [lib/Backend/CMakeFiles/Chakra.Backend.dir/all] Error 2
make[1]: *** Waiting for unfinished jobs....
[  5%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/ir.cc.o
[  5%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/strcat_s.c.o
[  5%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/expr-visitor.cc.o
[  5%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/strcpy_s.c.o
[  6%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/strncat_s.c.o
[  6%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/strncpy_s.c.o
[  6%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/swprintf.c.o
[  6%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/vsprintf.c.o
[  6%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/vswprint.c.o
[  6%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/wcscpy_s.c.o
[  7%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/wcsncpy_s.c.o
[  7%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/xtoa_s.c.o
[  7%] Building C object pal/src/CMakeFiles/Chakra.Pal.dir/safecrt/xtow_s.c.o
[  7%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/debug/debug.cpp.o
[  7%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/exception/seh.cpp.o
[  7%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/lexer-source.cc.o
[  7%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/exception/signal.cpp.o
[  7%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/file/directory.cpp.o
[  8%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/file/pal_file.cpp.o
[  8%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/lexer-source-line-finder.cc.o
[  8%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/file/filetime.cpp.o
[  8%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/wast-parser-lexer-shared.cc.o
[  8%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/file/pal_path.cpp.o
[  8%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/file/shmfilelockmgr.cpp.o
[  8%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/handlemgr/handleapi.cpp.o
[  8%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/handlemgr/handlemgr.cpp.o
[  8%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/init/pal.cpp.o
[  9%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/init/sxs.cpp.o
[  9%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/loader/module.cpp.o
[ 10%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/prebuilt/wast-lexer-gen.cc.o
[ 10%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/loader/modulename.cpp.o
[ 10%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/locale/unicode.cpp.o
[ 10%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/locale/unicode_data.cpp.o
[ 10%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/locale/utf8.cpp.o
[ 10%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/map/common.cpp.o
[ 11%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/map/map.cpp.o
[ 11%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/map/virtual.cpp.o
[ 11%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/memory/heap.cpp.o
[ 11%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/memory/local.cpp.o
[ 11%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/misc/bstr.cpp.o
[ 11%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/misc/dbgmsg.cpp.o
[ 11%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/misc/error.cpp.o
[ 11%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/wast-parser.cc.o
[ 12%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/misc/environ.cpp.o
[ 12%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/misc/random.cpp.o
[ 12%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/misc/strutil.cpp.o
[ 12%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/type-checker.cc.o
[ 12%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/misc/time.cpp.o
[ 12%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/misc/sysinfo.cpp.o
[ 12%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/misc/utils.cpp.o
[ 13%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/objmgr/palobjbase.cpp.o
[ 13%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/objmgr/shmobject.cpp.o
[ 13%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/validator.cc.o
[ 13%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/objmgr/shmobjectmanager.cpp.o
[ 13%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/shmemory/shmemory.cpp.o
[ 13%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/synchobj/event.cpp.o
[ 13%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/synchobj/mutex.cpp.o
[ 13%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/synchobj/semaphore.cpp.o
[ 14%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/synchmgr/synchcontrollers.cpp.o
[ 14%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/binary-reader.cc.o
[ 14%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/synchmgr/synchmanager.cpp.o
[ 14%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/synchmgr/wait.cpp.o
[ 14%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/sync/cs.cpp.o
[ 14%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/binary-reader-logging.cc.o
[ 14%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/sync/cclock.cpp.o
[ 14%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/thread/context.cpp.o
[ 14%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/thread/process.cpp.o
[ 14%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/binary-writer.cc.o
[ 15%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/thread/pal_thread.cpp.o
[ 15%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/thread/threadsusp.cpp.o
[ 16%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/binary-writer-spec.cc.o
[ 16%] Building ASM object pal/src/CMakeFiles/Chakra.Pal.dir/arch/i386/context2.S.o
[ 16%] Building ASM object pal/src/CMakeFiles/Chakra.Pal.dir/arch/i386/debugbreak.S.o
[ 16%] Building CXX object pal/src/CMakeFiles/Chakra.Pal.dir/arch/i386/processor.cpp.o
[ 16%] Building ASM object pal/src/CMakeFiles/Chakra.Pal.dir/arch/i386/asmhelpers.S.o
[ 16%] Built target Chakra.Pal
[ 16%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/binary-reader-ir.cc.o
[ 16%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/binding-hash.cc.o
[ 16%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/wat-writer.cc.o
[ 16%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/interp.cc.o
[ 16%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/binary-reader-interp.cc.o
[ 16%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/apply-names.cc.o
[ 17%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/generate-names.cc.o
[ 17%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/resolve-names.cc.o
[ 17%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/binary.cc.o
[ 17%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/color.cc.o
[ 17%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/common.cc.o
[ 17%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/config.cc.o
[ 17%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/feature.cc.o
[ 18%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/leb128.cc.o
[ 18%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/literal.cc.o
[ 18%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/option-parser.cc.o
[ 18%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/stream.cc.o
[ 18%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/tracing.cc.o
[ 18%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/src/utf8.cc.o
[ 19%] Building CXX object lib/wabt/CMakeFiles/libwabt.dir/chakra/wabtapi.cc.o
[ 19%] Built target libwabt
Makefile:83: recipe for target  all  failed
make: *** [all] Error 2
See error details above. Exit code was 2

```   
#### exitCode : 1
