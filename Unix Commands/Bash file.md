# Bash Scripts 📜
***Once the Vi command of [Bash Script](https://github.com/VC-Nithesh944/Unix-Shell-Program/blob/main/Unix%20Commands/Bash%20Scripts.md) is executed creates a required file with assigned file name then You can executed the following Scripts***

### 1. Hello World Script 🌍
This script prints **Hello World** to the terminal
```bash
  #!/bin/bash
  echo "Hello World"
```

### 2. Working With Variable 💡
This script shows how to **define** and **use** variable
```bash
  #!/bin/bash
  name=Nithesh        (Important: Not to leave any whitespace during variable declaration)
  age=19
  college=BMSCE

  echo My name is $name, I am $age years old and currently studying in $college college
  ($ is used to get the values from the variables)
```

### 3. Keyboard Input ⌨️
This script takes input from the **keyboard** and prints it.
```bash
  #!/bin/bash
  echo Enter your Blog Website name
  read websitename

  echo My Blog Websites name is $websitename.
```

### 4. Adding Two Numbers (User Input) ➕➗
This script reads two numbers from the user and adds them.
```bash
  #!/bin/bash
  echo Addition of two numbers
  echo
  echo Enter the First number
  read num1
  echo Enter the Second number
  read num2
  num3=$(($num1+$num2))         (The result must stored using $ sign)

  echo The sum of $num1 and $num2 is $num3.
```
### 5. If-Else Statement🗳️
This script is a basic demostration of **if else** by checking eligibility to vote.
```bash
  #!/bin/bash
  echo !!Welcome to Voting Center!!
  echo                                      (writing echo without commands gives newline)
  echo Enter your Name
  read name
  echo Enter your Age
  read age
  echo
  if [ $age -gt 18 ]
  then
            echo "You are Eligible to Vote"
  else
            echo "You are Not Eligible to Vote"
  fi
```

### 6. Switch Case Statement
This script uses a switch case to display a message based on the chosen option.
```bash
  #!/bin/bash

  echo Hello to Shell Scripting. This a switch case program to see all the syntax functions.
  echo
  echo Options:
  echo 1] To see the path
  echo 2] To clear the screen
  echo 3] To list the file
  echo 4] To quit
  
  echo Enter a choice
  read choice
  
  case $choice in
          1)pwd;;
          2)clear;;
          3)ls -ltr;;
          4)q;;
          *) echo Invalid Entry
  esac                           (esac is reverse of case)
```
