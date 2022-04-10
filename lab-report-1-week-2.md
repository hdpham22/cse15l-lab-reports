# Week 2 Lab Report
## Step 1: Install VSCode
![](images/VSCode.png)
Go to https://code.visualstudio.com/ and install the latest version of VS Code. After you install ad open it, you should see something like this.
## Step 2: Remotely Connecting
![](images/Remote.png)
Install OpenSSH and [follow these steps](https://code.visualstudio.com/docs/remote/ssh#_connect-to-a-remote-host). Next, open a terminal and enter: <br>
**⤇ ssh cs15lsp22zz@ieng6.ucsd.edu**<br>
*remember to replace "zz" with letters in your course-specific account.<br>
Answer the following prompts with "yes" and then type in your password.<br>
## Step 3: Trying Some Commands 
![](images/Commands.png)
Experiment with some commands in the terminal. Here are a few that you can use: <br>
* cd ~
* cd
* ls -lat
* ls -a
* ls <directory> where <directory> is /home/linux/ieng6/cs15lsp22/cs15lsp22abc, where the abc is one of the other group members’ username
* cp /home/linux/ieng6/cs15lsp22/public/hello.txt ~/
* cat /home/linux/ieng6/cs15lsp22/public/hello.txt
## Step 4: Moving Files With scp
![](images/WhereAmI.png)
In order to move files with scp, you can use this command: <br>
scp filename.java cs15lsp22zz@ieng6.ucsd.edu:~/
*Again "zz" is replaced with letters specific to your course account
## Step 5: Setting an SSH Key:
![](images/SSH.png)
Build the key by entering this command: <br>
ssh-keygen<br>
You should see this:<br>
Generating public/private rsa key pair. <br>
Enter file in which to save the key (/Users/<user-name>/.ssh/id_rsa): /Users/<user-name>/.ssh/id_rsa<br>
Enter passphrase (empty for no passphrase): <br>
Do not enter a passphrase.<br> 
If you are working on a Windows device, follow [these extra steps](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement#user-key-generation)
Your terminal should look like this:
![](images/Success.png)
Next, we have to create the public key by entering the following inputs: <br>
ssh cs15lsp22zz@ieng6.ucsd.edu <br>
Enter Password<br>
now on server<br>
mkdir .ssh<br>
logout<br>
back on client<br>
$ scp /Users/<user-name>/.ssh/id_rsa.pub cs15lsp22zz@ieng6.ucsd.edu:~/.ssh/authorized_keys<br>
You use your username and the path you saw in the command above<br>
Now you can access the server without a passphrase
## Step 6: Optimizing Remote Running:
You can use the following tips in order to optimize run time:
* using the up arrow key
* copying and pasting commands
* using quotes at the end of ssh commands
* using semicolons inbetween commands
![](images/Optimize.png)