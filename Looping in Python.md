#### Basics of Loops:

### For Loops: Start with simple for loops to iterate.



Here's a step-by-step guide to learning Python loops from scratch to advanced levels, covering both `for` and `while` loops with examples.

### 1. Basic Concepts of Loops

#### What is a Loop?
A loop is a programming structure that repeats a block of code until a specific count or condition is met. Python has two main types of loops:
- **For loop**: Iterates over a sequence (e.g., list, string, range).
- **While loop**: Repeats as long as a given condition is `True`.

---

### 2. The `for` Loop

#### Syntax of `for` Loop
```python
for variable in sequence:
    # code block
```

#### Example: Basic `for` Loop
Loop through a list of numbers.
```python
numbers = [1, 2, 3, 4]
for number in numbers:
    print(number)
```

#### Explanation:
- `variable`: A temporary placeholder for each item in the `sequence`.
- `sequence`: The list or range you’re iterating over.

---

### 3. The `while` Loop

#### Syntax of `while` Loop
```python
while condition:
    # code block
```

#### Example: Basic `while` Loop
Count up to a specified number.
```python
count = 1
while count <= 5:
    print(count)
    count += 1
```

#### Explanation:
- `condition`: Checked before each loop iteration. If `True`, the loop runs; if `False`, it stops.
- `count += 1`: Increments `count` by 1 after each loop.

---

### 4. Loop Control Statements

#### `break` Statement
- Stops the loop immediately.
```python
for number in range(1, 10):
    if number == 5:
        break
    print(number)
```

#### `continue` Statement
- Skips the current iteration and moves to the next.
```python
for number in range(1, 10):
    if number == 5:
        continue
    print(number)
```

---

### 5. Using `for` Loop with `range()`

#### Example: Loop with `range()`
```python
for i in range(5):
    print(i)  # Outputs 0, 1, 2, 3, 4
```

#### Example: Specifying Start, Stop, and Step
```python
for i in range(1, 10, 2):
    print(i)  # Outputs 1, 3, 5, 7, 9
```

---

### 6. Nested Loops

#### Example: Nested `for` Loop
```python
for i in range(1, 3):
    for j in range(1, 3):
        print(f"i = {i}, j = {j}")
```

---

### 7. Advanced `while` Loop with Conditions

#### Example: `while` Loop with Multiple Conditions
```python
count = 0
while count < 10:
    if count == 5:
        print("Count is 5, skipping.")
        count += 1
        continue
    print(count)
    count += 1
```

---

### 8. Using `else` with Loops

#### Example: `for` Loop with `else`
```python
for i in range(5):
    print(i)
else:
    print("Loop completed.")
```

---

### 9. Infinite Loops (Use with Caution)

#### Example: Infinite `while` Loop
```python
while True:
    print("This will run forever!")
    break  # Add break to stop the loop
```

---

### 10. Practical Examples of Loops

#### Example: Summing Numbers with a `for` Loop
```python
total = 0
for i in range(1, 6):
    total += i
print("Sum:", total)  # Outputs 15
```

#### Example: Counting Occurrences in a List with `while`
```python
values = [1, 2, 2, 3, 2, 4, 5]
target = 2
count = 0
i = 0
while i < len(values):
    if values[i] == target:
        count += 1
    i += 1
print("Count of 2:", count)  # Outputs 3
```

---

These steps cover essential, intermediate, and advanced loop concepts in Python. Practice each level to gain confidence in handling loops effectively!


```python
# For loop
numbers = [1, 2, 3, 4]
for number in numbers:
    print(number)
```

    1
    2
    3
    4
    


```python
#While loop
count = 1
while count <= 5:
    print(count)
    count += 1
```

    1
    2
    3
    4
    5
    


```python
# Break Statement
for number in range(1, 10):
    if number == 5:
        break
    print(number)
```

    1
    2
    3
    4
    


```python
for number in range(1, 10):
    if number == 5:
        break
    print(number)
```

    1
    2
    3
    4
    


```python
# Continue statement
for number in range(1, 10):
    if number == 5:
        continue
    print(number)
```

    1
    2
    3
    4
    6
    7
    8
    9
    


```python
# 5. Using for Loop with range() Example: Loop with range()

for i in range(5):
    print(i)  # Outputs 0, 1, 2, 3, 4

```

    0
    1
    2
    3
    4
    


```python
#Example: Specifying Start, Stop, and Step

for i in range(1, 10, 2):
    print(i)  # Outputs 1, 3, 5, 7, 9
```

    1
    3
    5
    7
    9
    


```python
#Example: Nested for Loop

for i in range(1, 3):
    for j in range(1, 3):
        print(f"i = {i}, j = {j}")
```

    i = 1, j = 1
    i = 1, j = 2
    i = 2, j = 1
    i = 2, j = 2
    


```python

```


```python
# Example: while Loop with Multiple Conditions

count = 0
while count < 10:
    if count == 5:
        print("Count is 5, skipping.")
        count += 1
        continue
    print(count)
    count += 1
```

    0
    1
    2
    3
    4
    Count is 5, skipping.
    6
    7
    8
    9
    


```python

```


```python
#Using else with Loops
#Example: for Loop with else


for i in range(5):
    print(i)
else:
    print("Loop completed.")
```

    0
    1
    2
    3
    4
    Loop completed.
    


```python

```


```python
#Example: Infinite while Loop

while True:
    print("This will run forever!")
    break  # Add break to stop the loop
```

    This will run forever!
    


```python

```


```python
# Example: Summing Numbers with a for Loop


total = 0
for i in range(1, 6):
    total += i
print("Sum:", total)  # Outputs 15
```

    Sum: 15
    


```python

```


```python
# Example: Counting Occurrences in a List with while

values = [1, 2, 2, 3, 2, 4, 5]
target = 2
count = 0
i = 0
while i < len(values):
    if values[i] == target:
        count += 1
    i += 1
print("Count of 2:", count)  # Outputs 3
```

    Count of 2: 3
    


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python
for i in range(10):
    print(i)
```

    0
    1
    2
    3
    4
    5
    6
    7
    8
    9
    

 ### While Loops: Understand while loops and practice using conditions to control the loop.


```python
n=10
a=0
i=0
while(i<n):
    a+=10
    print(a)
    i+=1
    
# You need to initialise a and i both as here before start.
# Else for you may get error and for i you may get wrong output as not initialised.
```

    10
    20
    30
    40
    50
    60
    70
    80
    90
    100
    

### 2. Loop Control Statements
##### Break: Exit the loop when a condition is met.
##### Continue: Skip the current iteration and continue with the next one.
##### Pass: Placeholder that does nothing but keeps the loop structure valid.


```python
for i in range(10):
    if i==3:
        print("Here the flow is broken for the particular iteration where i= 3")
        continue;
        print("it is forced to continue the loop but not the loop body anymore...")
    elif i==5:
        print("Here the whole loop is broken, though the iteration till pending.")
        break
        print("No more execution of the loop")
    print(i)
```

    0
    1
    2
    Here the flow is broken for the particular iteration where i= 3
    4
    here the whole loop is broken, though the iteration till pending.
    


```python
# Example of pass in a for loop
for i in range(5):
    if i == 2:
        # Placeholder for future code when i equals 2
        pass
    else:
        print("Processing number:", i)

```

    Processing number: 0
    Processing number: 1
    Processing number: 3
    Processing number: 4
    

The `pass` statement is often used as a placeholder in Python when you want to write code but haven’t implemented it yet. It does nothing and allows you to maintain the syntax structure of loops, functions, classes, or conditionals without running any code in those blocks. This can be especially useful if you’re planning to add functionality later.

### Explanation

In this example:
- When `i` is `2`, the `pass` statement does nothing, so the loop skips any action for that condition.
- For other values of `i`, the `print` statement runs as usual.

This code is helpful when you have not yet decided what to do in certain cases but want to keep the loop structure intact.

## Combined output of break, continue and pass


```python
for i in range(1, 6):
    if i == 2:
        pass  # Placeholder, does nothing; loop will continue as normal
        print(i)
        print("Pass - Do not stop the current iteration body")
    elif i == 3:
        print("i=",i)
        continue  # Skip the rest of this iteration, move to the next iteration
        print(i)
        print("Continue - Stop the current iteratio body.")
    elif i == 5:
        break  # Exit the loop entirely
        print(i)
        print("Break the comlete loop")
    print(f"Processing number: {i}")

```

    Processing number: 1
    2
    Pass - Do not stop the current iteration body
    Processing number: 2
    i= 3
    Processing number: 4
    

## Question 1
#### Write a program to find the largest, smallest and middle value out of three numbers.


```python
#Simple For-Loop Approach

# Input: Three numbers
numbers = [int(input("Enter first number: ")), 
           int(input("Enter second number: ")), 
           int(input("Enter third number: "))]

# Initialize variables to hold the largest, middle, and smallest values
largest = numbers[0]
smallest = numbers[0]

# Find the largest and smallest numbers using a simple for-loop
for num in numbers:
    if num > largest:
        largest = num
    if num < smallest:
        smallest = num

# The middle value is the one that is neither the smallest nor the largest
for num in numbers:
    if num != largest and num != smallest:
        middle = num

print(f"Largest: {largest}")
print(f"Middle: {middle}")
print(f"Smallest: {smallest}")

```

    Enter first number: 1
    Enter second number: 2
    Enter third number: 3
    Largest: 3
    Middle: 2
    Smallest: 1
    


```python
# Advanced Approach (Using Python's Built-In Functions)

# Input: Three numbers
numbers = [int(input("Enter first number: ")), 
           int(input("Enter second number: ")), 
           int(input("Enter third number: "))]

# Sort the list to get smallest, middle, and largest values
numbers.sort()

# Extract values after sorting
smallest = numbers[0]
middle = numbers[1]
largest = numbers[2]

print(f"Largest: {largest}")
print(f"Middle: {middle}")
print(f"Smallest: {smallest}")

```

    Enter first number: 3
    Enter second number: 6
    Enter third number: 9
    Largest: 9
    Middle: 6
    Smallest: 3
    

## Question 2
#### Write a program to find the largest, smallest and middle value out of five numbers.


```python
# Input: Five values
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
c = int(input("Enter third number: "))
d = int(input("Enter fourth number: "))
e = int(input("Enter fifth number: "))

# Initialize variables to hold the values
numbers = [a, b, c, d, e]

# Initialize the smallest and largest with the first value
smallest = numbers[0]
largest = numbers[0]
total_sum = 0  # For calculating the middle value later

# Iterate through each number to find the smallest and largest
for num in numbers:
    if num < smallest:
        smallest = num
    if num > largest:
        largest = num
    total_sum += num  # Sum up all numbers

# Calculate the middle value by excluding the smallest and largest
middle_sum = total_sum - smallest - largest
# Calculate average of remaining values for the middle value
middle_value = middle_sum / 3

print(f"Largest: {largest}")
print(f"Smallest: {smallest}")
print(f"Middle (average of remaining three values): {middle_value}")

```

    Enter first number: 5
    Enter second number: 9
    Enter third number: 7
    Enter fourth number: 2
    Enter fifth number: 0
    Largest: 9
    Smallest: 0
    Middle (average of remaining three values): 4.666666666666667
    

### Explanation

1. **Initialize** the smallest and largest values to the first value in the list.
2. **Loop through** each number to find the smallest and largest values.
3. **Sum up** all numbers to calculate the middle values later.
4. **Exclude** the largest and smallest values to get the middle three values.
5. **Print** the largest, smallest, and middle values.

This approach provides the largest and smallest values directly and computes the average of the middle three values for simplicity.


```python
numbers = [int(input("Enter 1st number")),int(input("Enter 2nd number")),int(input("Enter 3rd number"))]

largest = numbers[0]
smallest = numbers[0]

for num in numbers:
    if num>largest:
        largest = num
    if num<smallest:
        smallest = num
        
for num in numbers:
    if num!= largest and num!= smallest:
        middle=num
        
print("Largest=",largest)
print("Middle=",middle)
print("Smallest=",smallest)
```

    Enter 1st number1000
    Enter 2nd number3000
    Enter 3rd number100000
    Largest= 100000
    Middle= 3000
    Smallest= 1000
    

## Question 3
### pattern
    


```python
for i in range(1,10):
    for j in range(i,10):
        print("*",end='')
    print()
        
```

    *********
    ********
    *******
    ******
    *****
    ****
    ***
    **
    *
    


```python
for i in range(10):
    for j in range(1,i):
        print("*",end='')
    print()
```

    
    
    *
    **
    ***
    ****
    *****
    ******
    *******
    ********
    


```python
# Factorial:

fact =1
for i in range(1,4):
    fact*=i
print(fact)
```

    6
    


```python
# Square each value present in a list without using any other empty list.

l1 = [1,2,3,4,5]
for i in range(len(l1)):
    l1[i]=l1[i]**2
print(l1)
```

    [1, 4, 9, 16, 25]
    


```python
# 
l1=[10,20,30,40,50]
l1=[(i*2) for i in l1]
print(l1)

```

    [20, 40, 60, 80, 100]
    


```python

```
