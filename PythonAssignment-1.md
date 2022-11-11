## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?

ANS: Python is used in almost all the fields for automation, healthcare, industries etc. It is a solution for many different problems and not just single issue. It is high level because it is user-friendly compared to other programing languages such as Java, C, C++ etc.

Q2. Why is Python called a dynamically typed language?

ANS: Variables in python is automatically determined at the run time and its type of variables doesn't need to be explicitly mentioned unlike C++, C.

Q3. List some pros and cons of Python programming language?

ANS: PROS:
        1. User friendly
        2. Object oriented
        3. Versatile usage
        4. Wide varities of libraries available for all the software engineering fields
     CONS:
        1. As it is a interpreter languange it executes the code line by line making the execution speed slow
        
        

Q4. In what all domains can we use Python?

ANS: 1. Healthcare
     2. Game development
     3. Web development
     4. BigData
     5. Machine Learning and AI

Q5. What are variable and how can we declare them?

ANs: Variables are just name for the location which holds the values in the memory. In python we can just declare variables using "=" operator.

EX: a = 1 (Value of a holds int type)
    a = "Kannappan" (Value of a holds string type variable)
    a = [1,2,3] (Value of a holds array type)

Q6. How can we take an input from the user in Python?

ANS: Using input() method

Q7. What is the default datatype of the value that has been taken as an input using input() function?

AnS: Str

Q8. What is type casting?

AND: Converting the type of one variable to another is called as type casting
EX: a = "1"
    print(type(a)) #op=str
    a = int(1)
    print(type(a)) # op=int

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?

ANS: Yes we can take more that one inputs using a split() function.

EX: a,b,c = input("Enter 3 values").split()
    print(a + "-" + b + "-" +c)

OP: Enter 3 values:
    1 2 3
Code_res: 
    1-2-3
    
Q10. What are keywords?

ANS: Keywords are special words which has specific meaning and purpose. Ex: For, if, while, and, or etc.

Q11. Can we use keywords as a variable? Support your answer with reason.

ANS: No we can use keywords as variable as it by default has some pre-defined meaning allocated.

Q12. What is indentation? What's the use of indentaion in Python?

ANS: Python use indentation to depict a block of code. For other programming languages we use "{}" to indicate the block of code but for python correct space at the starting of every line i.e indentation indicates the block of code.

Q13. How can we throw some output in Python?

ANS: Output we can get it or verified using print statement. In python functions we can use return statement to throw an output

Q14. What are operators in Python?

ANS: Operators are used to perform some for of actions with the variables used in the program. 
EX: Arithmatic operator, binary operator, comparison operator etc

Q15. What is difference between / and // operators?

ANS: / -> It does the division with the decimal point result

    // -  It does the division withour decimal point result and get the value as a whole number

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```
ANS: print("iNeuroniNeuroniNeuroniNeuron")

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

ANS: num = int(input("Enter a number:"))
     if (num%2==0):
        print(str(num)+" is even")
     else:
        print(str(num)+ " is odd")


Q18. What are boolean operator?

ANS: and, or and not are known as boolean operators.

Q19. What will the output of the following?
```
1 or 0

0 and 0

True and False and True

1 or 0 or 0
```

ANS:

    1 or 0 => 1

    0 and 0 => 0

    True and False and True => False

    1 or 0 or 0 =? 1


Q20. What are conditional statements in Python?

ANS: ==, !=, <=,<,>=,> these are known as conditional operators

Q21. What is use of 'if', 'elif' and 'else' keywords?

ANS: To check the conditions we use if, elif and else statements. For making a decision we usually use these clauses.

elif is used for nested if else conditions.


Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".

ANS:

    age = int(input("Enter your age:"))
    if (age >= 18):
        print("I can vote")
    else:
        print("I can't vote")

Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```

ANS: 
```

numbers = [12, 75, 150, 180, 145, 525, 50]

def allowEvenNumbers(lst):
    even_lst=[]
    for num in lst:
        if num%2==0:
            even_lst.append(num)
    return even_lst


sum = 0
numbers_lst = numbers
evenNumList=allowEvenNumbers(numbers_lst)
for each_number in evenNumList:
    sum=sum+each_number
print(sum)
```
     

Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

ANS:
num1, num2, num3 = input("Enter 3 numbers seperated nu space:").split()

max = max(int(num1), int(num2), int(num3))

print(max)

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```

ANS:
op_lst = []
numbers = [12, 750, 150, 180, 145, 525, 50]
num_lst = numbers
for each_num in num_lst:
        if each_num > 500:
            break
        elif each_num > 150:
            continue
        else:
            if each_num%5 == 0:
                op_lst.append(each_num) 
print(op_lst)