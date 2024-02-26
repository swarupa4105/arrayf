# arrayf
# array functions
import numpy as np
a=np.zeros((3,3),dtype='int')
print(a) 
print("\n")
b=np.ones((4,4),dtype="int")
print(b)
print("\n")
c=np.eye((4),dtype="int")
print(c)
print("\n")
d=c.reshape((2,8))
print(d)
print("\n")
e=np.arange(0,50,5)
print(e)
print("\n")
f=np.linspace(0,5,100)
print(f)
print("\n")
g=np.array([[1,2,3],[4,5,6],[7,8,9]])
temp=g[:3,::2]
print(temp)
h=np.full((4,5),3)
print(h)
i=np.full((4,5),3,dtype="complex")
print(i)
j=[1,2,3,4]
you=np.fromiter(j,dtype="int")
print(you)
k=[83,119,97,114,117,112,97]
me=np.fromiter(k,dtype="U1")
print(ascii(me))
# to calculate time
import numpy as np
import timeit
print(np.sum(np.arange(15000)))
%timeit np.sum(np.arange(15000))
total=0
for i in range(0,15000):
    total=total+i
l=total
print(str(l))
%timeit l
# broad casting
import numpy as np
m=np.array([90,80,70,60,50])
n=np.array([90,80,70,60,50])
o=m*n
print(o)
