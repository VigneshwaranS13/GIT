## Git

### **Starting with the fresh Project**

To start a new project we need to move to the directory where we need to create a project 

>`pwd`

>`git init new_Project`

We can use below command to list all the files presnet in the initialized git directory

>`git ls -al`

To create new file we can use below command

>code newfilename.ext

#### Note : Here code (VisualStudio Code) is a default editor which is configured for Git

To add newly created file to git repository

>`git add fiename`

To remove a directory from gi

>`rm -rf diretory_name/`

---

## Adding Git to an existing project

Move to the root directory of the project  and type

> `git init`

This will create a new repository using a current folder as working directory.We can verify this by 

>`ls -al`

We can see the .git folder where git repsoitory live

To add all the untracked files into staging area, we can use

>`git add .`

This will recursively add  all the  files in the project











