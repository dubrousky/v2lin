# v2lin
Fork of the http://sourceforge.net/projects/v2lin/ project. The original project page is http://v2lin.sourceforge.net/

```
v2lin is a fork of outdated legacy2linux/v2linux project. v2lin supports recent POSIX-compliant glibc. If you port your application from VxWorks to GNU/Linux, this library will help you a lot. v2lin provides VxWorks compliant API for tasks, semaphores, message queues, etc.

We started porting our VxWorks applications to Linux and found several differences between the two systems which require some kind of adatation layer (middleware) to run our applications on Linux, otherwise we had to redesign our application and change many APIs we already use.

We found that v2linux can solve some of our problems, however we noticed that there were no updates since 2001.

We did some source code research, made several changes and eventually succeed to compile it and run the validate program attached with the library code.

Most of the tests performed well, however some tests failed because of obsolete assumptions concerning Linux behavior made in v2linux. For example thread suspension will not work the way it is implemented in v2linux, since in current pthread library implementation (NPTL) SIGSTOP always sent to a whole process and not to specific thread.

There are several additional issues that has to be covered before v2linux can be used to the fullest extent with current linux/gnu toolchains implementations.

During our v2linux research we studied its code and made some changes. We have an intention to perform additional changes.

We would like to contribute our current and future changes to the v2linux project, since we noticed that there are many projects involved in porting their legacy applications from VxWorks to Linux these days. And they desire an updated version of library like v2linux.

Since there are no plans for updates of original v2linux project in the near future, we created v2lin. We hope that our contribution will be useful.

v2lin team
```
