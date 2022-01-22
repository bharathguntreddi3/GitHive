# Git_GitHub_Test
Find everything about git and github you are looking for and the commands for git and github. Fully tested gateway to git &amp; github



/*--------------------------------------------------------------------------------------------------------*/
git config --global user.name [--username]

git config user.name #checkuser

git config --global user.email [--useremail]

git config user.email #checkmail



/*-----------------------------------------------------------------------------------------------------*/
git init #initiate the git

git status #files changed but not staged

git add [--file_name]or [space .] #add files to stagen area; '.' to select all files'

git rm --cached [--file_name]   #to unstage the files

git commit -m "[--any_msg_needed]"

git log #shows history of the commits

git log --oneline #shows history of commits in oneline

git diff #differences between states of the files



/*--------------------------------------------------------------------------------------------------------*/
git checkout [--unique_id_of_commit]

git checkout [--branch_name] #go to the last recent commit

git revert [--unique_id_of_commit] #revert the commit and and again commits the reverted_can change the msg

git reset [--unique_id_of_commit] #reset a commit and rollback

git reset [--unique_id_of_commit] --hard #hard flag to ratain no changes

git branch [--new_branch_name] #add new branch

git branch -a #check the branches

git checkout [--new_branch_name] #change to the new branch

git branch -D [--new_branch_name] #delete a branch '-D' used before merging

git checkout -b [--new_branch_name] -a #create and change to the new branch

#checkout to the master branch before merging the branches!!!

git merge [--branch_name] #merge the new_branch to master branch

git commit #conflict occurs when we merge the same file with different text





/*--------------------------------------------------------------------------------------------------------*/
/*--push to github*/

git push [--url_of_repo] [--branch] #push to repo to the branch

git remote add [--alias_name #generally_alias_is_origin] [url_of_repo] #add an alias name to the repo instead of link

git push origin master #pushing with the alias name

git clone [--repo_url] #cloning a repo locally

git remote -v #already stored to origin in the cloned repo

git pull origin master #pulls the all new chages and updates to our local repo





/*--------------------------------------------------------------------------------------------------------*/
/*-push conflict-*/

git push origin master --force

git push origin master -rebase





/*--------------------------------------------------------------------------------------------------------*/
/*-merge conflict-*/

#merge conflict occurs when there is a difference between the states of the files while merging

#edit the files and combine the different states of the files and then merge.After editing the file, then commit the changes and then merge the branches

git commit -m "[--any_message]"

git merge [--branch_name] #merge the edited file to the master branch




