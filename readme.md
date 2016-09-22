# SSH TOOL
A neat little tool for managing ssh connections.

## Example
```
  ## Append new ssh connection to config
  > ssh-tool -a andy myserver.com

  ## List configured connections
  > ssh-tool -l
  1: root@website.com
  2: andy@myserver.com

  ## Mount ssh connection
  > ssh-tool -m 2
  > ls /media/$USER/myserver.com
  boot   etc   lib   mnt   proc ...

  ## Connect to ssh connection
  > ssh-tool -c 2
  Welcome to Ubuntu 15.10 (GNU/Linux 4.2.0-27-generic x86_64
  andy@myserver.com:
```

## Synopsis
    ssh-tool [COMMAND]... [OPT1]... [OPT2]...

## Flags
`-h. --help` : Display help

`-l` :  List configured connections.

`-a [USER] [HOST]` : Append new connection

`-m [NUM]` : Mount ssh connection

`-c [NUM]` : Connect to ssh connection

## Usage
Feel free to use, modify and redistribute. Please provide credit where credit is due.
