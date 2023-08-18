# Test-1
def gcd_steps (a,b) :
  steps=0
  while b>0:
    b,a=a%b, b
    steps+=1
 return a, steps

a= eval(input("Enter the bigger number for calculating GCD- "))
b= eval(input("Enter the smaller number for calculating GCD-"))
print(gcd_steps (a,b)[0], "is the GCD")
print(gcd_steps(a,b)[1], "are the number of steps ")


k= eval(input("Enter the number of digits of whichyou eant GCD which will require maximum steps-"))
for i in range( 10**(k-1), 10**k) :
  for j in range( 10**(k-1), 10**k):
    n= gcd_steps(i,j).[2]
    
