---
layout: page
title: BeOS or NeXT. The Right Choice
---

### Multitasking

Multitasking is the ability to run more than one program at the exact same time. While this is impossible on a single processor system, it is possible on a multiprocessor system. On a single processor system, the CPU must quickly switch between programs to give the illusion that it is running more than one program at the same time.

This leads us to the two major types of multitasking: cooperative and preemptive. Mac OS 8 and Windows 3.1/95/98/Me use cooperative multitasking (Windows 3.1/95/98/Me use preemptive multiprocessing to switch between DOS sessions, but we will ignore that for now). Mac OS X and Windows NT/2000 use preemptive multitasking. Preemptive multitasking is better in most circumstances, but let's look at both.

### Cooperative Multitasking

Imagine that your computer is a kitchen. Instead of programs, you have three appliances: a blender, a clock, and a lamp. You are the CPU, and you have a single power cord that you have to switch between all of the appliances. Now this is part is tricky, each of the appliances has a "locking" power plug. In other words, when you plug the power into the appliance, the appliance "holds" onto the cord until it releases the cord, then you can move the cord to another appliance.

Everything is working well in your kitchen, and all three appliances are working in perfect harmony. Then you decide to add a stereo. You add the stereo, and there are problems. The clock starts showing the wrong time, and the lamp is flickering. Remember when I wrote about each appliance "'holding" on the cord until it lets go? Well, that is the problem with cooperative multitasking. The CPU can not move to the next process until the current process releases control. While this is nice for an application that sometimes needs a little extra CPU time, a poorly written application can hog the CPU and basically starve all of the other applications.

### Preemptive Multitasking

Preemptive multitasking works a bit differently. Imagine instead of plugging the power cord directly into the appliance, each appliance has an extension cord attached that runs to you. So instead of plugging directly into each appliance, you plug into the appliance's extension cord. So now you don't need to wait until the appliance releases the cord, you can switch cords whenever you like. That is preemptive multitasking. The CPU switches between the applications when it wants and each application thinks that it has full control of the CPU. With preemptive multitasking no one application can hog the entire system.

### Multithreading

If multitasking is running multiple applications at the same time, multithreading is running multiple parts of an application at the same time. An example would be a word processor. Remember when you had to type the document and then run the spellchecker? And remember how you had to wait for it to send your document to the printer? With multithreading, the spellchecker can run at the same time as you type. That way you see all of those little red lines immediately. And you can start typing immediately after you tell the file to print. When you tell the program to print the file, it spawns the process (creates a new process and executes it), and the CPU can send that process to the background so you can keep typing.

### Journaling File System

A journaling file system is always a good thing. However, a journaling file system will not prevent file system corruption, nor does it add any extra security. A journaling system will corrupt as easily as any other file system if a power outage occurs in the midst of a disk write. The benefit is on the restart.

A journaling file system keeps a log of all the file system writes. On a non-journaling file system, a disk repair program must check the entire file system for errors. On today's large hard drives this can take some time.

On a journaling file system, the disk repair program, which must still be executed, can read the journal entries of all of the open files. This way, the entire disk need not be scanned, only the previously open files.

Disk fragmentation will always occur. Here is a visual example of fragmentation. For simplicity sake, each file is represented by a number and each character equals one meg.

You have a clean disk and you save a 10 meg file. Your disk looks like this.
```
    1111111111
```
You then save a 5 meg file.
```
    111111111122222
```
You then save a 3 meg file.
```
    111111111122222333
```
You then add 2 megs to the '2' file.
```
    11111111112222233322
```
You add 1 meg to the '1' file.
```
    111111111122222333221
```
You delete the '2' file. See the 'open' spaces between the files?
```
    1111111111     333  1
```
You save a 4 meg file.
```
    11111111114444 333  1
```
You save a 6 meg file.
```
    111111111144445333551555
```
You add 2 more megs to the '1' file.
```
    1111111111444453335155511
```
As you can see, the file system has become fragmented. Fragmented just means that all of the files are not contiguous. You notice how the '5' file is located in three different parts of the disk. Rather than the hard drive reading the file at one time, it has to read parts of it from three different areas. This takes time. And when a file is scattered in thousands of places across a hard drive, you can understand how this can really slow down a system. BTW, if we ran a disk defragmenter on the above hard drive the result might look like this.
```
    11111111111114444333555555
```

### BeOS

I can speak well of Be. I was one that looked anxiously for the Be beta that was distributed with Mac Tech magazine. I was an original beta1 and beta2 tester. I bought the first release when it was available on the Intel platform. I was amazed at the spinning teapot demo. And that was the problem.

That is all the OS could do. It could spin a teapot and play several movies without dropping frames. A nice technological demo, but hardly a career choice. In other words, there were (and are) no apps for the wonderful little OS. Sure, Be designed it on a clean sheet of paper -- the same paper they could use to list every application ever written for Be and still have room to doodle.

*There is an old joke that goes like this. How was God able to create the world in 6 days? No backwards compatibility needed.*

When Apple decided to go with NeXT over Be, Be couldn't even print. Be, while blazingly fast, was blazing fast for a reason. Nothing was running on it. Apple chose to go with the OS that was stable, proven, and gorgeous. Apple also got NeXT's unbelievably fast development environment, the leading application server software WebObjects, and the Mac's father and Apple's savior, Steve Jobs. (Personal note: I still remember leaving work late for Christmas vacation ecstatic after reading that Steve Jobs was back at Apple.)

Speaking of NeXT's fast development environment, Steve Jobs used to demo it in a unique way. When Steve was giving a demo or seminar of NeXT, he would have a programmer onstage with him. The programmer would start writing an application at the start of the seminar. Steve would close the seminar by demonstrating the app that had just been written!

As for Apple choosing NeXT or Be, I think the choice was quite clear. So the next time you think that Mac OS X or OS 9 is holding your system back, you should thank Apple. Thank Apple that there are device drivers for hardware, extensions, and thousands of applications that "slow down" that wonderful computer with its gorgeous and elegant GUI.
