## Init Repository

1.Create a repository on Github

2.Create a folder (or an Unreal Project) on the local machine

3.Open a terminal inside that folder and run **git init**
**What this does:** It creates a hidden `.git` directory inside your folder. This directory is where Git stores all the tracking data, history, and configuration for your project.

4.Add the files present in the folder by running **git add .**

5.Create an initial commit by running **git commit -m "First commit"**

6.Upload to a remote host: 
**git remote add origin https://github.com/username/repo-name.git** 
**git branch -M main** 
**git push -u origin main**

## Show commit history
Show with a graph:
**git log --oneline --graph --all**

Show just the commits in reverse order (olderst at the top):
**git log --oneline --reverse**

Show the last 5 commits:
**git log --oneline --reverse -n 5**

## Look to a previous commit
If you want to look to a **previous commit**:
**git checkout "commit-hash"**

To switch back to the **main branch**:
**git checkout main**

## Move the repository back to a specific commit (HARD WAY)

1.Make sure you are on main:
**git checkout main**

2.Reset the branch to an old commit:
**git reset --hard "commit hash" 
WARNING: this will delete any current changes, the folder will look exactly like it di then.

3.Push to the remote host
**git push origin main --force**
