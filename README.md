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
```

After we make changes to the file, see that the changes are not tracked because we did not add the file. Use commands:
```
git add main.py
git commit -m "Change printing message to Hello, Summer!"
git log
```
Another useful commands at this stage:
```
git status
git diff
git log --oneline
```

Picture to explain possible status of the files:
![](lifecycle_of_files_in_git.png)
