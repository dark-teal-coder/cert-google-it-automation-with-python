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
