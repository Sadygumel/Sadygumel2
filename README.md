# A Python script that showcases the basics learned, demonstrating my understanding of Python programming.
# Numerical list and list comprehension
# Creating a numerical list manually
numerical_list = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Using list comprehension to create a numerical list
numerical_list_comprehension = [x for x in range(1, 11)]

# Printing the numerical list
print("Numerical List:")
print(numerical_list)

# Printing the numerical list created using list comprehension
print("\nNumerical List Comprehension:")
print(numerical_list_comprehension)

# The script above first creates a numerical list manually from 1 to 10, then it uses list comprehension to achieve the same result. Finally, it prints both lists for comparison

# Creating a list of numbers
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Slicing the list to get a subset
subset = numbers[2:7]  # This will slice elements from index 2 (inclusive) to index 7 (exclusive)

# Printing the original list and the subset
print("Original List:", numbers)
print("Subset:", subset)

# In this script, i first create a list of numbers from 1 to 10. Then, we slice the list to extract a subset containing elements from index 2 to index 6 (since slicing is exclusive of the end index). Finally, we print both the original list and the subset to see the results.

# Creating a tuple
my_tuple = (1, 'apple', 3.14)

# Accessing elements of a tuple
print("First element:", my_tuple[0])
print("Second element:", my_tuple[1])
print("Third element:", my_tuple[2])

# Tuple packing and unpacking
a, b, c = my_tuple
print("Tuple unpacking:")
print("a:", a)
print("b:", b)
print("c:", c)

# Iterating over a tuple
print("Iterating over the tuple:")
for item in my_tuple:
    print(item)

# This script creates a tuple my_tuple with three elements, then demonstrates accessing elements using indexing. Next, it showcases tuple packing and unpacking by assigning the values of the tuple to variables a, b, and c. Finally, it iterates over the tuple and prints each element.



# Example of using an if statement
x = 10

# Checking if x is greater than 5
if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")

# Example with multiple conditions
y = 3

# Checking if y is positive, negative, or zero
if y > 0:
    print("y is positive")
elif y < 0:
    print("y is negative")
else:
    print("y is zero")

# In this script: We define a variable x with the value 10. We use an if statement to check if x is greater than 5. If the condition is true, it prints "x is greater than 5"; otherwise, it prints "x is not greater than 5". We define another variable y with the value 3.
# We use an if-elif-else statement to check if y is positive, negative, or zero. Depending on the value of y, it prints the corresponding message.


# Creating a simple dictionary
my_dict = {
    'name': 'Sadiya Ahmad',
    'age': 40,
    'city': 'Dutse, Jigawa State'
}

# Looping through the dictionary
print("Key-Value pairs:")
for key, value in my_dict.items():
    print(f"{key}: {value}")

# In this script:
# I create a dictionary my_dict with three key-value pairs.
# I use a for loop to iterate over the items (key-value pairs) in the dictionary using the items() method.
# Within the loop, we print each key-value pair.


# Example of nesting in Python
# Creating a list of dictionaries
students = [
    {'name': 'Sadiya Ahmad', 'age': 40, 'major': 'B. Sc Biology'},
    {'name': 'Hafsat Ahmad', 'age': 35, 'major': 'Biology Education'},
    {'name': 'Khadija Ahmad', 'age': 30, 'major': 'Bilogy Education'},
]

# Looping through the list of dictionaries and printing information
print("Student Information:")
for student in students:
    print(f"Name: {student['name']}")
    print(f"Age: {student['age']}")
    print(f"Major: {student['major']}")
    print("-" * 20)

#In this script:

# I have a list called students, where each element is a dictionary containing information about a student.
# I use a for loop to iterate over each dictionary in the list.
# Inside the loop, i access the values of each dictionary using keys and print the student's information.
# This example demonstrates nesting by having a list of dictionaries, where each dictionary contains related information about a student.


# Creating sets
set1 = {1, 2, 3, 4, 5}
set2 = {4, 5, 6, 7, 8}

# Accessing elements in sets
print("Elements in set1:")
for element in set1:
    print(element)

# Set union
union_set = set1.union(set2)
print("Union of set1 and set2:", union_set)

# Set intersection
intersection_set = set1.intersection(set2)
print("Intersection of set1 and set2:", intersection_set)

# In this script:
# I create two sets, set1 and set2, with some elements in each set.
# I demonstrate accessing elements in a set using a for loop.
# I also use the union() method to compute the union of set1 and set2, which contains all unique elements from both sets.
# Lastly,i use the intersection() method to compute the intersection of set1 and set2, which contains elements common to both sets.



# Example of user input and while loop
# Prompting the user to enter their name
name = input("Enter your name: ")

# Greeting the user
print(f"Hello, {name}!")

# Asking the user for a number
number = int(input("Enter a number: "))
# Initializing a counter
count = 0

# Using a while loop to print numbers from 1 to the user input number
print("Numbers from 1 to", number, ":")
while count < number:
    count += 1
    print(count)


# In this script:

# I use the input() function to prompt the user to enter their name and store the input in the variable name.
# then use the print() function to greet the user with their name.
# I then use the input() function again to prompt the user to enter a number, which i convert to an integer using int() and store in the variable number.
# I then initialize a counter count to 0.
# I use a while loop to print numbers from 1 up to the user's input number. Inside the loop, we increment the counter count by 1 in each iteration and print its value. The loop continues until count is equal to the user's input number.


# Example of conditionals, loops, and recursion
def factorial(n):
    """Recursive function to calculate the factorial of a number."""
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial(n - 1)

# Using conditionals to check if a number is even or odd
def check_even_odd(num):
    """Function to check if a number is even or odd."""
    if num % 2 == 0:
        print(f"{num} is even.")
    else:
        print(f"{num} is odd.")

# Using loops to iterate through a range of numbers
def print_numbers(n):
    """Function to print numbers from 1 to n."""
    print("Numbers from 1 to", n, ":")
    for i in range(1, n + 1):
        print(i)

# Test the functions
number = 5
check_even_odd(number)
print_numbers(number)
print(f"The factorial of {number} is {factorial(number)}")

# In this script:

# I define a recursive function factorial() to calculate the factorial of a number.
# I then define a function check_even_odd() to check if a number is even or odd using conditionals.
# then define a function print_numbers() to print numbers from 1 up to a given number using a for loop.
# lastly test the functions by passing a number (in this case, 5) to each of them and printing the results
