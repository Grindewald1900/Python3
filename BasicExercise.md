## 1. I/O

### 1.1 
```Python
str = "abcdefg"
print(r"a\n")
print(str)
print("2:"+str[0:-1])
print(str[-1:0])
print(str[0:])
print(str*2)
print((str+"\n")*2)
input("\n Exit:")

```

### 1.2
```Python
import sys
print("======================= import module ============================")
print("CMD")
for i in sys.argv:
   print(i)
print("\n python path:",sys.path)
```

### 1.3
```Python
def reversewords(input):
   inputwords = input.split(" ")
   inputwords = inputwords[-1::-1]
   out = " ".join(inputwords)
   return out

result = reversewords(input("Input a string"))
print(result)
```

## 2. Basic data types
### 2.1
```Python
a = 1; b = 1.0; c = True
print(type(a),type(b),type(c))
list = [1,2,"a","b",5.00,6.00,True,False]

print(list)
print(list[0:5])
print(list[1:2])
print(list[0::2])
print((list[1:2])*2)
```
## 3. Namespace
### 3.1
```Python
num = 666

def changeGlobal(): #change the global value num
   global num
   print(num)
   num = 999
   print(num)

changeGlobal()
print(num)
```
