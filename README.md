# title()

``` python
string = "hello world"
titled_string = string.title()
print(titled_string) # Вывод: Hello World
```
# type()


```python
num = 10
string = "hello"
my_list = [1, 2, 3]

print(type(num))     # Вывод: <class 'int'>
print(type(string)) # Вывод: <class 'str'>
print(type(my_list)) # Вывод: <class 'list'>
```
Так же покажу как пофиксить и убрать <class> и тд
```python
num = 10
string = "hello"
my_list = [1, 2, 3]

print(type(num).__name__)     # Вывод: int
print(type(string).__name__) # Вывод: str
print(type(my_list).__name__) # Вывод: list
```
# islower()

```python
string1 = "hello"
string2 = "Hello"
string3 = "Hello World"

print(string1.islower()) # Вывод: True
print(string2.islower()) # Вывод: False
print(string3.islower()) # Вывод: False
```
# isupper()
```python
string1 = "HELLO"
string2 = "Hello"
string3 = "hello world"

print(string1.isupper()) # Вывод: True
print(string2.isupper()) # Вывод: False
print(string3.isupper()) # Вывод: False
```
# re.sub() (из модуля re)

```python
import re

string = "Hello world, hello Python!"
new_string = re.sub(r"hello", "hi", string, flags=re.IGNORECASE)
print(new_string) # Вывод: Hi world, hi Python!
print(re.sub(r'[^a-zA-Z0-9]', '', string))#Вывод:HelloworldhelloPython
```
# count()


```python
string = "abcabcabc"
count_a = string.count("a")
count_abc = string.count("abc")

print(count_a)    # Вывод: 3
print(count_abc) # Вывод: 3
```
# set()


```python
my_list = [1, 2, 2, 3, 4, 4, 5]
my_set = set(my_list)
print(my_set) # Вывод: {1, 2, 3, 4, 5}
```
# sorted()


```python
my_list = [3, 1, 4, 1, 5, 9, 2, 6]
sorted_list = sorted(my_list)
sorted_list_reverse = sorted(my_list, reverse=True)

print(sorted_list)       # Вывод: [1, 1, 2, 3, 4, 5, 6, 9]
print(sorted_list_reverse) # Вывод: [9, 6, 5, 4, 3, 2, 1, 1]
```
