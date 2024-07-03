# GIT PRACTICE EXERCISE 2

## Exercise 1
- Clone the repository at https://gitlab.cloudifyops.com/clops-training/git-practice-repo.git
- Add a file to the participants directory that describes you.
- Use git add to add that file to the repository.
- Use git commit to commit your change. Use a meaningful message like "Added information about YOUR NAME HERE."
- Use git push to send your change to the primary repository.
- Look online to see if your change has been pushed.
- Wait until your partner has pushed their update. Then use git pull to get their change into your repository. Verify that you have the new file.
- Use git log or git log | less to see a list of changes to the repository.
- Edit the file participants.md to add your name. Then add the file, commit it, and push it.
- Whoever tries to push the file first will likely succeed. Whoever tries to push the file second will likely get an error message. Figure out how to resolve the error message.
- Deal with any conflicts that have arisen and commit the result.

## Exercise 2
- Clone the repository at https://gitlab.cloudifyops.com/clops-training/git-practice-repo.git
- Create a new directory and change into it.
- Use the init command to create a Git repository in that directory.
- Observe that there is now a .git directory.
- Create a README file.
- Look at the output of the status command; the README you created should appear as an untracked file.
- Use the add command to add the new file to the staging area. Again, look at the output of the status command.
- Now use the commit command to commit the contents of the staging area.
- Create a src directory and add a couple of files to it.
- Use the add command, but name the directory, not the individual files. Use the status command. See how both files have been staged. Commit them.
- Make a change to one of the files. Use the diff command to view the details of the change.
- Next, add the changed file, and notice how it moves to the staging area in the status output. Also observe that the diff command you did before using add now gives no output. Why not? What do you have to do to see a diff of the things in the staging area? (Hint: review the slides if you can’t remember.)
- Now without committing, make another change to the same file you changed in step 10. Look at the status output, and the diff output. Notice how you can have both staged and unstaged changes, even when you are talking about a single file. Observe the difference when you use the add command to stage the latest round of changes. Finally, commit them. You should now have started to get a feel for the staging area.
- Use the log command in order to see all of the commits you made so far.
- Use the show command to look at an individual commit. How many characters of the commit identifier can you get away with typing at a minimum?
- Make a couple more commits, at least one of which should add an extra file.

- Use the Git rm command to remove a file. Look at the status afterwards. Now commit the deletion.
- Delete another file, but this time do not use Git to do it; e.g. if you are on Linux, just use the normal (non-Git) rm command; on Windows use del.
- Look at the status. Compare it to the status output you had after using the Git built-in rm command. Is anything different? After this, commit the deletion.
- Use the Git mv command to move or rename a file; for example, rename README to README.txt. Look at the status. Commit the change.
- Now do another rename, but this time using the operating system’s command to do so. How does the status look? Will you get the right outcome if you were to commit at this point? (Answer: almost certainly not, so do not. 🙂 Work out how to get the status to show that it will not lose the file, and then commit. Did Git at any point work out that you had done a rename?
- Use git help log to find out how to get Git to display just the most recent 3 commits. Try it.
- If you do not remember, look back in the slides to see what the –stat option did on the diff command. Find out if this also works with the show command. How about the log command?
- Imagine you want to see a diff that summarizes all that happened between two commit identifiers. Use the diff command, specifying two commit identifiers joined by two dots (that is, something like abc123..def456). Check the output is what you expect.
- Cut the branch out of the main branch, the branch name should be your_name and add a file to the code folder with your_name as the file name.
- Merge the branch with the main branch and check if the files added by you in the branch can be seen in the main branch.
