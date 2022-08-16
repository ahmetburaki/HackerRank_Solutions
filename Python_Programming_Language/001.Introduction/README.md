# [HackerRank Python Solutions - Introduction](https://www.hackerrank.com/domains/python?filters%5Bsubdomains%5D%5B%5D=py-introduction "Python - Introduction")

### [Say "Hello, World!" With Python](https://www.hackerrank.com/challenges/py-hello-world?isFullScreen=true "Say 'Hello, World!' With Python")

```python
print("Hello,World!")
```

### [Python If-Else](https://www.hackerrank.com/challenges/py-if-else?isFullScreen=true "Python If-Else")

```python
def wierd(n):
    if n % 2 == 1 or 6 <= n <= 20:
        print('Weird')
    else:
        print('Not Weird')

wierd(int(input()))
```
### [Arithmetic Operators](https://www.hackerrank.com/challenges/python-arithmetic-operators?isFullScreen=true "Arithmetic Operators")

```python
a, b = int(input()), int(input())
print((a + b), (a - b), (a * b), sep='\n')
```

### [Python: Division](https://www.hackerrank.com/challenges/python-division?isFullScreen=true "Python: Division")

```python
a, b = int(input()), int(input())
print(a // b, a / b, sep='\n')
```

### [Loops](https://www.hackerrank.com/challenges/python-loops?isFullScreen=true "Loops")

```python
for i in range(int(input())):
    print(i ** 2)
```

### [Write a Function](https://www.hackerrank.com/challenges/write-a-function?isFullScreen=true "Write a Function")

```python
def is_leap(YEAR):
    return YEAR % 4 == 0 and (YEAR % 400 == 0 or YEAR % 100 != 0)
    
year = int(input())
print(is_leap(year))
```

### [Print Function](https://www.hackerrank.com/challenges/python-print?isFullScreen=true "Print Function")

```python
n = int(input())

for _ in range(1, n+1):
    print(_, end="")

```

Congrats! You just solved all the Introduction challenges in Python!
