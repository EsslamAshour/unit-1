# 1. List of squares
For given integer n print all squares of integers where the square is less than or equal to n, in ascending order.
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
n = int(input("Input n: "))
# i can never be larger than n, if i > n then i**2 > n
for i in range(1, n+1):
    if i**2 <= n:
        print(i**2)
```

# 2. Least divisor
Given an integer not less than 2 print its smallest integer divisor greater than 1
<img src="images/least_divisor.png" width="40%">

```.py
n = int(input("Input n: "))
div = 2
while n % div != 0:
    div +=　1
print(div)
```
```.py
n = int(input("Input n: "))
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
For a given integer n, find the greatest integer x where 2**x is less than or equal to n, print the exponent value and the result of the expression 2**x
<img src="images/power_of_two.png" width="40%">
```.py
n = int(input())
exp = 1
res = 2
while res <= n:
    exp += 1
    res *= 2
print(exp-1)
print(res/2)
```
```.py
n = int(input("Input n: "))
exp = 1
res = 2
# No choice but to use very large number
for i in range(1, 10000):
    if res > n:
        break
    else:
        res *= 2
        exp += 1
print(exp-1)
print(res/2)
```


# 4. Morning jog
As a future athlete you just started your practice for an upcoming event. Given that on the first day you run x miles, and by the event you must be able to run y miles. Calculate the number of days required for you to finally reach the required distance for the event, if you increases your distance each day by 10% from the previous day.
<img src="images/morning_jog.png" width="40%">

```.py
n = int(input())
exp = 1
res = 2
while res <= n:
    exp += 1
    res *= 2
print(exp-1)
print(res/2)
```
```.py
n = int(input("Input n: "))
exp = 1
res = 2
# No choice but to use a very large number
for i in range(1, 10000):
    if res > n:
        break
    else:
        res *= 2
        exp += 1
print(exp-1)
print(res/2)
```

# 5. The length of a sequence 
Given a sequence of non-negative integers, where each number is written in a separate line. Determine the length of the sequence, where the sequence ends when the integer is equal to 0. Print the length of the sequence (not counting the integer 0). The numbers following the number 0 should be omitted. 
<img src="images/seq_length.png" width="40%">

```.py
num = -1
length = 0
while num != 0:
    num = int(input("Input number: "))
    length += 1
print(length-1)
```
```.py
length = 0
for i in range(10000):
    num = int(input("Input number: "))
    if num == 0:
        break
    else:
        length += 1
print(length)
```

# 5. The sum of a sequence
Determine the sum of all elements in the sequence, ending with the number 0. 
<img src="images/seq_sum.png" width="40%">

```.py
num = -1
sum = 0
while num != 0:
    num = int(input("Input number: "))
    sum += num
print(sum)
```
```.py

```

# 6. The average of a sequence
Determine the average of all elements of the sequence ending with the number 0. 
<img src="images/seq_avg.png" width="40%">
