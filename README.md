# PY-Practical-2 
n = int(input("Enter a value: "))
if n > 1:
    for i in range(2, int(n**0.5) + 1):  # Optimized to check only up to sqrt(n)
        if n % i == 0:
            print(n, "is not a prime number")
            break
    else:
        print(n, "is a prime number")
else:
    print(n, "is not a prime number")


'''output
Enter a value: 1
1 is not a prime number
'''
