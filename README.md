# LinuxCommandLine-MiniPrograms
I try to write codes in bash script to help developers

I have begun learning software development with Java. But I don't like IDEs much, however it is also unpractical to compile each of the java classes with javac. Another problem with javac is, it creates the executable (.class) files in the same directory. If you have to send the source codes, it is also unuseful to use javac, because you must search in the mixed diretory, which of those files are .java and which of them are .class.  For that reason I developped two commands instead of javac and java.

Theese commands are compile / exej: 

-compile: Similar to javac, it compiles all java classes in the directory and creates a folder, in which the .class files are stored. Extra option: It gets compile -o or compile --only, with that command you can compile java files one by one, but all .class files are stored in the new folder.

-exej: Same as java, it executes the .class files in the class folder. exej gets one parameter and it is the file, which must be executed

For setting up theese commands on Linux/Ubuntu you need to write theese commands on terminal:
chmod +x compile
chmod +x exej
cd /bin
sudo ln -s [directory_of_the_files]*/compile
sudo ln -s [directory_of_the_files]*/exej

*The directory, in which compile and exej source codes are stored
