# GoMyCode# 

Question 1
for i in range (2000,3201):
    if(i%7==0 and i%5!=0):
        print(i)



#Question 2
num = int (input("Please enter a number: "))
factorial = 1
if num < 0:
   print("Sorry, invalid entry: factorial does not exist for negative numbers")
elif num == 0:
   print("The factorial of 0 = 1")
else:
   for i in range(1,num + 1):
       factorial = factorial*i
   print("The factorial of",num,"is",factorial,".")



#Question 3 
n=int(input("Input a number "))
d = dict()

for i in range(1,n+1):
    d[i]=i*i

print(d)


#Question 4
string1 = input("enter the original word:")
print (string1)
n=int(input("Enter the position of the character to be removed: "))
if n in range (0,len(string1)):
    newstring= string1 [:n] + string1 [n+1:]
else:
    print ("error")
print (newstring) 


#Question 5
import numpy as np

x=np.array(input ("enter a Numpy array to convert: "))

y= x.tolist()
print (y)


#Question 6

import numpy as np

A=np.array([[0, 1, 2] , [2, 1 ,0] ])

print ("Covariance is = ", np.cov(A))


#Question 7 

import math

C=50
H=30
value = []
print ("Enter all the D values separated by a , : ")
items=[x for x in input().split(',')]

for d in items:
    value.append(str(int(round(math.sqrt(2*c*float(d)/h)))))

print(','.join(value))
