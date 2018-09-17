##### 1：
* (a): 
According to the **Normalization Axiom**, we have $ \displaystyle\sum_x\sum_y p_{X, Y}(x, y) = 1 $. Using the joint PMF:
$ \displaystyle\sum_x\sum_y p_{X, Y} (x, y) $
$ = c \cdot (2 + 10 + 5 + 13 + 17 + 25) $
$ = c \cdot 72 $
$ = 1 $
So, $ c = \boxed{\frac{1}{72}} $
<br/>
* (b): 
$ P(Y<X) $
$ = p_{X, Y}(2, 1) + p_{X, Y}(4, 1) + p_{X, Y}(4, 3) $
$ = \frac{1}{72} \cdot (5 + 17 + 25) $
$ = \boxed{\frac{47}{72}} $
<br/>
* (c):
$ P(Y>X) $
$ = p_{X, Y}(1, 3) + p_{X, Y}(2, 3) $
$ = \frac{1}{72} \cdot (10 + 13) $
$ = \boxed{\frac{23}{72}} $
<br/>
* (d):
$ P(X=Y) $
$ = p_{X, Y}(1, 1) $
$ = \boxed{\frac{2}{72}} $
<br/>
* (e):
$ P(Y=3) $
$ = p{X, Y}(1, 3) + p_{X, Y}(2, 3) + p_{X, Y}(4, 3) $
$ = \frac{1}{72} \cdot (10 + 13 + 25) $
$ = \boxed{\frac{48}{72}} $
* (f):
$ p_X(1) = p_{X, Y}(1, 1) + p_{X, Y}(1, 3) = \frac{12}{72} $
$ p_X(2) = p_{X, Y}(2, 1) + p_{X, Y}(2, 3) = \frac{18}{72} $
$ p_X(4) = p_{X, Y}(4, 1) + p_{X, Y}(4, 3) = \frac{42}{72} $
So, we have
$$ \boxed{p_X(x) = \begin{cases}
    \frac{12}{72} &\text{if } x=1\\
    \frac{18}{72} &\text{if } x=2\\
    \frac{42}{72} &\text{if } x=4\\
    0 &\text{otherwise}
    \end{cases}}$$
$ p_Y(1) = p_{X, Y}(1, 1) + p_{X, Y}(2, 1) + p_{X, Y}(4, 1) = \frac{24}{72} $
$ p_Y(3) = p_{X, Y}(1, 3) + p_{X, Y}(2, 3) + p_{X, Y}(4, 3) = \frac{48}{72} $
So, we have 
$$ \boxed{p_Y(y) = \begin{cases}
    \frac{24}{72} &\text{if } y=1\\
    \frac{48}{72} &\text{if } y=3\\
    0 &\text{otherwise}
    \end{cases}} $$
<br/>
* (g):
$ E[X] $
$ = 1 \cdot \frac{12}{72} + 2 \cdot \frac{18}{72} + 4 \cdot \frac{42}{72} $
$ = \boxed{3} $
$ E[Y] $
$ = 1 \cdot \frac{24}{72} + 3 \cdot \frac{48}{72} $
$ = \boxed{\frac{7}{3}} $
It is easy to verify that $X$ and $Y$ are **NOT** independent. So, we can't use the formula $ E[XY] = E[X]E[Y] $. 
$ E[XY] $
$ = \displaystyle\sum_x\sum_y xyp_{X, Y}(x, y) $
$ = 1 \cdot \frac{2}{72} + 3 \cdot \frac{10}{72} + 2 \cdot \frac{5}{72} + 6 \cdot \frac{13}{72} + 4 \cdot \frac{17}{72} + 12 \cdot \frac{25}{72} $
$ = \boxed{\frac{61}{9}} $
<br/>
* (h):
$ Var(X) $
$ = (1 - 3)^2 \cdot \frac{12}{72} + (2 - 3)^2 \cdot \frac{18}{72} + (4 -3)^2 \cdot \frac{42}{72} $
$ =\boxed{\frac{3}{2}} $
$ Var(Y) $
$ = (1 - \frac{7}{3})^2 \cdot \frac{24}{72} + (3 - \frac{7}{3})^2\cdot \frac{48}{72} $
$ = \boxed{\frac{8}{9}} $
$ Var(X+Y) $
$ =  E[(X+Y)^2] - (E[X+Y])^2 $
$ = \frac{547}{18} - (E[X] + E[Y])^2 $
$ = \frac{547}{18} - \frac{256}{9} $
$ = \boxed{\frac{35}{18}} $
<br/>
* (j):
First, we compute the conditional PMF of X。
$ p_{X|A}(1) = \frac{P({X=1}\cap A)}{P(A)} = \frac{2}{49} $
$ p_{X|A}(2) = \frac{P({X=2}\cap A)}{P(A)} = \frac{5}{49} $
$ p_{X|A}(4) = \frac{P({X=4}\cap A)}{P(A)} = \frac{42}{49} $
So, we have
$$ p_{X|A}(x) = \begin{cases}
    \frac{2}{49} &\text{if } x=1\\
    \frac{5}{49} &\text{if } x=2\\
    \frac{42}{49} &\text{if } x=4\\
    0 &\text{otherwise}
    \end{cases} $$
$ E[X|A] $
$ = 1 \cdot \frac{2}{49} + 2 \cdot \frac{5}{49} + 4 \cdot \frac{42}{49} $
$ = \boxed{\frac{180}{49}} $
$ Var[X|A] $
$ = (1 - \frac{180}{49})^2 \cdot \frac{2}{49} + (2 - \frac{180}{49})^2 \cdot \frac{5}{49} + (4 - \frac{180}{49})^2 \cdot \frac{42}{49}$
$ = \boxed{\frac{1606}{2401}} $
<br/>
##### 2:
* (a):
$$ \boxed{{6 \choose 3} \frac{1}{4}^3 (1 - \frac{1}{4})^3} $$
<br/>
* (b):
Define event $A=$ the first roll is 1, event $B=$ exactly two of the six rolls result in 1.
$$ P(A|B) = \frac{P(A\cap B)}{P(B)} = \frac{\frac{1}{2} \cdot {5 \choose 1} \cdot \frac{1}{2} \cdot (1-\frac{1}{2})^4}{{6 \choose 2} \cdot \frac{1}{2}^4 \cdot (1 - \frac{1}{2})^4} = \boxed{\frac{1}{3}} $$
<br/>
* (c):
Because we knew that among the 6 rolls, there are exactly three $2's$ and three $1's$, we just need to compute the fraction of $121212$ among all the permutation of 6 rolls. $$ P(121212|three1three2) = \frac{3!3!}{6!} = \boxed{\frac{1}{20}} $$
<br/>
* (d):
Let $A$ denotes the event that *at least one roll resulted in 3*, $Y$ denotes the number of 3's. First, we can compute $ P(A) = 1 - \frac{3}{4}^6 $. So, by definition, $$ p_{Y|A}(y|A) = \frac{P(\{Y = y\}\cap A)}{P(A)} = \boxed{\begin{cases}
\frac{{6 \choose y}\frac{1}{4}^y \frac{3}{4}^{6-y}}{1-\frac{3}{4}^6} &\text{if } y=1,2,3,4,5,6\\
0 &\text{otherwise}
\end{cases}} $$
<br/>
##### 3:
To use the definition $ P(X=i|X+Y=n) = \frac{P(\{X=i\} \cap \{X+Y=n\})}{P(\{X+Y=n\})} $, we first compute:
$ P(X+Y=n) $.
$ = \displaystyle\sum_{j=1}^{n-1}P(X=j)P(Y=n-j) $
$ = \displaystyle\sum_{j=1}^{n-1}(1-p)^{j-1}p \cdot (1-p)^{n-j-1}p $
$ = (n-1)(1-p)^{n-2}p^2 $
Then compute：
$ P(X=i \cap X+Y=n) $
$ = (1-p)^{i-1}p \cdot (1-p)^{n-i-1}p $
$ = (1-p)^{n-2}p^2 $
So, $$ P(X=i|X+Y=n) = \frac{(1-p)^{n-2}p^2}{(n-1)(1-p)^{n-2}p^2} = \boxed{\frac{1}{n-1}} $$
<br/>
##### 4:
* (a):
Since $P(A) \not = 0$, so we can use the formula $ P(B|A) = \frac{P(A \cap B)}{P(A)} $ to verify the independence: $$ P(B|A) = \frac{p \cdot {8 \choose 6}p^6(1-p)^2}{{8 \choose 6}p^6(1-p)^2} = p = P(B) $$
<br/> 
* (b):
Let $C$ and $D$ denote the events *3 heads in the first four tosses* and *2 heads in the last three tosses* repectively.
$$ P(C \cap D) = {4 \choose 3}p^3(1-p) \cdot {3 \choose 2}p^2(1-p) = \boxed{12p^5(1-p)^2} $$
<br/>
* (c):
Let $E$ and $F$ denote the events *4 heads in the first 7 tosses* and *2nd head occured in 4th toss* respectively.
$$ P(E|F) = \frac{P(E\cap F)}{P(F)} = \frac{{3 \choose 1}p(1-p)^2p{3 \choose 2}p^2(1-p)}{{7 \choose 4}p^4(1-p)^3} = \boxed{\frac{9}{35}} $$
<br/>
* (d):
Let $G$ and $H$ denote the events *5 heads in the first 8 tosses* and *3 heads in the last 5 tosses* respectively.  Using **Total Probability Law**, we have:
$ P(G \cap H) $
$ = P(G \cap H|I_1) + P(G \cap H|I_2) + P(G \cap H|I_3)  $
$ = {5 \choose 2}p^2(1-p)^3 \cdot p^3(1-p)^2 + {5 \choose 3}p^3(1-p)^2\cdot {3 \choose 2}p^2(1-p) \cdot {2 \choose 1}p(1-p) $
$ + {5 \choose 4}p^4(1-p)\cdot {3 \choose 1}p(1-p)^2 \cdot p^2 $
$ = \boxed{10p^5(1-p)^5 + 60p^6(1-p)^4 + 15p^7(1-p)^3} $
$I_1$, $I_2$, $I_3$ denote the events *2 heads in the first 5 tosses and 3 heads in 6-8 tosses*, *3 heads in the first 5 tosses and 2 heads in 6-8 tosses and 1 head in 9-10 tosses*, *4 heads in the first 5 tosses and 1 head in 6-8 tosses and 2 heads in 9-10 tosses*.
<br/>
##### 5:
Let $R_t$ denotes the reward gained at time $t$, So:
$E[R]$
$ = E[\sum_{t=1}^{n}R_t] $
$ = \displaystyle\sum_{t=1}^nE[R_t] $
$ = \displaystyle\sum_{t=1}^nP(R_t = 1) $
$ = \displaystyle\sum_{t=1}^nP(HeadatTime(t-1)AndTailatTime(t)) $
$ = np(1-p) $
To compute $Var(R)$, we first compute $E[(\sum_{t=1}^nR_t)^2]$.
$ E[(\sum_{t=1}^nR_t)^2] $
$ = E[\sum_{t=1}^nR_t^2 + \sum_{t_1 \not = t_2and|t_1-t_2|>1}R_{t_1}R_{t_2} + \sum_{t_1 \not = t_2and|t_1-t_2|=1}R_{t_1}R_{t_2}] $
$ =\displaystyle\sum_{t=1}^nE[R_t^2] + \sum_{t_1 \not = t_2and|t_1-t_2|>1}E[R_{t_1}R_{t_2}] +  \sum_{t_1 \not = t_2and|t_1-t_2|=1}E[R_{t_1}R_{t_2}] $
$ = np(1-p) + (n^2-n-(2n-2)) \cdot E[R_{t_1}R_{t_2}] + (2n-2) \cdot 0$
$ = np(1-p) + (n^2 -3n+2) \cdot p^2(1-p)^2 $
Then,
$ Var[R] $
$ = E[R^2] - E[R]^2 $
$ = np(1-p) +(n^2-3n+2) \cdot p^2(1-p)^2 - n^2p^2(1-p)^2 $
$ = \boxed{np(1-p) +(2-3n) \cdot p^2(1-p)^2} $
<br/>
##### G1:

