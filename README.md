| Category                | Command                                                    | Description                                                                                   |
|-------------------------|------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| Git Configuration       | git config --global user.name "Your Name"                  | Set your Git username globally                                                                |
|                         | git config --global user.email "Your Email"                | Set your Git email globally                                                                   |
| Initialize Git          | git init                                                   | Initialize a new Git repository in the current directory                                      |
| Terminal Navigation     | clear                                                      | Clear the terminal screen                                                                     |
|                         | cd ..                                                      | Change to the parent directory                                                                |
|                         | cd "Folder Name"                                           | Change to the specified directory                                                             |
|                         | ↑ (Up arrow)                                               | Recall the previous command                                                                   |
|                         | ls                                                         | List files and directories in the current directory                                           |
|                         | ls -lart (or ls -a)                                        | List all files and directories, including hidden ones, with detailed information              |
| File Management         | touch "File Name"                                          | Create a new empty file                                                                       |
|                         | touch index.html                                           | Create a new empty file named index.html                                                      |
|                         | touch about.html                                           | Create a new empty file named about.html                                                      |
|                         | mkdir "Folder Name"                                        | Create a new directory                                                                        |
|                         | mkdir css                                                  | Create a new directory named css                                                              |
|                         | mkdir js                                                   | Create a new directory named js                                                               |
|                         | cat "File Name"                                            | Display the contents of the specified file                                                    |
|                         | cat index.html                                             | Display the contents of index.html                                                            |
|                         | start "File Name"                                          | Open the specified file in the default web browser                                            |
|                         | start index.html                                           | Open index.html in the default web browser                                                    |
|                         | start chrome index.html                                    | Open index.html in Google Chrome                                                              |
| Git Basics              | git status                                                 | Show the working directory status, including staged, unstaged, and untracked files            |
|                         | git add "fileName"                                         | Stage the specified file                                                                      |
|                         | git add index.html                                         | Stage index.html file                                                                         |
|                         | git add -A                                                 | Stage all changes in the working directory                                                    |
|                         | git add .                                                  | Stage all changes in the current directory                                                    |
|                         | git add css                                                | Stage all changes in the css directory                                                        |
|                         | git add css/style.css                                      | Stage the style.css file under the css directory                                              |
|                         | git commit -m "Write Your Comment"                         | Commit staged changes with a descriptive message                                              |
|                         | git commit                                                 | Commit staged changes using a text editor (manual process)                                    |
|                         | (Press I → "Initial Commit" → ESC Button → :wq)            | Write commit message, then save and quit                                                      |
|                         | git log                                                    | Show the commit history                                                                       |
|                         | git log -p -1                                              | Show the changes introduced in the last commit                                                |
|                         | Q                                                          | Quit the log view and return to the command prompt                                            |
|                         | git diff                                                   | Show differences between working directory and the index or a tree                             |
|                         | git reset                                                  | Unstage all changes that have been added to the index                                         |
|                         | git reset --hard                                           | Reset the index and working directory to the last committed state                             |
|                         | .gitignore                                                 | Specify files and directories to be ignored by Git                                            |
| File & Folder Management| git rm "fileName" -f                                       | Remove the specified file from the working directory and the index                            |
|                         | git rm index.html -f                                       | Remove index.html from the working directory and the index                                    |
|                         | rmdir "folderName"                                         | Remove the specified empty directory                                                          |
|                         | rmdir css                                                  | Remove the css directory                                                                      |
| Undo Changes            | git checkout "fileName"                                    | Restore the specified committed file to the working directory                                 |
|                         | git checkout index.html                                    | Restore index.html to the working directory                                                   |
|                         | git checkout -f                                            | Discard changes in the working directory (force checkout)                                     |
| Branching               | git branch                                                 | List all branches                                                                             |
|                         | git branch "Branch Name"                                   | Create a new branch named 'Branch Name'                                                       |
|                         | git checkout -b "Branch Name"                              | Create a new branch and switch to it                                                          |
|                         | git checkout "Branch Name"                                 | Switch to the specified branch                                                                |
|                         | git merge "Sub_Branch Name" -m "Comment"                   | Merge the specified sub-branch into the current branch                                        |
| Remote Repositories     | git remote -v                                              | Show remote repository URLs                                                                   |
|                         | git remote add origin https://github.com/User/Repo.git     | Add a remote repository with HTTPS                                                            |
|                         | git remote add origin git@github.com:User/Repo.git         | Add a remote repository with SSH                                                              |
| SSH Key Setup           | ssh-keygen -t rsa -b 4096 -C "your_email@example.com"      | Generate a new SSH key with RSA algorithm and 4096-bit key size                               |
|                         | enter the name of folder, press enter                      | Follow the prompts to save the SSH key to the specified folder                                |
|                         | eval "$(ssh-agent -s)"                                     | Start the SSH agent                                                                           |
|                         | ssh-add ~/path/to/your/ssh_key                             | Add the SSH private key to the SSH agent                                                      |
|                         | cat ~/.ssh/id_rsa.pub                                      | Display the SSH public key                                                                    |
| Push to Remote Repo     | git push -u origin master                                  | Push the current branch to the remote repository and set the upstream branch                  |
|                         | git push                                                   | Push committed changes to the remote repository when the upstream branch is already set       |
