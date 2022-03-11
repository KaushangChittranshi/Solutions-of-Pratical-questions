# Solutions-of-Pratical-questions

Answer 1 ==
#Arithmetic Operators

33.33//11
((6+3)+2)
(2*(3*2))
10*-5
50/5*6
18%5
52+63
58-36

#Relational Operators

25==25
25<25
25>25
25<=25
25>=25
25!=25

#Logical Operators

(10<5)and(2<3)
(10<5)or(2<3)
not(10<5)

Answer 2 ==
size= int(input("Enter the size of the series")) # It takes input for the size of the series.
i=1
while(i<=size): # first loop.
   j=i
   while(j>=1): # inner loop.
       print(j, end = ' ')  # print the series.
       j=j-1
   i=i+1
   print("") # for line changes.
   
   
 Answer 3==
 
 import math
math.exp(20)
math.pow(25,5)
math.sqrt(2250)
math.floor(6.325)
math.log(25,5)
math.ceil(5.75)
math.fabs(-50)
math.log10(1)
math.cos(60)
math.asin(1)
math.degrees(math.pi/2)
math.radians(360)

Answer 4 ==

import math
def func():
    print('table of sin in the range of 0-10 with increament of 0.2')
    for x in range(0,10):
        print(math.sin(x))
        x=x+0.2
    print()
    print('table of cos')
   
    for x in range(0,10):
        print(math.cos(x))
        x=x+0.2
    print()
    print('table of tan')
    
    for x in range(0,10):
        print(math.tan(x))
        x=x+0.2
    print()
func()

Answer 5 ==

def main():
    year=int(input('\nenter year to check it is leap year or not'))
    if (year%4)==0:
       if (year%100)==0:
          if (year%400)==0:
           print('*\nIT IS A LEAP YEAR*')
          else:
              print('*\nIT IA NOT A LEAP YEAR*')
       else:
          print('*\nIT IS NOT LEAP YEAR*')
    else:
        print('*\nIT IS NOT A LEAP YEAR*')
if __name__=='__main__':
    main()

Answer 6 ==

 while True:

    print("AREA of type of building")
    print("1.Area of Circle type building")
    print("2.Area of Rectangle type building")
    print("3.Area of Square type building")
    print("4.Exit")
    choice = int(input("Enter your choice:"))
    if choice == 1:
        radius = int(input("Enter radius of Circle:"))
        print("Area of Circle", 3.14 * radius * radius)
        break
    elif choice == 2:
        length = int(input("Enter length of Rectangle:"))
        breadth = int(input("Enter breadth of Rectangle:"))
        print("Area of Rectangle:", length * breadth)
        break
    elif choice == 3:
        side = int(input("Enter side of Square:"))
        print("Area:", side * side)
        break
    elif choice == 4:
        break
    else:
      print("Wrong Choice")
      
 Answer 7
   i=int(input('enter the given number = '))
   fac=1
   while(i>0):
       fac=fac*i
       i=i-1
   print('factorial of the given number is = ', fac)
   
 Answer 8 ==
 
n=int(input('enter your number='))
x=0
y=1
z=0
while(z<=n):
    print(z,end=" ")
    x=y
    y=z
    z=x+y
    
 Answer 9
i=int(input('enter the number'))
rev=0
while(i>0):
    rev=(rev*10)+i%10
    i=i//10
print('reverse of the number is ', rev)
j=rev
sum=0
while(j>0):
    sum=sum+(j%10)
    j=j//10
print('sum of the digits= ', sum)

Answer 10
def compute_lcm(x,y):

  if x>y:
      greater = x
  else:
      greater = y

  while(True):
      if((greater % x== 0) and (greater % y == 0)) :
          lcm = greater
          break
      greater +=1

  return lcm

n1=int(input('enter the number'))
n2=int(input('enter the secnod number'))

print('the lcm of n1 and n2 is ', compute_lcm(n1,n2))

Answer 11

def prime(n):
    if n==1:
        return False
    for i in range(2,n):
        if n%i==0:
            return False
            break
    else:
        return True
    return prime(n)
def main():
    n=int(input('enter no.:'))
    result=prime(n)
    if result==True:
        print(n,'is a prime no.')
    else:
        print(n,'is not a prime no.')
if __name__=='__main__':
    main()

                           
ANSWER 12
                            
def main():
    a=input('enter a string:')
    b=a[-1::-1]
    if(a==b):
        print('palindrome string')
    else:
        print('not palindrome')
if __name__=='__main__':
    main()

                            
 ANSWER 14
                            
 def main():
    text = input('Enter a sentence:')
    freq = {}
    for i in text:
        if i in freq:
            freq[i] += 1
        else:
            freq[i] = 1
    print("Frequency of each letter are as follows:", freq)
if __name__=='__main__':
    main()

                            
ANSWER 15
                            
def main():
    d = dict()
    for x in range(1, 6):
        d[x] = x ** 3
    print("The required dictionary of cubes of keys are :", d)
if __name__=='__main__':
    main()
                            
                            
ANSWER 16
                            
#(A)
                            
t1=(1,2,3,4,5,6,7,8,9,10)
t1a=t1[:5]
t1b=t1[5:]
print(t1a)
print(t1b)
print()

#(B)
                            
t1=(1,2,3,4,5,6,7,8,9,10)
n=list(t1)
list1=list()
for i in n:
    if i in n:
        if i%2==0:
            list1.append(i)
    p=tuple(list1)
print('tuple:',p)
print()

#(C)
                            
t1=(1,2,3,4,5,6,7,8,9,10)
t2=(11,13,15)
a=list(t1)
b=list(t2)
c=(a+b)
print(c)

#(D)
                            
t1=(1,2,3,4,5,6,7,8,9,10)
max(t1)
min(t2)
print('max no. is',max(t1))
print('min no. is',min(t1))

                            
ANSWER 17                            

def check_duplicate(l):
    l2={}
    for i in l:
        if i in l2:
            l2[i]+=l
        else:
            l2[i]=l
        for i in l:
            if l2[i]>l:
                print('True',i,l2[i])
def main():
    n=int(input('enter no. of elements:'))
    l=[]
    for i in range(n):
        ele=int(input())
        l.append(ele)
print('original list',l)
check_duplicate
if __name__=='__main__':
    main()

                            
ANSWER 18
                            
class rectangle():
    def __init__(self,l,b):
        self.l=l
        self.b=b
    def area(self):
        return self.l*self.b
    def perimeter(self):
        print('destructor call!!')
x=int(input('enter length:'))
y=int(input('enter breadth:'))
a=rectangle(x,y)
print('area of rectangle is:',a.area())
print('perimeter of rectangle is:',a.perimeter())

                            
Answer 19
                            
def main():
    ch=int(input('Enter 1-length , 2=max of 3 strings,3=to print , 4=number of words='))
    if ch==1:
        n=input('Enter a string:')
        l=len(n)
        print('The length of the string is=',l)
    elif ch==2:
        n1=input('Enter string 1=')
        n2=input('Enter string 2=')
        n3=input('Enter string 3=')
        print('The maximum of the 3 strings is=',max(n1,n2,n3))
    elif ch==3:
        a=input('Enter a string:')
        s=''
        a=list(a)
        for i in range(len(a)):
            if (i%2!=0):
                if a[i]==' ':
                    a[i]=' '
                else:
                    a[i]='#'
        for e in a:
            s=s+e
        print('the new string=',s)    
    elif ch==4:
         b=input('Enter a string=')
        c=0
        for ch in b:
            if ch==' ':
                c+=1
        a=c+1
        print('The number of words:',a)
    else:
        print('invalid choice') 
if __name__=='__main__':
    main()

                            
Answer 20
                            
def inList():                                                                                                                                                                                                    
    num = input("Enter input :   ").split()
    n = list(num)
    for i in n:
        if not i.isdigit():
            print('not no.')
            break
        else:
            print('all are number')
            r = list(map (int,input('Enter input again :  ').split()))
            oddNo = 0
            for i in r:
                if (i % 2) != 0:
                    oddNo += 1
            print('Total odd no in the list is:', oddNo)
            break
    for i in n:
        if i.isalpha():
            print('The largest string is:   ', max(n))
# for reversing the input string
            h = n[-1::-1]
            print("The reverse of input list is  ",h)
# to find if the entered element is present in the input string
            found=input('Enter the element:  ')
            def findEle():
                for i in num:
                    if i == found:
                        print('Element found')
                        break
            findEle()
# to remove an element from the input string
            def delEle():
                k = found
                str = []
                for i in num:
                    if i != k:
                        str.append(i)
                print ('Element',k,'" Deleted ')
# to print updated list
                print('Updated list',str)
            delEle()
            break
inList()

                            
Answer 22
                            
#BINARY SEARCH
                            
def binarySearchAppr (arr,start, end, x):
    if end >= start:
        mid =start + (end- start)//2
    # If element is present at the middle
        if arr[mid] == x:
            return mid
   # If element is smaller than mid
        elif arr[mid] > x:
            return binarySearchAppr(arr, start, mid-1, x)
   # Else the element greator than mid
        else:
            return binarySearchAppr(arr, mid+1, end, x)
    else:
   # Element is not found in the array
      return -1
arr = [2,3,4,10,40]
x =10
result = binarySearchAppr(arr, 0, len(arr)-1, x)
if result != -1:
   print ("Element is present at index "+str(result))
else:
    print ("Element is not present in array")

#LINEAR SEARCH
                            
def search(arr,x):    
    for i in range(len(arr)):
        if arr[i]==x:
            return i        
         return -1
def main():
    n=int(input('enter no. of elements to be inserted:'))
    arr=[]
    for i in range(n):
        ele=int(input('enter elements:'))
        arr.append(ele)
    print(arr)
    x=int(input('enter value to be searched:'))
    result=search(arr,x)
    print(x,'found at index',result)
if __name__=='__main__':
    main()
                            
                            
Answer 23
                            
#SELECTION SORT
      
def selectSort(arr):
    for i in range(len(arr)):
        print(arr)
        minValue=min(arr[i:])
        minInd=arr.index(minValue)
        arr[i],arr[minInd]=arr[minInd],arr[i]
def main():
    arr=[]
    n=int(input('enter no. of elements:'))
    for i in range (n):
        ele=int(input())
        arr.append(ele)
    print('final arr to use selection sort is:',arr)
    selectSort(arr)
    print('sorted sum is:',arr)
if _name=='main_':
    main()
                            
#INSERTION SORT

def insertion(arr):
    for i in range(1,len(arr)):
        key=arr[i]
        j=i-1
        while j>=0 and key<arr[j]:
            arr[j+1]=arr[j]
            j=j-1
            arr[j+1]=key
            print(arr)
def main():
    arr=[]
    n=int(input('enter no. of elemenets:'))
    for i in range(n):
        ele=int(input())
        arr.append(ele)
    print('final arr to use insertion sort is:',arr)
    insertion(arr)
    print('sorted sum is',arr)
if _name=='main_':
    main()
                            
#BUBBLE SORT
                            
def bubbleSort(arr):
    for i in range (len(arr)-1,0,-1):
        for j in range(i):
            print(arr)
            if arr[j]>arr[j+1]:
                arr[j],arr[j+1]=arr[j+1],arr[j]
def main():
    arr=[]
    n=int(input('enter no. of elementes:'))
    for i in range(n):
        ele=int(input())
        arr.append(ele)
    print('final array to use bubble sort is is:',arr)
    bubbleSort(arr)
    print('sorted sum is:',arr)
if _name=='main_':
    main()     

 
