Tutorial on how to log into course-specific account on ieng6

* Install VSCode
* Remotely Connection
* Trying Some Commands

# **Logging Onto Course-Specific Account on ieng6**

---

## 1. Install Visual Studio Code (VSCode)

  * **Go to the [Visual Studio Code](https://code.visualstudio.com) website** 
  * **Download** the version of Visual Studio Code that matches your operating system *(eg. macOS for Mac, Windows for PCs)*
  * After installing, **click on the Visual Studio Code icon** to open a window that should look like this: 
<img width="1920" alt="vscode-starting-screen" src="https://user-images.githubusercontent.com/63514282/212158296-f69a178e-cdcb-49ed-9b53-c601281b6f7b.png">

*(**Tip**: If the colors or other icons don't look exactly like this, don't worry! Those are just a difference in settings and operating systems)*

## 2. Remotely Connecting

* *Install Git and Setting Up Git Bash (Only For Windows Users)*
  * **Go to the [Git for Windows](https://gitforwindows.org) website and click download**
  * Open Visual Studio Code 
  * Press and hold `Ctrl` + `` ` `` to open up the terminal
  <img width="1869" alt="image" src="https://user-images.githubusercontent.com/63514282/212164612-267ce18b-1c05-4e57-a0f0-f87de9dd4ffb.png">
  
  * Press and hold `Ctrl` + `Shift` + `P` to open up the command palette
  * Type and enter: `Select Default Profile` 
<img width="837" alt="image" src="https://user-images.githubusercontent.com/63514282/212164960-6a5c416c-1ec3-4b30-87da-9d609168689c.png">

  * Select Git Bash from the drop down 
  * Click the `+` icon on the right side of the terminal window
  <img width="333" alt="image" src="https://user-images.githubusercontent.com/63514282/212165734-5186bc2f-2457-4c53-8bf3-8847abea1eba.png">

* *Connecting to the Remote Server*
  * Go [here](https://sdacs.ucsd.edu/~icc/index.php) to locate your 15L username, which is highlighted in gray under Additional Accounts *(Tip: It starts with cs15lwi23)* 
  * In the git bash terminal, type `ssh <your 15L username>@ieng6.ucsd.edu` and enter
  * It should then prompt for password, where you will type your account password *(Tip: It will not show anything when you type your password. This is normal. If you type your password incorrectly, it will prompt again after.)*
  ![image](https://user-images.githubusercontent.com/63514282/212255673-1dc38c3c-6b83-4241-81c3-388704c8272b.png)
  
  * If it asks *Are you sure you want to continue connecting*, type yes.
  * After the terminal shows something similar to the image below, you are done!
  <img width="412" alt="image" src="https://user-images.githubusercontent.com/63514282/212255974-46162b0f-7439-49a1-9f94-75eb88c30af3.png">
  
## 3. Try Out Some Commands
 * Here are some commands to use to explore the new remote server's directories
  * *pwd*: Prints the current working directory
  * *cd*: Changes directory to whatever is specified after
   * *cd ~*: Changes directory to the home directory
  * *ls -a*: lists all files in current working directory
  * *cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/*: copies hello.text to home directory
  * *cat /home/linux/ieng6/cs15lwi23/public/hello.txt*: prints the content of hello.text 
![image](https://user-images.githubusercontent.com/63514282/212258834-27f0cfac-15b4-4d64-858e-d49714ab123d.png)
*An example of using these commands together*

 * To log out, type `Ctrl` + `D` in the terminal then type `exit`

## Congratulations! You've finished!


  
  
