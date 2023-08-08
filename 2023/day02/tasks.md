Day 2 Task: Basics linux command

Task: What is the linux command to 
1. Check your present working directory.
2. List all the files or directories including hidden files.
3. Create a nested directory A/B/C/D/E

Note: [Check this file for reference](basic_linux_commands.md)

Check the basic_linux_commands.md file on the same directory day2

----------------- Additions ----------------------
1. pwd
2. To list all files and directories, including hidden files, in a Linux terminal, you can use the ls command with the -a (or --all) option. Hidden files and directories in Linux are those whose names start with a dot (.).
   ls -a
If we want to list the details (permissions, owner, group, size, etc.) of each file and directory, we can use the -l option along with -a:
    ls -la
3. To create a nested directory (a directory within another directory) in a Linux terminal, we can use the mkdir command followed by the -p option. The -p option ensures that the entire directory path is created, including any parent directories that do not yet exist. Here's the general syntax:
   mkdir -p A/B/C/D/E
