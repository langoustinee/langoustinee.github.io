--- 
title: "[알고리즘 스터디] 백준 2588번" 

excerpt: "코딩테스트 준비를 위해 백준에서 알고리즘 공부를 시작했다." 

categories: 
- Blog 

tags: 
- [Blog, algorithm, study, Backjoon]

toc: true
toc_sticky: true

date: 2022-05-23
--- 

<img src="/_image/1.png">
코딩테스트 준비를 위해 백준에서 알고리즘 공부를 시작했다.
1단계 사칙연산 풀이의 마지막 문제인 2588번 곱셈문제 풀이를 기록한다.

<pre>
<code>
a,b = list(map(str,input())), list(map(str,input()))
for i in reversed(b):
    x = ''.join(a)
    y = ''.join(b)
    print(int(i)*int(x))
print(int(x)*int(y))
</code>
</pre>
