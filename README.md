# Test-1

a= eval(input("Enter the bigger number for calculating GCD- "))
b= eval(input("Enter the smaller number for calculating GCD-"))
print(gcd_steps (a,b)[0], "is the GCD") 
print(gcd_steps(a,b)[1], "are the number of steps ")

k= eval(input("Enter the number of digits of which you eant GCD which will require maximum steps-"))
z=0 
l=[] 
for i in range(10**(k-1),10**k) :
    for j in range(10**(k-1),10**k):  
      n= gcd_steps(i,j)[1]
      if n>z : 
          z=n 
          l.append([i,j])

print(l[len(l)-1])
