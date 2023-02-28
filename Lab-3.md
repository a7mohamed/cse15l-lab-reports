# Hello, this is my blog for Lab Report 3.
I will be showing some examples of ways you can use the grep command in the command line.
I will be writing my examples in my java terminal using bash.

When grep is executed, it searches for the specified pattern in each line of the input file or standard input. If a line matches the pattern, grep prints the line to standard output by default.

## For our first example, I will be showing you two examples of me using the command grep -c.
What grep -c does is that instead of returning the lines of the words grep finds, it return the how many times they were found. Here's an example of me using grep normally, and then grep -c after:


![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepCommand1%231.png)

As you can see, the word Oahu is found 2 times in my HandRHawaii.txt file. The grep command (with no extra option) returned the 2 lines were that word was found, while grep -c returned the **count** or the amount of times that word was found.

Here's another examples of using grep -c:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepCommand1%232.png)

Something you might notice differnetly here is that I have quotatins around "Las Vegas" in bash but I didn't have any in my previous example with "Oahu". All the quotations do is specify to bash that I'm looking for this term, so it wouldn't change if I used them on Oahu. However, if I tried taking off the quotations with Las Vegas, bash would give me an error saying it can't find a file or directory called Vegas:

![Image](https://raw.githubusercontent.com/a7mohamed/cse15l-lab-reports/main/GrepError1.png)

## For our second example, I will be showing you two examples of me using the command grep -i.

