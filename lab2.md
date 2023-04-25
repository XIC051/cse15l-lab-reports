# Part 1
* code for StringServer: 
![Image](code.png)
* screenshot of using 
![Image](hello.png)
```
/add-message?s=Hello
```
Which methods in your code are called?
* The **main method** of the StringServer class is called with the command-line arguments 4000
* After the client sends an request to the URL  http://localhost:8080/add-message?s=Hello, the handleRequest method of the StringHandler class is called with the requested URL as input

What are the relevant arguments to those methods, and the values of any relevant fields of the class?
* the URI argument: http://localhost:8080/add-message?s=Hello
* Relevant field: message field in StringHandler class
  * initial value of message field: ""
  * updated value of message field: "\nHello"
* newString value: "Hello"

How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.
* The message field changes from empty string to "\nHello" 

* screenshot of using 
![Image](how_are_you.png)
```
/add-message?s=How are you
```
Which methods in your code are called?
* The **main method** of the StringServer class is called with the command-line arguments 4000
* After the client sends an request to the URL http://localhost:4000/add-message?s=How%20are%20you, the handleRequest method of the StringHandler class is called with the requested URL as input

What are the relevant arguments to those methods, and the values of any relevant fields of the class?
* the URI argument: http://localhost:4000/add-message?s=How%20are%20you
* Relevant field: message field in StringHandler class
  * initial value of message field: "\nHello"
  * updated value of message field: "\nHello\nHow are you"
* newString value: "How are you"

How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.
* The message field changes from "\nHello" to "\nHello\nHow are you"


# Part 2

```
import static org.junit.Assert.*;
import org.junit.*;
public class ArrayTests {
   @Test 
   public void averageWithoutLowestTestFailure() { 
      double[] input1 = {1.0, 1.0, 1.0, 1.0};
      assertEquals(1/3, ArrayExamples.averageWithoutLowest(input1), 0.1);
   }
```

```
import static org.junit.Assert.*;
import org.junit.*;
public class ArrayTests {
   @Test 
   public void averageWithoutLowestTestSuccess() { 
      double[] input1 = {1.0, 2.0, 3.0, 4.0};
      assertEquals(3.0, ArrayExamples.averageWithoutLowest(input1), 0.1);
   }
```
* running the test
![Image](failture.png)
![Image](success.png)

* the bug
  * before
  ```
  double sum = 0;
  for(double num: arr) {
      if(num != lowest) { sum += num; }
    }
    return sum / (arr.length - 1);
  ```
  * after 
   ```
    double sum = 0;
    int counter = 0;
    int len = arr.length;
    for(double num: arr) {
      if(num == lowest) { 
        counter++;
      }
    }
    for(double num: arr) { 
      sum += num;
    }
    sum -= lowest;
    len--;
    return sum / (arr.length - 1);
   ```
  * explanations:
    * By adding a counter, 

# Part 3
From week 2 and 3, the biggest thing I learned is to create a web server. 

