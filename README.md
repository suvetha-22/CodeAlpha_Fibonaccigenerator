# CodeAlpha_Fibonaccigenerator
def generate_fibonacci(limit):
    fibonacci_sequence = [0, 1]
    while True:
        next_fib = fibonacci_sequence[-1] + fibonacci_sequence[-2]
        if next_fib > limit:
            break
        fibonacci_sequence.append(next_fib)
    return fibonacci_sequence

limit = int(input("Enter the limit for Fibonacci sequence: "))
fibonacci_numbers = generate_fibonacci(limit)
print("Fibonacci sequence up to", limit, ":", fibonacci_numbers)
