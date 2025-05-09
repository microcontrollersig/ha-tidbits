
# Free Disk Space

The possible sources of large disk space usage:

* Backups
* Home Assistant Database
* Addons data cache
* Media or share (if not network attached storage)

If you are on Home Assistant OS and have access to a shell(eg. using the Terminal&SSH Addon), make sure to run 

```sh
login
```
To get full access.

Then run

```sh
du -h -d 1 / | sort -h
```

You can play with variations of this, for example

```sh
du -h -d 1 /
du -ah -d4 / |sort -hr|head -n 20
```


<br><br>

*Problem encountered by Rob B. This writeup is based on his contribution.*