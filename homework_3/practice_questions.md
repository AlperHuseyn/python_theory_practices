
1. Please write the function named "puts" as follows:

The parameter structure of the function is as follows:
```python
def puts(text, **kwargs)
```

The function prints the text received as its first parameter to the console. The double-asterisk kwargs parameter of the
function accepts the following named arguments:

* `reverse`: This argument specifies whether the text should be printed backwards or forwards. If False, the text should
be printed forwards; if True, the text should be printed backwards. The default is False.

* `repeat`: This argument should be used with an int value. It specifies how many times the text should be printed.
The default value is 1.

* `center`: This argument should also be used with an int value. It centers the text within the specified area. If the
text is longer than the specified area, the entire text should be printed. The default value can be assumed to be 0
(i.e., if the argument is not specified, the entire text is printed).

* `fillchar`: This argument should be used with a one-character string value. It specifies which character should be used
to fill the left and right spaces in the center operation. The default value can be assumed to be SPACE character.
This argument cannot be used alone; it can only be used with the center argument. If this argument is used alone,
terminate the function with an error message.

If an invalid argument is used within the function, terminate the function with an error message.

---

2. Write a function named "disp_shape" that takes an int value as a parameter and prints the following pattern to the screen:

```python
1 2 3 4 5
 2 3 4 5
  3 4 5
   4 5
    5
   4 5
  3 4 5
 2 3 4 5
1 2 3 4 5
```

Above is the result of the disp_shape(5) call printed on the console.

---

3. Write a function called 'crown' that outputs the following pattern. The function should have the following parameter
structure:

```python
def crown(n)
```

Where n indicates the highest number in the pattern below.

```python
1      1      1
12    212    21
123  32123  321
123443212344321

n = 4.

1        1        1
12      212      21
123    32123    321
1234  4321234  4321
1234554321234554321

n = 5.

1          1          1
12        212        21
123      32123      321
1234    4321234    4321
12345  543212345  54321
12345665432123456654321

n = 6.
```

In this pattern, please note the following:

- There are no spaces on the bottom row, and the numbers range from 1 to n and back again. The given number
  is repeated in the rise and fall.

- There is a pattern of 2 spaces followed by 4 spaces above the bottom row. The number of spaces at the top is
  equal to the `given number * 2 - 2`.

Enter a value from the keyboard and call the function with that value to print the pattern to the screen.

```python
def crown(n):
    pass

val = int(input('Enter a value: '))
crown(val)
```
---

4. An Armstrong number is a number that is equal to the sum of the cubes of its digits (xyz is a three-digit
number and x^3+y^3+z^3=xyz). For example, the number 153 is an Armstrong number because 1^3+5^3+3^3=153. Write an
is_armstrong function that takes a number as a parameter and returns whether it is an Armstrong number. The function's
parameter structure is as follows:

```python
def is_armstrong(n)
```

The function should return a boolean value.

Then, in a loop, read a number from the keyboard and call the function with this number. Print whether the number is an
Armstrong number based on the return value. Exit the loop when 0 is entered. (For instance, 370 and 407 are Armstrong
numbers.) The code for this is given below:

```python
def is_armtrong(a):
    pass

while True:
    a = int(input('Enter a number:'))
    if a == 0:
        break
    print('Armstrong' if is_armtrong(a) else 'Not Armstrong')
```

After completing this question, write a print_armstrong function that calls the is_armstrong function in a loop and
prints all Armstrong numbers from 1 to n, separated by a space character, and call it with the value 1000000.
The parameter structure of the print_armstrong function should be as follows:

```python
def print_armstrongs(n)
```
---

5. Request a text from the stdin. Then, print the words in the text in reverse order, separated by a single space
character. The question will be solved using a single print call with a compact expression after the text has been
obtained. For example:

```python
Enter a text: today the weather is very cold
cold very is weather the today
```
---

6. Write a function called digitate that takes an iterable object consisting of int values as a parameter and returns
a tuple array by obtaining tuples of the digits of the numbers in the list:

```python
def digitate(vals):
    pass

vals = [23, 4, 765, 34589, 42]
result = digitate(vals)
print(result)  # [(2, 3), (4, ), (7, 6, 5), (3, 4, 5, 8, 9), (4, 2)]
```
---

7. Read a text from the keyboard. The text should consist of words separated by space characters. Place the words in a
list by eliminating same words. For example, if the entered text is as follows:

```
today the weather yes the weather is very very beautiful
```

As a result, the following list should be obtained:

```python
['today', 'the', 'weather', 'yes', 'is', 'very', 'beautiful']
```

The words in the obtained list should be in the order of the words in the text.

---

8. Write a function called "print_shape" that takes an integer value as a parameter and prints the following pattern
to the screen. The function's parameter structure is as follows:

```python
def print_shape(n)
```

Output: 

```python
**********
****  ****
***    ***
**      **
*        *
*        *
**      **
***    ***
****  ****
**********
```

Here, the parameter of the function is 5. Note that the first line has twice as many * as this number.

---

9. Please write a function called disp_char_pattern that takes a character as a parameter and prints the following
pattern to the screen. The character may be a capital or lowercase letter.

```python
def disp_char_pattern(ch)
```

Output:

```python
        A
       B B
      C   C
     D     D
    E       E
   F         F
    E       E
     D     D
      C   C
       B B
        A
```

This pattern is obtained by calling disp_char_pattern('F').

---

10. Write the functions that return the value of Pi as a return value as follows:


* 10.a) Implement the following series proposed by Newton with a function named newton_pi:

```python
def newton_pi(k)

pi = sum(n:0 -> k)(2^(n + 1) * (n!)^2) / (2 * n + 1)!
```

Here k indicates the final value that n can take. The function should return the sum of the series.

In the latest versions of Python, the factorial function has also been added in the math module.


* 10.b) Implement the series suggested by Nilakantha Somayaji using a function called somayaji_pi:

```python
def somayaji_pi(n)

pi = 3 + (4 / 3^3 - 3) - (4 / 5^3 - 5) + (4 / 7^3 - 7) - (4 / 9^3 - 9) + ...
```

The parameter n of the function specifies the number of terms. For example, in the image mentioned above, there are
4 terms. The function should return the sum of the series.


* 10.c) Implement the series suggested by Bailey, Borwein and Plouffe using a function called bailey_borwein_plouffe_pi:

```python
pi = sum(n:0 -> k)((1 / 16)^n * ((4 / 8 * n + 1) - (2 / 8 * n + 4) - (1 / 8 * n + 5) - (1 / 8 * n + 6))
```

The parameter of the function specifies the maximum value that n can take. The function should return the sum of
the series.

---

11. Write a function called sort_tuple_list that takes a list of tuples (tuples have one name, and two separate numbers)
as a parameter and sorts the list based on the first, second, and third elements of the tuple. If the first elements
of the tuples are equal, the second elements will be used for sorting, and if the second elements are also equal,
the third elements will be used. For example:

```python
def sort_tuple_list(a):
    pass

a = [('Tom', 19, 80), ('Json', 22, 90), ('Jony', 17, 91), ('Jony', 17, 93), ('Json',21, 85)]
sort_tuple_list(a)
print(a)
```

The result should be:

```python
[('Jony', 17, 91), ('Jony', 17, 93), ('Json', 21, 85), ('Json', 22, 90), ('Tom', 19, 80)]
```
---
