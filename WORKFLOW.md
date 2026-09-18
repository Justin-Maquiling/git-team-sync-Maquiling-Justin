Git Team Sync Workflow

1\. What did the rejected push error message tell you, and why did it happen?



The error message said that my push was rejected because the remote repository had changes that I did not have in my local copy. This happened because Clone A and Clone B made different changes and pushed them at different times. Git stopped the push so that one person's changes would not be overwritten.



2\. What's the actual difference between how you resolved Task 3 (merge) vs Task 4 (rebase)?



For Task 3, I used a merge. I fetched the changes from GitHub and merged them into my branch. When there was a conflict, I fixed the file and then made a merge commit.



For Task 4, I used a rebase. I fetched the changes from GitHub and put my commit on top of the newer remote changes. I fixed the conflict and then continued the rebase.



The main difference is that a merge joins the two histories, while a rebase puts my changes on top of the newer history.



3\. What one habit would have avoided both rejected pushes in this lab?



I could have checked for changes on the remote before starting my work. Running git fetch first would help me see if someone else had already pushed changes.



4\. Which approach - merge or rebase - would you default to on a shared team branch, and why?



I would normally use merge on a shared team branch because it is safer for a branch that other people are using. It keeps the history of both people's work and does not rewrite existing commits.

