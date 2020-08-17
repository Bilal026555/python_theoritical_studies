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

##Example: Python for Loop
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

## Features

This project makes it easy to:
* Bootstrap your open source project properly
* Make sure everyone gets what you're trying to achieve with your project
* Follow simple instructions for a perfect `README.md`

## Contributing

As I use this for my own projects, I know this might not be the perfect approach
for all the projects out there. If you have any ideas, just
[open an issue][issues] and tell me what you think.

If you'd like to contribute, please fork the repository and make changes as
you'd like. Pull requests are warmly welcome.

If your vision of a perfect `README.md` differs greatly from mine, it might be
because your projects are for vastly different. In this case, you can create a
new file `README-yourplatform.md` and create the perfect boilerplate for that.

E.g. if you have a perfect `README.md` for a Grunt project, just name it as
`README-grunt.md`.

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

