<style>
    r { color: Red }
    o { color: Orange }
    lg { color: Lime }
</style>


# peaceokay
This is a Markdown file.

### What I've done:
``` properties
cd <project path>

git config user.name "<myname>"
git config user.email "<myemail>"
git config --list --show-origin
git config --global user.name "<myglobalname>"
git config --global commit.template <myPath>

git add <filename>
git commit -m "first commit"

git branch -M master
git remote add origin https://github.com/ffyrikz/peaceokay.git
git remote -v

git push -u origin master

git pull https://github.com/ffyrikz/peaceokay.git
```

### What I've tried:
``` properties
git add <filename>
git commit -m "add I've done"
git status
git log
git diff HEAD^ HEAD

git checkout -b test2
git branch
git push -u origin test2
```

### Exercise 1
> Log tree: <br />
>       S - A - B <br />
> $~~~~~~~~~~$ \\ - C - D 

In this exercise, the HEAD of [<lg>master</lg>] points at B and branch [<r>branch_1</r>] for development. We would like to checkout between B and D but not to commit the half-done work, the command `git stash` come into use.
``` properties
git status
git stash
git status
git stash list

# Restore the modified content
git stash list
git stash apply
git status
git stash list
git stash drop
git stash list

# Remove all the untracked file in working directory
echo "Hello" > file_2.txt
git status -s
git clean -d -n    # do a dry run
git clean -d -f    # force to really do it
```

### What's new
> - Updating README file