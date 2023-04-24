# Lab Report 1
* Download visual studio code at  https://code.visualstudio.com/

* Open a window in VScode like this:  

  ![Image](vscode.png)

* Open your terminal inside VScode using the Terminal → New Terminal menu option

* Type the following command to the terminal:
    ```
    ssh cs15lsp23fq@ieng6.ucsd.edu
    ```

* Enter your password and if the connection is successful, the terminal should look like this:

  ![Image](new.png)

* Try some commands on the remote computer using the terminal in the vscode 
  * cd ~
    * changes the current directory to the home directory of the current user. 
  * cd
    * changes the current directory to the home directory of the current user (same as cd ~)
  * ls -lat
    * lists all files in the current directory, including hidden files (-a), sorted by modification time in reverse order (-t) and with details showing permissions and ownership (-l)
  * ls -a
    * lists all files in the current directory, including hidden files (-a)  
  * ls <directory> where <directory> is /home/linux/ieng6/cs15lsp23/cs15lsp23abc, where the abc is one of the other group members’ username
    * lists all files in the specified directory, where <directory> is the full path to the directory. In this case, the directory is /home/linux/ieng6/cs15lsp23/cs15lsp23abc, which is the home directory of another group member
  * cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/
    * copies the file hello.txt from the directory /home/linux/ieng6/cs15lsp23/public/ to the home directory of the current user (~)
  * cat /home/linux/ieng6/cs15lsp23/public/hello.txt
    * displays the contents of the file hello.txt on the terminal

  ![Image](command.png)
  
* Try the same commands on your own computer 
  
  ![Image](own.png)
  ![Image](own2.png)
  
* If you want to log out of the remote server in your terminal, use either
  * Ctrl-D
  * Run the command exit
