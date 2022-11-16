## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?
Ans: Due to the facts that python is easy for humans to understand and is broadly applicable across application domains. 

Q2. Why is Python called a dynamically typed language?
Ans: It doesn't know about the type of the variable until the code is run

Q3. List some pros and cons of Python programming language?
Ans:
    Pros:
    1. Beginner-friendly
    2. Large Community
    3. Flexible and Extensible
    4. Extensive Libraries

    Cons:
    1. Slower than compiled languages
    2. High memory consumption
    3. Weak in Mobile Computing

Q4. In what all domains can we use Python?
Ans: 1. Data Science
     2. Web Application
     3. AI & Machine Learning
     4. Automation
     5. Mobile Application
     6. Console Application
     7. Desktop GUI

Q5. What are variable and how can we declare them?
Ans: Variables are containers for storing data values. It can be declared by following rules:
        1. The first character of the variable can be an alphabet or (_) underscore.
        2. Special characters (@, #, %, ^, &, *) should not be used in variable name.
        3. Variable names are case sensitive. For example - age and AGE are two different variables.
        4. Reserve words cannot be declared as variables.

Q6. How can we take an input from the user in Python?
Ans: we can use in-built input() to take from user

Q7. What is the default datatype of the value that has been taken as an input using input() function?
Ans: string
Q8. What is type casting?
Ans: converting the datatype to another

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?
Ans: Yes, using split(). For e.g. a, b = input("Enter two values: ").split()

Q10. What are keywords?
Ans: special reserved words that have specific meanings and purposes and can't be used for anything but those specific purposes.

Q11. Can we use keywords as a variable? Support your answer with reason.
Ans: No. Since keywords are special reserved words that have specific meanings and purposes, it  can't be used for anything.

Q12. What is indentation? What's the use of indentaion in Python?
Ans: Indentation refers to the spaces at the beginning of a code line. Python uses indentation to indicate a block of code.

Q13. How can we throw some output in Python?
Ans: using print()

Q14. What are operators in Python?
Ans: In Python, operators are special symbols that designate that some sort of computation should be performed

Q15. What is difference between / and // operators?
Ans: operator '/' perform folating point division whereas operator '//' perform floor division.

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```
Ans:
    for each in range(4):
        print("iNeuron", end="")

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.
Ans: 
    num = input("Enter the number")
    if int(num) % 2 == 0:
        print("the number is even")
    else:
        print("the number is odd")

Q18. What are boolean operator?
Ans: Boolean Operator perform boolean operation(AND, OR, NOT, etc.)

Q19. What will the output of the following?
```
1 or 0   ----> 1 

0 and 0  -----> 0

True and False and True ----->False

1 or 0 or 0 -----> 1 
```

Q20. What are conditional statements in Python?
Ans:
    1. if...
    2. if....else...
    3. Nested if..elif..else

Q21. What is use of 'if', 'elif' and 'else' keywords?
Ans: these keywords are used to form conditional statements

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".
Ans:
    age = int(input("enter your age"))
    print("I can vote") if age >= 18 else print("I can't vote")

Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
Ans:
    sum = 0
    for each in numbers:
        if each % 2 == 0:
            sum = sum + each

    print(sum)

Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.
Ans:
    num1 = int(input("Enter 1st Number"))
    num2 = int(input("Enter 2nd Number"))
    num3 = int(input("Enter 3rd Number"))
    max(num1, num2, num3)


Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
Ans:
    for number in numbers:
        if number % 5 == 0:
            if number > 150 and number <= 500:
                continue
            if number > 500:
                break
            print(number)