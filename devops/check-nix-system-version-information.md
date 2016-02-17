#Check *nix system version information

When logging into a new OS I am always curious about the OS version. But what kind of command can be used to check it.

If I want to know the kernal version:

```bash
$ uname -a
```

For the distribution information there are several ways to use because of different distribution of Linux:

```bash
$ lsb_release -a

$ cat /etc/lsb_release

$ cat /etc/issue.net
```
Some or all the commands above can provide you the info.

[source](http://unix.stackexchange.com/questions/88644/how-to-check-os-and-version-using-a-linux-command)