- 👋 Hi, I’m @omaurodiaz
- 👀 I’m interested in fix my linux mindt
- 🌱 I’m currently learning for an error that describes below
-     Please, help me. My computer no work correctly. very slowly. Three days ago, I try to download a film in 4K and it began to crash
-     this is the information of the bug
GDB Log                                                           
===================================================================

warning: core file may not match specified executable file.
[New LWP 2189]
[New LWP 2202]
[New LWP 2201]
[Thread debugging using libthread_db enabled]
Using host libthread_db library "/lib/x86_64-linux-gnu/libthread_db.so.1".
Core was generated by `/usr/libexec/xdg-document-portal'.
Program terminated with signal SIGSEGV, Segmentation fault.
#0  0x00007f66c00008d0 in ?? ()
[Current thread is 1 (Thread 0x7f66db634880 (LWP 2189))]

===================================================================
 GDB Backtrace                                                     
===================================================================

warning: core file may not match specified executable file.
[New LWP 2189]
[New LWP 2202]
[New LWP 2201]
[Thread debugging using libthread_db enabled]
Using host libthread_db library "/lib/x86_64-linux-gnu/libthread_db.so.1".
Core was generated by `/usr/libexec/xdg-document-portal'.
Program terminated with signal SIGSEGV, Segmentation fault.
#0  0x00007f66c00008d0 in ?? ()
[Current thread is 1 (Thread 0x7f66db634880 (LWP 2189))]
#0  0x00007f66c00008d0 in ?? ()
#1  0x00007f66da908648 in fuse_session_exit () from /lib/x86_64-linux-gnu/libfuse.so.2
#2  0x00005637ebdb38c5 in ?? ()
#3  0x00005637ebda9bac in ?? ()
#4  0x00007f66da301c87 in __libc_start_main (main=0x5637ebda98a0, argc=1, argv=0x7ffc3fb617a8, init=<optimized out>, fini=<optimized out>, rtld_fini=<optimized out>, stack_end=0x7ffc3fb61798) at ../csu/libc-start.c:310
#5  0x00005637ebda9cca in ?? ()

===================================================================
 GDB Backtrace (all threads)                                       
===================================================================

warning: core file may not match specified executable file.
[New LWP 2189]
[New LWP 2202]
[New LWP 2201]
[Thread debugging using libthread_db enabled]
Using host libthread_db library "/lib/x86_64-linux-gnu/libthread_db.so.1".
Core was generated by `/usr/libexec/xdg-document-portal'.
Program terminated with signal SIGSEGV, Segmentation fault.
#0  0x00007f66c00008d0 in ?? ()
[Current thread is 1 (Thread 0x7f66db634880 (LWP 2189))]

Thread 3 (Thread 0x7f66d85fb700 (LWP 2201)):
#0  0x00007f66da3f4bb9 in __GI___poll (fds=0x5637edaeabc0, nfds=1, timeout=-1) at ../sysdeps/unix/sysv/linux/poll.c:29
        resultvar = 18446744073709551602
        sc_cancel_oldtype = 0
        sc_ret = <optimized out>
#1  0x00007f66dab786e9 in ?? () from /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0
No symbol table info available.
#2  0x00007f66dab787fc in g_main_context_iteration () from /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0
No symbol table info available.
#3  0x00007f66dab78841 in ?? () from /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0
No symbol table info available.
#4  0x00007f66daba02a5 in ?? () from /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0
No symbol table info available.
#5  0x00007f66da6d86db in start_thread (arg=0x7f66d85fb700) at pthread_create.c:463
        pd = 0x7f66d85fb700
        now = <optimized out>
        unwind_buf = {cancel_jmp_buf = {{jmp_buf = {140079693543168, -5472672831885577405, 140079693540992, 0, 94798210833408, 140721377383264, 5386474141166039875, 5386478692602180419}, mask_was_saved = 0}}, priv = {pad = {0x0, 0x0, 0x0, 0x0}, data = {prev = 0x0, cleanup = 0x0, canceltype = 0}}}
        not_first_call = <optimized out>
#6  0x00007f66da40161f in clone () at ../sysdeps/unix/sysv/linux/x86_64/clone.S:95
No locals.

Thread 2 (Thread 0x7f66d7dfa700 (LWP 2202)):
#0  0x00007f66dabbe421 in g_private_get () from /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0
No symbol table info available.
#1  0x00007f66daba0790 in g_thread_self () from /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0
No symbol table info available.
#2  0x00007f66dab7757c in g_main_context_acquire () from /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0
No symbol table info available.
#3  0x00007f66dab785a5 in ?? () from /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0
No symbol table info available.
#4  0x00007f66dab78a82 in g_main_loop_run () from /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0
No symbol table info available.
#5  0x00007f66db1662d6 in ?? () from /usr/lib/x86_64-linux-gnu/libgio-2.0.so.0
No symbol table info available.
#6  0x00007f66daba02a5 in ?? () from /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0
No symbol table info available.
#7  0x00007f66da6d86db in start_thread (arg=0x7f66d7dfa700) at pthread_create.c:463
        pd = 0x7f66d7dfa700
        now = <optimized out>
        unwind_buf = {cancel_jmp_buf = {{jmp_buf = {140079685150464, -5472672831885577405, 140079685148288, 0, 94798210833568, 140721377383648, 5386453249908241219, 5386478692602180419}, mask_was_saved = 0}}, priv = {pad = {0x0, 0x0, 0x0, 0x0}, data = {prev = 0x0, cleanup = 0x0, canceltype = 0}}}
        not_first_call = <optimized out>
#8  0x00007f66da40161f in clone () at ../sysdeps/unix/sysv/linux/x86_64/clone.S:95
No locals.

Thread 1 (Thread 0x7f66db634880 (LWP 2189)):
#0  0x00007f66c00008d0 in ?? ()
No symbol table info available.
#1  0x00007f66da908648 in fuse_session_exit () from /lib/x86_64-linux-gnu/libfuse.so.2
No symbol table info available.
#2  0x00005637ebdb38c5 in ?? ()
No symbol table info available.
#3  0x00005637ebda9bac in ?? ()
No symbol table info available.
#4  0x00007f66da301c87 in __libc_start_main (main=0x5637ebda98a0, argc=1, argv=0x7ffc3fb617a8, init=<optimized out>, fini=<optimized out>, rtld_fini=<optimized out>, stack_end=0x7ffc3fb61798) at ../csu/libc-start.c:310
        self = <optimized out>
        __self = <optimized out>
        result = <optimized out>
        unwind_buf = {cancel_jmp_buf = {{jmp_buf = {0, 1757246878099403587, 94798180162720, 140721377384352, 0, 0, 5473375901685609283, 5386478250979062595}, mask_was_saved = 0}}, priv = {pad = {0x0, 0x0, 0x7f66db4468d3 <_dl_init+259>, 0x7f66db42c5b8}, data = {prev = 0x0, cleanup = 0x0, canceltype = -616273709}}}
        not_first_call = <optimized out>
#5  0x00005637ebda9cca in ?? ()
No symbol table info available.
#0  0x00007f66c00008d0 in ?? ()
#1  0x00007f66da908648 in fuse_session_exit () from /lib/x86_64-linux-gnu/libfuse.so.2
#2  0x00005637ebdb38c5 in ?? ()
#3  0x00005637ebda9bac in ?? ()
#4  0x00007f66da301c87 in __libc_start_main (main=0x5637ebda98a0, argc=1, argv=0x7ffc3fb617a8, init=<optimized out>, fini=<optimized out>, rtld_fini=<optimized out>, stack_end=0x7ffc3fb61798) at ../csu/libc-start.c:310
#5  0x00005637ebda9cca in ?? ()

<!---
omaurodiaz/omaurodiaz is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
