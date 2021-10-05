1. Paulo's O's

```.py
def paulos_os(string):
    o_count = 0
    for char in string:
        if char.lower() == "o":
            o_count += 1
    return o_count
```
```.py
paulos_os("O o o oo that's cool") -> 7
```

2. Beril's more repeated letters

```.py
def berils_repeated(w1, w2):
    w1_letters = list(w1)
    w2_letters = list(w2)
    w1_count = 0
    w2_count = 0
    for letter in w1_letters:
        if w1_letters.count(letter) > 1:
            w1_count += 1
    for letter in w2_letters:
        if w2_letters.count(letter) > 1:
            w2_count += 1
    if w1_count > w2_count:
        output = w1
    elif w2_count > w1_count:
        output = w2
    else:
        output = "?"
    return output
```
```.py
berils_repeated("appreciate", "pumpkin") -> "appreciate"
```
3. Ryu's time

```.py
def ryus_time(h1, m1, h2, m2):
    h_diff = h2 - h1
    m_diff = m2 - m1
    total_diff = h_diff*60 + m_diff
    return total_diff
```
```.py
ryus_time(19, 25, 20, 25) -> 60
```

4. Esslam's unique letter (mine)

```.py
#def esslams_unqiue_letter(word):
    is_isogram = True
    letters = []
    for letter in word:
        if letter in letters:
            is_isogram = False
        else:
            letters.append(letter)
    return is_isogram
```

```.py
esslams_unique_letter("asdff") -> False
esslams_unique_letter("asdf") -> True
```
