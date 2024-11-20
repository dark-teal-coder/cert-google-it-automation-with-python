# Solutions to Problems in Crash Course on Python

There are a few types of questions in the quizzes in the course. See the list of the question types below.

1. Multiple choice
2. Code
3. Value input/output

For type 1, start the solution with `- [x]`; for type 2, use triple backticks to create a Python code block; for type 3, use single backticks.

The graded assessments usually have 10 questions in them but there is a pool of over 10 questions for every graded assessment. Therefore, we get different questions every time we attempt the assessments. The following solutions may not all be the same as what you see when you do the assessments.

---

## Module 01 Hello Python

### 01.02 Introduction to Programming

#### 01.02.07 Practice Quiz: Introduction to Programming

***Solution 01***

- [x] A list of instructions that the computer has to follow to reach a goal

***Solution 02***

- [x] The rules of how to express things in that language

***Solution 03***

- [x] There’s not much difference, but scripts are usually simpler and shorter.

***Solution 04***

Multiple answers:

- [x] Generating a sales report, split by region and product type
- [x] Copying a file to all computers in a company

***Solution 05***

- [x] The intended meaning or logic of coded statements

### 01.03 Introduction to Python

#### 01.03.07 Practice Quiz: Introduction to Python

***Solution 01***

```python
print("My first Python program")
```

***Solution 02***

- [x] General-purpose scripting language

***Solution 03***

```python
print("Have a nice day")
```

***Solution 04***

```python
for i in range(5):
  print("This is fun!")
```

***Solution 05***

Multiple answers:

- [x] Python is used in fast-growing areas of IT, like machine learning and data analytics.
- [x] Python works well as a scripting language for IT automation.
- [x] Python can be used to calculate statistics, run e-commerce sites, process images, interact with web services, and more.

### 01.04 Hello World

#### 01.04.08 Practice Quiz: Hello World

***Solution 01***

- [x] Functions are pieces of code that perform a unit of work.

***Solution 02***

- [x] Keywords are reserved words that are used to construct instructions.

***Solution 03***

- [x] The print function outputs messages to the screen

***Solution 04***

```python
print("Programming in Python is fun!")
```

***Solution 05***

```python
ratio = (1 + 5**(1/2))/2
print(ratio)
```

### Module 01 Review

#### 01.05.05 Quiz: Module 01 Graded Assessment

***Solution 01***

- [x] Step-by-step instructions on how to complete a set of tasks, to be executed by a computer.

***Solution 02***

- [x] Script

***Solution 03***

Multiple answers:

- [x] Detecting and removing duplicate data
- [x] Updating specific files on multiple computers

***Solution 04***

- [x] Syntax is a set of rules for how statements are constructed. Semantics refers to the intended meaning or effect of statements.

***Solution 05***

- [x] Interpreter

***Solution 06***

- [x] `print()`

***Solution 07***

- [x] 8.0

***Solution 08***

```python
# Enter code here:
print(24*60)

# Should print 1440
```

***Solution 09***

```python
# Should print 1000
print(10**3)
```

***Solution 10***

```python
download_size_kb = 200*1024
total_computers = 200
total_kbs = download_size_kb * total_computers

print(total_kbs) # Should print 40960000.0
```

---

## Module 02 Basic Python Syntax

### 02.01 Expressions and Variables

#### 02.01.10 Practice quiz: Expressions and Variables

***Solution 01***

```python
print("2 + 2 = " + str(2 + 2))
```

***Solution 02***

```python
bill = 47.28
tip = bill * 0.15
total = bill + tip
share = total / 2
print("Each person needs to pay:" + str(share))
```

***Solution 03***

```python
numerator = 10
denominator = 10
result = int(numerator / denominator)
print(result)
```

***Solution 04***

```python
word1 = "How"
word2 = "do"
word3 = "you"
word4 = "like"
word5 = "Python"
word6 = "so"
word7 = "far?"

print(word1, word2, word3, word4, word5, word6, word7, sep=" ")
```

***Solution 05***

- [x] An expression

### 02.02 Functions

#### 02.02.11 Practice Quiz: Functions

***Solution 01***

```python
# 1) Complete the code to return the result of the conversion
def convert_distance(km):
    m = km * 1000  # exactly 1000 meters in 1 kilometer
    return m

# Do not indent any of the following lines of code as they are
# meant to be located outside of the function above
my_trip_kilometers = 55

# 2) Convert my_trip_kilometers to meters by calling the function above
my_trip_meters = convert_distance(my_trip_kilometers)

# 3) Fill in the blank to print the result of converting my_trip_kilometers
print("The distance in meters is " + str(my_trip_meters))
```

***Solution 02***

- [x] Adding comments
- [x] Writing self-documenting code
- [x] Cleaning up duplicate code by creating a function that can be reused

***Solution 03***

- [x] Parameters

***Solution 04***

```python
def print_seconds(hours, minutes, seconds):
   print(hours*3600 + minutes*60 + seconds)

print_seconds(1,2,3)
```

***Solution 05***

- [x] Used to define a new function

### 02.03 Conditionals

#### 02.03.15 Practice Quiz: Conditionals

***Solution 01***

- [x] True

***Solution 02***

```python
def greeting(name):
  if name == "Taylor":
    return "Welcome back Taylor!"
  else:
    return "Hello there, " + name

print(greeting("Taylor"))
print(greeting("John"))
```

***Solution 03***

2

***Solution 04***

- [x] "A dog" is smaller than "A mouse" and 9999+8888 is larger than 100*100

***Solution 05***

```python
def calculate_storage(filesize):
    block_size = 4096
    # Use floor division to calculate how many blocks are fully occupied
    full_blocks = filesize // block_size
    # Use the modulo operator to check whether there's any remainder
    partial_block_remainder = filesize % block_size
    # Depending on whether there's a remainder or not, return
    # The total number of bytes required to allocate enough blocks
    # to store your data.
    if partial_block_remainder > 0:
        return block_size * (full_blocks + 1)
    return block_size * full_blocks

print(calculate_storage(1))    # Should be 4096
print(calculate_storage(4096)) # Should be 4096
print(calculate_storage(4097)) # Should be 8192
print(calculate_storage(6000)) # Should be 8192
```

### Module 02 Review

#### 02.04.04 Quiz: Module 02 Graded Assessment

***Solution 01***

```python
name = "Marjery"
home_address = "1234 Mockingbird Lane"
print(name + " lives at her home address of " + home_address)
# Should print "Marjery lives at her home address of 1234 Mockingbird Lane"
```

***Solution 02***

- [x] `TypeError`

***Solution 03***

- [x] 7

***Solution 04***

```python
def clothing_type(temp):
    if temp > 65:
        clothing = "T-Shirt"
    elif temp > 50 and temp <= 65:
        clothing = "Sweatshirt"
    elif temp > 32 and temp <= 50:
        clothing = "Jacket"
    else:
        clothing = "Heavy Coat"
    return clothing

print(clothing_type(72)) # Should print T-Shirt
print(clothing_type(55)) # Should print Sweatshirt
print(clothing_type(65)) # Should print Sweatshirt
print(clothing_type(50)) # Should print Jacket
print(clothing_type(45)) # Should print Jacket
print(clothing_type(32)) # Should print Heavy Coat
print(clothing_type(0)) # Should print Heavy Coat
```

***Solution 05***

- [x] 15

***Solution 06***

```python
def complementary_color(color):
    if color == "blue":
        complement = "orange"
    elif color == "yellow":
        complement = "purple"
    elif color == "red":
        complement = "green"
    else:
        complement = "unknown"
    return complement

print(complementary_color("blue")) # Should print orange
print(complementary_color("yellow")) # Should print purple
print(complementary_color("red")) # Should print green
print(complementary_color("black")) # Should print unknown
print(complementary_color("Blue")) # Should print unknown
print(complementary_color("")) # Should print unknown
```

***Solution 07***

`15`

***Solution 08***

- [x] `False`

***Solution 09***

```python
def return_nonnegative(first_num, second_num):
    if first_num > second_num:
        result = first_num - second_num
    else:
        result = second_num - first_num
    return result

print(return_nonnegative(5, 5)) # Should print 0
print(return_nonnegative(4, 5)) # Should print 1
print(return_nonnegative(5, 3)) # Should print 2
print(return_nonnegative(2, 5)) # Should print 3
print(return_nonnegative(5, 0)) # Should print 5
print(return_nonnegative(0, 5)) # Should print 5
```

***Solution 10***

Multiple answers:

- [x] Makes the intent of the code obvious
- [x] Easier to maintain

---

## Module 03 Loops

### 03.01 While Loops

#### 03.01.12 Practice Quiz: While Loops

***Solution 01***

- [x] while loops tell the computer to repeatedly execute a set of instructions while a condition is true.

***Solution 02***

- [x] Change the value of a variable used in the while condition
- [x] Use the break keyword

***Solution 03***

```python
def is_power_of_two(number):
    # This while loop checks if the "number" can be divided by 2 without leaving a remainder. How can you change the while loop to avoid a Python ZeroDivisionError?
    while number % 2 == 0 and number != 0:
        number = number / 2
    # If after dividing by 2 "number" equals 1, then "number" is a power of 2.
    if number == 1:
        return True
    return False
  
# Calls to the function
print(is_power_of_two(0)) # Should be False
print(is_power_of_two(1)) # Should be True
print(is_power_of_two(8)) # Should be True
print(is_power_of_two(9)) # Should be False
```

***Solution 04***

```python
def sum_of_integers(n):
    if n < 1:
        return 0
    i = 1
    sum = 0
    while i <= n:
        sum = sum + i
        i = i + 1
    return sum

print(sum_of_integers(3))  # should print 6
print(sum_of_integers(4))  # should print 10
print(sum_of_integers(5))  # should print 15
```

***Solution 05***

```python
def multiplication_table(number):
    # Initialize the appropriate variable
    multiplier = 1
    result = number
    # Complete the while loop condition.
    while multiplier <= 5:
        result = number * multiplier 
        if  result > 25:
            # Enter the action to take if the result > 25
            break
        print(str(number) + "x" + str(multiplier) + "=" + str(result))
        # Increment the appropriate variable
        multiplier += 1

multiplication_table(3) 
# Should print: 
# 3x1=3 
# 3x2=6 
# 3x3=9 
# 3x4=12 
# 3x5=15
multiplication_table(5) 
# Should print: 
# 5x1=5
# 5x2=10
# 5x3=15
# 5x4=20
# 5x5=25
multiplication_table(8) 
# Should print:
# 8x1=8
# 8x2=16
# 8x3=24
```

### 03.02 For Loops

#### 03.02.14 Practice Quiz: For Loops

***Solution 01***

- [x] While loops iterate while a condition is true, for loops iterate through a sequence of elements.

***Solution 02***

- [x] Choose this code below:

```python
for n in range(6,18+1,3):
    print(n*2)
```

***Solution 03***

Multiple answers:

- [x] Choose this code below:

```python
for n in range(19):
    if n % 2 == 0:
        print(n)
```

- [x] Choose this code below:

```python
for n in range(10):
    print(n+n)
```

***Solution 04***

```python
for x in range(1, 10+1):
    print(x**3)
```

***Solution 05***

```python
for x in range(0, 101, 7):
    print(x)
```

***Solution 06***

- [x] Choose this code below:

```python
for c in input:
    if c.lower() in ['a', 'e', 'i', 'o', 'u']:
        print(c)
```

- [x] Choose this code below:

```python
print([c for c in input if c.lower() in ['a', 'e', 'i', 'o', 'u']])
```

***Solution 07***

- [x] If the starting index is negative, Python counts backward from the end of the string.

### 03.03 Recursion (Optional)

#### 03.03.06 Practice Quiz: Recursion

***Solution 01***

- [x] Recursion is used to call a function from inside the same function.

***Solution 02***

- [x] Going through a file system collecting information related to directories and files.
- [x] Managing permissions assigned to groups inside a company, when each group can contain both subgroups and users.

***Solution 03***

```python
def is_power_of(number, base):
 # Base case: when number is smaller than base.
    if number < base:
        # If number is equal to 1, it's a power (base**0).
        return base**0 == number
    # Recursive case: keep dividing number by base.
    return is_power_of(number/base, base)

print(is_power_of(8,2))     # Should be True
print(is_power_of(64,4))    # Should be True
print(is_power_of(70,10))   # Should be False
```

***Solution 04***

```python
def count_users(group):
  count = 0
  for member in get_members(group):
    count += 1
    if is_group(member):
      count += count_users(member) - 1
  return count

print(count_users("sales")) # Should be 3
print(count_users("engineering")) # Should be 8
print(count_users("everyone")) # Should be 18
```

***Solution 05***

```python
def sum_positive_numbers(n):
  if n < 1:
    return 0
  return n + sum_positive_numbers(n - 1)

print(sum_positive_numbers(3)) # Should be 6
print(sum_positive_numbers(5)) # Should be 15
```

### Module 03 Review

#### 03.04.05 Quiz: Module 03 Graded Assessment

***Solution 01***

```python
number = 1 # Initialize the variable
while number <= 7: # Complete the while loop condition
    print(number, end=" ")
    number += 1 # Increment the variable
# Output: 1 2 3 4 5 6 7 
```

***Solution 02***

```python
for number in range(5,-1,-1):
    print(number)

# Output:
# 5
# 4
# 3
# 2
# 1
# 0
```

***Solution 03***

```python
def factorial(n):
    result = n
    start = n
    n -= 1
    while n > 0: # The while loop should execute as long as n is greater than 0
        result *= n # Multiply the current result by the current value of n
        n -= 1 # Decrement the appropriate variable by -1
    return result

print(factorial(3)) # Output: 6
print(factorial(9)) # Output: 362880
print(factorial(1)) # Output: 1
```

***Solution 04***

```python
def multiplication_table(start, stop):
    ## Complete the outer loop range
    for x in range(start, stop+1): 
        ## Complete the inner loop range
        for y in range(start, stop+1):
            ## Print the value of "x" multiplied by "y" 
            ## and inserts a space after each value
            print(str(x*y), end=" ")
        ## An empty print() function inserts a line break at the end of the row 
        print()

multiplication_table(1, 3)
```

***Solution 05***

```python
def divisible(max, divisor):
    count = 0 # Initialize an incremental variable
    for x in range(max): # Complete the for loop
        if x % divisor == 0:
            count += 1 # Increment the appropriate variable
    return count

print(divisible(100, 10)) # Output: 10
print(divisible(10, 3)) # Output: 4
print(divisible(144, 17)) # Output: 9
```

***Solution 06***

```python
def all_numbers(minimum, maximum):

    return_string = "" # Initializes variable as a string

    # Complete the for loop with a range that includes all 
    # numbers up to and including the "maximum" value.
    for i in range(minimum, maximum+1): 

        # Complete the body of the loop by appending the number
        # followed by a space to the "return_string" variable.
        return_string += str(i) + " "

    # This .strip command will remove the final " " space 
    # at the end of the "return_string".
    return return_string.strip()

print(all_numbers(2,6))  # Output: 2 3 4 5 6
print(all_numbers(3,10)) # Output: 3 4 5 6 7 8 9 10
print(all_numbers(-1,1)) # Output: -1 0 1
print(all_numbers(0,5))  # Output: 0 1 2 3 4 5
print(all_numbers(0,0))  # Output: 0
```

***Solution 07***

- [x] Will produce a NameError stating the variable is not defined

***Solution 08***

`7`

***Solution 09***

`8`

***Solution 10***

- [x] Variable `x` is not incremented

---

## Module 04 Strings, Lists and Dictionaries

### 04.01 Strings

#### 04.01.19 Practice Quiz: Strings

***Solution 01***

```python
def is_palindrome(input_string):
    # Two variables are initialized as string date types using empty 
    # quotes: "reverse_string" to hold the "input_string" in reverse
    # order and "new_string" to hold the "input_string" minus the 
    # spaces between words, if any are found.
    new_string = ""
    reverse_string = ""
    # Complete the for loop to iterate through each letter of the
    # "input_string"
    for letter in input_string.lower():
        # The if-statement checks if the "letter" is not a space.
        if letter != " ":
            # If True, add the "letter" to the end of "new_string" and
            # to the front of "reverse_string". If False (if a space
            # is detected), no action is needed. Exit the if-block.
            new_string = new_string + letter
            reverse_string = letter + reverse_string
    # Complete the if-statement to compare the "new_string" to the
    # "reverse_string". Remember that Python is case-sensitive when
    # creating the string comparison code. 
    if new_string == reverse_string:
        # If True, the "input_string" contains a palindrome.
        return True
    # Otherwise, return False.
    return False

print(is_palindrome("Never Odd or Even")) # Should be True
print(is_palindrome("abc")) # Should be False
print(is_palindrome("kayak")) # Should be True
```

***Solution 02***

```python
def convert_distance(miles):
    km = miles * 1.6
    result = "{} miles equals {:.1f} km".format(miles, km)
    return result

print(convert_distance(12)) # Should be: 12 miles equals 19.2 km
print(convert_distance(5.5)) # Should be: 5.5 miles equals 8.8 km
print(convert_distance(11)) # Should be: 11 miles equals 17.6 km
```

***Solution 03***

- [x] `print(Weather[:4])`

***Solution 04***

```python
def nametag(first_name, last_name):
    return("{} {}.".format(first_name, last_name[0]))

print(nametag("Jane", "Smith"))
# Should display "Jane S."
print(nametag("Francesco", "Rinaldi"))
# Should display "Francesco R."
print(nametag("Jean-Luc", "Grand-Pierre"))
# Should display "Jean-Luc G."
```

***Solution 05***

```python
def replace_ending(sentence, old, new):
    # Check if the old substring is at the end of the sentence 
    if sentence.endswith(old):
        # Using i as the slicing index, combine the part
        # of the sentence up to the matched string at the 
        # end with the new string
        i = -1*len(old)
        new_sentence = sentence[:i] + new
        return new_sentence
    # Return the original sentence if there is no match 
    return sentence
    
print(replace_ending("It's raining cats and cats", "cats", "dogs")) 
# Should display "It's raining cats and dogs"
print(replace_ending("She sells seashells by the seashore", "seashells", "donuts")) 
# Should display "She sells seashells by the seashore"
print(replace_ending("The weather is nice in May", "may", "april")) 
# Should display "The weather is nice in May"
print(replace_ending("The weather is nice in May", "May", "April")) 
# Should display "The weather is nice in April"
```

### 04.02 Lists

#### 04.02.17 Practice Quiz: Lists

***Solution 01***

```python
filenames = ["program.c", "stdio.hpp", "sample.hpp", "a.out", "math.hpp", "hpp.out"]
# Generate new_filenames as a list containing the new filenames using as many lines of code as your chosen method requires.
new_filenames = []
for filename in filenames:
    if filename.endswith("hpp"):
        new_filenames.append(filename[:filename.index(".") + 1] + "h")
    else:
        new_filenames.append(filename)

print(new_filenames)
# Should be ["program.c", "stdio.h", "sample.h", "a.out", "math.h", "hpp.out"]
```

***Solution 02***

```python
filenames = ["program.c", "stdio.hpp", "sample.hpp", "a.out", "math.hpp", "hpp.out"]
# Generate new_filenames as a list containing the new filenames using as many lines of code as your chosen method requires.
# Start your code here
new_filenames = [filename[:filename.index(".") + 1] + "h" if filename.endswith("hpp") else filename for filename in filenames]
print(new_filenames) 
# Should print ["program.c", "stdio.h", "sample.h", "a.out", "math.h", "hpp.out"]
```

***Solution 03***

```python
def pig_latin(text):
  say = ""
  # Separate the text into words
  # new_word = []
  words = text.split()
  for word in words:
    # Create the pig latin word and add it to the list
    # new_word.append(word[1:] + word[0] + "ay")
    say += word[1:] + word[0] + "ay" + " "
    # Turn the list back into a phrase
  return say.strip()
    
print(pig_latin("hello how are you")) # Should be "ellohay owhay reaay ouyay"
print(pig_latin("programming in python is fun")) # Should be "rogrammingpay niay ythonpay siay unfay"
```

***Solution 04***

- [x] `list.insert(index, x)`

***Solution 05***

- [x] A tuple is immutable

***Solution 06***

```python
def biography_list(people):
    # Iterate over each "person" in the given "people" list of tuples. 
    for person in people: 
        # Separate the 3 items in each tuple into 3 variables:
        # "name", "age", and "profession"   
        name, age, profession = person 
        # Format the required sentence and place the 3 variables 
        # in the correct placeholders using the .format() method.
        print("{} is {} years old and works as {}".format(name, age, profession))

# Call to the function:
biography_list([("Ira", 30, "a Chef"), ("Raj", 35, "a Lawyer"), ("Maria", 25, "an Engineer")])
# Output should match:
# Ira is 30 years old and works as a Chef
# Raj is 35 years old and works as a Lawyer
# Maria is 25 years old and works as an Engineer
```

### 04.03 Dictionaries

#### 04.03.09 Practice Quiz: Dictionaries

***Solution 01***

```python
def email_list(domains):
    emails = []
    for domain, users in domains.items():
      for user in users:
        emails.append(f"{user}@{domain}")
    return(emails)

print(email_list({"gmail.com": ["clark.kent", "diana.prince", "peter.parker"], "yahoo.com": ["barbara.gordon", "jean.grey"], "hotmail.com": ["bruce.wayne"]}))
```

***Solution 02***

```python
def groups_per_user(group_dictionary):
    user_groups = {}
    # Go through group_dictionary
    for group, users in group_dictionary.items():
        # Now go through the users in the group
        for user in users:
            # Now add the group to the the list of groups for this user,
            # creating the entry in the dictionary if necessary
            if user in user_groups:
                user_groups[user].append(group)
            else:
                user_groups[user] = [group]

    return(user_groups)

print(groups_per_user({"local": ["admin", "userA"], "public":  ["admin", "userB"], "administrator": ["admin"] }))
```

***Solution 03***

- [x] `{'shirt': ['red', 'blue', 'white'], 'jeans': ['white'], 'scarf': ['yellow'], 'socks': ['black', 'brown']}`

***Solution 04***

- [x] It’s quicker and easier to find a specific element in a dictionary

***Solution 05***

```python
def add_prices(basket):
    # Initialize the variable that will be used for the calculation
    total = 0
    # Iterate through the dictionary items
    for price in basket.values():
        # Add each price to the total calculation
        # Hint: how do you access the values of
        # dictionary items?
        total += price
    # Limit the return value to 2 decimal places
    return round(total, 2)

groceries = {"bananas": 1.56, "apples": 2.50, "oranges": 0.99, "bread": 4.59,
    "coffee": 6.99, "milk": 3.39, "eggs": 2.98, "cheese": 5.44}

print(add_prices(groceries)) # Should print 28.44
```

### Module 04 Review

#### 04.05.05 Quiz: Module 04 Graded Assessment

***Solution 01***

```python
def format_address(address_string):
    house_number = ""
    street_name = ""
    ## Separate the house number from the street name
    address_parts = address_string.split()
    
    for address_part in address_parts:
        ## Complete the if-statement with a string method  
        if address_part.isnumeric():
          house_number = address_part
        else:
          street_name += address_part + " "
    ## Remove the extra space at the end of the last "street_name"
    street_name = street_name.strip()
 
    ## Use a string method to return the required formatted string.
    return f"House number {house_number} on a street named {street_name}"

print(format_address("123 Main Street"))
## Output: "House number 123 on a street named Main Street"
print(format_address("1001 1st Ave"))
## Output: "House number 1001 on a street named 1st Ave"
print(format_address("55 North Center Drive"))
## Output: "House number 55 on a street named North Center Drive"
```

***Solution 02***

```python
def highlight_word(sentence, word):
    # Complete the return statement using a string method.
    return sentence.replace(word, word.upper())

print(highlight_word("Have a nice day", "nice"))
# Should print: "Have a NICE day"
print(highlight_word("Shhh, don't be so loud!", "loud"))
# Should print: "Shhh, don't be so LOUD!"
print(highlight_word("Automating with Python is fun", "fun"))
# Should print: "Automating with Python is FUN"
```

***Solution 03***

```python
def sort_distance(distances):
    # Sort the list
    # Reverse the order of the list
    distances.sort(reverse=True) 
    return distances

print(sort_distance([2,4,0,15,8,9]))
# Should print [15, 9, 8, 4, 2, 0]
```

***Solution 04***

```python
def even_numbers(first, last):
  return [num for num in range(first, last) if num%2==0]

print(even_numbers(4, 14)) ## Output: [4, 6, 8, 10, 12]
print(even_numbers(0, 9)) ## Output: [0, 2, 4, 6, 8]
print(even_numbers(2, 7)) ## Output: [2, 4, 6]
```

***Solution 05***

```python
def countries(countries_dict):
    result = ""
    ## Complete the for loop to iterate through the dictionary key and value items
    for countries in countries_dict.values():
        ## Use a string method to format the required string
        result += str(countries) + "\n"
    return result.strip()

print(countries({"Africa": ["Kenya", "Egypt", "Nigeria"], 
    "Asia":["China", "India", "Thailand"], 
    "South America": ["Ecuador", "Bolivia", "Brazil"]}))
## Output:
## ['Kenya', 'Egypt', 'Nigeria']
## ['China', 'India', 'Thailand']
## ['Ecuador', 'Bolivia', 'Brazil']
```

***Solution 06***

```python
def setup_guests(guest_list):
    # loop over the guest list and add each guest to the dictionary with
    # an initial value of 0
    result = {} # Initialize a new dictionary 
    for guest in guest_list: # Iterate over the elements in the list 
        result[guest] = 0 # Add each list element to the dictionary as a key with 
            # the starting value of 0
    return result

guests = ["Adam","Camila","David","Jamal","Charley","Titus","Raj","Noemi","Sakira","Chidi"]
print(setup_guests(guests))
# Should print {'Adam': 0, 'Camila': 0, 'David': 0, 'Jamal': 0, 'Charley': 0, 'Titus': 0, 'Raj': 0, 'Noemi': 0, 'Sakira': 0, 'Chidi': 0}
```

***Solution 07***

```python
def count_letters(text):
  ## Initialize a new dictionary
  dictionary = {}
  ## Complete the for loop to iterate through each "text" character and 
  ## use a string method to ensure all letters are lowercase.
  for ch in text.lower():   
    ## Complete the if-statement using a string method to check if the
    ## character is a letter.
    if ch.isalpha():
      ## Complete the if-statement using a logical operator to check if 
      ## the letter is not already in the dictionary.
      if ch not in dictionary: 
          ## Use a dictionary operation to add the letter as a key
          ## and set the initial count value to zero.
          dictionary[ch] = 0
      ## Use a dictionary operation to increment the letter count value 
      ## for the existing key.
      dictionary[ch] += 1 ## Increment the letter counter 
  return dictionary


print(count_letters("AaBbCc"))
## Output: {'a': 2, 'b': 2, 'c': 2}
print(count_letters("Math is fun! 2+2=4"))
## Output: {'m': 1, 'a': 1, 't': 1, 'h': 1, 'i': 1, 's': 1, 'f': 1, 'u': 1, 'n': 1}
print(count_letters("This is a sentence."))
## Output: {'t': 2, 'h': 1, 'i': 2, 's': 3, 'a': 1, 'e': 3, 'n': 2, 'c': 1}
```

***Solution 08***

- [x] `bor, hini, Lamborg`

***Solution 09***

- [x] `['rock', 'pop', 'country', 'blues']`

***Solution 10***

- [x] `dict_values(['Aniyah Cook', 'Ines Bisset', 'Wayne Branon'])`

---

### Module 05 Final Project

#### 05.01.13 Quiz: Module 05 Graded Assessment

***Solution 01***

- [x] To write code that will solve the problem in a clear and concise way
- [x] To identify the inputs and outputs of the problem
- [x] Ensure that you are writing a script that is efficient and effective

***Solution 02***

- [x] 1, 2, 3, 4, 5

***Solution 03***

- [x] The `sorted()` method

***Solution 04***

- [x] `reverse = True`

***Solution 05***

- [x] `['Ray', 'Alex', 'Kelly', 'Carlos']`

***Solution 06***

- [x] A dictionary

***Solution 07***

- [x] Allows code to be modified more easily
- [x] Improves code debugging
- [x] Processes data more easily

***Solution 08***

- [x] To execute a block of code only if a certain condition is true

***Solution 09***

- [x] To execute a block of code if a specific condition is true, otherwise execute an alternative block of code.

***Solution 10***

- [x] To create a list of all users currently logged into any machine and the machine they're logged into.
