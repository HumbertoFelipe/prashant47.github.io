# How Operating System works 
The primary objective of this project is to gain a detailed understanding of how computer systems work. For instance, when one types a command at the console, what is the chain of hardware and software events that lead to the command returning the correct value? This deep understanding is of practical and philosophical importance. It is practically immportant to understand how computer systems work when you are trying to make them do something new, either for research or industry. More philosophically, a computer scientist with an advanced degree should not view any part of the computer as "magic," but should either understand how it works or have the tools to figure it out

## What is xv6
xv6 is a simple unix-like teaching operating system developed at MIT [1]. xv6 is re-
implementation of Dennis Ritchies and Ken Thompsons Unix Version 6 (v6). xv6 is
implemented in ANSI C for an x86 based multiprocessors. Xv6 is simple enough to teach
operating system walking through its code in a semester. xv6 has implemented most of
modern operating system core functionalists which makes easier to start look through in
oper- ating system code for a newbie. Xv6 is around 8000 lines code yet still contains the
important concepts and organization of Unix. Current users of xv6 include MIT,Yale
[2],Columbia university, IIT Delhi.



## Reason for Porting of compiler and linkage editor to xv6

### Reason for porting Interpreter in education OS xv6:
During the software development cycle, programmer make frequent changes to source
code. When using a compiler, each time a change is made to the source, they must wait
for the compiler to translate the altered source files and link all of the binary code files to-
gether before the program can be executed. The larger the program , the longer the wait.
By contract a programmer using an interpreter does a lot less waiting, as the interpreter
usually just needs to translate the code being worked on to an intermediate representa-
tion ( or in other words Not translate it at all ), thus requiring much less time before the
changes can be tested since effects are evident upon saving the source and reloading the
program. Interpreting a language given implementations some additional flexibility over
compiled implementations.


### Reason for porting standalone Linkage editor to xv6: 
1. Understanding linkers will help you build large programs.Programmers who build
large programs often encounter linker errors caused by missing modules, missing li-
braries, or incompatible library versions. Unless you understand how a linker resolves
references, what a library is, and how a linker uses a library to resolve references,
these kinds of errors will be baffling and frustrating.
2. Understanding linkers will help you avoid dangerous programming errors The deci-
sions that Unix linkers make when they resolve symbol references can silently affect
the correctness of your programs. Programs that incorrectly define multiple global
variables pass through the linker without any warnings in the default case. The re-
sulting programs can exhibit baffling run-time behavior and are extremely difficult
to debug. We will show you how this happens and how to avoid it.
3. Understanding linking will help you understand how language scoping rules are
implemented.For example, what is the difference between global and local variables
?
4. Understanding linking will help you understand other important systems concepts.
The executable object files produced by linkers play key roles in important sys-
tems functions such as loading and running programs, virtual memory,paging, and
memory mapping.
5. Understanding linking will enable you to exploit shared libraries. For many years,
linking was considered to be fairly straightforward and uninteresting. However,
with the increased importance of shared libraries and dynamic linking in modern
operating systems, linking is a sophisticated process that provides the knowledgeable
programmer with significant power. For example, many software products use shared
libraries to upgrade shrink-wrapped binaries at run time. Also, most Web servers
rely on dynamic linking of shared libraries to serve dynamic content.


## Online Demo
	comming soon..

## References
1] http://pdos.csail.mit.edu/6.828/2014/overview.html
2] http://zoo.cs.yale.edu/classes/cs422/2014/
3] Robert Morris Russ Cox, Frans Kasshoek. xv6 a simple, Unix-like teaching operating
system. MIT, June 2009

##Lincese
MIT Lincese
