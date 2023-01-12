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

Q26. What is a string? How can we declare string in Python?
Ans: strings are arrays characters. Strings can be created by enclosing characters inside a single quote or double-quotes. For e.g. name = "rahul"

Q27. How can we access the string using its index?
Ans: Individual characters in a string can be accessed by specifying the string name followed by a number in square brackets ( [] ). String indexing in Python is zero-based: the first character in the string has index 0 , the next has index 1 , and so on.
For. eg. name = "Rahul"
        name[0] will point to "R"

Q28. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "iNeuron"
```
Ans:
    desired_output = string[9:]

Q29. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "norueNi"
```
Ans: desired_output = string[:-8:-1]

Q30. Resverse the string given in the above question.
Ans: desired_output = string[::-1]

Q31. How can you delete entire string at once?
Ans: Strings are immutable. Only we can make new string from old one.
    string = "Big Data iNeuron"
    new_string = string.replace(string, "")
    print(new_string)

Q32. What is escape sequence?
Ans: An escape sequence is a sequence of characters that, when used inside a character or string, does not represent itself but is converted into another character or series of characters that may be difficult or impossible to express directly, like newline (\n), tab (\t), and so on.

Q33. How can you print the below string?
```
'iNeuron's Big Data Course'
```
Ans: print("\'iNeuron\'s Big Data Course\'")

Q34. What is a list in Python?
Ans: it is a ordered collection of objects or items stored in single variable.

Q35. How can you create a list in Python?
Ans: using square brackets []. For e.g. number_list = [1,2,3,4]

Q36. How can we access the elements in a list?
Ans: We can access the list items by referring to the index number.

        number_list = [1,2,3,4]
        number_list[0]


Q37. Write a code to access the word "iNeuron" from the given list.
```
lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]
``` 
Ans: lst[4][2]

Q38. Take a list as an input from the user and find the length of the list.
Ans: 
    user_list = input("Enter the list item seperated by space").split()
    len(user_list)

Q39. Add the word "Big" in the 3rd index of the given list.
```
lst = ["Welcome", "to", "Data", "course"]
```
Ans:
    st = ["Welcome", "to", "Data", "course"]
    st.insert(2, "Big")

Q40. What is a tuple? How is it different from list?
Ans: Tuples are used to store multiple items in a single variable. tuple is immutable i.e. tuple items cannot be altered whereas list is mutable.

Q41. How can you create a tuple in Python?
Ans: tuple is created with ().
    t1 = (1,2,3,4) 

Q42. Create a tuple and try to add your name in the tuple. Are you able to do it? Support your answer with reason.
Ans: yes.
    a = (1,2)
    a = a + ('Rahul',)
    print(a)

Q43. Can two tuple be appended. If yes, write a code for it. If not, why?
    a = (1,2)
    a = a + ('Rahul',)
    print(a)

Q44. Take a tuple as an input and print the count of elements in it.
Ans :
    user_tuple = tuple(input("Enter the tuple item seperated by space").split())
    len(user_tuple)

Q45. What are sets in Python?
Ans: Sets are collection of unordered, unchangeble(only we can add/remove item) and unindexed items.

Q46. How can you create a set?
Ans: 
    set1 = set((1,2,3,))
    set2 = {1,2,3,}

Q47. Create a set and add "iNeuron" in your set.
Ans:
    set1 = set()
    set.add("iNeuron")

Q48. Try to add multiple values using add() function.
Ans:
    set.add(1)
    set.add("Rahul")

Q49. How is update() different from add()?
Ans: add() insert only one item into the set whereas update() add items of a set into another set.

Q50. What is clear() in sets?
Ans: Removes all the elements from the set

Q51. What is frozen set?
Ans: The frozenset() function returns an unchangeable frozenset object (which is like a set object)

Q52. How is frozen set different from set?
Ans: frozen set is immutable and set is unchangeble(only we can add/remove item)

Q53. What is union() in sets? Explain via code.
Ans: it is used to include the item of a set to another excluding duplicates.
    set1 = {1,2,3,4}
    set2 = {2,5,6,7}
    set1.union(set2)

    Output:
            {1,2,3,4,5,6,7}

Q54. What is intersection() in sets? Explain via code.
Ans: It is used to extract common items from given sets.
    set1 = {1,2,3,4}
    set2 = {2,5,6,7}
    set1.intersection(set2)

    Output:
        {2}


Q55. What is dictionary in Python?
Ans: Dictionary is the key-value paired collecton of items.
    e.g. dict1 = {"name": "Rahul"}

Q56. How is dictionary different from all other data structures.
Ans: While other Data Structures use only one value as the element, the dictionary is a slightly more compound data structure. It makes use of two elements i.e. a pair of elements, namely, a key and a value.

Q57. How can we delare a dictionary in Python?
Ans: Dictionaries are delclared using {} or dict() constructor.
    e.g. dict1 = {"name": "Rahul"}
         dict2 = dict(name="Rahul", age=18)

Q58. What will the output of the following?
```
var = {}
print(type(var))
```
Ans: <class 'dict'>

Q59. How can we add an element in a dictionary?
Ans: We can use either key as index inside [] or update() method.
     e.g. dict1 = {}
          dict1['key1'] = "value1"
          dict1.update({"key2":"value2"})

Q60. Create a dictionary and access all the values in that dictionary.
Ans: dict1 = {"a":1, "b":2, "c":3}
     dict1.values()

Q61. Create a nested dictionary and access all the element in the inner dictionary.
Ans: dict1 = {"a":1, "b":{"A":2, "B":3}}
     dict1["b"].values()

Q62. What is the use of get() function?
Ans: get() will return the value of given key otherwise will return None by default. So it is used when we are not sure whether the key is present or not.
        dict1 = {"a":1, "b":2}
        dict1.get("a")      # reurns 1
        dict1.get("c")      # returns None      

Q63. What is the use of items() function?
Ans: items() method will return all key-value pairs as a list of tuples.
    
    dict1 = {"a":1, "b":2}
    dict1.items()   # dict_items([('a', 1), ('b', 2)]

Q64. What is the use of pop() function?
Ans: this method is used to remove the dictionary item using the key as index

Q65. What is the use of popitems() function?
Ans: This method is used to remove the last item inserted

Q66. What is the use of keys() function?
Ans: It returns the list of keys

Q67. What is the use of values() function?
Ans: it returns the list of all values in dictionary

Q68. What are loops in Python?
Ans: Loops are nothing but the block of code which is executed repeatedly unless the specified condition becomes false

Q69. How many type of loop are there in Python?
Ans: for loop and while loop

Q70. What is the difference between for and while loops?
Ans: 
1) The while loop is slower than for loop.
2) In absence of condition, for loop runs infinite whereas while loop throws compile time error
3) Unlike while loop, For loop can be iterated on generators in Python

Q71. What is the use of continue statement?
Ans: to stop current iteration of loop and execute next iteration 

Q72. What is the use of break statement?
Ans: to come out of loop

Q73. What is the use of pass statement?
Ans: used as a placeholder for future code otherwise to avoid error since empty code is not allowed in block.

Q74. What is the use of range() function?
The range() function returns a sequence of numbers, starting from 0 by default, and increments by 1 (by default), and stops before a specified number.

Q75. How can you loop over a dictionary?
Ans: using for loop.
    thisdict =	{
                    "brand": "Ford",
                    "model": "Mustang",
                    "year": 1964
                }
<!-- Print all key names in the dictionary, one by one: -->
    for x in thisdict:
        print(x)

<!-- Print all values in the dictionary, one by one: -->
    for x in thisdict:
        print(thisdict[x])

    for x in thisdict.values():
        print(x)

<!-- Loop through both keys and values, by using the items() function: -->
    for key,value in thisdict.items():
        print(x, y)


### Coding problems
Q76. Write a Python program to find the factorial of a given number.
Ans: 
    num = int(input("Enter a number: "))

    factorial = 1

    # check if the number is negative, positive or zero
    if num < 0:
        print("Sorry, factorial does not exist for negative numbers")
    elif num == 0:
        print("The factorial of 0 is 1")
    else:
        for i in range(1,num + 1):
            factorial = factorial*i
        print("The factorial of",num,"is",factorial)

Q77. Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (P*R*T)/100
Ans:
   
    P = int(input("Enter the amount: "))
    T = int(input("Enter the number of years: "))
    R = float(input("Enter the rate of interest: "))
    SimpleInterset = (P*R*T)/100
    print("The simple interset is:", SimpleInterset)


Q78. Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t.
Ans:
    P = int(input("Enter the amount: "))
    T = float(input("Enter the number of years: "))
    R = float(input("Enter the rate of interest: "))
    CompoundInterset = P*(1+ R/100)**T
    print("The compound interset is:", CompoundInterset)

Q79. Write a Python program to check if a number is prime or not.
Ans:
    
    num = int(input("Enter a number: "))

    if num == 1:
        print(num, "is not a prime number")
    elif num > 1:
        # check for factors
        for i in range(2,num//2):
            if (num % i) == 0:
                print(num,"is not a prime number")
                break
        else:
            print(num,"is a prime number")
    
    else:
    print(num,"is not a prime number")

Q80. Write a Python program to check Armstrong Number.
Ans:
    num = input("Enter the number")

    order = len(num)
    num = int(num)
    # initialize sum
    sum = 0
 
    temp = num
    while temp > 0:
        digit = temp % 10
        sum += digit ** order
        temp //= 10

    # display the result
    if num == sum:
        print(num,"is an Armstrong number")
    else:
        print(num,"is not an Armstrong number")


Q81. Write a Python program to find the n-th Fibonacci Number.
Ans:
    def Fibonacci(n):
    if n <= 2:
        return n - 1
    else:
        return Fibonacci(n - 1) + Fibonacci(n - 2)

    n = int(input("Enter the number(n) to find n-th fibonacci number"))
    
    print(Fibonacci(n))

Q82. Write a Python program to interchange the first and last element in a list.
Ans:
    user_list = input("Enter the list item seperated by space").split()
    user_list[0], user_list[-1] = user_list[-1], user_list[0]
    print(user_list)


Q83. Write a Python program to swap two elements in a list.
Ans:
    user_list = input("Enter the list item seperated by space").split()
    index1, index2 = input("Enter the indices seperated by space to be swapped").split()

    user_list[int(index1)], user_list[int(index2)] = user_list[int(index2)], user_list[int(index1)]
    print(user_list)

Q84. Write a Python program to find N largest element from a list.
Ans:
    user_list = input("Enter the list item seperated by space").split()
    N = int(input("Enter the N"))
    user_list = [int(num) for num in user_list]
    user_list.sort(reverse=True)
    user_list[:N]

Q85. Write a Python program to find cumulative sum of a list.
Ans:
    user_list = input("Enter the list item seperated by space").split()
    user_list = [int(num) for num in user_list]
    sum = 0
    output = []
    for i in range(len(user_list)):
        sum += user_list[i]
        output.append(sum)
    print(output)

Q86. Write a Python program to check if a string is palindrome or not.
Ans:
    my_str = input("Enter the sring")

    # make it suitable for caseless comparison
    my_str = my_str.casefold()

    # reverse the string
    rev_str = reversed(my_str)

    # check if the string is equal to its reverse
    if list(my_str) == list(rev_str):
        print("The string is a palindrome.")
    else:
        print("The string is not a palindrome.")

Q87. Write a Python program to remove i'th element from a string.
Ans:
    user_string = input("Enter the string")
    index = int(input("Enter the index of item to be removed"))
    user_string.replace(user_string[index], "", 1)

Q88. Write a Python program to check if a substring is present in a given string.
Ans:
    user_string = input("Enter the string")
    substring = input("Enter the substring")

    if substring in user_string:
        print("Substring is present")
    else:
        print("Substring is not present")


Q89. Write a Python program to find words which are greater than given length k.
Ans:
    sentence = input("Enter the sentence").split()
    length = int(input("Enter the length"))
    output_string = [word for word in sentence if len(word) > length]
    output_string

Q90. Write a Python program to extract unquire dictionary values.
Ans:    
    # Initialising dictionary
    myDict = {'Scala': 2, 'Javascript': 1, 'Python': 8, 'C++': 1, 'Java': 4}

    # extracting unique values using set comprehension
    uniqueValues = list({val for val in myDict.values() })
    
    # Printing the dictionary and unique values...
    print("Dictionary = ", end = " ")
    print(myDict)
    print("Unique Values = ", end = " ")
    print(uniqueValues)

Q91. Write a Python program to merge two dictionary.
Ans:
    dict_1 = {1: 'a', 2: 'b'}
    dict_2 = {2: 'c', 4: 'd'}

    print(dict_1 | dict_2)

Q92. Write a Python program to convert a list of tuples into dictionary.

```
Input : [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
Output : {'Sachin': 10, 'MSD': 7, 'Kohli': 18, 'Rohit': 45}
```
Ans:
    
    tuple1 = [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
    dict(tuple1)

Q93. Write a Python program to create a list of tuples from given list having number and its cube in each tuple.
```
Input: list = [9, 5, 6]
Output: [(9, 729), (5, 125), (6, 216)]
```
Ans:
    list1 = [9, 5, 6]
    [(num, num**3) for num in list1]

Q94. Write a Python program to get all combinations of 2 tuples.
```
Input : test_tuple1 = (7, 2), test_tuple2 = (7, 8)
Output : [(7, 7), (7, 8), (2, 7), (2, 8), (7, 7), (7, 2), (8, 7), (8, 2)]
```
Ans:
    test_tuple1 = (7, 2)
    test_tuple2 = (7, 8)
    res =  [(a, b) for a in test_tuple1 for b in test_tuple2]
    res = res +  [(a, b) for a in test_tuple2 for b in test_tuple1]
  
    # printing result 
    print(res)

Q95. Write a Python program to sort a list of tuples by second item.
```
Input : [('for', 24), ('Geeks', 8), ('Geeks', 30)] 
Output : [('Geeks', 8), ('for', 24), ('Geeks', 30)]
```
Ans:
    list2 = [('for', 24), ('Geeks', 8), ('Geeks', 30)] 
    list2.sort(key=lambda x:x[1])
    list2

Q96. Write a python program to print below pattern.
```
* 
* * 
* * * 
* * * * 
* * * * * 
```
Ans:
    for i in range(0, 5):
     
        for j in range(0, i+1):
        
            # printing stars
            print("* ",end="")
    
    # ending line after each row
    print("\r")

Q97. Write a python program to print below pattern.
```
    *
   **
  ***
 ****
*****
```
Ans:
    height = 5
    for row in range(1, height+ 1):
        print(" " * (height - row) +"*" * row)

Q98. Write a python program to print below pattern.
```
    * 
   * * 
  * * * 
 * * * * 
* * * * * 
```
Ans:
    rows = 5

    k = 0

    for i in range(1, rows+1):
        for space in range(1, (rows-i)+1):
            print(end="  ")
    
        while k!=(2*i-1):
            print("* ", end="")
            k += 1
    
        k = 0
        print()

Q99. Write a python program to print below pattern.
```
1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5
```
Ans:
    rows = 5

    for i in range(rows):
        for j in range(i+1):
            print(j+1, end=" ")
        print("\n")

Q100. Write a python program to print below pattern.
```
A 
B B 
C C C 
D D D D 
E E E E E 
```
Ans:
    rows = 5

    ascii_value = 65

    for i in range(rows):
        for j in range(i+1):
            alphabet = chr(ascii_value)
            print(alphabet, end=" ")
        
        ascii_value += 1
        print("\n")