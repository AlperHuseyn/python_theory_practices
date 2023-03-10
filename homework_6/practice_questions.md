---

1. Write the set comprehension of vocal letters in a text as a single expression format. For example, if the text is
`"today the weather is very nice"`, the resulting set will contain the strings `'i', 'a', 'o', 'e'`.

---

2. Create a tuple list from the numbers in a list using a list comprehension. The first element of the tuple should
be the number itself and the second element should be the strings "odd" or "even", depending on whether the number
is odd or even. For example:


```python
a = [1, 2, 3, 4, 5]
```

When this list is processed through the list comprehension, the following tuple list should be obtained:

```python
[(1, 'odd'), (2, 'even'), (3, 'odd'), (4, 'even'), (5, 'odd')]
```

The code should be in a single expression.

Hint: You can use the ternary operator in the left expression of the list comprehension. But there is also a way
to do it without using the ternary operator.

---

3. Using list comprehension, transpose a matrix made up of columns of equal length into a single expression. For example:

```python
a = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
```

The list obtained from the list comprehension should be as follows:

```python
[[1, 4, 7], [2, 5, 8], [3, 6, 9]]
```

Hint: Another list comprehension can be used on the left side of the list comprehension expression to solve the question.

Also, solve this question without using list comprehension, using the classical method.

---

4. Solve the above question using list comprehension in a single expression for matrices with unequal column lengths.
For example, if the matrix is:

```python
a = [[1, 2, 3], [4, 5], [6, 7, 8, 9], [10]]
```

The matrix obtained from the list comprehension should be as follows:

```python
[[1, 4, 6, 10], [2, 5, 7], [3, 8], [9]]
```

Also, solve this question without using list comprehension, using the classical method.

---

5. Create an expression in a single line using list comprehensions to find the average of the averages of all n-sample
(n cannot be greater than the length of the list) subsets of a list. According to the Central Limit Theorem, this
average should be equal to the main mean. For example:


```python
a = [1, 2, 3, 4, 5]
```

In this case, calculate the average of the averages of all 2-sample subsets of this list. You should find all 2-sample
subsets of the list and calculate the average of their averages.

Hint: Use the itertools.combinations function for n-sample subsets of the list. You can use the statistics.mean function
to shorten your code for calculating averages.

---

6. In a variable named 's', there is a text. It is assumed that the words in the text are separated by space characters.
Write an expression that includes a list comprehension, so that as a result, the vowels in the words of the text are
eliminated. For example:

```python
s = 'today the weather is very beautiful'
```

The text obtained from the expression you will write should be like this:

```python
tdy th wthr s vry btfl
```

This operation should be done by a single expression.

---

7. The Traveling Salesman Problem (TSP) is a well-known combinatorial optimization problem in which the goal is to find
the shortest possible route that visits a given set of cities and returns to the starting city. In other words, in which
order should the salesman visit the cities to make the shortest trip? Please solve the Traveling Salesman Problem
specified below in the form presented.

* The city where the traveling salesman is located A, and the other cities are shown in the graph which can be
generated with the following code:

    
```python
    import networkx as nx
    import matplotlib.pyplot as plt
    
    # Create the graph
    G = nx.Graph()
    G.add_edge('A', 'B', weight=5)
    G.add_edge('A', 'C', weight=7)
    G.add_edge('A', 'D', weight=10)
    G.add_edge('B', 'D', weight=4)
    G.add_edge('B', 'E', weight=17)
    G.add_edge('B', 'G', weight=20)
    G.add_edge('C', 'D', weight=6)
    G.add_edge('C', 'F', weight=9)
    G.add_edge('D', 'E', weight=3)
    G.add_edge('D', 'F', weight=12)
    G.add_edge('E', 'F', weight=14)
    G.add_edge('E', 'G', weight=6)
    G.add_edge('F', 'G', weight=10)
    
    # Draw the graph
    pos = nx.spring_layout(G)
    nx.draw(G, pos, with_labels=True)
    
    # Write the weights on the edges
    edge_labels = nx.get_edge_attributes(G,'weight')
    nx.draw_networkx_edge_labels(G, pos, edge_labels=edge_labels)
    
    plt.show()
```

* The ability to go from one city to another and the distances between them should be held in a dictionary object.
The dictionary object can be like this:

```python
d = {'A': {'B': 5, 'C': 7, 'D': 10}, 'B': {'A': 5, 'D': 4, 'E': 17, 'G': 20}, ....} 
```

* The solution for the Traveling Salesman Problem using brute force logic in a case where there are n cities is done
by examining (n-1)!/2 tours. However, here, you can do this with (n-1)!. The thing to do here is to remove city A from
the total of 7 cities (i.e. ['A', 'B', 'C', 'D', 'E', 'F', 'G']) and create all permutations and calculate their path
lengths, then find the smallest one. Of course, there is not a path for each permutation. Because there is not a direct
path between each and every city. It is necessary not to calculate permutations without direct paths between them.

---

