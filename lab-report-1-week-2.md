#Remote Access

##What are the steps needed to connect to a remote server optimally?

**Step 1: Installing VSCode**

You need an editor or IDE (Integrated Development Environment) in order to create and run programs as well as connect to a remote server. In my personal opinion, the best one is VSCode. Here is what you need to do to install it.

Go to [Download VSCode](https://code.visualstudio.com/) and download VSCode for your specific operating system. It covers all three major OS's For Chromebook and tablets, you will need to inform your lab leader for additional information.

When done, it should look like this. Mine is on Mac OS and hence might look different on your screen if you're using a different OS.

![VScode](Vscode.png)

**Step 2: Remotely Connecting**

Now that we have an IDE to work, let's do the thing we came here to do: Remote Connecting to a server. This act is done everywhere from different CSE classes which  to even your future job, thus this is an important skill to learn.

If you're on Windows, bad luck, you need to install OpenSSH which allows you to remote connect to other computers and servers. 
Click to go to the site [OpenSSH Instructions](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse)

Aditionally you will need to find your course specific account using this site: [Course Login Details](https://sdacs.ucsd.edu/~icc/index.php)
If this is your first time using the UCSD server, you will need to change/create your password. How to do that is through above link.

Once you are ready, open up VSCode and access the terminal.

Now that we are ready to go, here are the pieces of code you will need to write to connect to the server.

1. `ssh cs15lwi22zz@ieng6.ucsd.edu` (replace the zz with the three letters you find in your own login details, refer above for more details)
2. If it's your first time accessing the server, you will get a message. There is no need to worry, just enter yes. 
```
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])? 

```
3. After you enter yes and your password, this message will pop up and you would have successfully connected to the remote server.

![Final Message](RemoteConnecting.png)

**Step 3: Trying some Commands

Now that we have connected to the server, let's try out some simple commands. 
There are hundereds of commands we could try but for now, we are going to use four of them 
`ls` - Informs you of the files in your directory.
`ls -lat` - Gives you a detailed description of the files in your directory including dates, types, names etc.
`cd` - changes directory to your home directory. You wouldn't see anything change and that is because you're already in your home directory.
`cd ~` - reverts back to the general directory, again no change is seen because you're in your general directory. Is more applicable in later stages of the course.

Here is what this commands should look like when executed.



Type `exit` to exit the server and return back to your laptop.
