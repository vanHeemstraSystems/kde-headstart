kde-headstart
# KDE - Headstart

Based on "KDE" at https://kde.org/

Based on "Getting KDE Software" at https://kde.org/download/

Based on "How to Install and Configure KDE on CentOS 7" at https://linuxhint.com/install_kde_centos7/

## 100 - Getting KDE Software

Linux

KDE is already available on majority of Linux distributions. 

It can be installed directly from 

- [Discover](appstream://.desktop), 

- [GNOME Software](appstream://.desktop) 

- or your distribution’s [software store](appstream://.desktop).

In the CentOS 7 installer, when you choose Server with GUI, GNOME desktop environment is installed by default. 

But you can also install KDE desktop environment on CentOS 7 as well. 

On CentOS 7, KDE 4 desktop environment is available in the official package repository of CentOS 7. 

KDE 4 desktop environment is beautiful and very customizable in every aspect.

In this article, I will show you how to install KDE desktop environment on CentOS 7. Let’s get started.

## 200 - Installing KDE on CentOS 7

I have a minimal CentOS 7 server virtual machine set up. It does not have any graphical desktop environment installed yet. I am going to install KDE desktop environment there.

KDE Desktop environment is available in the official package repository of CentOS 7. It is really easy to install as well.

First update the YUM package repository cache with the following command:

```$ sudo yum makecache```

Now you can install KDE desktop environment with the following command:

```$ sudo yum groups install "KDE Plasma Workspaces"```

Thousands of packages will be installed and about 984 MB of packages will be downloaded from the internet. Press y and then press <Enter> to continue.
  
The packages should start downloading. It should take a while.

Once the installation is complete, you should see the following.

```
Complete!
```

Now you have to tell CentOS 7 that you want to start graphical desktop environment when you start your computer by default. To do that, run the following command:

```
$ sudo systemctl set-default graphical.target
```

A graphical desktop environment should be loaded the next time you start your CentOS 7 machine.

Now restart your computer with the following command:

```
$ sudo reboot
```

When your computer boots, you may see the window, which is a license agreement window. Click on the section "LICENSE INFORMATION".

Now from the new window check I accept the license agreement checkbox and click on Done.

Now click on FINISH CONFIGURATION.

Now you should see the GDM login screen. Click on your user account to select it.

Now type in your login password and click on Sign In.

You should see the KDE splash screen as shown in the screenshot below.

After a while, KDE desktop environment should load

## 300 - Configuring KDE Desktop Environment on CentOS 7

See https://linuxhint.com/install_kde_centos7/

more ...









