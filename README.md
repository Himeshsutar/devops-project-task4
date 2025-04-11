🚀 TASK 4: Version-Controlled DevOps Project with Git

✅ Objective

Manage a DevOps project using Git best practices including version control, branching strategy, pull requests, commit conventions, file ignoring, tagging, and documentation.

🛠️ Tools & Technologies

Git

GitHub

.gitignore

Git Tags

Markdown


📁 Project Structure

README.md – Documentation

.gitignore – File to exclude unnecessary or sensitive files

login.txt – Sample feature file 

(Task4.md can optionally be added for step documentation)


🔧 Steps Performed

🔹 a. Initialize Repository and Push to GitHub

Created a new directory and initialized it using git init. Created a README.md with basic content and performed the first commit using:  

`git add .`

`git commit -m "Initial commit: Set up project structure"`

Connected the local repository to GitHub with:  

`git remote add origin https://github.com/your-username/devops-project-task4.git`  

Pushed the main branch using:  

`git branch -M main`  

`git push -u origin main`


🔹 b. Create Branches

Created a development branch using:  

`git checkout -b dev`  

`git push -u origin dev`  

Created a feature branch using:  

`git checkout -b feature/login`  

`git push -u origin feature/login`


🔹 c. Use Pull Requests to Merge

Made changes in the feature branch (e.g., added login.txt), then staged and committed using:  

`git add login.txt`  

`git commit -m "feat: add login feature"` 


Pushed the branch to GitHub with:  

`git push`  

Created a pull request from `feature/login` to `dev` via the GitHub UI, submitted it with a proper title and message, and merged after review.


🔹 d. Add a Proper README.md

Wrote a clean and comprehensive README.md file documenting objectives, tools used, structure, and the full workflow — including example commit messages such as:  

`feat: add login feature`  

`fix: resolve error in CI pipeline`  

`docs: update README.md`  

`chore: add .gitignore file`


🔹 e. Use .gitignore and Tags

Created a `.gitignore` file to exclude unwanted files such as:  

```
node_modules/  
.env  
*.log  
*.tmp  
__pycache__/  
.vscode/  
.idea/  
.DS_Store
```  

Committed and pushed using:  

`git add .gitignore`  

`git commit -m "chore: add .gitignore file"`  

`git push`  

Tagged the version with:  

`git tag -a v1.0.0 -m "Initial release"`  

`git push origin v1.0.0`


🔹 f. Document All Tasks

All steps were documented clearly using markdown in a single README.md file to ensure easy reference and reproducibility.

✅ Result

Successfully built a version-controlled DevOps project using Git. Demonstrated a full Git workflow including repo setup, branching, pull requests, commit standards, file exclusions, version tagging, and markdown documentation. All operations are tracked and versioned through Git, establishing best practices for collaborative DevOps work.


📎 Notes

Make sure to configure your GitHub remote properly and follow the correct branching model. Always test pull requests in the `dev` branch before merging into `main`. Use semantic commit messages to maintain clean history. Tags are helpful to mark release points for easier rollbacks or deployments.