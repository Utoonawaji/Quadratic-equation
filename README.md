# Quadratic-equation

#solve the quadratic equation ax**2 + bx + c = 0
#import complex math module
import cmath
print("Calculations for quadratic equation")
print(" of the form ax² + bx + c = 0 ")
print("where a !=0 i.e not equal zero")
a = float(input("Please Enter a the coefficient x²: "))
b = float(input("Please Enter b the coefficient of x: "))
c = float(input("Please Enter the constant; c : "))
#calculate the discriminant
d = (b**2) - (4*a*c)
if d ==0:
    print("equal roots:")
elif d>0:
    print("unequal roots:")
elif d<0:
    print("complex roots:")
#find two solutions
x1 = (-b-cmath.sqrt(d))/(2*a)
x2 = (-b+cmath.sqrt(d))/(2*a)
print("The solution x1 = {0} and x2 = {1}".format(x1, x2))
