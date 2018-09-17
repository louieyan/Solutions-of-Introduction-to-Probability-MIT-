##### 1:
* (a) $ A \cup B \cup C$
* (b) $$ (A^{\complement} \cap B^{\complement} \cap
C^{\complement}) \cup (A \cap B^{\complement} \cap 
C^{\complement}) \cup (A^{\complement} \cap B \cap 
C^{\complement}) \cup (A^{\complement} \cap B^{\complement} \cap C) $$
* (c) $ A^{\complement} \cap B^{\complement} \cap
C^{\complement} $
* (d) $ A \cap B \cap C $
* (e) $ (A \cap B^{\complement} \cap 
C^{\complement}) \cup (A^{\complement} \cap B \cap 
C^{\complement}) \cup (A^{\complement} \cap B^{\complement} \cap C) $
* (f) $ A \cap B \cap C^{\complement} $
* (g) $ A \cup (A^{\complement} \cap B^{\complement}) $

##### 2:
* (a) $ P = \frac{1}{2} \times \frac{1}{2} \times 
\frac{1}{2} = \frac{1}{8} $
* (b) $ P = \frac{1}{8} $
* (c) Three possibilities here: HHT, HTH, THH. So $ P =
3 \times \frac{1}{8} = \frac{3}{8} $
* (d) It could be two heads and one tail or three heads. Using the solution of (c), we have $ P = \frac{3}{8} + \frac{1}{2}^3 = \frac{1}{2} $

##### 3:
die1 | die2 | sum | P(sum) 
:---:| :--: | :-: | :----:
| 1  |  1   |  2  |  2p
| 1  |  2   |  3  |  3p
| 1  |  3   |  4  |  4p
| 1  |  4   |  5  |  5p
| 2  |  1   |  3  |  3p
| 2  |  2   |  4  |  4p
| 2  |  3   |  5  |  5p
| 2  |  4   |  6  |  6p
| 3  |  1   |  4  |  4p
| 3  |  2   |  5  |  5p
| 3  |  3   |  6  |  6p
| 3  |  4   |  7  |  7p
| 4  |  1   |  5  |  5p
| 4  |  2   |  6  |  6p
| 4  |  3   |  7  |  7p
| 4  |  4   |  8  |  8p
$ \sum{sum} = 80 $
$ \sum{P(sum)} = 80p = 1 $
So, $ p = \frac{1}{80} $ 
* (a) According to the table above, we can see $ P(even) = \frac{8}{16} = \frac{1}{2} $
* (b) $ P(2 and 3) = P((2, 3)) + P((3, 2)) = 5p + 5p = 10p = 10 \times \frac{1}{80} = \frac{1}{8} $

##### 4:
* $ P(B) = 1 - P(twoNumAreLessThan\frac{1}{3}) = 1 - \frac{1}{3} \times \frac{1}{3} \div 4 = \frac{35}{36} $
* Because the area of a line is equal to zero, so $ P(C) = 0 $
* **WRONG:** ($ P(A \cap D) = \frac{\frac{5}{3} \times \frac{5}{3} \times \frac{1}{2}}{4} = \frac{25}{76} $)
 **CORRECT:** $ P(A \cap D) = \frac{\frac{5}{3} \times \frac{5}{3} \times \frac{1}{2} + \frac{4}{3} \times \frac{4}{3} \times \frac{1}{2}}{4} = \frac{41}{72} $


##### 5：
* (a) $ P(50points) = \frac{\pi \times r^2}{\pi \times R^2} = \frac{1}{100} $
<br/>
* (b) $ P(30points) = \frac{\pi \times 3^2 - \pi \times 1^2}{\pi \times 10^2} = \frac{2}{25} $
<br/>
* (c) Same as Mike's probabilities.

##### 6:
To prove: $$ P(A \cap B \cap C) > P(A) + P(B) + P(C) - 2 $$
Useing the equation: $ P(A \cup B) = P(A) + P(B) - P(A \cap B) $.
Move $ P(A \cap B) $ to the left side, we have: $$ P(A \cap B) = P(A) + P(B) - P(A \cup B) $$
With the above equation, we can easily wirte: 
$$
\begin{aligned} 
P(A \cap B \cap C) = P((A \cap B) \cap C) 
= P(A \cap B) + P(C) \\
= P(A \cap B) + P(C) - P((A \cap B) \cup C) \\
= P(A) + P(B) + P(C) - P(A \cup B) - P((A \cap B) \cup C) > \\
P(A) + P(B) + P(C) - 2
\end{aligned}
$$
We must prove that at least one of  $ P(A \cup B) $ and $ P((A \cap B) \cup C) $ can't equal to 1. Suppose $ P(A \cup B) = 1 $ and $ P((A \cap B) \cup C) = 1 $, then $ A \cup B = \Omega $, so $ C = \emptyset $. Because $ P((A \cap B) \cup C) = 1 $ and $ C = \emptyset $, we can find $ A \cap B = \Omega $. But, we know that $ A \cup B = \Omega $. So, it must be $ A = B = \Omega $, which contradict the condition.

G1：
* (a) $ {a_n} $ and $ {b_n} $ are increasing sequence and decreasing sequence respectively. 
To prove: $$ \lim\limits_{n\rightarrow\infty}P([a_n, b_n]) = P([a, b]) $$
Define $ A_n = [a_n, b_n], A = [a, b] $, so we have $ A_n \supset A_{n+1} $ and $ A = \displaystyle\bigcap_{n=1}^\infty A_n $. So, according to the **Continuity property of probability**, we get the answer: $$ P(A) = \lim\limits_{n\rightarrow\infty}P(A_n) $$
</br>
* (b) Same question for this part. But the condition here is $ a_n $ and $ b_n $ are decreasing and increasing sequence respectively. We still use the definition of part a, and we have $ A_n \subset A_{n+1} $ and $ (a, b) = \displaystyle\bigcup_{n=1}^\infty A_n $. It is easy to see that $ (a, b) \not= [a, b] $. So if we define a probability low that $ P(a) \cup P(b) = 1 $, then $ P((a, b)) = 0 \not= P([a, b]) = 1$















