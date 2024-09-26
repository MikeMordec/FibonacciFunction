FibonacciFunction
Overview

The FibonacciFunction is a Python implementation that calculates the nth Fibonacci number using a recursive approach. This project serves as a demonstration of fundamental programming concepts such as recursion, base cases, and error handling in Python.
Table of Contents

    Features
    Usage
    Code Structure
    Performance Considerations
    Contributing
    License

Features

    Calculates Fibonacci numbers for any non-negative integer.
    Includes error handling for invalid inputs.
    Simple and intuitive recursive implementation.

Usage

To use the Fibonacci function, simply call it with a non-negative integer. Here's an example:

python

print(Fibonacci(9))  # Output: 34

Example Input/Output

    Input: Fibonacci(0)
    Output: 0

    Input: Fibonacci(1)
    Output: 1

    Input: Fibonacci(9)
    Output: 34

Code Structure

The main function Fibonacci(n) follows this structure:

python

def Fibonacci(n):
    # Base cases
    if n < 0:
        print("Incorrect input")
    elif n == 0:
        return 0
    elif n == 1 or n == 2:
        return 1
    else:
        return Fibonacci(n - 1) + Fibonacci(n - 2)

Performance Considerations

While this implementation demonstrates the concept of recursion, it is not optimized for large values of nn due to its exponential time complexity. For practical applications, consider using iterative approaches or memoization to improve efficiency.
Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue to discuss enhancements, optimizations, or any other suggestions you may have.
