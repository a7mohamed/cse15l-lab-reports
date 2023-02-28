# Hello, this is my blog for Lab Report 3.
I will be showing some examples of ways you can use the grep command in the command line.
I will be writing my examples in my java terminal using bash.

When grep is executed, it searches for the specified pattern in each line of the input file or standard input. If a line matches the pattern, grep prints the line to standard output by default.

## For our first example, I will be showing you two examples of the command grep -c.
What grep -c does is that instead of returning the lines of the words grep finds, it return the how many times they were found. Here's an example of me using grep normally, and then grep -c after:


![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepCommand1%231.png)

As you can see, the word Oahu is found 2 times in my HandRHawaii.txt file. The grep command (with no extra option) returned the 2 lines were that word was found, while grep -c returned the **count** or the amount of times that word was found.

Here's another examples of using grep -c:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepCommand1%232.png)

Something you might notice differnetly here is that I have quotatins around "Las Vegas" in bash but I didn't have any in my previous example with "Oahu". All the quotations do is specify to bash that I'm looking for this term, so it wouldn't change if I used them on Oahu. However, if I tried taking off the quotations with Las Vegas, bash would give me an error saying it can't find a file or directory called Vegas:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepError1.png)

## For our second example, I will be showing you two examples of the command grep -i.
What grep -i does is that it essentially doesn't care about case sensitivity and grabs the word however it is written (whether it has uppercases or lowercases, it doesn't matter!). Here's a quick look at how it works:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepCommand2%231.png)

You see how for the first option, I look specifically for the word "Hotels" and I only get back one line of code, but when I try using grep -i, I see that the word hotel is used 3 other times! Only the first instance of hotel started with a capital H while the others began with a lowercase h. Let's see another example of grep -i:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepCommand2%232.png)

I did this example vice versa from the previous one by showing you that you can start the search with a lowercase letter and still find that word with capitals in it with grep -i. Pretty neat, huh?

## For our third example, I will be showing you two examples of the command grep -v.
Now, for me personally, grep -v is my favorite grep command because of how weird it is. It is essentially the opposite of the grep command. Grep -v returns the lines that **don't** contain the word/s that you are looking for. Look at this example:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepCommand3%231.png)

There are a total of 16 lines in HandRIstanbul.txt. Four of those lines have the word the, while the other twelve do not, as you can see by the result. Grep -v is also known as the inverse grep. Let's look at another example shall we:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepCommand3%232.png)

In this example, I tried searching for a word that wasn't in my HandRLisbon.txt file, and of course, when I ran the grep command, nothing was printed out. However, when I ran grep -v with the same word, the entire file was printed out. That's because the word "hello" is nowhere to be found in that file.

## For our fourth example, I will be showing you two examples of the command grep -l.

And for our last command, I chose grep -l. It seems like the most useful command to use and it's pretty simple to understand. What grep -l does is it returns the names of the files that contains the word/s you give to it. Let's see which txt files have the word "bedroom" in them:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepCommand4%231.png)

Wow! These are all the files that contain the word "bedroom" and the other files don't have that word at all. This could be pretty useful when your looking for a file that talks about a specific thing, so you could just grep -l it and find the important files you need. Let's try it again:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepCommand4%232.png)

I think I know where to start looking if I'm interested in dessert! This is just one of the few ways that grep -l can help you pinpoint and find specific entries that have the information you need.

There were many more grep commands to choose from, but these were the 4 that I found the most interesting or the most useful. Hopefully, you did too. See you next blog!

PS: All of my grep commands came from this [link.](https://phoenixnap.com/kb/grep-command-linux-unix-examples)
