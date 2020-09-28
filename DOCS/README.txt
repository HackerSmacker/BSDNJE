HackerSmacker's BSDNJE
Based on Moshix' linuxNJE, which is based on FunetNJE, which is based on HUJI-NJE.

Compiling:
You need GCC, and a GNU Make. 
gmake

Installing:
Edit /etc/group and add a group for BSDNJE named funetnje.
gmake install1
mkdir /etc/funetnje
mv /etc/funetnje.cf /etc/funetnje
gmake install

As you can see, I need to edit the Makefile.
