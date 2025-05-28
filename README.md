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
