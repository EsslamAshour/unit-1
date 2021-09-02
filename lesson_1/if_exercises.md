# Snakify chapter 3 exercises

## 1. Minimum of two numbers
<img src="images/minimum_of_two.png" width="30%">

```.py
a = int(input())
b = int(input())
if a < b:
    print(a)
else:
    print(b)
```

## 2. Sign function
<img src="images/sign_func.png" width="30%">

```.py
x = int(input())
if x > 0:
    print(1)
elif x < 0:
    print(-1)
else:
    print(0)
```

## 3. Minimum of three numbers
<img src="images/minimum_of_three.png" width="30%">

```.py
a = int(input())
b = int(input())
c = int(input())
if a < b and a < c:
    print(a)
elif b < a and b < c:
    print(b)
else:
    print(c)
```

## 4. Equal numbers
<img src="images/equal_numbers.png" width="30%">

```.py
a = int(input())
b = int(input())
c = int(input())
if a == b and b == c:
    print(3)
elif a == b or a == c or b == c:
    print(2)
else:
    print(0)
```

