# Find-the-Roots-of-a-Quadratic-Equation-Correct-Code
import math

a = float(input("Enter the first coefficient: "))
b = float(input("Enter the second coefficient: "))
c = float(input("Enter the third coefficient: "))

if a != 0:
    d = b * b - 4 * a * c

    if d == 0:
        r = -b / (2 * a)
        print("The roots are real and equal")
        print("Root:", r)

    elif d > 0:
        r1 = (-b + math.sqrt(d)) / (2 * a)
        r2 = (-b - math.sqrt(d)) / (2 * a)
        print("The roots are real and distinct")
        print("Root1:", r1)
        print("Root2:", r2)

    else:
        rp = -b / (2 * a)
        ip = math.sqrt(-d) / (2 * a)
        print("The roots are imaginary")
        print("Root1:", rp, "+ i", ip)
        print("Root2:", rp, "- i", ip)
else:
    print("Not a quadratic equation")

Output:
Enter the first coefficient: 1
Enter the second coefficient: -5
Enter the third coefficient: 6
The roots are real and distinct
Root1: 3.0
Root2: 2.0
