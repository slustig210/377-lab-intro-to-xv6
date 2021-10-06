# 377-lab-intro-to-xv6

## Purpose

This lab is designed to introduce you to the xv6 operating system.

From the xv6 README file:
"xv6 is a re-implementation of Dennis Ritchie's and Ken Thompson's Unix
Version 6 (v6).  xv6 loosely follows the structure and style of v6,
but is implemented for a modern x86-based multiprocessor using ANSI C."

Please make sure that all of your answers to questions in these labs come from work done on the Edlab environment – otherwise, they may be inconsistent results and will not receive points.

Please submit your answers to this lab on Gradescope in the assignment marked "Lab #x". All answers are due by the time specified on Gradescope. The TA present in your lab will do a brief explanation of the various parts of this lab, but you are expected to answer all questions by yourself. Please raise your hand if you have any questions during the lab section – TAs will be notified you are asking a question. Questions and Parts have a number of points marked next to them to signify their weight in this lab’s final grade. Labs are weighted equally, regardless of their total points.

Once you have logged in to Edlab, you can clone xv6 using
```bash
git clone https://github.com/mit-pdos/xv6-public.git
```
Then you can use `cd` to open the directory you just cloned:
```bash
cd xv6-public
```

## Part 1: Running xv6

To run xv6 on qemu (an emulator) with GDB, use the command:
```bash
make qemu-nox-gdb
```
Then, in a second terminal, navigate to the `xv6-public` folder and run gdb with the `.gdbinit` that was created by `make`:
```bash
gdb -x .gdbinit
```
If you type `c` or `continue` into gdb and hit enter, you should see xv6 running in the other terminal.

To run without GDB, simply run `make qemu-nox` in the `xv6-public` directory.

Now, you can run shell commands, such as `ls`, from `sh` in the terminal running xv6. Try some commands!

## Part 2: Exploring xv6

In the `xv6-public` directory on Edlab, explore some of the files. What are some common included files? What are in these common files?
