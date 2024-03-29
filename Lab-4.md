# Hello, this is my blog for Lab Report 4.
I'm going to go over my exact process on completing the Week 7 lab's 10 step process, but I will only document what I press from steps 4 to 9. Let's go!

Step 4 tells me to log into ieng6, so that's what I'll do first. This is what I typed into the terminal: ***ssh cs15lwi23ako@ieng6.ucsd.edu*** and this was its output:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/SSHLogin.png)


Step 5 tells me to clone my fork of the repository from your Github account, so I went to the lab 7 repository [link](https://github.com/ucsd-cse15l-w23/lab7) and clicked the fork button on the top right. Once it was forked, I cloned it in my terminal. I typed exactly this into my terminal: *git clone* and then I copied and pasted this portion of the code from the link from the green Code button *https://github.com/a7mohamed/lab7.git* and this was the output: 

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GitClone.png)

The reason why this response is here is because I had already cloned this repository, so the terminal lets me know this by printing out this message. This doesn't mess up the code in any way, it's just letting me know that this action has already been done before.

Step 6 tells me to run the tests, demonstrating that they fail. In order to run the code, I have to go back to week 3 and find copy and paste the javac and java commands. But before I did that, I had to correctly be in the right directly. This is what I typed in my terminal: __ls, cd la (it was here that I pressed tab and it autocompleted to lab7/)__, then my copied javac command ___javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java___, and then my copied java command ___java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore___ with an additional ___TestListExamples___ that I typed at the end because that's what we want to run. My output looked like this:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/TestListExamples.png)

Step 7 asks me to edit the code file to fix the failing test. After looking at the ListExamples file, I realized that the last while loop was causing the error. index1 had been incrementing on line 43 when it should have been index2 because index2 keeps track of list2's size. 

For Step 8, I fixed the error and my code worked, however, my system wasn't showing me the tests passing for some reason, so the best I could do is show a screenshot of my JUnit tests passing. Sorry:(

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/JUnitTestsPassed.png)

And lastly for step 9, all I need to do is push the changes to my Github account. Luckily for me, I opened the code using my Github desktop and commiting changes is really easy from there. I opened up my github desktop browser and pressed the "commit to main" button on the bottom left, then pressed "push to origin". Here are all the changes I made (it was only one number):

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GithubDesktopIndex.png)

Now when we go to my forked Lab 7 repository and look into the ListExamples.java file, we can see that it's been updated:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/FixedIndex.png)

So these are the steps that I took in order to complete this lab. In short, I made a fork of the repo, made some changes to it, and saved those changes. Hope you liked it. See you next blog!
