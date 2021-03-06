# linux-sql
### A few sample files to introduce SQL Like Concepts

The file systems on Mac, PC, and Linux operating systems are essentially database systems. In this short demo I will ```gitclone``` the files in this repository into my opal account and use the ``ls`` command with some wildcards. You will need to use wildcards in SQL, so the purpose of this demo is to show how the same query concepts can work across multiple operation systems and applications.

```
Mac > 
terminal > 
ssh onyen@opal.ils.unc.edu 
password > enter it
cd into public_html > 
git clone https://github.com/ljonesdesign/linux-sql
cd linux (hit tab to complete)

PC > 
Secure shell client >
onyen@opal.ils.unc.edu 
password > enter it
cd into public_html > 
cd git clone https://github.com/ljonesdesign/linux-sql (hit tab to complete)
```

here are some commands to try:

## Find files with Martha in the name:
```
ls -l *martha*
```
this will list all files that contain the string LIKE martha:

```
[lblakej@opal linux-access]$ ls -l *martha*
-rw-rw-r-- 1 lblakej lblakej 9 Apr 10 09:04 martha.jpg
-rw-rw-r-- 1 lblakej lblakej 9 Apr 10 09:04 martha.txt
```

## Find files that have a capital M:
```
ls -l *M*
```
Remember that Linux is case sensitive. Capital M will only yield the readme file which contains a capital M:
```
[lblakej@opal linux-access]$ ls -l *M*
-rw-rw-r-- 1 lblakej lblakej 463 Apr 10 09:04 README.md
```

## Sort all files by file extension (e-**X**-tension)

```
ls -lX
```

Sorted by extension ascending (ASC):
```
-rw-rw-r-- 1 lblakej lblakej   9 Apr 10 09:04 kathy.jpg
-rw-rw-r-- 1 lblakej lblakej   9 Apr 10 09:04 kelly.jpg
-rw-rw-r-- 1 lblakej lblakej   9 Apr 10 09:04 martha.jpg
-rw-rw-r-- 1 lblakej lblakej 463 Apr 10 09:04 README.md
-rw-rw-r-- 1 lblakej lblakej   9 Apr 10 09:04 jackie.txt
-rw-rw-r-- 1 lblakej lblakej   9 Apr 10 09:04 jake.txt
-rw-rw-r-- 1 lblakej lblakej   9 Apr 10 09:04 janice.txt
-rw-rw-r-- 1 lblakej lblakej   9 Apr 10 09:04 karen.txt
-rw-rw-r-- 1 lblakej lblakej   9 Apr 10 09:04 kathy.txt
-rw-rw-r-- 1 lblakej lblakej   9 Apr 10 09:04 kelly.txt
-rw-rw-r-- 1 lblakej lblakej   9 Apr 10 09:04 martha.txt
-rw-rw-r-- 1 lblakej lblakej   9 Apr 10 09:04 sam.txt
-rw-rw-r-- 1 lblakej lblakej   9 Apr 10 09:04 william.txt
```
## Find all files that start with ma OR ka and sort them by file extension.

```
[lblakej@opal linux-access]$ ls -lX {ma*,ka*}
```
result:

```
-rw-rw-r-- 1 lblakej lblakej 9 Apr 10 09:04 kathy.jpg
-rw-rw-r-- 1 lblakej lblakej 9 Apr 10 09:04 martha.jpg
-rw-rw-r-- 1 lblakej lblakej 9 Apr 10 09:04 karen.txt
-rw-rw-r-- 1 lblakej lblakej 9 Apr 10 09:04 kathy.txt
-rw-rw-r-- 1 lblakej lblakej 9 Apr 10 09:04 martha.txt
```
