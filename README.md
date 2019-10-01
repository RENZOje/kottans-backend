# Stage 0. Self-Study

* Git Basics ![done](https://i.imgur.com/qfeOuJ5.png)
* Unix Shell ![done](https://i.imgur.com/qfeOuJ5.png)
* VCS (hello gitty), GitHub and Collaboration ![done](https://i.imgur.com/qfeOuJ5.png)
* Language-specific Topics: Part I 🔤
* Memory Management ![done](https://i.imgur.com/qfeOuJ5.png)
* TCP, UDP, Network 🔤
* HTTP & HTTPs
* Design Patterns: Intro
* Data Structures 🔤
* File System
* Runtime, Ecosystem and I/O 🔤
* Databases
* Language-specific Topics: Part II 🔤

---

# Git Basics 

![done_first_task](https://github.com/RENZOje/kottans-backend/blob/master/git_and_github/version_cont_git.png)
First task successfully complete. During this assignment, I repeated the basic *Git* commands. That are really powerful and useful. There is no doubt, it will help me in future work.

---

# Unix Shell

| [Quiz_1](https://github.com/RENZOje/kottans-backend/blob/master/unix_shell/quiz_1.png) | [Quiz_2](https://github.com/RENZOje/kottans-backend/blob/master/unix_shell/quiz_2.png) |
| ---      | ---       |
| [Quiz_3](https://github.com/RENZOje/kottans-backend/blob/master/unix_shell/quiz_3.png) | [Quiz_4](https://github.com/RENZOje/kottans-backend/blob/master/unix_shell/quiz_4.png) |

Unix Shell done! At this task I updated my knowledge of Linux basics commands.

---

# Git Collaboration
![done_third_task](https://github.com/RENZOje/kottans-backend/blob/master/github_coloboration/git_coloboration.png)

In my opinion, [GitHub & Collaboration](https://classroom.udacity.com/courses/ud456) perfectly demonstrates how to work with remote repositories and describe more powerful commands.
I'm sure, this knowledge indispensable, when u work with huge team at real project.

---

# Memory Management

> What's going to happen if program reaches maximum limit of stack ?

*  **Stack overflow** will be if program reaches maximum limit of stack. 

> What's going to happen if program requests a big (more then 128KB) memory allocation on heap ?

 *  When program requests a big block of memory allocation **will create not on heap, but in the memory mapping segment.**


> What's the difference between Text and Data memory segments ?

*  **Text segment of memory** is where a portion of an object file or the corresponding section of the program's virtual address space  is stored and is generally read-only and fixed size.

*  In **Data segment of memory** shows the typical layout of a simple computer's program memory with the text, various data, and stack and heap sections.The  segment contains any global or static variables which have a pre-defined value and can be modified. 

Output of `proc`/`vmmap` command:

```md
5634f0bdf000-5634f0be3000 r-xp 00000000 08:01 3017652                    /usr/lib/gnome-settings-daemon/gsd-mouse
5634f0de3000-5634f0de4000 r--p 00004000 08:01 3017652                    /usr/lib/gnome-settings-daemon/gsd-mouse
5634f0de4000-5634f0de5000 rw-p 00005000 08:01 3017652                    /usr/lib/gnome-settings-daemon/gsd-mouse
5634f1b2c000-5634f1bb2000 rw-p 00000000 00:00 0                          [heap]
7fb486e26000-7fb486e32000 r-xp 00000000 08:01 262725                     /usr/lib/x86_64-linux-gnu/gio/modules/libdconfsettings.so
7fb486e32000-7fb487031000 ---p 0000c000 08:01 262725                     /usr/lib/x86_64-linux-gnu/gio/modules/libdconfsettings.so
7fb487031000-7fb487032000 r--p 0000b000 08:01 262725                     /usr/lib/x86_64-linux-gnu/gio/modules/libdconfsettings.so
7fb487032000-7fb487033000 rw-p 0000c000 08:01 262725                     /usr/lib/x86_64-linux-gnu/gio/modules/libdconfsettings.so
7fb487033000-7fb48704d000 r-xp 00000000 08:01 262729                     /usr/lib/x86_64-linux-gnu/gio/modules/libgioremote-volume-monitor.so
7fb48704d000-7fb48724c000 ---p 0001a000 08:01 262729                     /usr/lib/x86_64-linux-gnu/gio/modules/libgioremote-volume-monitor.so
7fb48724c000-7fb48724f000 r--p 00019000 08:01 262729                     /usr/lib/x86_64-linux-gnu/gio/modules/libgioremote-volume-monitor.so
7fb48724f000-7fb487250000 rw-p 0001c000 08:01 262729                     /usr/lib/x86_64-linux-gnu/gio/modules/libgioremote-volume-monitor.so
7fb487250000-7fb487286000 r-xp 00000000 08:01 133954                     /usr/lib/x86_64-linux-gnu/gvfs/libgvfscommon.so
7fb487286000-7fb487486000 ---p 00036000 08:01 133954                     /usr/lib/x86_64-linux-gnu/gvfs/libgvfscommon.so
7fb487486000-7fb48748c000 r--p 00036000 08:01 133954                     /usr/lib/x86_64-linux-gnu/gvfs/libgvfscommon.so
7fb48748c000-7fb48748d000 rw-p 0003c000 08:01 133954                     /usr/lib/x86_64-linux-gnu/gvfs/libgvfscommon.so
7fb48748d000-7fb4874be000 r-xp 00000000 08:01 262730                     /usr/lib/x86_64-linux-gnu/gio/modules/libgvfsdbus.so
7fb4876be000-7fb4876c0000 r--p 00031000 08:01 262730                     /usr/lib/x86_64-linux-gnu/gio/modules/libgvfsdbus.so
7fb4876c0000-7fb4876c1000 rw-p 00033000 08:01 262730                     /usr/lib/x86_64-linux-gnu/gio/modules/libgvfsdbus.so
7fb4876c1000-7fb48785e000 r-xp 00000000 08:01 2758170                    /lib/x86_64-linux-gnu/libm-2.27.so
7fb48785e000-7fb487a5d000 ---p 0019d000 08:01 2758170                    /lib/x86_64-linux-gnu/libm-2.27.so
7fb487a5d000-7fb487a5e000 r--p 0019c000 08:01 2758170                    /lib/x86_64-linux-gnu/libm-2.27.so
7fb487a5e000-7fb487a5f000 rw-p 0019d000 08:01 2758170                    /lib/x86_64-linux-gnu/libm-2.27.so
7fb487a5f000-7fb487a76000 r-xp 00000000 08:01 2758144                    /lib/x86_64-linux-gnu/libgcc_s.so.1
7fb487a76000-7fb487c75000 ---p 00017000 08:01 2758144                    /lib/x86_64-linux-gnu/libgcc_s.so.1
7fb487c75000-7fb487c76000 r--p 00016000 08:01 2758144                    /lib/x86_64-linux-gnu/libgcc_s.so.1
7fb487c76000-7fb487c77000 rw-p 00017000 08:01 2758144                    /lib/x86_64-linux-gnu/libgcc_s.so.1
7fb487c77000-7fb487df0000 r-xp 00000000 08:01 3021320                    /usr/lib/x86_64-linux-gnu/libstdc++.so.6.0.25
7fb487df0000-7fb487ff0000 ---p 00179000 08:01 3021320                    /usr/lib/x86_64-linux-gnu/libstdc++.so.6.0.25
7fb487ff0000-7fb487ffa000 r--p 00179000 08:01 3021320                    /usr/lib/x86_64-linux-gnu/libstdc++.so.6.0.25
7fb487ffa000-7fb487ffc000 rw-p 00183000 08:01 3021320                    /usr/lib/x86_64-linux-gnu/libstdc++.so.6.0.25
7fb48facf000-7fb48fad0000 r--p 00002000 08:01 3020739                    /usr/lib/x86_64-linux-gnu/libgmodule-2.0.so.0.5600.4
7fb48fad0000-7fb48fad1000 rw-p 00003000 08:01 3020739                    /usr/lib/x86_64-linux-gnu/libgmodule-2.0.so.0.5600.4
7fb48fad1000-7fb48fade000 r-xp 00000000 08:01 3021423                    /usr/lib/x86_64-linux-gnu/libwayland-client.so.0.3.0
7fb48fade000-7fb48fcdd000 ---p 0000d000 08:01 3021423                    /usr/lib/x86_64-linux-gnu/libwayland-client.so.0.3.0
7fb48fcdd000-7fb48fcdf000 r--p 0000c000 08:01 3021423                    /usr/lib/x86_64-linux-gnu/libwayland-client.so.0.3.0
7fb48fcdf000-7fb48fce0000 rw-p 0000e000 08:01 3021423                    /usr/lib/x86_64-linux-gnu/libwayland-client.so.0.3.0
7fb48fce0000-7fb48fec7000 r-xp 00000000 08:01 2758107                    /lib/x86_64-linux-gnu/libc-2.27.so
7fb48fec7000-7fb4900c7000 ---p 001e7000 08:01 2758107                    /lib/x86_64-linux-gnu/libc-2.27.so
7fb4900c7000-7fb4900cb000 r--p 001e7000 08:01 2758107                    /lib/x86_64-linux-gnu/libc-2.27.so
7fb4900cb000-7fb4900cd000 rw-p 001eb000 08:01 2758107                    /lib/x86_64-linux-gnu/libc-2.27.so
7fb4900cd000-7fb4900d1000 rw-p 00000000 00:00 0 
7fb4900d1000-7fb4901e5000 r-xp 00000000 08:01 3020735                    /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0.5600.4
7fb4901e5000-7fb4903e5000 ---p 00114000 08:01 3020735                    /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0.5600.4
7fb4903e5000-7fb4903e6000 r--p 00114000 08:01 3020735                    /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0.5600.4
7fb4903e6000-7fb4903e7000 rw-p 00115000 08:01 3020735                    /usr/lib/x86_64-linux-gnu/libglib-2.0.so.0.5600.4
7fb49063a000-7fb49063b000 r--p 00052000 08:01 3020763                    /usr/lib/x86_64-linux-gnu/libgobject-2.0.so.0.5600.4
7fb49063b000-7fb49063c000 rw-p 00053000 08:01 3020763                    /usr/lib/x86_64-linux-gnu/libgobject-2.0.so.0.5600.4
7fb49063c000-7fb4907d1000 r-xp 00000000 08:01 3020729                    /usr/lib/x86_64-linux-gnu/libgio-2.0.so.0.5600.4
7fb4907d1000-7fb4909d1000 ---p 00195000 08:01 3020729                    /usr/lib/x86_64-linux-gnu/libgio-2.0.so.0.5600.4
7fb4909d1000-7fb4909d8000 r--p 00195000 08:01 3020729                    /usr/lib/x86_64-linux-gnu/libgio-2.0.so.0.5600.4
7fb4909d8000-7fb4909d9000 rw-p 0019c000 08:01 3020729                    /usr/lib/x86_64-linux-gnu/libgio-2.0.so.0.5600.4
7fb4909d9000-7fb4909db000 rw-p 00000000 00:00 0 
7fb4909db000-7fb4909ef000 r-xp 00000000 08:01 3017667                    /usr/lib/gnome-settings-daemon-3.0/libgsd.so
7fb4909ef000-7fb490bee000 ---p 00014000 08:01 3017667                    /usr/lib/gnome-settings-daemon-3.0/libgsd.so
7fb490bee000-7fb490bf0000 r--p 00013000 08:01 3017667                    /usr/lib/gnome-settings-daemon-3.0/libgsd.so
7fb490bf0000-7fb490bf1000 rw-p 00015000 08:01 3017667                    /usr/lib/gnome-settings-daemon-3.0/libgsd.so
7fb490bf1000-7fb490c18000 r-xp 00000000 08:01 2758079                    /lib/x86_64-linux-gnu/ld-2.27.so
7fb490dcd000-7fb490dfa000 r--p 00000000 08:01 786463                     /usr/share/glib-2.0/schemas/gschemas.compiled
7fb490dfa000-7fb490e02000 rw-p 00000000 00:00 0 
7fb490e14000-7fb490e15000 r--p 00000000 08:01 2359335                    /home/renzo/.config/dconf/user (deleted)
7fb490e15000-7fb490e16000 r--s 00000000 00:32 27                         /run/user/1000/dconf/user (deleted)
7fb490e16000-7fb490e18000 rw-p 00000000 00:00 0 
7fb490e18000-7fb490e19000 r--p 00027000 08:01 2758079                    /lib/x86_64-linux-gnu/ld-2.27.so
7fb490e19000-7fb490e1a000 rw-p 00028000 08:01 2758079                    /lib/x86_64-linux-gnu/ld-2.27.so
7fb490e1a000-7fb490e1b000 rw-p 00000000 00:00 0 
7ffd990da000-7ffd990fb000 rw-p 00000000 00:00 0                          [stack]
7ffd9919e000-7ffd991a1000 r--p 00000000 00:00 0                          [vvar]
7ffd991a1000-7ffd991a2000 r-xp 00000000 00:00 0                          [vdso]
ffffffffff600000-ffffffffff601000 r-xp 00000000 00:00 0                  [vsyscall]
```

`Heap - 5634f1b2c000-5634f1bb2000`, `Stack - 7ffd990da000-7ffd990fb000`, `MMS - 7fb486e26000-7fb486e32000`.


**What was new?**

* Whole the time I thought, that don’t have to worry about allocating or deallocating memory in our Python programs. It’s taken care of automatically by the language and the runtime.

* However, in practice, programs eventually do run out of memory due to held references. 

* Memory leak occurs when we create a memory in heap and forget to delete it. They are particularly serious issues for programs like daemons and servers which by definition never terminate. 
