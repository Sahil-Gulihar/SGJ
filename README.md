README: Using a Bash Script as an Executable

This guide will walk you through the process of cloning a Git repository and moving a Bash script file to binary directories on your system.
Step 1: Clone the Git Repository

    Open a Terminal:
        On macOS and Linux: Use Terminal (you can find it in Applications -> Utilities).
        On Windows: Use Git Bash or another terminal emulator like PowerShell.

    Clone the Repository:

    bash

git clone [<repository_url>](https://github.com/Sahil-Gulihar/SGJ)



Navigate to the Repository Directory:

bash

    cd SGJ

    Replace SGJ with the name of the directory that was created when you cloned the repository.

Step 2: Move the Bash Script to Binary Directories

    Locate Your Bash Script:
        Navigate to the directory where your Bash script (sgj) is located. Typically, this will be within the cloned repository.

    Make the Script Executable:

    bash

chmod +x sgj

This command makes your Bash script executable.

Move the Script to a Binary Directory:

    Identify a suitable binary directory. Common choices include /usr/local/bin or /usr/bin.

bash

    sudo mv sgj /usr/local/bin

    You might need superuser (sudo) privileges to move files into system directories.

    Verify the Script is Accessible:
        Open a new terminal window or tab.
        Type sgj (or just your_script if you removed the .sh extension) and press Enter. The script should execute if it's in your system's PATH.

Step 3: Run the Script

    Execute the Script:
        Now that your script is in a binary directory, you can execute it from anywhere in your terminal:

sgj

