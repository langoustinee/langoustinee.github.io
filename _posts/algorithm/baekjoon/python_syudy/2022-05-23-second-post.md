--- 
title: "[알고리즘 스터디] 백준 2588번" 

excerpt: "코딩테스트 준비를 위해 백준에서 알고리즘 공부를 시작했다." 

categories: 
- Python

tags: 
- [Blog, algorithm, study, python, baekjoon]

toc: true
toc_sticky: true

date: 2022-05-23
--- 
<center><img src="https://d2gd6pc034wcta.cloudfront.net/images/logo@2x.png"></center>

# 백준 알고리즘 스터디 시작!
코딩테스트 준비를 위해 백준에서 알고리즘 공부를 시작했다.
1단계 사칙연산 풀이의 마지막 문제인 2588번 곱셈문제 풀이를 기록한다.

<center><img src="/assets/images/1.png"></center>

(1)과 (2)위치에 들어갈 세 자리 자연수가 주어질 때 (3), (4), (5), (6)위치에 들어갈 값을 구하는 프로그램을 작성하시오.

문제: 입력받은 세자리수의 인덱스를 찾아서 곱해줘야 하는데 어떻게 인덱싱을 하여 곱해줄지가 문제였다.

해결: 반복문을 통해 두번째 세자리수(B)를 거꾸로 반복하여 첫번째 세자리수(A)를 반복할 때마다 곱해주니 3, 4, 5 위치의 값을 알 수 있었다.
<script src="https://gist.github.com/Jooney-95/c01302e3e30577e135f9027b28acf655.js"></script>

```python
a,b = list(map(str,input())), list(map(str,input()))
for i in reversed(b):
    x = ''.join(a)
    y = ''.join(b)
    print(int(i)*int(x))
print(int(x)*int(y))
```
