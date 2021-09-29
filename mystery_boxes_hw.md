# Mystery Box 1

```.py
def mystery_box1(word, capitalize):
    if not capitalize:
        word = word.lower()
    return word[::-1]
```

# Mystery Box 2

```.py
def mystery_box2(email):
    split_email = email.split("@")
    mail_suffix = split_email[1]
    name_lower = split_email[0].split(".")
    name_upper = " ".join([str.capitalize(name_part) for name_part in name_lower])
    # We can also do return but we'd have to use two variables (x, y = func())
    print(name_upper)
    print(mail_suffix)
```

# Mystery Box 3

```.py

```


# Mystery Box 4 

```.py
# Remove the 2 largest numbers in the list, return the resulting list and its average.
def mystery_box_4(lst):
    for i in range(2):
        lst.remove(max(lst))
    print(lst)
    print(sum(lst)/len(lst))
```
