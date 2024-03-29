<!-- for readme.md -->
For 
===
> 이 문서는 For 반복문에 대해 설명하는 문서입니다.
> 
> 해당 문서를 읽기전 [같이사용되는함수](../../%EA%B0%99%EC%9D%B4_%EC%82%AC%EC%9A%A9%EB%90%98%EB%8A%94_%ED%95%A8%EC%88%98/README.MD) 와 [반복문](../../%EB%B0%98%EB%B3%B5%EB%AC%B8/README.md) 선행해서 읽기 권장합니다.

## For 반복문
    For 반복문은  프로그래밍 작성시 반복의 범위가 정해지는 경우 사용한다.
    타 언어에서 사용하는 for 반복문과는 조금 다르지만 익숙해진다면 효율 적인 코드를 작성할수있다.

    
     

## 기본적인 For 🙃

    


```python 
# 기본형 ! 

for 반복자 in 반복할수있는것(리슽, 튜플, 문자열 등등):
    수행할 작업 1
    수행할 작업 2
    수행할 작업 3
    ...

```


> 오 . . 이렇게 봐서는 어떻게 사용하는지 나도 모를거같다.  
> 예문을 통해 조금더 쉽게 배워보자.


```python
# = 을 5번 출력하는코드
# 예제 1
for value in range(5) :
    print("=", end =" ")

>>> = = = = = 
```
> range의 범위만큼 for 문의 내용을 반복한다. range()함수는 [알아보기](../../%EA%B0%99%EC%9D%B4_%EC%82%AC%EC%9A%A9%EB%90%98%EB%8A%94_%ED%95%A8%EC%88%98/README.MD#range) 에서 간략하게 확인 할수있다.
>
> 🤨 : "range()에 대해서는 얼추 알겠는데.. for 뒤에있는 value 는 전혀 모르겠는데요 ?"
>
> 이번 예문에서는 value 변수에 대한 정보도 없고 사용하지않아 추측하기 어렵다. 
다음 예문을 통해 반복자를 이해 해보자.


```python
# 반복자를 사용하는 반복문
# 예제 2
value_list = [1,2,3,4]

for value in value_list :
    print(value , end = " ")

>>> 1 2 3 4 
```
> 간략하게 설명을 더해보자면 value_list = [1,2,3,4] 안에 들어있는 값을 하나씩 value에 넣어 더 이상 넣을수 없을떄 까지 반복한다고 이해하면 된다.
> 


## Example  


```python

    for number in reversed(range(5)):
        print(number ,end =" ") 

```

<details>
  <summary>Answer</summary>

    ```python
        >>> 4 3 2 1 0
    ```

</details>


```python

    for odd in range(1,10):
        if odd%2==1:
            print(odd , end=" ")
```



<details>
  <summary>Answer</summary>

    ```python
        >>> 1 3 5 7 9
    ```

</details>


```python

        for number in range(1,4):
            for num in range(1,5):
                print(f"{number} * {num}= {number*num}" , end =" ")
            print()

```

<details>
  <summary>Answer</summary>

    ```python
        
        >>>1 * 1= 1 1 * 2= 2 1 * 3= 3 1 * 4= 4 
        >>>2 * 1= 2 2 * 2= 4 2 * 3= 6 2 * 4= 8
        >>>3 * 1= 3 3 * 2= 6 3 * 3= 9 3 * 4= 12

    ```

</details>

