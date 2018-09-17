##### 1:
* (a) Define $ A = $ *forecast rain*, $ B = $ *actually rain*. So the problem here is to compute $ P(A \mid B) $. In the winter situation, $ P(A \mid B) = \frac{P(A \cap B)}{P(B)} = \frac{0.7 \times 0.8}{0.7 \times 0.8 + 0.3 \times 0.1} = {56\over59} $. In the summer situation,  $ P(A \mid B) = {P(A \cap B) \over P(B)} ={0.2 \times 0.8 \over 0.2 \times 0.8 + 0.8 \times 0.1} $
<br/>
* (b) Define $ C = $ *Victor is carrying an umbrella*, $ D = $ *The forecast is no rain*. So what we only need to do is to verify $ P(C \cap D) = P(C)P(D) $. 
**Winter:** $ P(C) = P(missingForecast) \times 0.5 + P(seeForecast) \times P(forecastRain) = 0.2 \times 0.5 + 0.8 \times 0.7 = 0.66 $
$ P(D) = 0.3 $
$ P(C \cap D) = P(missingForecast) \times 0.5 * 0.3 = 0.03 $ . So we have $ P(C)P(D) = 0.198 \not = P(C \cap D)$. Hence, C and D are **dependent**.
**Summer:**
$ P(C) = 0.2 \times 0.5 + 0.8 \times 0.2 = 0.26 $
$ P(D) = 0.8 $
$ P(C \cap D) = 0.2 \times 0.5 \times 0.8 = 0.08 $
So we have $ P(C)P(D) = 0.208 \not = P(C \cap D) $. Hece, C and D are **dependent**
<br/>
* (c) Define $ E = $ *Victor is carrying an umberlla and it is not raining*, $ F = $ *he saw the forecast*. We need to compute $ P(F \mid E) $ using definition of conditional probability.
**Winter:**
$ P(E) = P(missingForecast) \times 0.5 \times (0.7 \times 0.2 + 0.3 \times 0.9) + P(seeForecast)P(forecastRain)P(noRain) $
$ P(E \cap F) = P(seeForecast)P(forecastRain)P(noRain) = 0.8 \times 0.7 \times 0.2 = 0.112 $
So, $ P(F \mid E) = {P(E \cap F) \over P(E)} = {0.112 \over 0.153} = {112 \over 153} $. 
**Summer:**
$ P(E) = 0.2 \times 0.5 \times (0.2 \times 0.2 + 0.8 \times 0.9) + 0.8 \times 0.2 \times 0.2 = 0.108 $
$ P(E \cap F) = 0.8 \times 0.2 \times 0.2 = 0.032 $
So, $ P(F \mid E) = {0.032 \over 0.108} = {8 \over 27} $
<br/>
##### 2:
* (a) 
    1. We need to compute $ P(A \cap B) $ and $ P(A)P(B) $ and compare the tow values.
    $ P(A) = P((5, 5)) = \frac{1}{25} $
    $ P(B) = \displaystyle\sum_{i=1}^4 P((i, 5)) + \displaystyle\sum_{i=1}^5 P((5, i)) = \frac{9}{25} $
    $ P(A \cap B) = P((5, 5)) = \frac{1}{25} $
    Because $ P(A \cap B) \not = P(A)P(B) $, A and B are **dependent**.
    <br/>
    2. Same process. 
    $ P(C) = \frac{9}{25} $
    $ P(A \cap C) = 0 $
    So, A and C are **dependent**.
<br/>
* (b)

| E      | F      | D      | 
| :--:   | :---:  | :--:   |
| (1, 2) | (1, 2) | (2, 5) |
| (2, 1) | (1, 3) | (3, 4) |
| (2, 3) | (1, 4) | (4, 3) |
| (3, 2) | (1, 5) | (5, 2) |
| (3, 4) | (2, 3)
| (4, 3) | (2, 4)
| (4, 5) | (2, 5)
| (5, 4) | (3, 4)
|        | (3, 5)
|        | (4, 5)

1. 
$ P(E) = \frac{8}{25} $
$ P(F) = \frac{10}{25} $
$ P(E \cap F) = \frac{4}{25} \not = \frac{16}{125} = P(E)P(F) $
**NOT** independent.
2. 
$ P(E \mid D) = \frac{1}{2} $
$ P(F \mid D) = \frac{1}{2} $
$ P(E \cap F \mid D) = \frac{1}{4} = \frac{1}{2} \times \frac{1}{2} = P(E \mid D)P(F \mid D) $
**Conditional** independent

##### 3:
* (a)
Defeine event $ A = $ *both defective*, event $ B = $ *buy old*, event $ C = $ *buy new*. By Law of total probability: $ P(A) = P(B)P(A \mid B) + P(C)P(A \mid C) $.
$ P(B) = P(C) = 0.5 $
$ P(A \mid B) = \frac{75}{500} \times \frac{74}{499} \approx 0.0222 $
$ P(A \mid C) = \frac{75}{1500} \times \frac{74}{1499} \approx 0.00247 $
So, $ P(A) \approx 0.5 \times (0.0222 + 0.00247) = 0.012335 $
<br/>
* (b)
$ P(B \mid A) = {P(A \cap B) \over P(A)} = \frac{0.0222 \times 0.5}{0.012335} \approx 0.9   $

##### 4:
* (a)
Define event $ A = $ *Dog is in A*, event $ B = $ *Dog is in B*, event $ C = $ *find the dog*. We need to compare $ P(C \cap A) $ and $ P(C \cap B) $.
$ P(C \cap A) = P(A)P(C \mid A) = 0.4 \times 0.25 = 0.1 $
$ P(C \cap B) = P(B)P(C \mid B) = 0.6 \times 0.15 = 0.09 $
So, Oscar should should search forest $A$.
<br/>
* (b)
Define event $ D = $ *not find in A*. Use Baye's Rule:$$ P(A \mid D) = \frac{P(A)P(D\mid A)}{P(A)P(D\mid A)+P(B)P(D\mid B)} = \frac{0.4 \times 0.75}{0.4\times 0.75 + 0.6 \times 1} = \frac{1}{3}  $$
<br/>
* (c)
Also use Baye's Rule: $$ P(A \mid C) = \frac{0.5 \times P(A)P(C \mid A)}{0.5\times P(A)P(C \mid A) + 0.5 \times P(B)P(C\mid B)} = \frac{10}{19} $$
<br/>
* (d)
$ P(findLiveDogInADay2) $
$ = P(A)P(notFind\mid A)P(liveInDay2)P(findDog\mid A) $
$= 0.4\times 0.75\times (1 - \frac{1}{1+2})\times 0.25 = 0.05 $
<br/>
##### 5:
* (a)
$ P(A \cap (B \cup C)) $
$ = P((A\cap B)\cup(A\cap C))$
$ = P(A \cap B) + P(A \cap C) - P(A\cap B \cap C) $
$ \overset{*}{=} P(A)P(B) + P(A)P(C) - P(A)P(B)P(C) $
$ = P(A)(P(B)+P(C)-P(B\cap C)) $
$ = P(A)P(B\cup C) $
The 3rd step which is denoted by * uses the independence of A, B, C.
<br/>
* (b)
We use Mathematical Induction to prove:
$$ P(A_1\cup A_2\cup \dots \cup A_n) = 1 - \displaystyle\prod_{i=1}^n(1-P(A_i)) $$
**Base case:**
Show that the statement holds for $ n = 1 $.
It is easy to see that $ P(A_1) = 1 - (1 - P(A_1)) $.
**Inductive step:**
Assume the equation holds for some positive integer $ k $. It must be shown that the equation also holds for $ k+1 $.
Define $ P(B) = P(A_1\cup A_2 \cup \dots \cup A_k) = 1 - \displaystyle\prod_{i=1}^k(1 - P(A_i)) $
Then for the case $ k+1 $:
$ P(A_1 \cup A_2 \cup \dots \cup A_{k+1}) $
$ = P(B \cup A_{k+1}) $
$ = P(B) + P(A_{k+1}) - P(B \cap A_{k+1}) $
$ \overset{*}{=} P(B) + P(A_{k+1}) - P(B)P(A_{k+1}) $
$ = P(A_{k+1})(1 - P(B)) + P(B) - 1 + 1 $
$ = 1 - (1 - P(B))(1 - P(A_{k+1})) $
$ \overset{**}{=} 1 - \displaystyle\prod_{i=1}^{k+1}(1 - P(A_i)) $
The steps which are denoted by * and ** use the **independece** and the **induction hypothesis** respectively.
<br/>
##### G1
* (a) The sequential description is very **important**.
<br/>
* (b):
Nonnegativity: $ P(k) = 2 \cdot \frac{1}{2^k} \ge 0$
Additivity: $ P(k_1 \cup k_2) = 2 \cdot (\frac{1}{2^{k_1}} + \frac{1}{2^{k_2}}) = P(k_1) + P(k_2) $
Normalization: $ \displaystyle\sum_{k=2}^\infty P(k) = \displaystyle\sum_{k=2}^\infty 2 \cdot \frac{1}{2^k} = \displaystyle\sum_{k=1}^\infty \frac{1}{2^k} = \lim\limits_{n \to \infty} \frac{\frac{1}{2}(1-\frac{1}{2^n})}{1-\frac{1}{2}} = 1 $
<br/>
* (c): Define event $ D = $ *no more than 5 games*
$ P(D) = \displaystyle\sum_{k=2}^52 \cdot\frac{1}{2^k} = \frac{15}{16} $
Next we compute the probability for each of Alice, Bob, and Caroll winning the tournament.
$ P(A) = (\frac{1}{2^2} + \frac{1}{2^5} + \frac{1}{2^8} + \dots) + (\frac{1}{2^4} + \frac{1}{2^7} + \frac{1}{2^{10}} + \dots) = \frac{5}{14} $
(The above calculation is inspireb by the **sequential description** of sample space.) 
By symmetry, we have $ P(B) = \frac{5}{14} $.
So, $ P(C) = 1 - \frac{5}{14} - \frac{5}{14} = \frac{4}{14} $





