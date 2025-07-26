✅ STEP 1: Configure Git (First Time Only)
<pre> 
  git config --global user.name "Chetanpatil03"
  git config --global user.email "your-email"
  git config --list
</pre>

✅ STEP 2: Initialize a Git Repository
<pre>
  git init
</pre>

✅ STEP 3: Stage and Commit Files
<pre>
  git add . 
  git commit -m "Initial commit"

</pre>
`git add .` for all files in the directory.
to add specific file : 
<pre>
  git add <file_name>
</pre>

✅ STEP 4: Create a New Repo on GitHub<br>
1 Go to https://github.com<br>
2 Click ➕ → "New repository"<br>
3 Don’t initialize with a README (optional)<br>
4 Copy the repo URL (HTTPS or SSH)<br>

✅ STEP 5: Connect Local Repo to GitHub
<pre>
  git remote add origin https://github.com/yourusername/your-repo.git
</pre>

✅ STEP 6: Push Code to GitHub
<pre>
git branch -M main         
git push -u origin main
  
</pre>


✅ STEP 7: Make Ongoing Changes
<pre>
  git add .
  git commit -m "Describe your changes"
  git push

</pre>

✅ Optional Commands You’ll Often Use:

| Task                     | Command                 |
| ------------------------ | ----------------------- |
| Check status             | `git status`            |
| See commit history       | `git log --oneline`     |
| Switch branch            | `git checkout <branch>` |
| Pull changes from GitHub | `git pull`              |


## ALL logs :
<pre>
git init
git remote add origin https://github.com/yourusername/yourrepo.git
git add .
git commit -m "Initial commit"
git branch -M main
git push -u origin main
</pre>

## Some useful commands
-- to check url 
<pre>
  git remote -v
</pre>

# creating branches
to create and use braches 
# 1. create branch 
<pre>
  git branch <branch_name>
</pre>

# 2. shift branch 
<pre>
  git checkout <branch_name>
</pre>

# 3. Combine both commands 
<pre>
  git checkout -b <branch_name>
</pre>
<br><br>
## credential Manager 
if you pc/laptop have multiple git account and you are confused how to config and error occured then
-> Search for `credential manager` in `searchbar`
-> Go to `Windows crediential ` 
-> Locate `github` and remove it.


## Pull Request : 
1. Clone the GitHub Repo to Your Local Machine
First, open your terminal (or Git Bash, if on Windows).

Run:
<pre>
  git clone https://github.com/username/repo-name.git
</pre>

Replace username and repo-name with the actual repo info.
This will download the entire repo into a folder named repo-name on your machine.

2. Navigate Into the Repo Folder
<pre>
  cd repo-name
</pre>

3. Create and Switch to a New Branch
To create a new branch and switch to it immediately, run:
<pre>
  git checkout -b new-branch-name
</pre>
Replace new-branch-name with your branch name (e.g., feature/login).

4. Make Your Changes
Edit files as needed in your local files.

5. Stage and Commit Your Changes
<pre>
  git add .
</pre>
Then commit:
<pre>
  git commit -m "Describe your changes here"
</pre>

6. Push Your Branch to GitHub
To publish your branch on GitHub:
<pre>
  git push origin new-branch-name
</pre>

##summary : 
<pre>
git clone https://github.com/username/repo-name.git
cd repo-name
git checkout -b new-branch-name
# make changes to files
git add .
git commit -m "Your commit message"
git push origin new-branch-name
</pre>
