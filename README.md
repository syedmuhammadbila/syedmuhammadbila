def fibonacci_series(n):
    fib_series = [0, 1]

    for i in range(2, n):
        next_term = fib_series[i-1] + fib_series[i-2]
        fib_series.append(next_term)

    return fib_series

# Example usage:
num_terms = int(input("Enter the number of terms in the Fibonacci series: "))
result_series = fibonacci_series(num_terms)

print("Fibonacci Series:")
print(result_series)
