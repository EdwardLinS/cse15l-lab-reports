# Part 1
Code

```java
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    String output = "";
    
    public String handleRequest(URI url) {
        if (url.getPath().contains("/add-message")) {
            String message = url.getQuery().split("=")[1];
            output += message + '\n';

            return output;
        } else if (output.equals("")) {
            return "Input a message";
        } else {
            return "404 NOT FOUND!";
        }
    }
}

class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```

![image](https://user-images.githubusercontent.com/63514282/214727849-ab22d6cd-d131-4497-b7ed-30413cc89f4c.png)
- **Methods:** handleRequest and main
- **Arguments/Values:** 
  - args = `[4000]`
  -  url = `"http://localhost:4000/add-message?s=Hello"` 
- **Fields:** 
  - port = `4000`
  - message = `"Hello"`
  - output = `"Hello\n"`
  


![image](https://user-images.githubusercontent.com/63514282/214728423-a1f2d657-cd13-4a9d-84d9-33931dbeabf6.png)
- **Methods:** handleRequest and main
- **Arguments/Values:** 
  - args = `[4000]`
  -  url = `"http://localhost:4000/add-message?s=How are you"`
- **Fields:** 
  - port = `4000`
  - message = `"How are you"`
  - output = `"Hello\nHow are you\n"`

- **Changes**
    - _url_ changes to whatever the user types 
    - _message_ changes to match String in query
    - _output_ changes to add message and a new line 

# Part 2

**Failure Inducing Test**
```java
@Test
  public void testReverseInPlace2() {
    int[] input1 = {1,2};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{2,1}, input1);
  }
 ```
 
**Non-Failure Inducing Tests**
```java
 @Test 
	public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
	}

  @Test
  public void testReverseInPlace1() {
    int[] input1 = { };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ }, input1);
	}
```
 
 **Symptoms**
 
<img width="2620" alt="image" src="https://user-images.githubusercontent.com/63514282/215261504-c0e2819c-ccfa-4ac5-8605-439804b334d5.png">

 **Before / After**
 
 _Before:_
 ```java
 static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
 ```
 
 _After:_
 ```java
 static void reverseInPlace(int[] arr) {
    int[] arrClone = arr.clone();
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arrClone[arr.length - i - 1];
    }
  }
 ```
 
 _Explaination:_
Before, the code wasn't storing the elements of the array before the changes so a lot of elements were replaced incorectly. For example, `[1, 2]` would become `[2, 2]` since the 1 was never stored and was replaced by 2. Thus, a solution would be to create a clone of the list that contains the original elements then replace `arr` elements with elements from the clone. 

# Part 3

I learned how to create a web server that used the url to receive inputs. From these inputs, I could use conditionals to check for certain things in the path and query. Then, I would be able to display certain things based on what the conditionals got.
