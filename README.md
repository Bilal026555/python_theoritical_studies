# Introduction to Programming with Python
> read README.md file
## For Loop
The for loop in Python is used to iterate over a sequence (list, tuple, string) or other iterable objects. Iterating over a sequence is called traversal.
### Syntax
```shell
for val in sequence:
	Body of for
```
Here, `val` is the variable that takes the value of the item inside the sequence on each iteration.Loop continues until we reach the last item in the sequence. The body of for loop is separated from the rest of the code using indentation.
### Example: Python for Loop
```shell 
# Program to find the sum of all numbers stored in a list

# List of numbers
numbers = [6, 5, 3, 8, 4, 2, 5, 4, 11]

# variable to store the sum
sum = 0

# iterate over the list
for val in numbers:
	sum = sum+val

print("The sum is", sum)
```
When you run the program, the output will be:
```shell
The sum is 48
```
### The range() function
We can generate a sequence of numbers using `range()` function. range(10) will generate numbers from 0 to 9 (10 numbers).

We can also define the start, stop and step size as `range(start, stop,step_size)`. step_size defaults to 1 if not provided.

The range object is `"lazy"` in a sense because it doesn't generate every number that it "contains" when we create it. However, it is not an iterator since it supports `in`, `len` and `__getitem__` operations.

This function does not store all the values in memory; it would be inefficient. So it remembers the start, stop, step size and generates the next number on the go.

To force this function to output all the items, we can use the function `list().`
```shell
print(range(10))

print(list(range(10)))

print(list(range(2, 8)))

print(list(range(2, 20, 3)))
```
### Output
```shell
range(0, 10)
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
[2, 3, 4, 5, 6, 7]
[2, 5, 8, 11, 14, 17]
```
### Practice problem
Write a program that asks the user for an input 'n' (assume that the user enters a positive integer) and prints a sequence of powers of 10 from 10^0 to 10^n in separate lines. For example if 'n' is equal to 4 then the output should look like the following: 
```shell
# Type your code here
user_input=input("Please enter a positive interger")
n=int(user_input)
for i in range(0,n+1):
    print(10**i)
```
### Output for n=8
```shell
1
10
100
1000
10000
100000
1000000
10000000
100000000
```
We can use the `range()` function in for loops to iterate through a sequence of numbers. It can be combined with the `len()` function to iterate through a sequence using indexing. Here is an example.
```shell
# Program to iterate through a list using indexing

genre = ['pop', 'rock', 'jazz']

# iterate over the list using index
for i in range(len(genre)):
	print("I like", genre[i])
```
### Output 
```shell
I like pop
I like rock
I like jazz
```
### for loop with else
A `for` loop can have an optional else block as well. The else part is executed if the items in the sequence used in for loop exhausts.

The `break` keyword can be used to stop a for loop. In such cases, the else part is ignored.

Hence, a for loop's else part runs if no break occurs.
## Break and Continue statement in Python
[Break and Continue statement:](https://www.programiz.com/python-programming/break-continue)

This project makes it easy to:
* Bootstrap your open source project properly
* Make sure everyone gets what you're trying to achieve with your project
* Follow simple instructions for a perfect `README.md`

## Contributing

As I use this for my own projects, I know this might not be the perfect approach
for all the projects out there. If you have any ideas, just
[open an issue][issues] and tell me what you think.

## Related projects

Here's a list of other related projects where you can find inspiration for
creating the best possible README for your own project:

- [Billie Thompson's README template](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
- [A list of awesome READMEs](https://github.com/matiassingers/awesome-readme)
- [Akash Nimare's kickass README guide](https://gist.github.com/akashnimare/7b065c12d9750578de8e705fb4771d2f)
- [Dan Bader's README template](https://github.com/dbader/readme-template)

## Licensing

This project is licensed under Unlicense license. This license does not require
you to take the license with you to your project.

[issues]:https://github.com/jehna/readme-best-practices/issues/new

