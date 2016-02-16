# How to copy files between servers

Scp stands for secure cp. It uses ssh to transfer data.

```bash
scp user@myhost.com:/home/to/directory/file.txt auser@myhost2.com:/home/to/directory/afile.txt
```
Nice command to master when dealing with multiple servers.

[source](http://www.computerhope.com/unix/scp.htm)