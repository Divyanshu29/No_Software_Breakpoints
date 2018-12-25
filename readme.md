This is the solution for root-me No Software Breakpoint Challenge. A very good challenege for beigneers.
The binary is stripped and as a result in gdb we have to find the starting address of the binary and print instructions from there. 
Be carefull to not print assebmly for dynamic linkers as they will simply confuse you and are not relevent at present.There is 
a function which generates checksum of the binary.
Thoery of Checksum:
  Whenever we insert a breakpoint we add 0xcc at that line and if we do in here we disrupt the checksum and hence even if we give correct password we wont be able to get the flag.
