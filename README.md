# Exp. No: 2a  
# Prime Number Test

## AIM  
To write a Python program to test whether a given number is prime or not.

## ALGORITHM  
1. Begin the program.  
2. Read an integer number `a` from the user.  
3. If `a` is less than or equal to 1, it is not a prime number.  
4. Else, assume the number is prime.  
5. Iterate from `2` to `sqrt(a)` and check if any number divides `a`:  
   - If divisible, set the flag as not prime and break the loop.  
6. If the flag remains true, print that the number is prime.  
7. Else, print that the number is not prime.  
8. Terminate the program.

## PROGRAM
```python
a = int(input())

if a <= 1:
    is_prime = False
else:
    is_prime = True
    for i in range(2, int(a**0.5) + 1):
        if a % i == 0:
            is_prime = False
            break

if is_prime:
    print(f"Given number {a} is a Prime Number")
else:
    print(f"Given number {a} is not a Prime Number")

```
### OUTPUT
![image](https://github.com/user-attachments/assets/baabaa4f-97c3-4b78-ae2a-b41919e50e20)

### RESULT
Thus, the Python program to test whether a given number is prime has been implemented and executed successfully.


# Experiment No: 2b Strong Number Check

## AIM  
To write a Python program to check if a number is a strong number using a function.

---

### ALGORITHM  
1. Begin the program.  
2. Define a function `strong(num)` to check if the given number is a strong number.
3. Inside the function:
   - Initialize a variable `sum1` to store the sum of the factorials of digits.
   - Copy the input number to a temporary variable `temp`.
   - Extract each digit of the number.
   - For each digit, calculate the factorial and add it to `sum1`.
4. Compare `sum1` with `temp`. If they are equal, the number is a strong number.
5. If the number is a strong number, print **"The number is a strong number"**. Otherwise, print **"The number is not a strong number"**.
6. Terminate the program.

---

### 🧾 PROGRAM

```python
def strong(num):
    sum1 = 0
    temp = num
    while(num):
        i = 1
        f = 1
        r = num % 10
        while(i <= r):
            f = f * i
            i = i + 1
        sum1 = sum1 + f
        num = num // 10
    if(sum1 == temp):
        print("The number is a strong number")
    else:
        print("The number is not a strong number")
    
n = int(input())
strong(n)
```

## OUTPUT
![image](https://github.com/user-attachments/assets/0b428a0c-cb1c-424e-a495-f98e8dfc8968)

## RESULT
Thus, the Python program to check if a number is a strong number using a function has been implemented and executed successfully.



# Experiment No: 2c Multiplication Using Lambda Function

## AIM  
To write a Python program that defines a function using a lambda expression to multiply two numbers.

---

### ALGORITHM  
1. Begin the program.  
2. Use `input()` to read the two numbers `a` and `b` from the user.
3. Convert the inputs to integers.
4. Create a lambda function that takes two arguments `a` and `b`, and returns their multiplication `a * b`.
5. Assign the lambda function to a variable `f`.
6. Call the function `f(a, b)` to compute the multiplication and print the result.
7. Terminate the program.

---

### 🧾 PROGRAM

```python
a = int(input())
b = int(input())

f = lambda a, b: a * b
print(f(a, b))
```

### OUTPUT
![image](https://github.com/user-attachments/assets/002dfc63-ee1f-48d9-878e-8b3075c9f652)

### RESULT
Thus, the Python program that defines a lambda function for multiplication of two numbers has been implemented and executed successfully.


# Experiment No: 2d Inverted Pyramid Pattern of Numbers

## AIM  
To write a Python program to print an inverted pyramid pattern of numbers based on user input.

---

### ALGORITHM  
1. Begin the program.
2. Use `input()` to read the number of rows, `a`, from the user.
3. Convert the input to an integer.
4. Initialize a variable `num` to 1 for the first number to print.
5. Use a nested `for` loop:
   - The outer loop runs from `1` to `a`.
   - The inner loop prints the current number `num` repeatedly, with the number of repetitions decreasing each row.
6. Increment `num` after each row.
7. Print a newline after each row.
8. Terminate the program.

---

### 🧾 PROGRAM

```python
a = int(input())

num = 1
for i in range(1, a + 1):
    for j in range(i, a + 1):
        print(num, end=" ")
    num += 1
    print("")

```

### OUTPUT
![image](https://github.com/user-attachments/assets/fbe84cf0-0cae-4713-ae7c-a4056a477812)

### RESULT
Thus, the Python program to print an inverted pyramid pattern of numbers has been implemented and executed successfully.


# Experiment No: 2e – SEB-Mean Value Calculation

## AIM  
To write a Python program to define a function that accepts 3 values and returns their mean value.

---

### ALGORITHM  
1. Begin the program.  
2. Define a function `result(a, b, c)` that accepts three numbers as arguments.
3. Inside the function:
   - Calculate the sum of `a`, `b`, and `c`.
   - Compute the mean by dividing the sum by 3.
   - Return the calculated mean value.
4. Use `input()` to read three numbers from the user.
5. Convert the inputs to integers.
6. Call the `result()` function with the three numbers as arguments and display the returned mean value.
7. Terminate the program.

---

### 🧾 PROGRAM

```python
def result(a, b, c):
    sum = a + b + c
    mean = sum / 3
    return mean

a = int(input())
b = int(input())
c = int(input())

print(f"mean is {result(a, b, c)}")

```
### OUTPUT
![image](https://github.com/user-attachments/assets/f4f2b95a-dde8-41bf-999d-ffa9b0db735f)

### RESULT
Thus, the Python program to define a function that accepts 3 values and returns their mean value has been implemented and executed successfully.


