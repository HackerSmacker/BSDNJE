HackerSmacker's BSDNJE
BITNET emulation for modern BSD systems

Compiling and installing:
1. Add a group called "funetnje"
2. gmake (Don't do a recursive make, it'll fail)
3. gmake install1
4. gmake install
5. Edit /etc/funetnje/funetnje.cf
6. /usr/local/funetnje/funetnje

Configuring:
Edit /etc/funetnje/funetnje.cf with the text editor of your choice.
The options that stick out (the ones that you really need to change) are:
- your NAME
- your IP address (do not enter 0.0.0.0)
- your INFORM parameter (OPERATOR@VM370 is a good one if you're running 6Pext all the time)
- your DEFAULT-ROUTE
- your lines:
  - line name
  - line TCPNAME (or as normal people call it, IP address)
  - line IPPORT (also called the port number, 175 is the default)
Now, do a "pkill -HUP funetnje" to make it reload your config file.


Other cool stuff:
There's a file named "funetnje.rc" that you can copy to /etc/rc.d and rename to funetnje to make NJE start on boot.


There! That's all. For bug reports, please message HackerSmacker#8496 on Discord.

