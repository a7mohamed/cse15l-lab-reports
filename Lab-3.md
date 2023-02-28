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
Now, for me personally, grep -v is my favortie grep command because of how weird it is. It is essentially the opposite of the grep command. Grep -v returns the lines that **don't** contain the word/s that you are looking for. Look at this example:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepCommand3%231.png)
