# .PYTHON
import random
def findpn(f):
    if (f > 0):
        return f, "is a positive number"
    else:
        return f, "is a negative number"
def findeo(f):
    if (f % 2 == 0):
        return f, "is an even number"
    else:
        return f, "is an odd number"
def findpc(f):
    if(f>2):
        for i in range(2,f):
            c=0
            if(f%i==0):
                c+=1
                if c>1:
                    return f,"is a composite number"
                else:
                    return f,"is a prime number"
            else:
                return f,"is a prime number"
    else:
        return f,"is a prime number"
a=int(input("Start"))
b=int(input("End"))
f=random.randrange(a,b)
print(findpn(f))
print(findeo(f))
print(findpc(f))
