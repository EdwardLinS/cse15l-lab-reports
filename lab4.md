# Lab 4 Steps

## Setup

### 1. Delete previous lab7 repositories (only if there is any)
- Go to settings in your old lab7 fork repository
  - <img width="1835" alt="image" src="https://user-images.githubusercontent.com/63514282/221434590-7834efb5-6fa4-44e6-beda-d8cc479ba4bb.png">
- Scroll all the way down the page
  - <img width="1772" alt="image" src="https://user-images.githubusercontent.com/63514282/221434651-497e931c-cc52-4965-a46b-102c4ab5d718.png">
- Click the `Delete this repository` button 
  - Type what the instructions say then hit `<enter>` or the button that says `I understand the consequences, please delete this repository` 
    - <img width="586" alt="image" src="https://user-images.githubusercontent.com/63514282/221434840-d666a342-6c4f-493b-8fb0-007744802150.png">

### 2. Fork repository
- Go to this [repository](https://github.com/ucsd-cse15l-w23/lab7) 
- Click the `Fork` button at the top right
  - <img width="1848" alt="image" src="https://user-images.githubusercontent.com/63514282/221434087-ac29b9b9-71ad-4153-ac54-255f8807b096.png">
- Click the green `Create fork` button at the bottom
  - <img width="1843" alt="image" src="https://user-images.githubusercontent.com/63514282/221434171-67288da8-c170-40b4-8a75-4c940056fb8c.png">

## Tasks

### 3. Log into the ieng6 remote server
  - `ssh cs15lwi23<last three letters of username>@ieng6.ucsd.edu` `<enter>`
  - <img width="635" alt="image" src="https://user-images.githubusercontent.com/63514282/221264856-59af94fb-6513-40c8-a19e-33fa22398495.png">
    
    - *It may not look exactly like this but as long as it says successfully logged in it is correct.*

### 4. Clone your forked repository
  - `git clone <forked repository link>` `<enter>`
    - The forked repository link can be found by clicking the green `<> Code` button and copying the https link or ssh link if you have set up ssh
  - git clone with https
    - <img width="930" alt="image" src="https://user-images.githubusercontent.com/63514282/221383951-a608a4b8-c701-4893-a145-53a2ff02efd6.png">
  - git clone with ssh 
    - <img width="884" alt="image" src="https://user-images.githubusercontent.com/63514282/221383927-a5eaf476-a163-4435-bdc1-9b39ab4f15e8.png">

### 5. Change directories into lab7
  - `cd lab7` `<enter>`
    - <img width="466" alt="image" src="https://user-images.githubusercontent.com/63514282/221383965-523d7c86-82e3-4163-a1dd-9fa80c78e135.png">

### 6. Run the tests
  - `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` `<enter>`
  - `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` `<enter>`
    - <img width="1590" alt="image" src="https://user-images.githubusercontent.com/63514282/221384047-bcc19db5-0652-4419-9c66-9cf6800eafaa.png">
    
### 7. Fix bug in ListExamples file
  - `nano ListExamples.java` `<enter>`
    - <img width="671" alt="image" src="https://user-images.githubusercontent.com/63514282/221384233-c485a768-4308-46d8-9352-22f53fdeb2c3.png">
    - <img width="1585" alt="image" src="https://user-images.githubusercontent.com/63514282/221384244-a40b0304-0c27-4555-8edb-9f1719d6ddee.png">

  - Navigate to bug
    - `alt` + `/`
      - Jumps to bottom of the file
      - <img width="915" alt="image" src="https://user-images.githubusercontent.com/63514282/221384277-9f1aae44-bd67-4f8c-8b4b-c40f4d61bc15.png">

    - `<up><up><up><up><up><up><up><right><right><right><right><right><right><right><right><right><right><right>`
      - <img width="885" alt="image" src="https://user-images.githubusercontent.com/63514282/221384350-415fe637-0820-4e81-af21-3f2071b67a94.png">
  
  - Delete the bug and replace it with the correct variable
    - `<delete>` `2`
    - <img width="881" alt="image" src="https://user-images.githubusercontent.com/63514282/221432010-82012222-63d3-47a9-a3e4-12bf118ab19b.png">
  - Save file and exit
    - `ctrl` + `o` 
      - save file changes 
    - `<enter>`
      - confirm file name 
    - <img width="904" alt="image" src="https://user-images.githubusercontent.com/63514282/221432551-5eeb5ac6-eab6-45ba-9f64-007eb1114977.png"> 
    - `ctrl` + `x` 
      - close nano 
    

### 8. Run Tests Again
- `ctrl` + `r` `javac` `<enter>`
  - brings up past compile call
  - <img width="1071" alt="image" src="https://user-images.githubusercontent.com/63514282/221433448-40bde553-9c08-4e41-95fa-6cfab09c7800.png">
- `ctrl` + `r` `java<space>` `<enter>`
  - brings up past java run call 
  - <img width="1497" alt="image" src="https://user-images.githubusercontent.com/63514282/221433618-07e29644-342c-404c-95f4-f25b1b3b22cc.png">
- <img width="1583" alt="image" src="https://user-images.githubusercontent.com/63514282/221433628-2213cba2-9779-4369-b109-c7a301e13c55.png">

### 9. Add, Commit, Push Changes
- `git add ListExamples.java` `<enter>`
  - <img width="695" alt="image" src="https://user-images.githubusercontent.com/63514282/221431872-8c1a5507-25bd-4822-be94-c3c02915fe3a.png"> 
- `git commit -m "Fix bug"` `<enter>`
  - <img width="810" alt="image" src="https://user-images.githubusercontent.com/63514282/221431904-e88b6ad6-da6c-4d33-b999-8acf98defc19.png">
- `git push` `<enter>`
  - <img width="789" alt="image" src="https://user-images.githubusercontent.com/63514282/221432225-e4e8f72b-9ef7-4961-adc5-44e953bd3064.png"> 






  

