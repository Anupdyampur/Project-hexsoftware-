# Project-hexsoftware-
Finding fibanice sequence using generator
# Fibonacci Generator in Python (Jupyter-friendly)

def fibonacci_gener
ator(n):
    """
    Generate the first n numbers of the Fibonacci series.
    
    Parameters:
        n (int): Number of terms to generate.
    
    Yields:
        int: Next Fibonacci number in sequence.
    """
    a, b = 0, 1
    for _ in range(n):
        yield a
        a, b = b, a + b  # Update to the next pair

# Example: Generate and display first 10 Fibonacci numbers
fib_numbers = list(fibonacci_generator(10))
print("First 10 Fibonacci numbers:", fib_numbers)
