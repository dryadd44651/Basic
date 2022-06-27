Time Complexity
It measures the time taken to execute each statement of code in an algorithm.
f(n): function f with input n
Asymptotic Notation
g(n) is an arbitrary time complexity you are trying to relate to your algorithm.
Big-Theta Θ(·): find upper bound and lower bound for f(n)
f(n)=2n+1
We can find a c1 g(n) and c2 g(n) for Θ
Here, g(n) = n
c1=1,c2=3
n<=2n+1<=3n
f(n)∈Θ(n)

Big-O: upper bound O(·)>=f(·)
Big-Omega: lower bound Ω(·)<=f(·)
Little-O: upper bound o(·)>f(·)
Little-Omega: lower bound ω(·)<f(·)
When we present the time complexity, we will remove the coefficient and constant
Example:
When n is big enough.
100n+10000<n^2
Coefficients and constant is meaningless.
O(1)<O(logN)<O(N)<O(NlogN)<O(N^2)<O(2^N)<O(N!)

![img](https://www.freecodecamp.org/news/content/images/2021/06/0_MPwgKd4lgXACfuNt.png)

O(1)
1+1
O(logN)
Binary search
O(N)
Find max, find mini, search
O(NlogN)
Merge Sort
O(N^2)
Select sort, bubble sort
http://alrightchiu.github.io/SecondRound/complexityasymptotic-notationjian-jin-fu-hao.html#bw
Why people always use Big O not big theta
https://www.zhihu.com/question/20677334
https://softwareengineering.stackexchange.com/questions/99372/why-is-big-o-taught-instead-of
-big-theta
When people saying big O, they actually want you to answer big theta.
But people still saying big O, because sometimes big theta is hard to find.
