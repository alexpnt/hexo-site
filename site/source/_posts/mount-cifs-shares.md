---
title: Mouting CIFS shares on a Linux/UNIX box  
date: 2017-07-23 16:11:15
tags:
- linux
- cifs
- windows
---

Occasionally, there is the need to access files from a remote host which uses a diferent operating system or is located in a different network. The CIFS (Common Internet File System) is a sharing protocol that lets users share files across different systems. 

On a Linux/UNIX box we can mount our shared folder as follows:

```bash
$ sudo mount -t cifs //remoteserver/shared /mnt/shared/ -o username=myusername,password=mypassword --verbose
```

where:

* _-t cifs_ is the filesystem type (cifs in our case)

* _//remoteserver/shared_ is our remote host ('shared' is the shared folder)

* _/mnt/shared/_ is the local folder that will be mounted

* _-o username=myusername,password=mypassword_  are the authentication credentials

__Disclaimer:__ You might need to install CIFS utilities before attempting to run the above command.