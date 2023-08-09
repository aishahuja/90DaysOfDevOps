Day 3 Task: Basic Linux Commands

Task: What is the linux command to

1. To view what's written in a file.
2. To change the access permissions of files.
3. To check which commands you have run till now.
4. To remove a directory/ Folder.
5. To create a fruits.txt file and to view the content.
6. Add content in devops.txt (One in each line) - Apple, Mango, Banana, Cherry, Kiwi, Orange, Guava.
7. To Show only top three fruits from the file.
8. To Show only bottom three fruits from the file.
9. To create another file Colors.txt and to view the content.
10. Add content in Colors.txt (One in each line) - Red, Pink, White, Black, Blue, Orange, Purple, Grey.
11. To find the difference between fruits.txt and Colors.txt file.


Reference: https://www.linkedin.com/pulse/linux-commands-devops-used-day-to-day-activit-chetan-/

-----------------------Additions (17/Jul/23) ------------------------------
1. To view what's written in a file.
       cat fileName
   If the file is long or contains a lot of text, we might want to use a pager such as less to view the contents in a more controlled way:
       less fileName
   using cat or less is suitable for viewing the contents of small to moderate-sized text files. If we're dealing with larger files, we might want to use other commands like head or tail to view just the beginning or the end of the file, respectively.

2. To change the access permissions of files in a Linux terminal, we can use the chmod command. The chmod command allows us to modify the read, write, and execute permissions for the owner, group, and others on the file. Here's the basic syntax:
       chmod permission fileName
   The permissions parameter is typically represented using a three-digit octal number, where each digit represents the permissions for the owner, group, and others, respectively. The permission values are as follows:
  4: Read (r)
  2: Write (w)
  1: Execute (x)
  0: No permission
     To change permissions for multiple categories (owner, group, others) simultaneously, you can use the following format:
         chmod ugo permissions fileName
here u represents the owner, g represents the group, and o represents others.
    ex. : chmod u=rwx,g=rx,o=r fileName

3. To check which commands you have run till now.
     We can use the history command to view a list of the commands that we have run during our current session. By default, the history command displays a numbered list of previously executed commands along with their corresponding line numbers.
     If we want to search for specific commands or filter the history output, we can use other commands like grep.
For example, to search for a specific command (e.g., "ls") in our command history, we can use:
       history | grep "ls"
     This will show us a list of commands containing the term "ls".
Keep in mind that the history is typically stored for the duration of our session. If we close the terminal, the history will be lost.

4. To remove a directory/ Folder.
          To remove a directory (folder) in a Linux terminal, we can use the rmdir or rm command. The rmdir command is used to remove empty directories, while the rm command is used to remove both directories and files. Here's how you can use these commands:
       Using rmdir (for empty directories):
              rmdir directoryName : This command will only work if the directory is empty.
       Using rm (for directories and files):

          rm -r directory_name
       The -r flag stands for "recursive" and is necessary to remove directories and their contents. We should be cautious when using rm -r as it will delete the directory and all its contents, including subdirectories and files, without confirmation.
If you want to be prompted for confirmation before removing each file or directory, you can use the -i flag:
       rm -ri directory_name
This will prompt you for confirmation before removing each file or directory within the specified directory.

5. To create a fruits.txt file and to view the content.
8. Add content in devops.txt (One in each line) - Apple, Mango, Banana, Cherry, Kiwi, Orange, Guava.
9. To Show only top three fruits from the file.
10. To Show only bottom three fruits from the file.
11. To create another file Colors.txt and to view the content.
12. Add content in Colors.txt (One in each line) - Red, Pink, White, Black, Blue, Orange, Purple, Grey.
13. To find the difference between fruits.txt and Colors.txt file.
