# Day 4 Task: Basic Linux Shell Scripting for DevOps Engineers.

 ## What is Kernel

 The kernel is a computer program that is the core of a computer’s operating system, with complete control over everything in the system.
 
 ## What is Shell

 A shell is special user program which provide an interface to user to use operating system services. Shell accept human readable commands from user and convert them into something which kernel can understand. It is a command language interpreter that execute commands read from input devices such as keyboards or from files. The shell gets started when the user logs in or start the terminal.
 
 ## What is Linux Shell Scripting?

 A shell script is a computer program designed to be run by a linux shell, a command-line interpreter. The various dialects of shell scripts are considered to be scripting languages. Typical operations performed by shell scripts include file manipulation, program execution, and printing text.

 **Tasks**

 - Explain in your own words and examples, what is Shell Scripting for DevOps.
      Shell is a command-line interpreter and shell script is nothing but a list of commands executed by the shell.
 Shell scripting for DevOps refers to the commands used to automate the tasks written in the .sh file.
 
 - What is `#!/bin/bash?` can we write `#!/bin/sh` as well?
       #!/bin/bash and #!/bin/sh are known as shebang lines or hashbangs. They are used in shell scripts to specify the interpreter that should be used to execute the script.
#!/bin/bash:
This shebang line specifies that the script should be interpreted and executed using the Bash shell, which is a widely used and powerful shell in Unix-like operating systems.
Bash (Bourne-Again SHell) is an enhanced version of the original Bourne shell (/bin/sh), providing additional features and capabilities.
#!/bin/sh:
This shebang line specifies that the script should be interpreted and executed using the system's default shell, which is typically the Bourne shell.
The Bourne shell (/bin/sh) is a standard and fundamental shell in Unix-like operating systems, and it's usually available by default.
In general, using #!/bin/bash explicitly is often preferred when writing scripts that specifically require Bash features or syntax. However, if your script only uses features that are standard across all POSIX-compliant shells, using #!/bin/sh is a good practice to ensure portability and compatibility across different systems.
For simple scripts that do not require any Bash-specific features, using #!/bin/sh is a good choice to keep the script more portable and accessible on a wider range of systems. Bash is backward-compatible with the Bourne shell, so scripts written for /bin/sh will generally work when executed with #!/bin/bash as well.

 - Write a Shell Script which prints `I will complete #90DaysOofDevOps challenge`
     #!/bin/bash
     echo "I will complete #90DaysOofDevOps challenge"
   
 - Write a Shell Script to take user input, input from arguments and print the variables.
      #!/bin/bash
      # Take user input
        echo "Enter your name: "
        read user_input
      # Use an argument if provided, else use a default value
        argument_input=${1:-"Default Argument"}
      # Print the inputs
        echo "User input: $user_input"
        echo "Argument input: $argument_input"
   
 - Write an Example of If else in Shell Scripting by comparing 2 numbers
      #!/bin/bash
      echo "Enter the first number: "
      read num1
      echo "Enter the second number: "
      read num2
      if [ "$num1" -eq "$num2" ]; then
      echo "The numbers are equal."
      elif [ "$num1" -gt "$num2" ]; then
      echo "The first number is greater than the second number."
      else
      echo "The second number is greater than the first number."
      fi


 Was it difficult?
 
 - Post about it on LinkedIn and Let me know :)

 Article Reference: [Click here to read basic Linux Shell Scripting](https://devopscube.com/linux-shell-scripting-for-devops/)

 YouTube Vedio: [EASIEST Shell Scripting Tutorial for DevOps Engineers](https://www.youtube.com/watch?v=_-D6gkRj7xc&list=PLlfy9GnSVerQr-Se9JRE_tZJk3OUoHCkh&index=3)
