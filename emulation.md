# Emulation

Old HW is deying, we need to run the old software on new machines. This means emulation. 

## DoxBox - recommended
The recommended way is using [DosBox](https://www.dosbox.com/). This is a piece of software that opens a window, in which a full DOS runs. You can map a directory on your real OS to be a drive on the emulated DOS machine.

This way you can edit code with modern tools, and use git for version control on the host, and then just compile on the DOS window. I find myself using good old TP7 

I added these lines to the end of  `~/.dosbox/dosbox-0.74-2.conf` 

```
[autoexec]
# Lines in this section will be run at startup.
# You can put your MOUNT lines here.


mount c /home/diego/src/dosdrive
mount d /home/diego/src/darkcloud
PATH=%PATH%;c:\tp7\bin;c:\tp16\bp7\c:\tp16\demo\;c:\ndn\
d:
```

## Full emulation

I would once recommend using [DosEMU](http://www.dosemu.org/)+[FreeDOS](http://freedos.org/), but I see that DosEMU is no longer maintained (see [DosEMU's git](https://sourceforge.net/p/dosemu/code/ci/35054ba7e9f827abff097a5fe5b8d4654b7a84f4/log/?path=) - last commit in 2013). The best alternative is using something like [VirtualBox](https://www.virtualbox.org/) (or [GNome's boxes](https://help.gnome.org/users/gnome-boxes/stable/)).

I think the best documentation on this subject can be found in FreeDOS pages, http://wiki.freedos.org/wiki/index.php/VirtualBox http://wiki.freedos.org/install/

## Real hardware

You are brave. Please  

---

[[Game sources](index.html)] - [[Programming](programming.html)] - [[About](about.html)] - [[Emulation](emulation.html)]
