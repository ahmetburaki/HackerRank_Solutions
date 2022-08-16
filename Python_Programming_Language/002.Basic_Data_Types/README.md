# [HackerRank Python Solutions - Basic Data Types](https://www.hackerrank.com/domains/python?filters%5Bsubdomains%5D%5B%5D=py-basic-data-types "Python - Basic Data Types")

### [List Comprehensions](https://www.hackerrank.com/challenges/list-comprehensions?isFullScreen=true "List Comprehensions")

```python
    x = int(input())
    y = int(input())
    z = int(input())
    n = int(input())
    
    result = []
    
    for i in range(0, x+1):
        for a in range(0, y+1):
            for b in range(0, z+1):
                if(i+a+b) !=n:
                    result.append([i,a,b])
print(result)
```

### [Find the Runner-Up Score!](https://www.hackerrank.com/challenges/find-second-maximum-number-in-a-list?isFullScreen=true "Find the Runner-Up Score!")

```python
    n = int(input())
    arr = map(int, input().split())
    my_list=list(arr)
    
    my_list.sort()
    highest_num = max(my_list)
    
    for i in range(len(my_list)-1, -1, -1):
        if my_list[i] < highest_num:
            break
            
    print(my_list[i])
```

### [Nestes Lists](https://www.hackerrank.com/challenges/nested-list?isFullScreen=true "Nested Lists")

```python
    students = []
    for _ in range(int(input())):
        name = input()
        score = float(input())
        
        students.append([name, score])
    
    lowest = min([a[1] for a in students])
    second_low = min(list(filter(lambda a: a > lowest, [a[1] for a in students])))
    
    out = [a[0] for a in students if (a[1] == second_low)]
    out.sort()
    
    print("\n".join(out))
```

### [Finding the Percentage](https://www.hackerrank.com/challenges/finding-the-percentage?isFullScreen=true "Finding the Percentage")

```python
    n = int(input())
    student_marks = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        student_marks[name] = scores
    query_name = input()
    score_rec = []
    score_rec = student_marks[query_name]

    sum_marks = 0
    for i in score_rec:
        sum_marks += i
    percent = "{:.2f}".format(sum_marks/len(score_rec))
    print(percent)
```

### [Lists](https://www.hackerrank.com/challenges/python-lists?isFullScreen=true "Lists")

```python
    n = int(input())
    list_of_nums = []
    for _ in range(n):
        a = input().split()
        cmd = a[0]
        arg = a[1:]
        if cmd !="print":
            cmd += "("+ ",".join(arg) +")"
            eval("list_of_nums ."+cmd)
        else:
            print (list_of_nums)
```

### [Tuples](https://www.hackerrank.com/challenges/python-tuples?isFullScreen=true "Tubles")

```python
    print(hash(tuple(integer_list)))
```

Congrats! You just solved all the Basic Data Types challenges in Python!