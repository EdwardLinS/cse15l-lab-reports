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
