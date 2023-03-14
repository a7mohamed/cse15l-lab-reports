# Hello, this is my blog for Lab Report 5.

For this lab, we get to choose a favorite lab report of ours and try to complete them in a different way. Personally, my favorite lab was lab report 3 because we were able to go a little deeper into on of the three commands we had learned then: grep, find and less. I chose to go deeper into the grep command, but this time, I want to go learn more about the find command.

So first off, let's go over one of the most noticeable find commands: "find <directory> -name <filename>". This command finds files in the specified directory with the 
given filename. Here's how it works:

![Image](https://raw.githubusercontents.com/a7mohamed/cse15l-lab-reports/main/FindCommand.png)

I've decided to look into the berlitz1/ file and search for any file that ends in .txt (which is what the *.txt means), and it found many files that end in .txt (it showed more but I only screenshotted a couple).

Next, let's look at another command that could be very useful: "find <directory> -print". This command prints the filenames of the files found by the find command. This option is used by default if no other action is specified. Here's how it works:

![Image](https://raw.githubusercontents.com/a7mohamed/cse15l-lab-reports/main/FindCommand2.png)
  
Notice how this command has almost exaclty the same output as the previous command (yet again I only screenshotted some files). However, you may notice something different with the very first file the -print command finds. It is simply berlitz1/. When I used -name *.txt, it only found files that ended in .txt, however -print gives me everything. If berlitz1/ had more that just .txt files, it would've been easier to see the differene between the two.
  
And lastly, let's look at a brand new command that we haven't seen or does something new. "find <directory> -newer <file>". This command finds files in the specified directory that are newer than the specified file. This option can be used to find all files that have been modified since a certain date or time. Before I explain how this command works, I need to explain its usefulness. Say for example you have a system crash. In case of a system crash or data loss, you can use this command to quickly identify the files that have been modified since the last backup and recover them. You will be able to tell which files have been changed or lost and will be able to act accordingly. Now, let's take a look: 
  
![Image](https://raw.githubusercontents.com/a7mohamed/cse15l-lab-reports/main/FindCommand3.png)
