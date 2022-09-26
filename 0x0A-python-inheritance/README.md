0x0A. Python - Inheritance
An introductory project on inheritance in Python

File Descriptions
(0-lookup.py)[0-lookup.py] - A function that returns the list of available attributes and methods of an object:
Prototype: def lookup(obj):
Returns a list object
Not allowed to import any module
guillaume@ubuntu:~/0x0A$ cat 0-main.py
#!/usr/bin/python3
lookup = __import__('0-lookup').lookup

class MyClass1(object):
    pass

class MyClass2(object):
    my_attr1 = 3
    def my_meth(self):
        pass

print(lookup(MyClass1))
print(lookup(MyClass2))
print(lookup(int))

 
(1-my_list.py)[1-my_list.py] - A class MyList that inherits from list:
Public instance method: def print_sorted(self): that prints the list, but sorted (ascending sort)
Assumes that all the elements of the list will be of type int
Not allowed to import any module
guillaume@ubuntu:~/0x0A$ cat 1-main.py
#!/usr/bin/python3
MyList = __import__('1-my_list').MyList

my_list = MyList()
my_list.append(1)
my_list.append(4)
my_list.append(2)
my_list.append(3)
my_list.append(5)
print(my_list)
my_list.print_sorted()
print(my_list)

0x0A$ ./1-main.py
[1, 4, 2, 3, 5]
[1, 2, 3, 4, 5]
[1, 4, 2, 3, 5]
 
(2-is_same_class.py)[2-is_same_class.py] - A function that returns True if the object is exactly an instance of the specified class; otherwise False:
Prototype: def is_same_class(obj, a_class):
Not allowed to import any module

#!/usr/bin/python3
is_same_class = __import__('2-is_same_class').is_same_class

a = 1
if is_same_class(a, int):
    print("{} is an instance of the class {}".format(a, int.__name__))
if is_same_class(a, float):
    print("{} is an instance of the class {}".format(a, float.__name__))
if is_same_class(a, object):
    print("{} is an instance of the class {}".format(a, object.__name__))

a = 1
if is_kind_of_class(a, int):
    print("{} comes from {}".format(a, int.__name__))
if is_kind_of_class(a, float):
    print("{} comes from {}".format(a, float.__name__))
if is_kind_of_class(a, object):
    print("{} comes from {}".format(a, object.__name__))

 
(4-inherits_from.py)[4-inherits_from.py] - A function that returns True if the object is an instance of a class that inherited (directly or indirectly) from the specified class ; otherwise False:
Prototype: def inherits_from(obj, a_class):
Not allowed to import any module
guillaume@ubuntu:~/0x0A$ cat 4-main.py
#!/usr/bin/python3
inherits_from = __import__('4-inherits_from').inherits_from

a = True
if inherits_from(a, int):
    print("{} inherited from class {}".format(a, int.__name__))
if inherits_from(a, bool):
    print("{} inherited from class {}".format(a, bool.__name__))
if inherits_from(a, object):
    print("{} inherited from class {}".format(a, object.__name__))




__________________________________________________WRITTEN AND MANAGED BY


JUSTICEMENSAH-ALX    AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAALLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLXXXXXXXXXXXXXXXXXXXXXXXXXXX 
