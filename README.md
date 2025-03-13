# pwn.college helper environment for kernel development and exploitation

**NOTE: you don't need to interact with this repo in the course of interacting with pwn.college. The kernel challenges can be solved in the infrastructure; this is just here as a way to reproduce the infrastructure locally.**

Pre-requistite:

Building the kernel, busybox, and demo modules:

```
$ ./build.sh
```

Running the kernel:

```
$ ./launch.sh
```

All modules will be in `/`, ready to be `insmod`ed, and the host's home directory will be mounted as `/home/ctf` in the guest.


require：


gcc make libssl-dev bc bzip2 libncurses5-dev


docker:


ubuntu 22.04



my compile env : 


* ubuntu 22.04, sha256:97271d29cb7956f0908cfb1449610a2cd9cb46b004ac8af25f0255663eb364ba


* gcc 11.4.0


* glibc 2.35


busybox menuconfig:


   exclude: Applets->Shells->job control

 
solve the problem: 


```
 /bin/sh: can't access tty; job control turned off
```
