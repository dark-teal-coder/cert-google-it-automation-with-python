# Solutions to Problems in Crash Course on Python

## Week 1

### Course Introduction

### Introduction to Programming

#### Practice Quiz: Introduction to Programming

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

### Introduction to Python

#### Practice Quiz: Introduction to Python

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

### Hello World

#### Practice Quiz: Hello World

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

### Module 1 Review

#### Week 1 Graded Assessment

***Solution 01***

- [x] Step-by-step instructions on how to complete a set of tasks, to be executed by a computer.

***Solution 02***

Multiple answers:

- [x] Similar to human language, programming languages use syntax and semantics.
- [x] Programming languages are used to write computer programs and scripts.
- [x] Some common programming languages include Python, Java, C, C++, C#, and R.

***Solution 03***

Multiple answers:

- [x] Detecting and removing duplicate data
- [x] Updating specific files on multiple computers

***Solution 04***

- [x] Syntax

***Solution 05***

- [x] Code is similar to the English language.

***Solution 06***

```python
print("I am writing Python code!")
```

***Solution 07***

- [x] 3.16

***Solution 08***

```python
## Output: 525600
print(365*24*60)
```

***Solution 09***

```python
## Output: 100000000
# print(10*10*10*10*10*10*10*10)
print(10**8)
```

***Solution 10***

```python
total_computers = 30*20
replacement_cycle = 5
computers_per_year = total_computers / replacement_cycle
## Output: 120.0
print(computers_per_year)
```

## Week 2

### Expressions and Variables

#### Practice Quiz: Expressions and Variables

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

### Functions

#### Practice Quiz: Functions

***Solution 01***

```python
# 1) Complete the function to return the result of the conversion
def convert_distance(miles):
    km = miles * 1.6  # approximately 1.6 km in 1 mile
    return km

my_trip_miles = 55

# 2) Convert my_trip_miles to kilometers by calling the function above
my_trip_km = convert_distance(my_trip_miles)

# 3) Fill in the blank to print the result of the conversion
print("The distance in kilometers is " + str(my_trip_km))

# 4) Calculate the round-trip in kilometers by doubling the result,
#    and fill in the blank to print the result
print("The round-trip in kilometers is " + str(my_trip_km * 2))
```

***Solution 02***

```python
# This function compares two numbers and returns them in increasing order.
def order_numbers(number1, number2):
    if number2 > number1:
        return number1, number2
    else:
        return number2, number1

# Fill in the blanks so the print statement displays the result of the function call
smaller, bigger = order_numbers(100, 99)
print(smaller, bigger)
```

***Solution 03***

- [x] Parameters

***Solution 04***

```python
def print_seconds(hours, minutes, seconds):
    print(hours*3600+minutes*60+seconds)


print_seconds(1,20,30)
```

***Solution 05***

- [x] Used to define a new function

### Conditionals

#### Practice Quiz: Conditionals

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

### Module 2 Review

#### Week 2 Graded Assessment

***Solution 01***

```python
IP_address = "192.168.1.10"
host_name = "Printer Server 1"
## Output: "192.168.1.10 is the IP address of Printer Server 1"
print(IP_address + " is the IP address of " + host_name)
```

***Solution 02***

- [x] False

***Solution 03***

- [x] A comparison

***Solution 04***

```python
def speeding_ticket(speed):
    if speed >= 80:
        ticket = "Reckless Driving"
    elif speed > 65:
        ticket = "Speeding"
    else:
        ticket = "Safe"
    return ticket


print(speeding_ticket(87)) ## Output: "Reckless Driving"
print(speeding_ticket(66)) ## Output: "Speeding"
print(speeding_ticket(65)) ## Output: "Safe"
print(speeding_ticket(85)) ## Output: "Reckless Driving"
print(speeding_ticket(35)) ## Output: "Safe"
print(speeding_ticket(77)) ## Output: "Speeding"
```

***Solution 05***

- [x] 15

***Solution 06***

```python
def identify_IP(IP_address):
    if IP_address == "192.168.1.1":
        IP_description = "Network router"
    elif IP_address == "8.8.8.8" or IP_address == "8.8.4.4":
        IP_description = "Google DNS server"
    elif IP_address == "142.250.191.46":
        IP_description = "Google.com"
    else:
        IP_description = "unknown"
    return IP_description


print(identify_IP("8.8.4.4")) ## Output: "Google DNS server"
print(identify_IP("142.250.191.46")) ## Output: "Google.com"
print(identify_IP("192.168.1.1")) ## Output: "Network router"
print(identify_IP("8.8.8.8")) ## Output: "Google DNS server"
print(identify_IP("10.10.10.10")) ## Output: "unknown"
print(identify_IP("")) ## Output: "unknown"
```

***Solution 07***

- [x] 2

***Solution 08***

- [x] False

***Solution 09***

```python
def make_positive(number):
    if number < 0:
        result = number * -1 
    else:
        result = number
    return result


print(make_positive(-4)) ## Output: 4
print(make_positive(0)) ## Output: 0
print(make_positive(-.25)) ## Output: 0.25
print(make_positive(5)) ## Output: 5
```

***Solution 10***

- [x] Self-documenting code

## Week 3

### While Loops

#### Practice Quiz: While Loops

***Solution 01***

- [x] while loops tell the computer to repeatedly execute a set of instructions while a condition is true.

***Solution 02***

- [x] Change the value of a variable used in the while condition
- [x] Use the break keyword

***Solution 03***

```python
def is_power_of_two(number):
  # This while loop checks if the "number" can be divided by two
  # without leaving a remainder. How can you change the while loop to
  # avoid a Python ZeroDivisionError?
  while number % 2 == 0:
    if number == 0:
      return False
      break
    number = number / 2
  # If after dividing by 2 "number" equals 1, then "number" is a power
  # of 2.
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
# Fill in the blanks so that the while loop continues to run while the
# "divisor" variable is less than the "number" parameter.

def sum_divisors(number):
# Initialize the appropriate variables
  divisor = 1
  total = 0

  # Avoid dividing by 0 and negative numbers in the while loop by
  # exiting the function if "number" is less than one
  if number < 1:
    return 0

  # Complete the while loop
  while divisor < number:
    if number % divisor == 0:
      total += divisor
    # Increment the correct variable
    divisor += 1

  # Return the correct variable
  return total


print(sum_divisors(0)) # Should print 0
print(sum_divisors(3)) # Should print 1
# 1
print(sum_divisors(36)) # Should print 1+2+3+4+6+9+12+18
# 55
print(sum_divisors(102)) # Should print 1+2+3+6+17+34+51
# 114
```

***Solution 05***

```python
def multiplication_table(number):
    # Initialize the appropriate variable
    multiplier = 1

    # Complete the while loop condition.
    while multiplier <= 5:
        result = number * multiplier
        if  result > 25 :
            # Enter the action to take if the result is greater than 25
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

### For Loops

#### Practice Quiz: For Loops

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

### Recursion (Optional)

#### Practice Quiz: Recursion

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
    if number == 1:
      return True
    else:
      return False
  # Recursive case: keep dividing number by base.
  return is_power_of(number/base, base)

print(is_power_of(8,2)) # Should be True
print(is_power_of(64,4)) # Should be True
print(is_power_of(70,10)) # Should be False
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

### Module 3 Review

#### Week 3 Graded Assessment

***Solution 01***

```python
## Initialize the variable
number = 15 
while number >= 5: 
    print(number, end=" ")
    ## Decrement the variable
    number -= 5 

## Output: 15 10 5
```

***Solution 02***

```python
for number in range(2, 12+1):
    if number % 2 == 0:
        print(number)

## Output:
## 2
## 4
## 6
## 8
## 10
## 12
```

***Solution 03***

```python
def even_numbers(n):
    count = 0
    current_number = 0
    while current_number <= n: ## Complete the while loop condition
        if current_number % 2 == 0:
            count += 1 ## Increment the appropriate variable
        current_number += 1 ## Increment the appropriate variable
    return count


print(even_numbers(25)) ## Output: 13
print(even_numbers(144)) ## Output: 73
print(even_numbers(1000)) ## Output: 501
print(even_numbers(0)) ## Output: 1
```

***Solution 04***

```python
def rows_asterisks(rows):
    ## Complete the outer loop range to control the number of rows
    for x in range(rows): 
        ## Complete the inner loop range to control the number of asterisks per row
        for y in range(x+1): 
            ## Print 1 asterisk and 1 space
            print("*", end=" ")
        ## An empty print() function inserts a line break at the end of the row 
        print()


rows_asterisks(5)
```

***Solution 05***

```python
def countdown(start):
    x = start
    if x > 0:
        return_string = "Counting down to 0: "
        while x >= 0: ## Complete the while loop
            return_string += str(x) ## Add the numbers to the "return_string"
            if x > 0:
                return_string += ","
            x -= 1 ## Decrement the appropriate variable
    else:
        return_string = "Cannot count down to 0"
    return return_string


print(countdown(10)) ## Output: "Counting down to 0: 10,9,8,7,6,5,4,3,2,1,0"
print(countdown(2)) ## Output: "Counting down to 0: 2,1,0"
print(countdown(0)) ## Output: "Cannot count down to 0"
```

***Solution 06***

```python
def odd_numbers(maximum):
    ## Initialize variable as a string
    return_string = ""
    ## Complete the for loop with a range that includes all odd numbers 
    ## up to and including the "maximum" value.
    for num in range(0, maximum+1): 
        ## Complete the body of the loop by appending the odd number
        ## followed by a space to the "return_string" variable.
        if num % 2 == 1:
            return_string += str(num) + " " 
    ## strip() will remove the final " " space at the end of the "return_string".
    return return_string.strip()


print(odd_numbers(6)) ## Output: 1 3 5
print(odd_numbers(10)) ## Output: 1 3 5 7 9
print(odd_numbers(1)) ## Output: 1
print(odd_numbers(3)) ## Output: 1 3
print(odd_numbers(0)) ## No numbers displayed
```

***Solution 07***

- [x] Will produce a NameError stating the variable is not defined

***Solution 08***

- [x] 2

***Solution 09***

- [x] 8

***Solution 10***

- [x] Variable "x" is assigned the value 1 in every loop

## Week 4

### Strings

#### Practice Quiz: Strings

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
    for letter in input_string:

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
    if new_string.lower() == reverse_string.lower():
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
    # Check if the old string is at the end of the sentence
    if old == sentence[-len(old):]:
        # Using i as the slicing index, combine the part
        # of the sentence up to the matched string at the end with the new string
        i = -len(old)
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

### Lists

#### Practice Quiz: Lists

***Solution 01***

```python
filenames = ["program.c", "stdio.hpp", "sample.hpp", "a.out", "math.hpp", "hpp.out"]
# Generate newfilenames as a list containing the new filenames
# using as many lines of code as your chosen method requires.
newfilenames = []
for i, item in enumerate(filenames):
    if item.endswith(".hpp"):
        newfilenames.append(item.replace(".hpp", ".h"))
    else:
        newfilenames.append(item)

print(newfilenames)
# Should be ["program.c", "stdio.h", "sample.h", "a.out", "math.h", "hpp.out"]
```

***Solution 02***

```python
def pig_latin(text):
  say = ""
  # Separate the text into words
  words = text.split()
  for word in words:
    # Create the pig latin word and add it to the list
    say += word[1:] + word[0] + "ay" + " " if word != words[-1] else word[1:] + word[0] + "ay"
    # Turn the list back into a phrase
  return say

print(pig_latin("hello how are you")) # Should be "ellohay owhay reaay ouyay"
print(pig_latin("programming in python is fun")) # Should be "rogrammingpay niay ythonpay siay unfay"
```

***Solution 03***

- [x] `list.insert(index, x)`

***Solution 04***

- [x] A tuple is immutable

***Solution 05***

```python
def group_list(group, users):
  members = ", ".join(users)
  return "{}: {}".format(group, members)

print(group_list("Marketing", ["Mike", "Karen", "Jake", "Tasha"])) # Should be "Marketing: Mike, Karen, Jake, Tasha"
print(group_list("Engineering", ["Kim", "Jay", "Tom"])) # Should be "Engineering: Kim, Jay, Tom"
print(group_list("Users", "")) # Should be "Users:"
```

***Solution 06***

```python
def guest_list(guests):
    for name, age, pro in guests:
        print("{} is {} years old and works as {}".format(name, age, pro))

guest_list([('Ken', 30, "Chef"), ("Pat", 35, 'Lawyer'), ('Amanda', 25, "Engineer")])

"""
Output should match:
Ken is 30 years old and works as Chef
Pat is 35 years old and works as Lawyer
Amanda is 25 years old and works as Engineer
"""
```

### Dictionaries

#### Practice Quiz: Dictionaries

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

print(groups_per_user({"local": ["admin", "userA"],
        "public":  ["admin", "userB"],
        "administrator": ["admin"] }))
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

### Module 4 Review

#### Week 4 Graded Assessment

***Solution 01***

```python
def format_address(address_string):
    house_number = ""
    street_name = ""
    # Separate the house number from the street name.
    address_parts = address_string.split()

    for address_part in address_parts:
       # Complete the if-statement with a string method.
       if address_part.isnumeric():
         house_number = address_part
       else:
         street_name += address_part + " "
    # Remove the extra space at the end of the last "street_name".
    street_name = street_name.strip()

    # Use a string method to return the required formatted string.
    return f"House number {house_number} on a street named {street_name}"


print(format_address("123 Main Street"))
# Should print: "House number 123 on a street named Main Street"

print(format_address("1001 1st Ave"))
# Should print: "House number 1001 on a street named 1st Ave"

print(format_address("55 North Center Drive"))
# Should print "House number 55 on a street named North Center Drive"
```

***Solution 02***

```python
def string_words(string):
    # Complete the return statement using both a string operation and
    # a string method in a single line.
    return len(string.split())


print(string_words("Hello, World")) # Should print 2
print(string_words("Python is awesome")) # Should print 3
print(string_words("Keep going")) # Should print 2
print(string_words("Have a nice day")) # Should print 4
```

***Solution 03***

```python
def combine_lists(list1, list2):
  combined_list = [] # Initialize an empty list variable
  list1.reverse() # Reverse the order of "list1"
  list2 += list1 # Combine the two lists
  combined_list = list2
  return combined_list

Jaimes_list = ["Alma", "Chika", "Benjamin", "Jocelyn", "Oakley"]
Drews_list = ["Minna", "Carol", "Gunnar", "Malena"]


print(combine_lists(Jaimes_list, Drews_list))
# Should print ['Minna', 'Carol', 'Gunnar', 'Malena', 'Oakley', 'Jocelyn', 'Benjamin', 'Chika', 'Alma']
```

***Solution 04***

```python
def increments(start, end):
    return [n + 2 for n in range(start, end+1)] # Create the required list comprehension.


print(increments(2, 3)) # Should print [4, 5]
print(increments(1, 5)) # Should print [3, 4, 5, 6, 7]
print(increments(0, 10)) # Should print [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]
```

***Solution 05***

```python
def car_listing(car_prices):
  result = ""
  # Complete the for loop to iterate through the key and value items
  # in the dictionary.
  for car, price in car_prices.items():
    result += f"A {car} costs {price} dolloars.\n" # Use a string method to format the required string.
  return result

print(car_listing({"Kia Soul":19000, "Lamborghini Diablo":55000, "Ford Fiesta":13000, "Toyota Prius":24000}))

# Should print:
# A Kia Soul costs 19000 dollars
# A Lamborghini Diablo costs 55000 dollars
# A Ford Fiesta costs 13000 dollars
# A Toyota Prius costs 24000 dollars
```

***Solution 06***

```python
def setup_guests(guest_list):
    # loop over the guest list and add each guest to the dictionary with
    # an initial value of 0
    result = {} # Initialize a new dictionary
    for guest in guest_list: # Iterate over the elements in the list
        result.update({guest: 0}) # Add each list element to the dictionary as a key with the starting value of 0
    return result

guests = ["Adam","Camila","David","Jamal","Charley","Titus","Raj","Noemi","Sakira","Chidi"]

print(setup_guests(guests))
# Should print {'Adam': 0, 'Camila': 0, 'David': 0, 'Jamal': 0, 'Charley': 0, 'Titus': 0, 'Raj': 0, 'Noemi': 0, 'Sakira': 0, 'Chidi': 0}
```

***Solution 07***

```python
def setup_gradebook(old_gradebook):
  # Use a dictionary method to create a new copy of the "old_gradebook".
  new_gradebook = old_gradebook.copy()
    # Complete the for loop to iterate over the new gradebook.
  for name in new_gradebook.keys():
    # Use a dictionary operation to reset the grade values to 0.
    new_gradebook.update({name:0})
  return new_gradebook

fall_gradebook = {"James": 93, "Felicity": 98, "Barakaa": 80}
print(setup_gradebook(fall_gradebook))
# Should output {'James': 0, 'Felicity': 0, 'Barakaa': 0}
```

***Solution 08***

- [x] transc, nd

***Solution 09***

- [x] ['red', 'white', 'yellow', 'blue']

***Solution 10***

- [x] ['Aniyah Cook', 'Ines Bisset', 'Wayne Branon']

## Week 5

### Object-oriented Programming (Optional)

### Classes and Methods (Optional)

### Code Reuse

### Module 5 Review

#### Practice Notebook: Object Oriented Programming (Optional)

## Week 6

### Writing a Script from the Ground Up

### Course Wrap-Up
