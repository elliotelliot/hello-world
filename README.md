# hello-world

Hi there!

This is Elliot, just learning how to use github

Now I'm going to try something else

Just checking something to see if it works...

OK, now I am ready to add some instructions!

\textbf{Creating and Deleting Branches}
\textit{A local branch is on your PC, but won't be on your online repository unless you specifically put it there. Vice versa for a remote branch}

Create local branch `$ git branch [branch-name]`
Delete local branch `$ git branch -d [branch-name]`
Copy local branch to remote branch `$ git push --set -upstream origin [branch-name]`
	or `$ git push origin [local-branch-name]:[remote-branch-name]`
	or, if the remote and local branches will be called the same thing `$ git push origin [branch-name]`
Create remote branch: you need to create a local one first!
Delete remote branch: `$ git push origin --delete [branch-name]`

\textbf{Navigating Between Branches}

Navigate to local branch `$ git checkout [branch-name]`

\textbf{Making Changes}

1. Create a local branch `$ git branch myBranch`
2. Navigate to that branch `$ git checkout myBranch`
3. Open the file in question `$ open myFile.extension`
4. Make your changes and save them
5. Add the file to a list of those to be committed `$ git add myFile.extension` (you can look at this list with `$git status`)
6. Commit the changes to the local branch `$ git commit -m "I added a new function to help make better ice-cream"
7. Upload online `$ git push myRemoteBranch myBranch` or `$git push myBranch` if the remote branch is called the same thing

\textbf{Merging Branches}

1. Compare differences to check what you're merging `$ git diff [branch-name1] [branch-name2]`e.g. `$ git diff master myBranch`
2. Navigate to branch you want to merge into `$ git checkout master`
3. Merge `$ git merge myBranch`
4. You might want to compare the differences again as a sanity check, then delete the branch