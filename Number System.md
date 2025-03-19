x = 2345
multiplier = 1
result = 0
mybase = 6

    x = 2345
    multiplier = 1
    result = 0
    mybase = 6
​
    print("=="*10)
    print:("Number: ", x)
    d = x % 10
    print("Last Digit: ", d)
    print("Multiplier: ", multiplier)
    result = result + d*multiplier
    print("Result: ", result)
    x = x // 10
    x
    multiplier = multiplier * mybase
    print("New Number: ", x)
    print("Multiplier: ", multiplier)
    
    print("**"*10)
    print:("Number: ", x)
    d = x % 10
    print("Last Digit: ", d)
    print("Multiplier: ", multiplier)
    result = result + d*multiplier
    print("Result: ", result)
    x = x // 10
    x
    multiplier = multiplier * mybase
    print("New Number: ", x)
    print("Multiplier: ", multiplier)
    
    print("=="*10)
    print:("Number: ", x)
    d = x % 10
    print("Last Digit: ", d)
    print("Multiplier: ", multiplier)
    result = result + d*multiplier
    print("Result: ", result)
    x = x // 10
    x
    multiplier = multiplier * mybase
    print("New Number: ", x)
    print("Multiplier: ", multiplier)
    
    print("**"*10)
    print:("Number: ", x)
    d = x % 10
    print("Last Digit: ", d)
    print("Multiplier: ", multiplier)
    result = result + d*multiplier
    print("Result: ", result)
    x = x // 10
    x
    multiplier = multiplier * mybase
    print("New Number: ", x)
    print("Multiplier: ", multiplier)
====================
Last Digit:  5
Multiplier:  1
Result:  5
New Number:  234
Multiplier:  6
********************
Last Digit:  4
Multiplier:  6
Result:  29
New Number:  23
Multiplier:  36
====================
Last Digit:  3
Multiplier:  36
Result:  137
New Number:  2
Multiplier:  216
********************
Last Digit:  2
Multiplier:  216
Result:  569
New Number:  0
Multiplier:  1296

def extract_last_digit():
    global x
    global result
    global multiplier
    print("=="*10)
    print("Number: ", x)
    d = x % 10
    print("Last Digit: ", d)
    print("Multiplier: ", multiplier)
    result = result + d*multiplier
    print("Result: ", result)
    x = x // 10
    multiplier = multiplier * mybase
    print("New Number: ", x)
    print("New Multiplier:", multiplier)
extract_last_digit()
====================
Number:  0
Last Digit:  0
Multiplier:  10077696
Result:  569
New Number:  0
New Multiplier: 60466176

def extract_last_digit_recursion():
    global x
    global result
    global multiplier
    print("Number: ", x)
    if x == 0:
        print("The niumber is zero, Stop!")
        print("Final result" , result)
    else:
        d = x % 10
        print("Last Digit: ", d)
        print("Multiplier: ", multiplier)
        result = result + d*multiplier
        print("Result: ", result)
        x = x // 10
        multiplier = multiplier * mybase
        print("New Number: ", x)
        print("New Multiplier:", multiplier)
        
extract_last_digit_recursion()
Number:  0
Last Digit:  0
Multiplier:  60466176
Result:  569
New Number:  0
New Multiplier: 362797056
The number is zero, Stop!

def extract_last_digit_recursion():
    global x
    global result
    global multiplier
    print("Number: ", x)
   
    d = x % 10
    print("Last Digit: ", d)
    print("Multiplier: ", multiplier)
    result = result + d*multiplier
    print("Result: ", result)
    x = x // 10
    multiplier = multiplier * mybase
    print("New Number: ", x)
    print("New Multiplier:", multiplier)
    if x == 0:
        print("The number is zero, Stop!")
    elif x < 0:
        print("Impossibile")
    else:
        extract_last_digit_recursion()
extract_last_digit_recursion()
Number:  0
Last Digit:  0
Multiplier:  279936
Result:  569
New Number:  0
New Multiplier: 1679616
The number is zero, Stop!

x = 2345
multiplier = 1
result = 0
mybase = 6
​
while x > 0:
    print("x in the loop: ", x)
    extract_last_digit()
x in the loop:  2345
====================
Number:  2345
Last Digit:  5
Multiplier:  1
Result:  5
New Number:  234
New Multiplier: 6
x in the loop:  234
====================
Number:  234
Last Digit:  4
Multiplier:  6
Result:  29
New Number:  23
New Multiplier: 36
x in the loop:  23
====================
Number:  23
Last Digit:  3
Multiplier:  36
Result:  137
New Number:  2
New Multiplier: 216
x in the loop:  2
====================
Number:  2
Last Digit:  2
Multiplier:  216
Result:  569
New Number:  0
New Multiplier: 1296
​
