
# Steps

## Setup

MAYBE ADD THE DELETE REPO THING HERE

1. Fork this [repository](https://github.com/ucsd-cse15l-w23/lab7) 

## Tasks

### 1. Log into the ieng6 remote server
  - `ssh cs15lwi23<last three letters of username>@ieng6.ucsd.edu` `<enter>`
  - <img width="635" alt="image" src="https://user-images.githubusercontent.com/63514282/221264856-59af94fb-6513-40c8-a19e-33fa22398495.png">
    
    - *It may not look exactly like this but as long as it doesn't prompt for the password again, login is successful.*
### 2. Clone your forked repository
  - `git clone <forked repository link>` `<enter>`
    - The forked repository link can be found by clicking the green `<> Code` button and copying the https link or ssh link if you have set up ssh
  - git clone with https
    - <img width="930" alt="image" src="https://user-images.githubusercontent.com/63514282/221383951-a608a4b8-c701-4893-a145-53a2ff02efd6.png">
  - git clone with ssh 
    - <img width="884" alt="image" src="https://user-images.githubusercontent.com/63514282/221383927-a5eaf476-a163-4435-bdc1-9b39ab4f15e8.png">
### 3. Change directories into lab7
  - `cd lab7` `<enter>`
    - <img width="466" alt="image" src="https://user-images.githubusercontent.com/63514282/221383965-523d7c86-82e3-4163-a1dd-9fa80c78e135.png">
### 4. Run the tests
  - `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` `<enter>`
  - `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` `<enter>
    - <img width="1590" alt="image" src="https://user-images.githubusercontent.com/63514282/221384047-bcc19db5-0652-4419-9c66-9cf6800eafaa.png">
### 5. Fix bug in ListExamples file
  - `nano ListExamples.java` `<enter>`
    - <img width="671" alt="image" src="https://user-images.githubusercontent.com/63514282/221384233-c485a768-4308-46d8-9352-22f53fdeb2c3.png">
    - <img width="1585" alt="image" src="https://user-images.githubusercontent.com/63514282/221384244-a40b0304-0c27-4555-8edb-9f1719d6ddee.png">

  - Navigate to bug
    - `alt` + `/`
      - Jumps to bottom of the file
      - <img width="915" alt="image" src="https://user-images.githubusercontent.com/63514282/221384277-9f1aae44-bd67-4f8c-8b4b-c40f4d61bc15.png">

    - `<up> <up> <up> <up> <up> <up> <up> <right> <right> <right> <right> <right> <right> <right> <right> <right> <right> <right>`
      - <img width="885" alt="image" src="https://user-images.githubusercontent.com/63514282/221384350-415fe637-0820-4e81-af21-3f2071b67a94.png">
  

  - Delete the bug and replace it with the correct variable
    - `<delete>`


  

