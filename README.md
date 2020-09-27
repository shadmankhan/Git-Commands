# Git-Commands


## Creating a File
`$ touch file_name.txt`

## To see file content
`$ cat filename.txt`


## To create directory
`$ mkdir directory_name`

## To change the current directory
`$ cd directory_name`

## Checking the current directory
`$ pwd 			[pwd stands for "Print Working Directory"]`

## Displaying the Content of the Directory
`$ ls`

## Moving to parent or home directory
`$ cd .. OR $ cd`

## Moving a file
```
$ mv file_name.txt destination
eg - $ mv header.txt html <-- here html is directory and header.txt is the file in different directory which is now moved to the html directory
```

## Moving a directory
`$ mv directory_name destination_directory <-- [functions similar to the moving of the file]`

## Renaming a file
`$ mv current_filename.txt new_filename.txt`

## Copying a file
`$ cp file_to_copy new_file_name`

## Copying a Directory
`$ cp -r directory_to_copy new_directory_name		<-- [-r : recursive directory IMPORTANT!!]`

## Removing a File
`$ rm file_to_remove <-- [rm short for "remove"]`

## Removing a Directory
`$ rm -r dir_to_remove`


# Team Development with Git-

## First step: To initialize the git
`$ git init`

## To share your file with others
```
Process is of three steps -
1. Select the file 2. Save the file 3. Share the file:

Step1. $ git add file_name 		<-- [to select the file you want to share]

Step2. $ git commit -m "commit message"	<-- [To record/save a selected file with a msg / commit is to save the file / -m : for msg]

Step3. ## Adding a Remote
To add a new remote, use the git remote add command on the terminal, in the directory your repository is stored at.
The git remote add command takes two arguments:
	- [] A remote name, for example, origin
	- [] A remote URL, for example, https://github.com/user/repo.git
	
	## Set a new remote
	$ git remote add remote_name URL
	Example: $ git remote add origin https://github.com/user/repo.git
	
	## Verify new remote
	$ git remote -v
	> origin  https://github.com/user/repo.git (fetch)
	> origin  https://github.com/user/repo.git (push)

	## Now upload files to remote
	$ git push remote_name master	<-- [push is used to upload files to the remote]

  	## Downloading Files from a Remote
  	$ git pull remote_name master			<-- [pull is used for downloading files from remote]
```

## Important Points About Git#
_In team development, it is important to clearly recognize the changes you have made and select which changes should be shared with your partners._
```
You can check if the and where your changes have been made by
$ git status
```

## To see the modified content in the file
`$ git diff 			<-- [ Now you can see the changes/modifications in the files in the git.`

## To see changes acc to files
```
$ git log
or 
$ git log -p
```

## Git Stash

_Suppose you have made changes into your team project repository and you don't want to push your changes into the main repository (master: develop). In that case, you can use git stash which will keep your changes into a stash and then let you make a new branch or switch to different branch. After switching, you can push all your changes into that branch with git stash apply._
```
	## To keep all the changes into Stash
	$ git stash

	## To check all the stashes
	$ git stash list

	## To apply your stash
	$ git stash apply
```
