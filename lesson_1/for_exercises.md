# Snakify chapter 4 exercises - for loop

# 1. Series - 1 
<img src="images/series_1.png" width="40%">

```.py
# Print all numbers from a to b inclusively given a <= b
a = int(input("Input a: "))
b = int(input("Input b: "))
for num in range(a, b+1):
  print(num)
```

# 2. Series - 2
<img src="images/series_2.png" width="40%">

```.py
# Print all numbers from a to b inclusively, in ascending order if a < b
# or in descending order if a >= b
a = int(input("Input a: "))
b = int(input("Input b: "))
if a < b:
    for num in range(a, b+1):
        print(num)
else:
    for num in range(a, b-1, -1):
        print(num)
```
