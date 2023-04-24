## **LAB REPORT ONE**
**Part I: Installing VScode**

In order to install Visual Studio Code (VScode), visit the website [visual studio](https://code.visualstudio.com/) and make sure to obtain the appropriate download according to your operating system.
![Image](vscode1.png)
You should then be able to open Visual Studio on your computer. Happy coding! :D
![Image](vscode2.png)

**Part II: Remotely Connecting**

Open a new terminal in VScode and enter `ssh cs15lsp23zz@ieng6.ucsd.edu` into the terminal, but replace the `zz` portion with your specific cse 15l account (which you can find by visiting [this ucsd website](https://sdacs.ucsd.edu/~icc/index.php)). If asked if you want to keep connecting, enter yes, and make sure to enter your password as well when prompted. 
![Image](1.png)
I was able to login using the `cs15lsp23zz@ieng6.ucsd.edu` account given by the TA, since my own account (`cs15lsp23mi@ieng6.ucsd.edu`) gives the following error.
![Image](2.png)

**Part III: Trying Some Commands**

Ater remotely connecting, you should be able to practice using some commands, try the following commands in the terminal: 
1. `cd ~`
2. `cd`
3. `ls -lat`
5. `ls -a`
6. `cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/`
7. `cat /home/linux/ieng6/cs15lsp23/public/hello.txt` 

Also try the commands in different ways: `cd` which allows you to change your current working directory, `ls` which lists information about directories/files in your current working directory, `pwd` which gives you what your current working directory is, `mkdir` which lets you make a directory, `cat` which reads the contents of a file, and `cp` which allows you to copy files. In the following image, some commands are printed such as the `cat /home/linux/ieng6/cs15lsp23/public/hello.txt` which prints the contents of a specific file and `ls lat` lists directories/files in your current working directory, including hidden directories/files, and are listed according to the last time each file/directory has been edited (with the most recently edited being printed last).
![Image](3.png)
