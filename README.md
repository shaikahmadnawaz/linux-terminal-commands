# Linux & Terminal Commands

### What is Linux?

Linux is an operating system's kernel. You might have heard of UNIX. Well, Linux is a UNIX clone. But it was actually created by Linus Torvalds from Scratch. Linux is free and open-source, that means that you can simply change anything in Linux and redistribute it in your own name! There are several Linux Distributions.

- Ubuntu Linux
- Red Hat Enterprise Linux
- Linux Mint
- Debian
- Fedora

Linux is Mainly used in servers. About 90% of the internet is powered by Linux servers. This is because Linux is fast, secure, and free! The main problem of using Windows servers are their cost. This is solved by using Linux servers. The OS that runs in about 80% of the smartphones in the world, Android, is also made from the Linux kernel. Most of the viruses in the world run on Windows, but not on Linux!

### What Is a Linux Command?

A Linux command is a program or utility that runs on the CLI – a console that interacts with the system via texts and processes. It’s similar to the Command Prompt application in Windows.

Linux commands are executed on Terminal by pressing Enter at the end of the line. You can run commands to perform various tasks, from package installation to user management and file manipulation.

Here’s what a Linux command’s general syntax looks like:

**CommandName [option(s)] [parameter(s)]**

A command may contain an option or a parameter. In some cases, it can still run without them. These are the three most common parts of a command:

- **CommandName** is the rule that you want to perform.
- **Option** or **flag** modifies a command’s operation. To invoke it, use hyphens (–) or double hyphens (—).
- **Parameter** or **argument** specifies any necessary information for the command.

**Keep in mind that all Linux commands are case-sensitive.**

### 1. ls

In the current folder, if you want to list the all the items you can use **ls command**

`ls`

To see other directories content, type ls followed by the desired path. For example, to view files in the Documents folder, enter:

`ls /home/username/Documents`

Here are some options you can use with the ls command:

- `ls -R` lists all the files in the subdirectories.
- `ls -a` shows hidden files in addition to the visible ones.
- `ls -lh` shows the file sizes in easily readable formats, such as MB, GB, and TB.

### 2. mkdir

**mkdir command** is used to create a directory

`mkdir dirname`

**-p** or **–parents** create a directory between two existing folders. For example, `mkdir -p Music/2020/Songs` will make the new “2020” directory.

### 3. cd

To navigate through the directories, use the **cd command.**

`cd dirname`

Here are some shortcuts to help you navigate:

- `cd ~[username]` goes to another user’s home directory.
- `cd ..` moves one directory up (move back).

### 4. pwd

Use the pwd command to find the path of your current working directory. Simply entering pwd will return the full current path.

`pwd`

### 5. cat

Concatenate, or **cat**, is one of the most frequently used Linux commands. It lists, combines, and writes file content to the standard output. To run the **cat** command, type cat followed by the file name and its extension.

`cat filename.txt`

Here are other ways to use the **cat** command:

- `cat > filename.txt` creates a new file.
- `cat filename1.txt filename2.txt > filename3.txt` merges **filename1.txt** and **filename2.txt** and stores the output in **filename3.txt**.
- `tac filename.txt` displays content in reverse order.

### 6. man

The **man** command provides a user manual of any commands or utilities you can run in Terminal, including the name, description, and options.

It consists of nine sections:

- Executable programs or shell commands
- System calls
- Library calls
- Games
- Special files
- File formats and conventions
- System administration commands
- Kernel routines
- Miscellaneous
- To display the complete manual, enter:

`man [command_name]`

For example, you want to access the manual for the ls command:

`man ls`

### 7. tr

**tr** is used to translate like lower to upper case vice versa.

`cat old.txt | tr a-z A-Z > new.txt`

### 8. touch

The **touch command** allows you to create an empty file

`touch Web.html`

### 9. cp

Use the **cp** command to copy files or directories and their content.

`cp file.txt copy.txt`

To copy an entire directory, pass the **-R** flag before typing the source directory, followed by the destination directory:

`cp -R /home/username/Documents /home/username/Documents_backup`

### 10. mv

The primary use of the **mv command** is to move and rename files and directories. Additionally, it doesn’t produce an output upon execution.

Simply type **mv** followed by the filename and the destination directory. For example, you want to move filename.txt to the /home/username/Documents directory:

`mv filename.txt /home/username/Documents`.

You can also use the mv command to rename a file:

`mv old_filename.txt new_filename.txt`

### 11. rm

The **rm** command is used to delete files within a directory. Make sure that the user performing this command has write permissions.

Remember the directory’s location as this will remove the file(s) and you can’t undo it.

Here’s the general syntax:

`rm filename`

To remove multiple files, enter the following command:

`rm filename1 filename2 filename3`

Here are some acceptable options you can add:

- `-i` prompts system confirmation before deleting a file.
- `-f` allows the system to remove without a confirmation.
- `-r` deletes files and directories recursively.

### 12. sudo

Short for superuser do, **sudo** is one of the most popular basic Linux commands that lets you perform tasks that require administrative or root permissions.

When using sudo, the system will prompt users to authenticate themselves with a password. Then, the Linux system will log a timestamp as a tracker. By default, every root user can run sudo commands for **15 minutes/session**.

If you try to run sudo in the command line without authenticating yourself, the system will log the activity as a security event.

`sudo`

You can also add an option, such as:

- **-k** or **–reset-timestamp** invalidates the timestamp file.
- **-g** or **–group=group** runs commands as a specified group name or ID.
- **-h** or **–host=host** runs commands on the host.
