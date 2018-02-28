Hello everyone,

to get your system ready there are two ways to proceed. One using a Virtualbox setup, the other installing all needed on your personal machines.

## VirtualBox version
You need to install VirtualBox. Go to https://www.virtualbox.org/ and Download and install the application (for linux users, you can check if your distro has official packages). After you have done that you will want to download and unzip the file https://s3.eu-west-2.amazonaws.com/emacs-workshop/emacs-vdi.zip (2.6 Gb compressed, 6.2 expanded) and the virtualbox file https://s3.eu-west-2.amazonaws.com/emacs-workshop/Emacs-Basic.vbox (both on the same folder). You can then proceed to add it into Virtualbox (On the Menu Machine->Add).

After that, make sure that you can log into the machine (username and password are emacs). You should see the Emacs icon on the left hand launcher.

## Your machine
The following things need to be installed:

Emacs itself. You can find download packages at https://www.gnu.org/software/emacs/download
The init file at https://gist.github.com/MiyamotoAkira/5ed869fbaeb2044e1215741bae04c4e5  Save it as init.el inside a folder called .emacs.d under your home directory (`~/.emacs.d/init.el` for Linux and MacOs systems, and `%userprofile%/.emacs.d/init.el` for Windows)

For part of the workshop we are going to use a small bit of Clojure (don't worry, no need to know anything about Clojure, is just a simple example to show what Emacs can do). So you will need to install Java 8 (for linux users, openjdk-8 is fine), which you can find at http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html . You will need to also install leiningen. Instructions for installation are at https://leiningen.org/

Finally, in which ever folder you prefer, run the command `lein new testemacs` to create a new basic project.
If you start Emacs now, it should get all things needed for the workshop.

