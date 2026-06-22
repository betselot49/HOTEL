# HOTEL

HOTEL

## Codex cloud setup check

This README update confirms that Codex can access this repository workspace, edit project files, and commit changes from the current branch.

Codex cannot directly access a Windows-only local path such as `D:\Project` from this Linux cloud workspace. To give Codex full GitHub push and pull access, clone the GitHub repository into your Windows project folder and make sure the repository has an `origin` remote.

From Windows PowerShell:

```powershell
mkdir D:\Project
cd D:\Project
git clone <your-github-repo-url> HOTEL
cd HOTEL
git remote -v
```

For a Node.js project workflow, use GitHub branches and pull requests for each task, and run the project checks before merging. Common commands are:

```bash
npm ci
npm test
npm run build --if-present
```
