[^_^]: YanLei 2018/9/6
##### 1:
* (a): $ P(everyPersonGetsHis/HerHatBack) = \frac{1}{n!} $
* (b): $ P(firstMPersonsGetTheirOwnHatBack) = \frac{(n-m)!}{n!} $
* (c): $ P(firstMPersonGetLastMPersonsHat) = \frac{m!(n-m)!}{n!} $
* (d): $ P(firstMPersonsPickUpCleanHats) = (1-p)^m $
* (e): $ P(exactlyMPersonsWillPickUpCleanHats) = {n \choose m}\cdot(1-p)^mp^{n-m} $
<br/>
##### 2:
$ P(AliceWins) = \frac{{4 \choose 4}{48 \choose 4}}{52 \choose 8} $
<br/>
##### 3:
* (a): First, We can rewrite the terms of right-hand side: $ P(X \ge k) = \displaystyle\sum_{j=k}^\infty p_X(j)  $. Then processed as follows:
$ \displaystyle\sum_{k=1}^{\infty}P(X \ge k) $
$ =\displaystyle\sum_{k=1}^{\infty}\displaystyle\sum_{j=k}^{\infty}p_X(j) $
$ =\displaystyle\sum_{j=1}^{\infty}\displaystyle\sum_{k=1}^{j}p_X(j) $
$ =\displaystyle\sum_{j=1}^{\infty}j\cdot p_X(j) $
$ =E[X] $
* (b):First we consider the situation where $ a=1, b=n $.According to the formula in the previous part, we have:
$ E[Y] = \displaystyle\sum_{k=1}^{\infty}P(Y\ge k) $
$ =\displaystyle\sum_{k=1}^{a-1}P(Y \ge k) + \displaystyle\sum_{k=a}^bP(Y\ge k) + \displaystyle\sum_{k=b+1}^{\infty}P(Y\ge k) $
$ =a - 1 + \displaystyle\sum_{k=1}^{b-a+1}\frac{k}{b-a+1} + 0 $
$ = a - 1 + \frac{b-a+2}{2} $
$ =\frac{a+b}{2} $
<br/>
##### 4:
X   |  Y   | Difference
:--:| :--: | :--:
1   |  1   | 0
2   |  2   | 0
3   |  3   | 0
1   |  2   | 1
2   |  1   | -1
2   |  3   | 1
3   |  2   | -1
1   |  3   | 2
3   |  1   | -2
* (a)
PMF: $$ p_X(k) = \begin{cases}
         \frac{1}{3} &\text{if } k = 0\\
         \frac{2}{9} &\text{if } k = 1, -1\\
         \frac{1}{9} &\text{if } k = 2, -2\\
         0 &\text{otherwise}  
        \end{cases}
     $$  
Expected value:$$ E[X] = 0 \cdot \frac{1}{3} + (1-1) \cdot \frac{2}{9} + (2-2) \cdot \frac{1}{9} = 0 $$
Variance: $$ var(X) = 0^2 \cdot \frac{1}{3} + (1^2 + (-1)^2) \cdot \frac{2}{9} + (2^2 + (-2)^2) \cdot \frac{1}{9} = \frac{4}{3} $$
* (b)
PMF of $X^2$:
$$ 
    p_X(k) = \begin{cases}
     \frac{1}{3} &\text{if } k = 0\\
     \frac{4}{9} &\text{if } k = 1\\
     \frac{2}{9} &\text{if } k = 4\\
     0 &\text{otherwise}
    \end{cases} 
$$
<br/>
##### 5:
Suppose we have a group of n persons. Consider clubs that consist of a chair and a vice chair and a number of (possibly zero) of additional club members. Let us count the number of all possible clubs of this type in two different ways, thereby obtaining an algebraic identity.
There are $n$ choices for the chair and $n-1$ choices for the vice chair. Once the leaders is chosen, we are left with a set of $n-2$ persons, and all the possible subsets can be chosen. So, the total number is $n(n-1)2^{n-2}$.
Alternatively, for a fixed k, we have $ n \choose k $ choices. Then, we can select a chair and a vice chair from these $k$ persons, so we have $k(k-1)$ choices. By adding over all possible club sizes k, we obtain the number of possible clubs as $ \displaystyle\sum_{k=2}^n k(k-1){n \choose k} $, thereby showing the identity:$$ \displaystyle\sum_{k=2}^{n}k(k-1){n \choose k} = n(n-1)2^{n-2} $$
<br/>
##### G1:
Let $N_1, N_2, N_3, N_4, N_5, N_6, N_7, N_8$ denote the numbers of red, orange, yellow, green, blue, black, white, and violet jelly beans in a jar. So we have $ \displaystyle\sum_{i=1}^8N_i = 200 $. And according to the description, we know $ N_1 = N_2, N_3 = N_4, N_5 = N_6-1, N_7 = N_8 - 3 $. Then $ \displaystyle\sum_{i=1}^8 N_i = 2 \cdot(N_1 + N_3 + N_5 + N_7) + 4 = 200 $. So, what we need to do is to solve the equation blow:
$$ N_1 + N_3 + N_5 + N_7 = 98$$
Suppose there are $98$ balls arranged in a straight line. How many methods do you have to cut the line into $4$ segements(possibly zero length)? 
You just need to put $4-1$ sticks to separate those balls. So the total number of methods is $ {98+4-1 \choose 4-1} $. This can easily generalize to $ {n+k-1 \choose k-1} $.
