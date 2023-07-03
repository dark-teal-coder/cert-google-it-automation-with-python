# Crash Course on Python

## Week 1 >> Week 1 Graded Assessment

**Question 01**

Step-by-step instructions on how to complete a set of tasks, to be executed by a computer.

**Question 02**

Multiple answers:
- [x] Similar to human language, programming languages use syntax and semantics.
- [x] Programming languages are used to write computer programs and scripts.
- [x] Some common programming languages include Python, Java, C, C++, C#, and R.

**Question 03**

Multiple answers:
- [x] Detecting and removing duplicate data
- [x] Updating specific files on multiple computers

**Question 04**

Syntax

**Question 05**

Code is similar to the English language.

**Question 06**

```python
print("I am writing Python code!")
```

**Question 07**

3.16

**Question 08**

```python
# It should print: 525600
print(365*24*60)
```

**Question 09**

```python
## It should print: 100000000
# print(10*10*10*10*10*10*10*10)
print(10**8)
```

**Question 10**

```python
total_computers = 30*20
replacement_cycle = 5
computers_per_year = total_computers / replacement_cycle

print(computers_per_year) # Should print 120.0
```

## Week 2 >> Week 2 Graded Assessment

**Question 01**

```python
IP_address = "192.168.1.10"
host_name = "Printer Server 1"
print(IP_address + " is the IP address of " + host_name)
# Should print "192.168.1.10 is the IP address of Printer Server 1"
```

**Question 02**

False

**Question 03**

A comparison

**Question 04**

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

**Question 05**

15

**Question 06**

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

**Question 07**

2

**Question 08**

False

**Question 09**

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

**Question 10**

Self-documenting code

## Week 3 >> Week 3 Graded Assessment

**Question 01**

```python
number = 15 # Initialize the variable
while number >= 5: # Complete the while loop condition
    print(number, end=" ")
    number -= 5 # Decrement the variable

# Should print 15 10 5 
```

**Question 02**

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

**Question 03**

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

**Question 04**

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

**Question 05**

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

**Question 06**

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

**Question 07**

The "sum" variable is initialized with the wrong value

**Question 08**

5

**Question 09**

0

**Question 10**

When called with 0, it triggers an infinite loop

## Week 4 >> Week 4 Graded Assessment

**Question 01**

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

**Question 02**

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

**Question 03**

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

**Question 04**

```python
def increments(start, end):
    return [n + 2 for n in range(start, end+1)] # Create the required list comprehension.


print(increments(2, 3)) # Should print [4, 5]
print(increments(1, 5)) # Should print [3, 4, 5, 6, 7]
print(increments(0, 10)) # Should print [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]
```

**Question 05**

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

**Question 06**

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

**Question 07**

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

**Question 08**

transc, nd

**Question 09**

['red', 'white', 'yellow', 'blue']

**Question 10**

['Aniyah Cook', 'Ines Bisset', 'Wayne Branon'']
