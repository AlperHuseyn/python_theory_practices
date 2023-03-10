---

1. Request a string consisting of numeric characters using the input function from the stdin. Convert this str value
into an int value without using int(...) built-in function, and print the "**value * 2**" calculation to the console. There
may be trailing and the leading spaces in the text. These characters should not interfere with the operation of your code.


An example request:

```
Please enter a text consisting of numeric characters: 123
246
```

Explanation

You can convert the characters of the textual number you will read from the keyboard into the int type using the ord
function. For example, if the character is ch, `ord(ch) - ord('0')` gives the numerical equivalent of that character.

----

2. Write the code that does the reverse of the operation done in the above question without ever calling the str function.
That is, you will read an int value using the `int(input(...))` call. Then you will decompose this number into digits
and convert it back into text.

Explanation

You can convert the digits of the number you will read from the keyboard into the str type using the chr function.
For instance, if d is a one-digit number, it can be converted to a character using the operation `chr(ord('0') + d)`.

----

3. Read a value n from the keyboard and create a square unit matrix of size `n x n` in the form of a list. Print this list
using nested loops and print. For example:

```python
Enter a number for n: 5

[[1, 0, 0, 0, 0], [0, 1, 0, 0, 0], [0, 0, 1, 0, 0], [0, 0, 0, 1, 0], [0, 0, 0, 0, 1]]

1 0 0 0 0
0 1 0 0 0
0 0 1 0 0
0 0 0 1 0
0 0 0 0 1
```
----

4. Read a text from the keyboard. Place the words in the text into a list and print the list.

```python
Enter a text: Today the weather is very nice. Ali (our Ali) - Veli - and Selami went to the park.

['Today', 'the', 'weather', 'is', 'very', 'nice', 'Ali', 'our', 'Ali', 'Veli', 'and', 'Selami', 'went', 'to', 'the', 'park']
```

Explanation:

Please note that punctuation marks and special characters like parentheses are not part of words.

----
5. Please enter a number n from the keyboard. Print all numbers between 0 and n (inclusive) that have all their digits
as even numbers. For example, if the value 5000 is entered from the keyboard, all printed numbers must have all their
digits as even numbers `(0, 2, 4, 6, 8, 20, 22, 24, ..., 4882, ... etc.)`

----

6. Request a text from the keyboard. Print out how many upper case letters and how many lower case letters there are
in the text. (Non-alphabetic characters will not be taken into account)

----

7. Enter a text from the keyboard. Place the number of characters in the text in a dictionary. The keys of the dictionary
should be characters and the values should be their counts. For example, if the text "ankara" is entered, the created
dictionary object should contain the following elements:

```python
{'a': 3, 'n': 1, 'k': 1, 'r': 1}
```
----

8. Create a list of two-digit int numbers. Then rearrange the elements of this list into a form where their digits are
swapped. For example:

```python
a = [12, 56, 89, 32, 19, 99, 43]
```

This list should be converted to the following:

```python
[21, 65, 98, 23, 91, 99, 34]
```
----

9. Please read in the variables 'height' and 'width' from the keyboard and create the following pattern (our example is
height = 9, width = 7):

```python
|*      |
| *     |
|  *    |
|   *   |
|    *  |
|     * |
|      *|
|     * |
|    *  |
```

Here, 'height' is the total number of rows, and 'width' is the number of characters between the '|' characters.

----

10. Read a number n from the keyboard and write a program to create the following pattern (our example is n = 6):

```python
     *
    ***
   *****
  *******
 *********
***********
 *********
  *******
   *****
    ***
     *
```
----

