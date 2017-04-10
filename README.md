# linux-access
A few sample files to introduce Access Queries

The file systems on Mac, PC, and Linux operating systems are essentially database systems. In this short demo I will ```gitclone``` the files in this repository into my opal account and use the ``ls`` command with some wildcards. You will need to use wildcards in Access, so the purpose of this demo is to show how the same query concepts can work across multiple operation systems and applications. 

I am only going to spend a few minutes on this so if you want to follow along with me you need to log into opal via ssh.

If you have this on your 

Mac > 
terminal > 
ssh onyen@opal.ils.unc.edu 
password > enter it
cd into public_html > 
git clone https://github.com/ljonesdesign/linux-access
cd linux (hit tab to complete)


PC > 
Secure shell client >
onyen@opal.ils.unc.edu 
password > enter it
cd into public_html > 
cd git clone https://github.com/ljonesdesign/linux-accessinux (hit tab to complete)

here are some commands to try:
```
ls -l *martha*
```
this will list all files that contain the string LIKE martha:

```
[lblakej@opal linux-access]$ ls -l *martha*
-rw-rw-r-- 1 lblakej lblakej 9 Apr 10 09:04 martha.jpg
-rw-rw-r-- 1 lblakej lblakej 9 Apr 10 09:04 martha.txt
```
