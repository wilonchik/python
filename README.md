# `title()`

``` python
string = "hello world"
titled_string = string.title()
print(titled_string) # Вывод: Hello World
```
# `type()`


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
# `islower()`

```python
string1 = "hello"
string2 = "Hello"
string3 = "Hello World"

print(string1.islower()) # Вывод: True
print(string2.islower()) # Вывод: False
print(string3.islower()) # Вывод: False
```
# `isupper()`
```python
string1 = "HELLO"
string2 = "Hello"
string3 = "hello world"

print(string1.isupper()) # Вывод: True
print(string2.isupper()) # Вывод: False
print(string3.isupper()) # Вывод: False
```
# `re.sub() (из модуля re)`

```python
import re

string = "Hello world, hello Python!"
new_string = re.sub(r"hello", "hi", string, flags=re.IGNORECASE)
print(new_string) # Вывод: Hi world, hi Python!
print(re.sub(r'[^a-zA-Z0-9]', '', string))#Вывод:HelloworldhelloPython
```
# `count()`


```python
string = "abcabcabc"
count_a = string.count("a")
count_abc = string.count("abc")

print(count_a)    # Вывод: 3
print(count_abc) # Вывод: 3
```
# `set()`


```python
my_list = [1, 2, 2, 3, 4, 4, 5]
my_set = set(my_list)
print(my_set) # Вывод: {1, 2, 3, 4, 5}
```
# `sorted()`


```python
my_list = [3, 1, 4, 1, 5, 9, 2, 6]
sorted_list = sorted(my_list)
sorted_list_reverse = sorted(my_list, reverse=True)

print(sorted_list)       # Вывод: [1, 1, 2, 3, 4, 5, 6, 9]
print(sorted_list_reverse) # Вывод: [9, 6, 5, 4, 3, 2, 1, 1]
```
# `" ".join()`

1. Объединение списка строк:
```python
words = ["This", "is", "a", "sentence."]
sentence = " ".join(words)
print(sentence) # Вывод: This is a sentence.
```

Здесь пробел (" ") используется в качестве разделителя.

2. Объединение списка чисел (после преобразования в строки):
```python
numbers = [1, 2, 3, 4, 5]
number_string = ", ".join(map(str, numbers)) # map(str, numbers) преобразует числа в строки
print(number_string) # Вывод: 1, 2, 3, 4, 5
```

Обратите внимание на использование функции `map(str, numbers)` для преобразования чисел в строки, так как `join()` работает только со строками.

3. Использование пустой строки для конкатенации:
```python
parts = ["Hello", "world"]
combined = "".join(parts)
print(combined) # Вывод: HelloWorld
```

Пустая строка "" используется для объединения без разделителя.

4. Объединение строк с другим разделителем:
```python
items = ["apple", "banana", "cherry"]
result = "-".join(items)
print(result) # Вывод: apple-banana-cherry
```
# `isdigit()`

```python
string1 = "12345"
string2 = "123abc"
string3 = "12.34" # Точка не является цифрой
string4 = "-123" # Минус не является цифрой
string5 = ""       # Пустая строка

print(string1.isdigit()) # Вывод: True
print(string2.isdigit()) # Вывод: False
print(string3.isdigit()) # Вывод: False
print(string4.isdigit()) # Вывод: False
print(string5.isdigit()) # Вывод: False
```

# `isalpha()`


```python
string1 = "hello"
string2 = "Hello World" # Пробел делает результат False
string3 = "Hello123"     # Цифры делают результат False
string4 = "你好世界"   # Работает с нелатинскими алфавитами
string5 = ""             # Пустая строка

print(string1.isalpha()) # Вывод: True
print(string2.isalpha()) # Вывод: False
print(string3.isalpha()) # Вывод: False
print(string4.isalpha()) # Вывод: True
print(string5.isalpha()) # Вывод: False
```
