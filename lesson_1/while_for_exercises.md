# 1. List of squares
For given integer n print all squares of integers where the square is less than or equal to n, in ascending order
<img src="images/list_of_sqrs.png" width="40%">

```.py
n = int(input("Input n: "))
num = 1
sqr = 1
while sqr <= n:
    print(sqr)
    num += 1
    sqr = num ** 2
```
```.py
n = int(input())
for i in range(1, n+1):
    if i**2 <= n:
        print(i**2)
```

# 2. Least divisor
<img src="images/list_of_sqrs.png" width="40%">

```.py
# Given an integer not less than 2 print its smallest integer divisor greater than 1  
n = int(input())
div = 2
while n % div != 0:
    div +=1
print(div)
```
```.py
n = int(input())
div = 2
# The least divisor will never be larger than the number itself
for i in range(1, n+1):
    if n % div != 0:
        div +=1
    else:
        break
print(div)
```

# 3. The power of two

```.py
# For a given integer n, find the greatest integer x where 2**x is less than or equal to n
# Print the exponent value and the result of the expression 2x

```

# 4. Morning jog
As a future athlete you just started your practice for an upcoming event. Given that on the first day you run x miles, and by the event you must be able to run y miles. Calculate the number of days required for you to finally reach the required distance for the event, if you increases your distance each day by 10% from the previous day. 
