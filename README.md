# ALFN---Arch-Linux-For-Noobs

You saw the arch hype and their long ass guides on the websites? 
Great, now you're here. 

## Installation Hacks

`archinstall` for the classic debian style noob installer.

### Important Setup Steps
* Make sure to set the proper keyboard layout (for your password to work)
* Make sure to put the right Timezone (for server handshakes) 
* Right target drive and default format, press yes to defaults, default format. 
* Set a root password (and a user without sudo, even better)
* Go to profile > type > and select a desktop environment (Window managers can be more complex for beginners)
* Recommended desktop environment: 
  * Try Budgie, it looks much more modern and slick than most in 2025

Now press install > wait for it to finish. 

IMPORTANT: 

**When the install is over will prompt you with would you like to chroot... No we are noobs.**

You will get to shell at the end of installation, we are noobs so we don't care `exit`. 

It brings you to another shell, damn.(I think for proper clean-up): `shutdown -h now`

## Starting out. 

Reboot from the drive you installed on. 

Depending on if you set a profile up in the installer you either log in as root or as your profile name.

You can now Cristiano Ronaldo you arch install `sudo pacman -Syyu` to update core or extra packages. 

This also comes with essentials such as file browser, terminal, ressource monitor, and more... 

Make sure to create a user with a different password as root. 
Now you can simply `sudo pacman -S firefox` careful for case sensitive :)

----

## Desktop Env : What hopping 250 times has tought me.

The simplicity of Budgie is what makes it such a strong choice. Yet both system settings and appearence modifications are extensive. 
My favourite is workspaces and keyboard shortcuts. 

Makes me think of KDE with less clutter which is great for this type of more minimal install. 
People always show how great there distro looks but reality is I want it the be efficient and simple. 

### Enough ranting now time for the big boy stuff:

`cd /etc` Here you will find many system configurations. `ls -l` 

Let's modify the most important one our bash tool :)
`nano bash.bashrc` 

Found this really cool script that looks like the parrotOS config files, it says Ubuntu or Debians but since it's bash shoud work for any bash shell:

Thanks to user @Calvince

https://gist.github.com/calvince/b4f1a321369ade869789d99a2604670f

You can simply relaunch the shell and get something like this :)

![Screenshot 2025-02-24 16-22-38](https://github.com/user-attachments/assets/b4aa7396-fc9c-4225-9fe3-578990555ff5)

Now this was just an example but the idea is that you can edit most of the system through this /etc configurations. 

You can also `sudo pacman -S bash-completion` reload your terminal and press tab while typing a command.


