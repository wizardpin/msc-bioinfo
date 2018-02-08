# How to SSH from your own computer to Birkbeck Crystallography 

## A quick intro to `ssh`

`SSH` is -as its name implies- a secure shell. It creates a strongly encrypted connection between a local (your device) and a remote server (a machine you can't usually physically access.)

In our case, we need to access the server of Birkbeck Biology Department (a.k.a. hope) using our own device (a laptop, desktop, et.c.)

insert LOCAL - REMOTE diagram

## Ever quickest intro to CLI

Command Line Interface (or CLI), is an the most ancient interface of all. The mighty command line or terminal, stemming from the physical terminals of the 70's (e.g. insert ANYTHING here somtimes without even a display).


![an old terminal](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2c/IBM2741.JPG/1280px-IBM2741.JPG)


Luckilly enough today most laptops ship with a display :D CLI can be used to access the filesystem, installed programs in the remote machine (like editors or databases e.tc.) or even connected peripherals (like a printer).

![a screen terminal](https://upload.wikimedia.org/wikipedia/commons/8/87/Televideo925Terminal.jpg)

The most used and useful commands for CLI are:
- `whoami` (sounds philosophical but it's helpful)
- `pwd` (Print Working Directory)
- `ls` (LiSt the contents of the current directory)
- `cd foo` (Change Directory, foo can be anything)
- `mkdir foo` (MaKe a new DIRectory with the name foo)
- `nano foo.py` (a command line text editor)`


##Linux and Mac OsX
You are quite lucky here as there is no need to install anything external. A terminal emulator is included, as those systems are are based on Unix/BSD Unix.

To access the remote server do the following:
- Open a new terminal window (on mac just hit Apple+Spacebar and type terminal, if you 're in Linux I assume you know already how to ;) )

- Create a secure connection between your machine and the Birkbeck Crystallography server (let's call it the 'remote machine/server'):

```
ssh user@ssh.cryst.bbk.ac.uk
```

where `user` is your provided username by the department. Same goes for the password that you are going to be asked.

Now you are connected to the Command Line Interface (CLI) of the server. Keep in mind that nothing of what you write, save or execute is happens in your computer but rather in the remote server. 

If you need to edit a file using your favourite text editor (Atom is a good one for beginners), then you need to save your file locally and transfer using the `scp` command (that is secure copy)

##Windows


One of the best options is to download and install [SmarTTY](http://smartty.sysprogs.com/), then follow the instructions above.

![ssh](https://imgs.xkcd.com/comics/im_an_idiot.png)

## Contribute

If you notice any mistakes in content or formatting, please send a pull request with your correction.

##Copyright
This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>