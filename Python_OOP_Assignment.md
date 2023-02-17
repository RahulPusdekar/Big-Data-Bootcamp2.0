## Python OOP Assignment
Q1. What is the purpose of Python's OOP?
Ans:The main aim of object-oriented programming is to implement real-world entities, for example, object, classes, abstraction, inheritance, polymorphism, encapsulation etc.

Q2. Where does an inheritance search look for an attribute?
Ans:
    the child class will first search the attribute in its own class, if not, then search in its parent classes in depth-first, left-right order.

Q3. How do you distinguish between a class object and an instance object?
Ans: when we create class, class object is created automatically i.e. we can access class varibles by using class name direclty. On the other hand, we have to create instance object explictly using constructor. We can have multile instance object but a single class object.

Q4. What makes the first argument in a class’s method function special?
Ans: the first argument in a class’s method i.e. cls refers to the class.

Q5. What is the purpose of the init method?
Ans: init method is used to initialze the object

Q6. What is the process for creating a class instance?
Ans: To create instances of a class, you call the class using class name and pass in whatever arguments its __init__ method accepts.

Q7. What is the process for creating a class?
Ans: Class can be created by using the keyword class, followed by the class name.
     
     class TestClass:
        pass
        
Q8. How would you define the superclasses of a class?
Ans: just as mentioned in Q7

Q9. What is the relationship between classes and modules?
Ans: modules may contain classes, function, varibales. If we want to use a class, we have to import the modules

Q10. How do you make instances and classes?
Ans:
class A:
    def __init__(self, a , b):
        self.a = a 
        self.b = b

instance1 = A(10,20)

Q11. Where and how should be class attributes created?
Ans: Class attributes are created in the body of class but outside the __init__() method, usually at the top.

class A:
    number = 2   # class attribute
    def __init__(self, a, b):
        self.a = a      # instance attribute
        self.b = b      # instance attribute

Q12. Where and how are instance attributes created?
Ans: inside the __init__() constructor of class.

class A:
    
    def __init__(self, a, b):
        self.a = a      # instance attribute
        self.b = b      # instance attribute

Q13. What does the term "self" in a Python class mean?
Ans: It is a keyword which points to the current passed instance. By using the “self”  we can access the attributes and methods of the class in python.

Q14. How does a Python class handle operator overloading?
Ans: In Python, operator overloading is achieved by defining special methods in a class with a double underscore (e.g. add). These special methods determine the behavior of operators (e.g. +) when used on instances of the class. For example, defining a __add__ method in a class allows instances of the class to be added together using the + operator.

Q15. When do you consider allowing operator overloading of your classes?
Ans: You should consider allowing operator overloading in your classes when it makes sense for instances of the class to support the corresponding operations and when it improves code readability and maintainability. For example, if you are defining a class for a mathematical vector, overloading the + and - operators for vector addition and subtraction can make the code more intuitive and easier to understand. However, if the overloaded operators do not have a clear and well-defined meaning for instances of the class, it is better not to overload them.

Q16. What is the most popular form of operator overloading?
Ans: Addition (+) operator

Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?
Ans:
1. Classes and objects
2. Inheritance and polymorphism.

Q18. Describe three applications for exception processing.
Ans:
1. Error handling: Exception processing can be used to handle unexpected errors or exceptions that occur during the execution of a program and allow it to continue running instead of crashing.

2. Input Validation: Exception handling can be used to validate user input and ensure that only valid data is processed.

3. Resource Management: Exception handling can be used to manage resources, such as files or database connections, by ensuring that they are properly closed or released even if an exception occurs during their use.

Q19. What happens if you don't do something extra to treat an exception?
Ans: If an exception is not handled, it will propagate and cause the program to crash or stop executing. The program will stop executing at the point where the exception occurred, and an error message will be displayed to the user indicating what went wrong.

Q20. What are your options for recovering from an exception in your script?
Ans:
1. Try-Except block: Catch the exception using a try-except block and handle it appropriately, such as by logging the error or displaying a user-friendly message.

2. Finally block: Use a finally block to ensure that any necessary cleanup actions are performed, such as closing a file or releasing resources, even if an exception occurs.

3. Raising an exception: Catch the exception, process it, and then raise a new exception with a more appropriate error message.

4. Return a default value: Return a default value or an error code when an exception occurs, allowing the program to continue running.

5. Terminate the program: Terminate the program gracefully, such as by displaying a message to the user or logging the error, when an exception occurs.

Q21. Describe two methods for triggering exceptions in your script.
Ans:
1. Raise statement: Use the "raise" statement to explicitly trigger an exception. This allows you to throw an exception when a certain condition is met or an error occurs in your code.

2. Built-in exceptions: Use built-in exceptions, such as "ValueError" or "IndexError", which are raised automatically by the Python interpreter in response to certain conditions, such as an invalid argument value or an out-of-range index.

Q22. Identify two methods for specifying actions to be executed at termination time, regardless of whether or not an exception exists.
Ans: 
1. The finally block
2. The atexit module

Q23. What is the purpose of the try statement?
Ans: It is used to check for exceptions/erros

Q24. What are the two most popular try statement variations?
Ans:
1. try-except
2. try-finally

Q25. What is the purpose of the raise statement?
Ans: to raise an exception/error

Q26. What does the assert statement do, and what other statement is it like?
Ans:
The assert statement is used to check if an expression is true, and if not, it raises an AssertionError with an optional error message. The assert statement is similar to the if statement in that it checks a condition and takes an action based on the result

Q27. What is the purpose of the with/as argument, and what other statement is it like?
Ans:
The main purpose of the with/as statement is to ensure that a certain block of code is executed within the context of a certain context manager, and that the context is properly entered and exited even in the case of exceptions or errors.

he with statement is similar in some ways to a try/finally statement.

Q28. What are *args, **kwargs?
Ans: 
The *args is used to pass a variable number of non-keyworded arguments to a function. When *args is used in a function definition, it allows the function to accept any number of positional arguments, which are then captured as a tuple of arguments inside the function.

The **kwargs is used to pass a variable number of keyworded arguments to a function. When **kwargs is used in a function definition, it allows the function to accept any number of keyword arguments, which are then captured as a dictionary of arguments inside the function


Q29. How can I pass optional or keyword parameters from one function to another?
Ans:
To pass optional or keyword parameters using, you can define the optional or keyword parameters in the function definition with a default value, and then pass them as arguments to another function

Q30. What are Lambda Functions?
Ans: Lambda function is a small anonymous function. A lambda function can take any number of arguments, but can only have one expression.

x = lambda a : a + 10
print(x(5))


Q31. Explain Inheritance in Python with an example?
Ans:
Inheritance is a mechanism in object-oriented programming where a child class inherits properties and methods from a parent class. This allows for code reusability and makes it easier to maintain and extend code.

class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def introduce(self):
        print(f"Hello, my name is {self.name} and I am {self.age} years old.")

class Student(Person):
    def __init__(self, name, age, major, student_id):
        super().__init__(name, age)
        self.major = major
        self.student_id = student_id

    def enroll(self):
        print(f"I am a student in {self.major} with ID {self.student_id}.")

student = Student("John", 20, "Computer Science", "12345")
student.introduce() # "Hello, my name is John and I am 20 years old."
student.enroll()    # "I am a student in Computer Science with ID 12345."


For example, let's say we have a Person class with properties such as name and age, and methods such as introduce(). We can create a child class Student that inherits from Person. The Student class can have additional properties such as major and student_id, and methods such as enroll().

In this example, Student class is inheriting from Person class. Student class has all the properties and methods of Person class and additional properties and methods of its own.

The super() function is used to call the __init__ method of the parent class. The super() function returns a temporary object of the parent class, which allows you to call its methods.

Q32. Suppose class C inherits from classes A and B as class C(A,B).Classes A and B both have their own versions of method func(). If we call func() from an object of 
class C, which version gets invoked?
Ans: class A's version


Q33. Which methods/functions do we use to determine the type of instance and inheritance?
Ans: The built-in type() function can be used to determine the type of an instance in Python. The isinstance() function can be used to check if an instance is of a certain class or a subclass thereof. The issubclass() function can be used to check if a class is a subclass of another class.

Q34.Explain the use of the 'nonlocal' keyword in Python.
Ans: nonlocal keyword is used to reference a variable in the nearest scope.The nonlocal keyword won’t work on local or global variables and therefore must be used to reference variables in another scope except the global and local one. The nonlocal keyword is used in nested functions to reference a variable in the parent function. 

Q35. What is the global keyword?
Ans: global keyword is a keyword that allows a user to modify a variable outside the current scope. It is used to create global variables in Python from a non-global scope, i.e. inside a function. Global keyword is used inside a function only when we want to do assignments or when we want to change a variable