# Git Bash Commands 
--

## Creating repo and publishing
--
### ✅ STEP 1: Configure Git (First Time Only)
<pre> 
  git config --global user.name "Chetanpatil03"
  git config --global user.email "your-email"
  git config --list
</pre>

### ✅ STEP 2: Initialize a Git Repository
<pre>
  git init
</pre>

### ✅ STEP 3: Stage and Commit Files
<pre>
  git add . 
  git commit -m "Initial commit"

</pre>
`git add .` for all files in the directory.
to add specific file : 
<pre>
  git add <file_name>
</pre>

### ✅ STEP 4: Create a New Repo on GitHub<br>
1 Go to https://github.com<br>
2 Click ➕ → "New repository"<br>
3 Don’t initialize with a README (optional)<br>
4 Copy the repo URL (HTTPS or SSH)<br>

### ✅ STEP 5: Connect Local Repo to GitHub
<pre>
  git remote add origin https://github.com/yourusername/your-repo.git
</pre>

### ✅ STEP 6: Push Code to GitHub
<pre>
git branch -M main         
git push -u origin main
  
</pre>


### ✅ STEP 7: Make Ongoing Changes
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
-- to see the history
<pre>
  git log
</pre>
-- To Find the difference between two commits
<pre>
  git diff
</pre>

# Creating branches 
To create and use braches 
## 1. Create branch 
<pre>
  git branch <branch_name>
</pre>

## 2. Shift branch 
<pre>
  git checkout <branch_name>
</pre>

## 3. Combine both commands 
<pre>
  git checkout -b <branch_name>
</pre>
<br><br>

# Credential Manager 
if you pc/laptop have multiple git account and you are confused how to config and error occured then<br>
-> Search for `credential manager` in `searchbar`<br>
-> Go to `Windows crediential ` <br>
-> Locate `github` and remove it.<br>

--
# Pull Request : 
## 1. Clone the GitHub Repo to Your Local Machine
First, open your terminal (or Git Bash, if on Windows).
Run:
<pre>
  git clone https://github.com/username/repo-name.git
</pre>

Replace username and repo-name with the actual repo info.
This will download the entire repo into a folder named repo-name on your machine.

## 2. Navigate Into the Repo Folder
<pre>
  cd repo-name
</pre>

## 3. Create and Switch to a New Branch
To create a new branch and switch to it immediately, run:
<pre>
  git checkout -b new-branch-name
</pre>
Replace new-branch-name with your branch name (e.g., feature/login).

## 4. Make Your Changes
Edit files as needed in your local files.

## 5. Stage and Commit Your Changes
<pre>
  git add .
</pre>
Then commit:
<pre>
  git commit -m "Describe your changes here"
</pre>

## 6. Push Your Branch to GitHub
To publish your branch on GitHub:
<pre>
  git push origin new-branch-name
</pre>

## 7. Checkout to main for merge the branch into main branch
   <pre>
     git chechout main
   </pre>
## 8. Merge the branch
   <pre>
     git merge -new-branch-name
   </pre>
## 9. Push the merge to remote
  <pre>
      git push -u origin main
  </pre>

# Summary Pull/Clone Requests: 
<pre>
git clone https://github.com/username/repo-name.git
cd repo-name
git checkout -b new-branch-name
# make changes to files
git add .
git commit -m "Your commit message"
git push origin new-branch-name
git checkout main
git merge new-branch-name
git push origin main
</pre>

# Reverting Changes/ Undo the changes
To revert the changes we can use the ```git revert``` command.

## 🔁 **To Revert a Commit (Safe for Pushed Commits)**

This method creates a new commit that undoes the changes from a previous one.

### ✅ Step-by-Step:

1. **View the commit history:**

   ```bash
   git log --oneline
   ```

   Example output:

   ```
   a1b2c3d Revert "Add login feature"
   1234567 Add login feature
   89abcde Initial commit
   ```

2. **Copy the hash** of the commit you want to revert (e.g., `1234567`).

3. **Revert the commit:**

   ```bash
   git revert 1234567
   ```

4. **Save the commit message** (Git will open your default editor — just save and close).

5. **Push the changes (if needed):**

   ```bash
   git push origin <branch-name>
   ```

---

## 🧹 **To Completely Undo a Commit (Local Only)**

This is for when you **haven't pushed the commit yet** and want to **erase it**.

### Option 1: Keep the changes (just undo the commit)

```bash
git reset --soft HEAD~1
```

### Option 2: Unstage and keep changes

```bash
git reset --mixed HEAD~1
```

### Option 3: Remove commit and discard changes

```bash
git reset --hard HEAD~1
```

> Replace `HEAD~1` with `HEAD~2`, etc., if you're undoing further back.

## docker file 
1. Creating html file (index.html)
2. creating docker file (dockerfile)
<pre>
FROM nginx
COPY index.html /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
</pre>

3. build docker image
```docker build -t <docker_app>```

4. Run webapp 
```docker run -d -p 8080:80 <docker_app>```

5. Test docker image with ```http://localhost:8080```

This is primarily created for Github practicals 
-- 
Created by CHETAN ❤️


