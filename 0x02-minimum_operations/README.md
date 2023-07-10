# Minimum Operations

This program calculates the fewest number of operations needed to result in exactly `n` 'H' characters in a text file, given that the text editor can only perform two operations: Copy All and Paste.

## Approach

The program uses a greedy approach to find the largest factor of the given number `n` and divides `n` by that factor. It continues dividing `n` by its factors until `n` becomes 1. The sum of the factors used in the divisions represents the minimum number of operations required.

## Example

```python
n = 4
print("Min # of operations to reach {} char: {}".format(n, minOperations(n)))
```

Output:
```
Min # of operations to reach 4 char: 4
```

```python
n = 12
print("Min # of operations to reach {} char: {}".format(n, minOperations(n)))
```

Output:
```
Min # of operations to reach 12 char: 7
```

## Time Complexity

The time complexity of the solution is O(sqrt(n)) because the loop iterates up to the square root of `n` in the worst case.

## Repository

The code for this program can be found in the following GitHub repository:

Repository: [alx-interview](https://github.com/ThengweTheFirst/alx-interview)

Directory: 0x02-minimum_operations

File: 0-minoperations.py
