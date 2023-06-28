# Crash Course on Python

## Week 1 >> Week 1 Graded Assessment

**Question 01**

Step-by-step instructions on how to complete a set of tasks, to be executed by a computer.

**Question 02**

Multiple answers:
[x] Similar to human language, programming languages use syntax and semantics.
[x] Programming languages are used to write computer programs and scripts.
[x] Some common programming languages include Python, Java, C, C++, C#, and R.

**Question 03**

Multiple answers:
[x] Detecting and removing duplicate data
[x] Updating specific files on multiple computers

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
