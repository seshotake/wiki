# Linux Commands

Some useful linux commands

## differences of /etc/profile, ~/.bash_profile, ~/.bashrc

Output of `man bash`:

```
FILES
  /bin/bash
    The bash executable

  /etc/profile
    The systemwide initialization file, executed for login shells

  /etc/bash.bashrc
    The systemwide per-interactive-shell startup file

  /etc/bash.bash.logout
    The systemwide login shell cleanup file, executed when a login shell exists

  ~/.bash_profile
    The personal initialization file, executed for logins shells

  ~/.bashrc
    The individual per-interactive-shell startup file

  ~/.bash_logout
    The individual login shell cleanup file, executed when a login shell exits

  ~/.inputrc
    Individual readline initialization file
```

## check boot/shutdown log

```sh
last reboot      # check boot log
last -x shutdown # check shutdown log
```

## switch to root environment

```sh
sudo -s # ~/.bashrc is respected
sudo -i # ~/.bashrc is ignored
```

## restrast bash

```sh
exec bash
```

## list all commands recognized by linux shell

```sh
compgen -c
```

## check manual of a command

```sh
man ls # manual for `ls` command
```

## find out where command exists

```sh
which ls
```

or

```sh
whereis ls # used to locate binary, source for a command
```

## check system information

```sh
hostnamectl
uname -a
cat /etc/*-release # or use `bat` for highlighting
```

## list all users

```sh
less /etc/passwd # or use `bat` for highlighting
```

## check cpu specification

```sh
lscpu
```

or

```sh
cat /proc/cpuinfo # or use `bat`
```

## get logical core count

```sh
echo $(nrpoc) # 4
```

## list all locale

```sh
locale -a
```

## check current date and time

```sh
date
```

## measure running time of a command

```sh
time <command>
```

## get ipaddress

```sh
hostname -i
```
