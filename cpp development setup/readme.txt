Copy these files to this similar location relative to your pc

C:\Users\Akash Pandit\AppData\Roaming\Sublime Text 3\Packages\User

»Select the build system by going to Menu»Tools»Build System»Select cpp-run

---------Other Info--------
cpp-run→ build the file and runs it in external cmd

cpp-buil→ just builds the file

Note:
         I have also installed c++11 package using package control so if there are any issue while run or compiling  the file try installing it.

**************************  SFML DEVELOPMENT *********************
1.Change this to the location where you put your SFML folder
»D:/Others/SFML-2.5.1

→sfml-build (system system)
     build and runs the file it also creates an executable file with the name of the file

Note:
        I moved all the files present in SFML_FOLDER(/bin,/include,lib) to their respective folders present in the location where I installed mingw compiler but I have also added the location of these files in sfml folder in the build file so it shouldn't matter

----------------------------------------------------------------
NOT IMPORTANT
Makefile (not important to setup)   ============
         Trials(irrelevent):
               1. I tried make a makefile but it didn't run as I expected it always gave me error 
               2.use mingw32-make to run the make file in command like folder where the makefile is located

https://forum.sublimetext.com/t/compile-with-dynamic-libs-g-and-sfml-linux/21136/2

