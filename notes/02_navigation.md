# navigation 
- - - 

- a unix-like operating system such as linux, organises its files in what is called a hierarchical directory structure (meaning they are organised in a tree-like pattern of directories)
- the first directory in the file system is called the **root directory**, it contains files and subdirectories, which contain more files and subdirectories and so on
- note that unlike windows, which has a seperate file-system tree for each storage device, linux always has a single file-system tree regardless of how many drives or storage devices are attached to the computer
- if you think of the file system as a maze shaped like an upside down tree and we're standing in the middle of it, at any given time we are inside a single directory and we can see the files contained within that directory and the pathway to the directory above us (parent directory) or any subdirectories below us
- to display the current working directory - use `pwd`
- when we first log into our system, our current working directory is set to the **home** directory, and each user is given their own home directory (if you have multiple users sharing your system), it is the only place a regular user is allowed to write files
- to list the files and directories of the current working directory - use `ls`
- to change the current working directory - use `cd` followed by the pathname of the desired working directory
- a pathname begins with the root directory and follows the tree, branch by branch until the path to the desired directory is completed
- an absolute pathname starts from the root directory and leads to its destination, a relative pathname starts from the working directory, to do this it uses a couple of special notations to represent the relative positions in the file system tree, these special notations are '.' and '..'
- '.' refers to the working directory and '..' refers to the working directory's parent directory, for example when you change your working directory to /usr/bin and you wanted to go to /usr (the parent directory), you could either use the absolute pathname: `cd /usr` or using the relative pathname: `cd ..`, both of them lead to /usr as the current working directory
- if you do not specify a pathname to something, the working directory will be assumed, in general
- some helpful shortcuts: 
    1. `cd` changes the working directory to your home directory
    2. `cd -` changes the working directory to the previous working directory
    3. `cd ~user_name` changes the working directory to the home directory of user_name
