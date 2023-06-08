#### 1. Login to ieng6
##### Key Pressed: 
- `ssh<Space>cs15lsp23fq@ieng6.ucsd.edu<Enter>`

Explanation: 

to login to ieng6 directly

![Image](eng.png)

#### 2. Clone your fork of the repository from your Github account
##### Key Pressed: 
- `git<Space>clone<Space>https://github.com/ucsd-cse15l-s23/lab7.git<Enter>` 

Explanation:

to clone my fork of the repository

![Image](git.png)

#### 3. Run the tests, demonstrating that they fail
##### Key Pressed: 
- `cd<Space>lab7<Enter>bash<Space>test.sh<Enter>` 

Explanation:

- `cd<Space>lab7<Enter>` to change my working directory to lab7

- `bash<Space>test.sh<Enter>` to run the test. 

![Image](run_fail.png)

#### 4. Edit the code file to fix the failing test
##### Key Pressed: 

- `vim<Space>ListExamples.javakkkkkklllllllllllxi2<esc>:wq<enter>`

Explanation: 

- `vim<Space>ListExamples.java` to enter vim. 

- **k** 6 times to move the cursor to the line of the while loop. 

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

#### 5. Run the tests, demonstrating that they now succeed
##### Key Pressed: 
  
- `bash<Space>grade.sh<Enter>`
  
Explanation:
  
to run the test again. 
  
![Image](run_success.png) 
  
#### 6. Commit and push the resulting change to your Github account 
##### Key Pressed: 
  
- `git<Space>add<Space>ListExamples.java<Enter>git<Space>commit<Space>-m<Space>"index1 to index2"<Enter>git<Space>remote<Space>add<Space>origin<Space>git@github.com:XIC051/lab7.git<Enter>git<Space>push<Space>origin<Space>main<Enter>`

Explanation: 
- `git<Space>add<Space>ListExamples.java` 
  
This command adds the file "ListExamples.java" to the Git staging area. It prepares the file to be included in the next commit.
  
- `git<Space>commit<Space>-m<Space>"index1 to index2"` 
 
creates a new commit with commit message "index1 to index2"

- `git<Space>remote<Space>add<Space>origin<Space>git@github.com:XIC051/lab7.git`
  
adds a new remote named "origin" to my Git repository. 
  
- `git<Space>push<Space>origin<Space>main`
  
This command pushes the commits in local branch "main" to the remote repository named "origin". It uploads the changes I just made to the remote repository on GitHub.
  
![Image](github.png)
![Image](git_push.png)
  
  
  
  
  
