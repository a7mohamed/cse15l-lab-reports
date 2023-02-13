# Hello, this is my blog for Lab Report 2.
So the first part of this Lab Report asks us to write a webserver called StringServer that keeps track of a single string that gets added to by incoming requests. My code looks like this:

![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/ImportsStringServer.png)
![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/StringServerCode.png)
When you type in mulitple strings, they should be printed on separate lines. It should look like this:
![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/LocalHostOneItem.png)
![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/LocalHostTwoItems.png)


Now, here are some questions that will clarify a few questions pertaining to the code.

Which methods in your code are called?
In the duration of this code running, many methods are called. We can see methods like getPath() and getQuery() which are built in java commands that come from the imported file java.net.URI. I had also written a method called handleRequest which takes a url and adds words to a list when the path is equal to add-message?s=(string) where (string) is any string word of your choosing.

What are the relevant arguments to those methods, and the values of any relevant fields of the class?
For the handleRequest method, it takes in a url as an argument. That url represents the link that I used to make my lists of words. Methods like getPath() and getQuery() also require a url as an argument and takes the parts of the url that they need (the path and the query) and put them into strings.

How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.
What does this even mean? I can try answering it right now, OR i can go to 11am-1pm office hours in B270A

Now, for the second part of this Lab Report asks us to choose a bug from lab 3 and show us these 4 things:

A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown)

An input that doesn’t induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown)

The symptom, as the output of running the tests (provide it as a screenshot of running JUnit with at least the two inputs above)

The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown)
 
