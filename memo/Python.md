## Handling recursion limit  

- [Reference]](https://www.geeksforgeeks.org/python-handling-recursion-limit/)

``` python
import sys
sys.setrecursionlimit(10**6)
```

파이썬의 재귀 제한을 늘리는 코드입니다  
파이썬의 recursionlimit의 default값은 1000입니다  

``` shell
$python
>>> import sys
>>> sys.getrecursionlimit()
1000
>>> 
```

## 자료구조의 Empty 판단  

str, list, set, tuple, dict 등 자료구조의 Empty 판단은 bool() 메소드를 사용하거나 조건문에 해당 객체를 바로 써주면 됩니다  

``` python
if items:
    print("items is not Empty")
elif not items:
    print("items is Empty")
```  

``` python
if bool(items):
    print("items is not Empty")
elif not bool(items):
    print("items is Empty")
```  

bool()을 사용하는 방법은 숫자형 데이터도 사용 가능합니다  
  
단, None 여부를 판단할 때는 아래 방법을 사용합니다  

``` python
if item is None:
    print("item is None")
```  