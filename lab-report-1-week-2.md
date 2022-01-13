# How to log into a course-specific account on `ieng6`

1. Installing VS Code

* First go to [Visual Studio Code](https://code.visualstudio.com/) and install the VSCode app

* Once installed you should see this when VSCode opens: 
![Image](Screenshot%20(22).png)



2. Remotely Connecting 

* If you are on Windows first install [OpenSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse)

* Next look up your course-specific account for CSE15L [here](https://sdacs.ucsd.edu/~icc/index.php)

* Now we will connect to the remote computer

* Open a new terminal in VSCode by clicking the terminal tab at the top left and click new terminal

* Enter the following command into the terminal `ssh cs15lwi22zz@ieng6.ucsd.edu` except replace the `zz` with the letters from your course-specific account that you looked up earlier. Then click yes to the prompt that is given to you, and once you enter your password you should be logged in! The whole process should look something like this: 

![Image](Screenshot%20(24).png)
![Image](Screenshot%20(23).png)

* The second screenshot is what will show up after you are logged in



3. Running some commands

* Now try running some commands in your terminal

* Try these ones out specifically: `cd~`, `cd`, `ls -lat`, `ls -a`, `ls <directory>` where the `<directory>` is `/home/linux/ieng6/cs15lwi22/cs15lwi22abc` and `abc` is one of the other members of your group's username, `cp /home/linux/ieng6/cs15lwi22/public/hello.txt ~/`

* note why the output was different for that last command

* here is what the output of those commands should look like

![Image](Screenshot%20(25).png)


4. Moving Files with `scp`

* `scp` is a command used to copy files from your computer to a remote computer

* You can type `scp <File name> cs15lwi22zz@ieng6.ucsd.edu:~/` where `<File name>` is whatever file you want to copy here is what it should look like in the terminal it will prompt you to enter your passowrd, once that is done you have successfully copied the file here is an example image: 

![Image](Screenshot%20(36).png)


5. SSH Keys

* For windows follow [these](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement#user-key-generation) steps first to set up a key

* Once you see a randomart image like this you'll know that you are done: 
![Image](Screenshot%20(33).png)

* Now you need to copy the public key to the `ssh` directory on your computer do thet by entering this command `mkdir .ssh`

* Now you should be able to log into your ssh without typing your password here is what that will look like

![Image](Screenshot%20(34).png)

* This will save you loads of time 

6. Optimizing Remote Running

* Here are some commands that can make working on a remote server easier 

* The up arrow can give you teh last command you ran, and you can click it many times to go further back and recall other commands you ran

* You can use semicolons to chain commands together

* You can also use quotations around a command to run the command on the remote server then exit

![Image](Screenshot%20(37).png)




