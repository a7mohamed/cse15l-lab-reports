# Hello, this is my blog for Lab 1.
Ok, so the first thing we were told to do was to download VSCODE using this link. After clicking the link and installing it, you should see a page that looks like this.
![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/Screenshot%202023-01-11%20124000.png)
Once you have that installed and you see this, the next thing you want to do is open up your terminal which is located on the top left of the screen, or you can press the keys CTRL + SHIFT + ` (Don't include the pluses).
While your terminal is open, you are going to want to connect to the remote server by using your course specific account for CSE 15L. To find your course specific account info, click this [link](http://sdacs.ucsd.edu/~icc/index.php).
Once you are connected to this link, find your account and change your password and remember it, because we will be using that password to sign into the remote server.
Once you have your account name and new password, type ssh yourusername@ieng6.ucsd.edu where "yourusername" is your course specific account name. It should look something like this when you've connected. 
![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/Terminal.png)
You might've noticed that the Password box remains empty even when you type, but you don't have to worry because it is meant to be like that. You also might have a lot more stuff pop up on your screen because it's your first time signing in, but that shouldn't be an issue either. The only thing that is an issue is when it keeps repeating to put in a password after you've entered it. When that happens, it's just the computer telling you that it hasn't noticed the password change yet, so wait 15-60 minutes and try again.
So, on to the next step. Now that we are successfully signed into the remote server, let's try running some commands. There are a list of commands that we could run. Some of them are: cd, ls -lat, pwd, cd ~, and more. Here are a few I tried:![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/Running%20Commands.png)
These commands that I wrote print out some useful information. For example, ls -a command printed out all of the files that were in remote server account. Pretty cool huh?

Now that we were successfully able to access the remote server and check that we were able to run some commands, that marks the end of the tutorial! I hope these instructions were clear and you were able to finish this with relative ease. Until next blog!
