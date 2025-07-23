✅ STEP 1: Configure Git (First Time Only)
<pre> 
  git config --user.name "Chetanpatil03"
  git config --user.pass "pass"
</pre>

✅ STEP 2: Initialize a Git Repository
<pre>
  git init
</pre>

✅ STEP 3: Stage and Commit Files
<pre>
  git add .           # Stage all files
  git commit -m "Initial commit"

</pre>

✅ STEP 4: Create a New Repo on GitHub
1 Go to https://github.com
2 Click ➕ → "New repository"
3 Don’t initialize with a README (optional)
4 Copy the repo URL (HTTPS or SSH)

✅ STEP 5: Connect Local Repo to GitHub
<pre>
  git remote add origin https://github.com/yourusername/your-repo.git
</pre>

✅ STEP 6: Push Code to GitHub
<pre>
git branch -M main               # Rename to main if needed
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

##Some useful commands
-- to check url 
<pre>
  git remote -v
</pre>

-- creating branches
create branch 
<pre>
  git branch <branch_name>
</pre>

shift branch 
<pre>
  git checkout <branch_name>
</pre>

