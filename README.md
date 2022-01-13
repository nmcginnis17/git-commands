<h1>Git Commands</h1>

<h2>How to check your Git configuration:</h2>
<b>The command below returns a list of information about your git configuration including user name and email:</b>

<code>git config -l</code>

<h2>How to setup your Git username:</h2>
<b>With the command below you can configure your user name:</b>

<code>git config --global user.name "User-Name"</code>

<h2>How to setup your Git user email:</h2>
<b>This command lets you setup the user email address you'll use in your commits.</b>

<code>git config --global user.email "your-email@example.com"</code>

<h2>How to cache your login credentials in Git:</h2>
<b>You can store login credentials in the cache so you don't have to type them in each time. Just use this command:</b>

<code>git config --global credential.helper cache</code>

<h2>How to initialize a Git repo:</h2>
<b>Everything starts from here. The first step is to initialize a new Git repo locally in your project root. You can do so with the command below:</b>

<code>git init</code>

<h2>How to add a file to the staging area in Git:</h2>
<b>The command below will add a file to the staging area. Just replace filename_here with the name of the file you want to add to the staging area.</b>

<code>git add filename_here</code>

<h2>How to add all files in the staging area in Git</h2>
<b>If you want to add all files in your project to the staging area, you can use a wildcard . and every file will be added for you.</b>

<code>git add .</code>

<h2>How to add only certain files to the staging area in Git</h2>
<b>With the asterisk in the command below, you can add all files starting with 'fil' in the staging area.</b>

<code>git add fil*</code>

<h2>How to check a repository's status in Git:</h2>
<b>This command will show the status of the current repository including staged, unstaged, and untracked files.</b>

<code>git status</code>

<h2>How to commit changes in the editor in Git:</h2>
<b>This command will open a text editor in the terminal where you can write a full commit message.

A commit message is made up of a short summary of changes, an empty line, and a full description of the changes after it.</b>

<code>git commit</code>

<h2>How to commit changes with a message in Git:</h2>
<b>You can add a commit message without opening the editor. This command lets you only specify a short summary for your commit message.</b>

<code>git commit -m "your commit message here"</code>

<h2>How to commit changes (and skip the staging area) in Git:</h2>
<b>You can add and commit tracked files with a single command by using the -a and -m options.</b>

<code>git commit -a -m"your commit message here"</code>

<h2>How to see your commit history in Git:</h2>
<b>This command shows the commit history for the current repository:</b>

<code>git log</code>

<h2>How to see your commit history including changes in Git:</h2>
<b>This command shows the commit's history including all files and their changes:</b>

<code>git log -p</code>

<h2>How to see a specific commit in Git:</h2>
<b>This command shows a specific commit.

Replace commit-id with the id of the commit that you find in the commit log after the word commit.</b>

<code>git show commit-id</code>

<h2>How to see log stats in Git:</h2>
<b>This command will cause the Git log to show some statistics about the changes in each commit, including line(s) changed and file names.</b>

<code>git log --stat</code>

<h2>How to see changes made before committing them using "diff" in Git:</h2>
<b>You can pass a file as a parameter to only see changes on a specific file.
git diff shows only unstaged changes by default.

We can call diff with the --staged flag to see any staged changes.</b>

<code>git diff</code><br>
<code>git diff all_checks.py</code><br>
<code>git diff --staged</code>

<h2>How to see changes using "git add -p":</h2>
<b>This command opens a prompt and asks if you want to stage changes or not, and includes other options.</b>

<code>git add -p</code>

<h2>How to remove tracked files from the current working tree in Git:</h2>
<b>This command expects a commit message to explain why the file was deleted.</b>

<code>git rm filename</code>

<h2>How to rename files in Git:</h2>
<b>This command stages the changes, then it expects a commit message.</b>

<code>git mv oldfile newfile</code>

<h2>How to ignore files in Git:</h2>
<b>Create a <code>.gitignore</code> file and commit it.</b>

<h2>How to revert unstaged changes in Git:</h2>
<code>git checkout filename</code>

<h2>How to revert staged changes in Git:</h2>
<b>You can use the -p option flag to specify the changes you want to reset.</b>

<code>git reset HEAD filename</code><br>
<code>git reset HEAD -p</code>

<h2>How to amend the most recent commit in Git:</h2>
<b>git commit --amend allows you to modify and add changes to the most recent commit.</b>
<h6>Note: Fixing up a local commit with amend is great and you can push it to a shared repository after you've fixed it. But you should avoid amending commits that have already been made public.</h6>

<code>git commit --amend</code>

<h2>How to rollback the last commit in Git:</h2>
<b>git revert will create a new commit that is the opposite of everything in the given commit.
We can revert the latest commit by using the head alias like this:</b>

<code>git revert HEAD</code>

<h2>How to rollback an old commit in Git:</h2>
<b>You can revert an old commit using its commit id. This opens the editor so you can add a commit message.</b>

<code>git revert comit_id_here</code>

<h2>How to create a new branch in Git:</h2>
<b>By default, you have one branch, the main branch. With this command, you can create a new branch. Git won't switch to it automatically – you will need to do it manually with the next command.</b>

<code>git branch branch_name</code>

<h2>How to switch to a newly created branch in Git:</h2>
<b>When you want to use a different or a newly created branch you can use this command:</b>

<code>git checkout branch_name</code>

<h2>How to list branches in Git:</h2>
<b>You can view all created branches using the git branch command. It will show a list of all branches and mark the current branch with an asterisk and highlight it in green.</b>

<code>git branch</code>

<h2>How to create a branch in Git and switch to it immediately:</h2>
<b>In a single command, you can create and switch to a new branch right away.</b>

<code>git checkout -b branch_name</code>

<h2>How to delete a branch in Git:</h2>
<b>When you are done working with a branch and have merged it, you can delete it using the command below:</b>

<code>git branch -d branch_name</code>

<h2>How to merge two branches in Git:</h2>
<b>To merge the history of the branch you are currently in with the branch_name, you will need to use the command below:</b>

<code>git merge branch_name</code>

<h2>How to show the commit log as a graph in Git:</h2>
<b>We can use <code>--graph</code> to get the commit log to show as a graph. Also,
<code>--oneline</code> will limit commit messages to a single line.</b>

<code>git log --graph --oneline</code>

<h2>How to show the commit log as a graph of all branches in Git:</h2>
<b>Does the same as the command above, but for all branches.</b>

<code>git log --graph --oneline --all</code>

<h2>How to abort a conflicting merge in Git:</h2>
<b>If you want to throw a merge away and start over, you can run the following command:</b>

<code>git merge --abort</code>

<h2>How to add a remote repository in Git</h2>
<b>This command adds a remote repository to your local repository (just replace https://repo_here with your remote repo URL).</b>

<code>git add remote https://repo_here</code>

<h2>How to see remote URLs in Git:</h2>
<b>You can see all remote repositories for your local repository with this command:</b>

<code>git remote -v</code>

<h2>How to get more info about a remote repo in Git:</h2>
<b>Just replace origin with the name of the remote obtained by
running the git remote -v command.</b>

<code>git remote show origin</code>

<h2>How to push changes to a remote repo in Git:</h2>
<b>When all your work is ready to be saved on a remote repository, you can push all changes using the command below:</b>

<code>git push</code>

<h2>How to pull changes from a remote repo in Git:</h2>
<b>If other team members are working on your repository, you can retrieve the latest changes made to the remote repository with the command below:</b>

<code>git pull</code>

<h2>How to check remote branches that Git is tracking:</h2>
<b>This command shows the name of all remote branches that Git is tracking for the current repository:</b>

<code>git branch -r</code>

<h2>How to fetch remote repo changes in Git:</h2>
<b>This command will download the changes from a remote repo but will not perform a merge on your local branch (as git pull does that instead).</b>

<code>git fetch</code>

<h2>How to check the current commits log of a remote repo in Git:</h2>
<b>Commit after commit, Git builds up a log. You can find out the remote repository log by using this command</b>

<code>git log origin/main</code>

<h2>How to merge a remote repo with your local repo in Git:</h2>
<b>If the remote repository has changes you want to merge with your local, then this command will do that for you:</b>

<code>git merge origin/main</code>

<h2>How to get the contents of remote branches in Git without automatically merging:</h2>
<b>This lets you update the remote without merging any content into the
local branches. You can call git merge or git checkout to do the merge.</b>

<code>git remote update</code>

<h2>How to push a new branch to a remote repo in Git:</h2>
<b>If you want to push a branch to a remote repository you can use the command below. Just remember to add -u to create the branch upstream:</b>

<code>git push -u origin branch_name</code>

<h2>How to remove a remote branch in Git:</h2>
<b>If you no longer need a remote branch you can remove it using the command below:</b>

<code>git push --delete origin branch_name</code>

<h2>How to use Git rebase:</h2>
<b>You can transfer completed work from one branch to another using git rebase.</b><br>
<b>Git Rebase can get really messy if you don't do it properly. Before using this command I suggest that you re-read the official documentation <i style="text-decoration: underline"><a href="https://git-scm.com/book/it/v2/Git-Branching-Rebasing">here</a></i></b>

<code>git rebase branch_name</code>

<h2>How to run rebase interactively in Git:</h2>
<b>You can run git rebase interactively using the -i flag.<br>
It will open the editor and present a set of commands you can use.</b>

<code>git rebase -i master</code><br>
<code># p, pick = use commit</code><br>
<code># r, reword = use commit, but edit the commit message</code><br>
<code># e, edit = use commit, but stop for amending</code><br>
<code># s, squash = use commit, but meld into previous commit</code><br>
<code># f, fixup = like "squash", but discard this commit's log message</code><br>
<code># x, exec = run command (the rest of the line) using shell</code><br>
<code># d, drop = remove commit</code>

<h2>How to force a push request in Git:</h2>
<b>This command will force a push request. This is usually fine for pull request branches because nobody else should have cloned them.
But this isn't something that you want to do with public repos.</b>

<code>git push -f</code>
