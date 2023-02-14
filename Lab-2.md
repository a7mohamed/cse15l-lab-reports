# Hello, this is my blog for Lab Report 2.
**So the first part of this Lab Report** asks us to write a webserver called StringServer that keeps track of a single string that gets added to by incoming requests. My code looks like this:

![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/ImportsStringServer.png)
![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/StringServerCode.png)
When you type in mulitple strings, they should be printed on separate lines. It should look like this:
![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/LocalHostOneItem.png)
![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/LocalHostTwoItems.png)


Now, here are some questions that will clarify a few questions pertaining to the screenshots.

1. Which methods in your code are called?
In the duration of this code running, many methods are called. We can see methods like getPath() and getQuery() which are built in java commands that come from the imported file java.net.URI. I had also written a method called handleRequest which takes a url and adds words to a list when the path is equal to add-message?s=(string) where (string) is any string word of your choosing.

2. What are the relevant arguments to those methods, and the values of any relevant fields of the class?
For the handleRequest method, it takes in a url as an argument. That url represents the link that I used to make my lists of words. Methods like getPath() and getQuery() also require a url as an argument. They are methods of the class java.net.URI, and are used to retrieve the path and query components of a URI, respectively.

3. How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.
The values are all turned into strings and are added on to the list. For example, when I add to the url /add-message?s=140, the number 140 is added onto the list, however, because of my split method, each object is taken in as a string.

**Now, for the part 2 of this Lab Report,** I get to choose a bug from lab 3 and have to answer 4 questions:

1. A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown).

In my ArrayTests.java, my reverse methods were failing. This was one of the failure-inducing inputs:
```
  @Test
  public void testReverseInPlace2(){
    int[] input2 = {1, 2, 3};
    ArrayExamples.reverseInPlace(input2); 
    //What I actually expect: {3, 2, 1}
    //What I actually get : {2, 2, 2}
    assertArrayEquals(new int[]{3, 2, 1}, input2);
  }
  ```
2. An input that doesn’t induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown).
```
  @Test 
  public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
  }
```
3. The symptom, as the output of running the tests (provide it as a screenshot of running JUnit with at least the two inputs above).

Here is a symptom from the first question:

![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/Input1Lab2.png)
![Image](https://github.com/a7mohamed/cse15l-lab-reports/blob/main/Input2Lab2.png)

4. The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown).

Before:
```
// Changes the input array to be in reversed order
  static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[(arr.length - i - 1)/2];
    }
  }
```
After:
```
// Changes the input array to be in reversed order
  static void reverseInPlace(int[] arr) {
    for( int i = 0; i < arr.length/2; i +=1){
      int temp = arr[i];
      arr[i] = arr[arr.length-i-1];
      arr[arr.length - i -1] = temp;
    }
  }
```
What the fixed after code does differently is that it copies the values of the array into a temp integer and it copies the values into the array ```arr``` backwards.

**And finally, for part 3 of the Lab Report,** I need to describe something that I have learned in the week 2 or week 3 lab. 

I feel like something crucial I have learned in those weeks is the process of debugging. Ever since I started coding, I have come across so many simple errors that I thought were impossible to overcome at the time, and ever single time after I was able to get finally get the answer, I was ashamed at how long it took me to find out.

I have learned that debugging requires patience and calculated moves; I can't just change a random piece of code and hope for the best, I need to remind myself what the code is meant to accomplish, maybe look at what some methods do again, refamiliarize myself with the code, and always stay hopeful because debugging with a negative attitude will make it harder to get the work done. 

Welp, that's it from me this week. Until next time!

