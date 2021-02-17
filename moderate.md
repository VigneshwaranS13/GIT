- to add and commit the file directly

`git commit -am "msg"`

This can be only done in files that are being tracked.Tracked files are the files which are already passed min till  staging area.To check the file is tracked or not we can execute the below    command

`git ls-files`

this will give all files which git is tracking in the current repository


- To recurively add all the files,we can use below command

`git add .`

If we want to move all the untracked files and tracked files from local to git statging area above command will be useful.`Git status` -will provvide the changes in the current directory only,in that case if we add all the files using above command then we can see all the changes
