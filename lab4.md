#### 1. Login to ieng6
##### Key Pressed: 
- `ssh cs15lsp23fq@ieng6.ucsd.edu` to login to ieng6 directly. 
![Image](eng.png)

#### 2. Clone your fork of the repository from your Github account
##### Key Pressed: 
- `git clone https://github.com/ucsd-cse15l-s23/lab7.git"` to clone my fork of the repository.
![Image](git.png)

#### 3. Run the tests, demonstrating that they fail
##### Key Pressed: 
- `cd lab7` to change my working directory to lab7.
- `bash test.sh` to run the test. 
![Image](run_fail.png)

#### 4. Edit the code file to fix the failing test
##### Key Pressed: 
- `vim ListExamples.java` to enter vim. 
- I scrolled my mouse down until the cursor reaches the start of the while loop. 
- **j** 17 times so that the cursor reaches the line I need to make edits on. 
- **l** 11 times so that the cursor reaches the character "1" in "index1" exactly. 
- **x** to delete character "1".

![Image](1_vim.png) 

- **i** to enter insertion mode. 

![Image](before_vim.png) 

- **2** so "index1" is changed to "index2".

![Image](after_vim.png) 

- **<esc>** to exit insertion mode. 
- **:**, **w**, **q**, respectively to save my changes and exit vim. 
  
![Image](exit_vim.png)
  
- <enter> to exit officially
  
![Image](vim.png)

#### 5. Run the tests, demonstrating that they now succeed
##### Key Pressed: 
- control + R (to access command history) 
- <up> <up> <enter>
`bash test.sh` is 2 up in the bash history, so I used up arrow to access it. Then I pressed enter to run this command. 
  
![Image](run_success.png) 
  
#### 6. Commit and push the resulting change to your Github account 
- I type in `git add ListExamples.java`.
- I type in `git commit -m "index1 to index2"` with "index1 to index2" as my commit message. 
  
![Image](git.png)  
  
  
  
  
  
