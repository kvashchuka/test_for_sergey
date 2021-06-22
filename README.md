# gitCrashCourse

Git book:
https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository

### Step 1 - local repository
We create local folder and a python file in it. 
For example, using this commands in terminal:
```
mkdir gitCourse
cd gitCourse
nano main.py
```
In the file main we only write print message, save and exit. It can be, for example:
```
print("Hello, World!")
```

Now we initialize the repository:
```
git init
ls -a
```
Now we see `.git` folder in it.
Let's try now:
```
git status
git diff
git log 
```

Picture to explain possible status of the files:
![](lifecycle_of_files_in_git.png)

1. Make some changes to the file 
2. Do
```
git status
git diff
```
2. Now add the file:
```
git add main.py
```
3. Do some more changes
4. Again
```
git status
git diff
```
5. Finally 
```
git add main.py
git commit -m "Add main.py and change print message in it"
```

Repeat one more time, but now commit after creating and adding the file and second time after making changes.

Do `git log` and `git log --oneline` and inspect the history.

Note: no, you do not need to make a separate commit when you start from empty file. 
However, it definitely make sense to add file and track it';s changes. 
Especially when you start from some file that you want to modify.

**Important: Commit often! Commit with good commit messages!**
![](git_commit_messages.png)

### Step 2 - remotes
```
git remote
git remote -v
```
Now we do not have any remote repository. Let's connect one.
First, we need to create a repository on GitHub.

Second:
```
git remote add origin git@github.com:kvashchuka/gitCrashCourseProject.git
git push -u origin main
```

Now we run into problems with naming of branches.