- to add and commit the file directly

`git commit -am "msg"`

This can be only done in files that are being tracked.Tracked files are the files which are already passed min till  staging area.To check the file is tracked or not we can execute the below    command

`git ls-files`

this will give all files which git is tracking in the current repository


- To recurively add all the files,we can use below command

`git add .`

If we want to move all the untracked files and tracked files from local to git statging area above command will be useful.`Git status` -will provvide the changes in the current directory only,in that case if we add all the files using above command then we can see all the changes


##### Backing out changes

- if we want to revert the changes which is moved to staging area for particular file

`git restore --staged <path/filename>`


or

`git reset Head <path/filename>`

- if we want to revert the chagnes in local working directory.But we can to checkout on tracked file.For the new file if we dont require chages then we need to delete that file

` git checkout -- <path/filename>`


#### Rename

- if we want to rename the file we can use two ways
1. Using git

`git mv oldfilename.ext newfilename.ext`

- so by using git rename the changes will automatically moved to staging area
- we have to commit to get the changes reflected in local repository

2. Using OS

`mv oldfilename.ext newfilename.ext`

- if we rename using OS then git will consider this as a two changes,the first one will be the old file is deleted and new file has been created.

- so even the tracked file will be untracked after renaming the file using OS

- To know the git it was rename we can use below command

`git add -A`

- After this command if you checked the status,then the file will automatically moved to staging area with the new name


##### Note:
-we can move the file to differnt folder using git as well as using normal command

- using git
`git mv filename.ext folder1/folder2/folder3`
`git mv filename.ext ../folder1/folder2/folder3` - it will move backwards

- using git
`mv filename.ext folder1/folder2/folder3`
`mv filename.ext ../folder1/folder2/folder3` - it will move backwards




