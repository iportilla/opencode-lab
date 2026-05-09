# Fibonacci Sequence Calculator

This Python script calculates the Fibonacci sequence for a given number.

## Features

The script uses a recursive approach to calculate the Fibonacci sequence, where each number is the sum of the two preceding ones.

## Usage

To run the script, save it as `fibo.py` and execute:

```bash
python3 fibo.py
```

## Code

```python
def fibonacci(n):
    if n <= 1:
        return n
    else:
        return fibonacci(n-1) + fibonacci(n-2)

n = int(input("Enter a number: "))
print(fibonacci(n))
```

## How it works

The script calculates the Fibonacci sequence using a simple recursive approach. The function `fibonacci(n)` returns the nth number in the Fibonacci sequence, where each number is the sum of the two preceding numbers.

Here's a diagram showing how the function works:

```mermaid
graph TD
    A[n] --> B{Base case?};
    B --> C[Yes: return n]
    B --> D[No: calculate fibonacci(n-1) + fibonacci(n-2)]
```

## Target Audience

This documentation is intended for junior Python developers who are learning about:

1. Recursion
2. Basic input/output operations
3. Number sequences

## Key Concepts

The Fibonacci sequence is a series of numbers where each number is the sum of the two preceding ones, usually starting with 0 and 1. The sequence goes: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, ...

## Example Usage

```python
# Example of how the function works
def fibonacci(n):
    if n <= 1:
        return n
    else:
        return fibonacci(n-1) + fibonacci(n-2)

# To use the function
n = int(input("Enter a number: "))
print(fibonacci(n))
```

## Recursion

The function uses recursion, which means the function calls itself. This is a common pattern in computer science and is often used to solve problems that can be broken down into smaller, similar problems.

## Contributing

Contributions are welcome! Please read the contributing guide before making any changes.

## License

This project is licensed under the MIT License.