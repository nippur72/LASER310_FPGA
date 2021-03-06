Laser310 System B readme  

System B is a utility published on Aug 16 of 1987 issue of "Software" journal. Authors are Luo, Shouzhang and Luo, Ya.
When loading a binary file from cassette on Laser 310, the ROM binary program loader will automatically make a call to the entry point and start running it.
With this utility you can load a binary file from cassette and floppy, make a copy of this file to casette.  

The System B itself is only 190 bytes, designed to be loaded to the high end of display RAM.
Commands:  
R ["filename"] - Load binary file from cassette  
L "filename" - Load binary file from floppy  
W ["filename"] - Write file to cassette as binary file  
V ["filename"] - Verify binary file on cassette  
E - Exit from system  

Notes:  
* System B is compatible with Laser 310 Monitor and DOS Basic 1.2 or any file lives from 7AE9 to B7FF and 7200 to 76FF.
* L command is NOP on diskless system.
* W command will create an identical copy of loadded B file, runs well without System B.
* R/L command, it stores the start address and end address in 77BB and 77BE. They remain unchanged after you exit from System B.
* System B is loadded in high-end of VRAM, MODE(1) command will clean this area.
