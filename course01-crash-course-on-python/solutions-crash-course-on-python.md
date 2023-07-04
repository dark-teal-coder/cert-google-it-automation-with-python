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

- [x] General purpose scripting language

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

### Module Review

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
# It should print: 525600
print(365*24*60)
```

***Solution 09***

```python
## It should print: 100000000
# print(10*10*10*10*10*10*10*10)
print(10***8)
```

***Solution 10***

```python
total_computers = 30*20
replacement_cycle = 5
computers_per_year = total_computers / replacement_cycle

print(computers_per_year) # Should print 120.0
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

### Module Review

#### Week 2 Graded Assessment

***Solution 01***

```python
IP_address = "192.168.1.10"
host_name = "Printer Server 1"
print(IP_address + " is the IP address of " + host_name)
# Should print "192.168.1.10 is the IP address of Printer Server 1"
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


print(speeding_ticket(87)) # Should print Reckless Driving
print(speeding_ticket(66)) # Should print Speeding
print(speeding_ticket(65)) # Should print Safe
print(speeding_ticket(85)) # Should print Reckless Driving
print(speeding_ticket(35)) # Should print Safe
print(speeding_ticket(77)) # Should print Speeding
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


print(identify_IP("8.8.4.4")) # Should print 'Google DNS server'
print(identify_IP("142.250.191.46")) # Should print 'Google.com'
print(identify_IP("192.168.1.1")) # Should print 'Network router'
print(identify_IP("8.8.8.8")) # Should print 'Google DNS server'
print(identify_IP("10.10.10.10")) # Should print 'unknown'
print(identify_IP("")) # Should Should print 'unknown'
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


print(make_positive(-4))   # Should print 4
print(make_positive(0))    # Should print 0
print(make_positive(-.25)) # Should print 0.25
print(make_positive(5))    # Should print 5
```

***Solution 10***

- [x] Self-documenting code

## Week 3

### While Loops

### For Loops

### Recursion (Optional)

### Module Review

#### Week 3 Graded Assessment

***Solution 01***

```python
number = 15 # Initialize the variable
while number >= 5: # Complete the while loop condition
    print(number, end=" ")
    number -= 5 # Decrement the variable

# Should print 15 10 5
```

***Solution 02***

```python
for number in range(1, 5+1):
    if number % 2 == 0:
        print("even")
    else:
        print("odd")


# Should print:
# odd
# even
# odd
# even
# odd
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


print(factorial(3)) # Should print 6
print(factorial(9)) # Should print 362880
print(factorial(1)) # Should print 1
```

***Solution 04***

```python
def multiplication_table(start, stop):
    # Complete the outer loop range
    for x in range(1, 3+1):
         # Complete the inner loop range
        for y in range(1, 3+1):
            # Prints the value of "x" multiplied by "y"
            # and inserts a space after each value
            print(str(x*y), end=" ")
        # An empty print() function inserts a line break at the end of the row
        print()


multiplication_table(1, 3)
```

***Solution 05***

```python
def counter(start, stop):
    if start > stop:
        return_string = "Counting down: "
        while start >= stop: # Complete the while loop
            return_string += str(start) # Add the numbers to the "return_string"
            if start > stop:
                return_string += ","
            start -= 1 # Decrement the appropriate variable
    else:
        return_string = "Counting up: "
        while start <= stop: # Complete the while loop
            return_string += str(start) # Add the numbers to the "return_string"
            if start < stop:
                return_string += ","
            start += 1 # Increment the appropriate variable
    return return_string


print(counter(1, 10)) # Should be "Counting up: 1,2,3,4,5,6,7,8,9,10"
print(counter(2, 1)) # Should be "Counting down: 2,1"
print(counter(5, 5)) # Should be "Counting up: 5"
```

***Solution 06***

```python
def all_numbers(minimum, maximum):
    return_string = "" # Initializes variable as a string

    # Complete the for loop with a range that includes all
    # numbers up to and including the "maximum" value.
    for n in range(minimum, maximum+1):
        # Complete the body of the loop by appending the number
        # followed by a space to the "return_string" variable.
        return_string += str(n) + " "

    # This .strip command will remove the final " " space
    # at the end of the "return_string".
    return return_string.strip()


print(all_numbers(2,6))  # Should be 2 3 4 5 6
print(all_numbers(3,10)) # Should be 3 4 5 6 7 8 9 10
print(all_numbers(-1,1)) # Should be -1 0 1
print(all_numbers(0,5))  # Should be 0 1 2 3 4 5
print(all_numbers(0,0))  # Should be 0
```

***Solution 07***

- [x] The "sum" variable is initialized with the wrong value

***Solution 08***

- [x] 5

***Solution 09***

- [x] 0

***Solution 10***

- [x] When called with 0, it triggers an infinite loop

## Week 4

### Strings

### Lists

### Dictionaries

### Module Review

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

### Module Review

#### Practice Notebook: Object Oriented Programming (Optional)

## Week 6

### Writing a Script from the Ground Up

### Course Wrap-Up
