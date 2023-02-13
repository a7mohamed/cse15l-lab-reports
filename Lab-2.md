# Hello, this is my blog for Lab Report 2.
So the first part of this Lab Report asks us to write a webserver called StringServer that keeps track of a single string that gets added to by incoming requests. My code looks like this:
![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/ImportsStringServer.png)
![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/StringServerCode.png)
When you type in mulitple strings, they should be printed on separate lines. It should look like this:
![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/LocalHostOneItem.png)
![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/LocalHostTwoItems.png)


Now, here are some questions that will clarify a few questions pertaining to the code.

Which methods in your code are called?
In the duration of this code running, many methods are called. We can see methods like getPath() and getQuery() which are built in java commands that come from the imported file java.net.URI. I had also written a method called handleRequest which takes a url and adds words to a list when the path is equal to add-message?s=<string> where <string> is any string word of your choosing.

What are the relevant arguments to those methods, and the values of any relevant fields of the class?
For the handleRequest method, it takes in a url as an argument. That url represents the link that I used to make my lists of words.
How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

 
