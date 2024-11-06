# PY-Practical-2
a.  n = int(input("Enter a value: "))
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


b.  n = int(input("Enter a value: "))
for num in range(2, n):
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            break
    else:
        print(num, end=',')



'''output
Enter a value: 100
2,3,5,7,11,13,17,19,23,29,31,37,41,43,47,53,59,61,67,71,73,79,83,89,97,
'''


c.  n = int(input("Enter the number of prime numbers to generate: "))
count = 0
number = 2

while count < n:
    for i in range(2, int(number**0.5) + 1):
        if number % i == 0:
            break
    else:
        print(number, end=',')
        count += 1
    number += 1


'''output
Enter the number of prime numbers to generate: 20
2,3,5,7,11,13,17,19,23,29,31,37,41,43,47,53,59,61,67,71,\
'''


d.  n = int(input("Enter a value: "))
sum_n = sum(range(1, n + 1))
print("The sum of the first", n, "natural numbers is:", sum_n)


'''output
Enter a value: 50
The sum of the first 50 natural numbers is: 1275
'''
