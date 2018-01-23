---
layout: post
title: gdb Code Signing on MacOSX
category: Code
---

My computer has been running slow recently from the random junk I installed onto my computer from these couple of years. Besides that, my battery started to discharge really fast -- Even the "service battery" warning came up on the battery indicator sign on the top right of the screen.

So I thought since I have a free weekend coming up, I might as well try and factory reset my entire macbook and see if things get better. It will also be a nice way for me to clean up my computer.

When the weekend came, I wiped the entire computer clean. I reformatted the entire disk to make sure nothing gets saved. I wiped it so clean that when I booted up, there was nothing left of the computer, no Apple logo nor a BIOS, only a question mark showed up. I had to reinstall my OS thru the network recovery mode (by pressing ctrl + command + r at startup).

That went ok, and eventually I got my macbook reset to look like it was just out the box. (Well at least software wise.) Once everything is wiped, I had to start installing all the stuff I need on my computer. This includes stuff like chrome, alfred, vlc, iterm, and sublime. After I got all that I had to install the packages I need in the terminal. Those went easy since there was homebrew. Remember how to setup my vim and its color scheme was a lot of work that I can make another
post on it next time.

But anyways, today I was working on a computer security puzzle called the Buffer Overflow Attack. What it is is also for another post in the future. But anyways, I needed to use gdb to look at the stack. However, when I tried to run gdb, I keep getting an error of the lines of "Unable to find Mach task port for process-id 39655: (os/kern) failure (0x5). (please check gdb is codesigned - see taskgated(8))"

This reminded me of how way back in sophmore year when I took the computer architecture class (CSE30) which was the first time I learned gdb. I remembered installing gdb on MacOS was a hassle.

Apparently, Apple does not allow programs to have that much of an access privilege that is needed for gdb. A program must be "code signed" for Apple to allow it to run.

Therefore, we had to "code sign" our gdb by creating a certificate saying that we should "trust" whatever program is in this certificate.

And here are the steps:
[https://apple.stackexchange.com/questions/309017/unknown-error-2-147-414-007-on-creating-certificate-with-certificate-assist](https://apple.stackexchange.com/questions/309017/unknown-error-2-147-414-007-on-creating-certificate-with-certificate-assist)
