# 🤖 Automata Exam 3 Study Guide

📚 This study guide is intended to help you prepare for your Automata Exam 3. It assumes you have no prior knowledge of automata, and provides the resources each step of the way to learn and solve the types of problem on exam 3. Previous exams are available in the resources section of the discord. 

### Knowledge Needed From Exam 1 & 2:
1. Context-Free Languages
2. GNF

## 🔎 Question Navigation

- [Question 1](#question-1)
- [Question 2](#question-2)
- [Question 3](#question-3)
- [Question 4](#question-4)
- [Question 5](#question-5)

## Question 1

> Prove that the following language L is not context-free.

$$
\text{Spring 2008}\\quad
L = [0^k 1^j 2^i \quad \text{|}\  i>j>k\geq 0]
$$

$$
\text{Summer 2008}\\quad
L = [0^k 1^j 2^i \quad \text{|}\  i>j>k\geq 1]
$$

$$
\text{Spring 2009}\\quad
L = [0^k 1^j 0^i \quad \text{|}\  i>j>k\geq 0]
$$

$$
\text{Summer 2009}\\quad
L = [a^k b^j a^i \quad \text{|}\  i>j>k\geq 0]
$$

$$
\text{Summer 2010}\\quad
L = [a^k b^j a^i \quad \text{|}\  i>j>k\geq 1]
$$

$$
\text{Summer 2012, 2017}\\quad
L = [a^i b^j a^i \quad \text{|}\  j\geq i \geq 1]
$$

$$
\text{Summer 2013, 2015}\\quad
L = [a^i b^j a^i \quad \text{|}\  j>i \geq 1]
$$

$$
\text{Summer 2022}\\quad
L = [a^i b^i a^j \quad \text{|}\  j\geq i \geq 1]
$$

- Leiss on Pumping Lemma (0:00 - 12:28) [[Video](https://www.youtube.com/watch?v=VVbsZKxvLM8)]

- Pumping Lemma (For CFL) 📹 [[Video](https://www.youtube.com/watch?v=jRhqx1_KcCk)]
- Example 1 📹 [[Video](https://youtu.be/eQ0XkUk3qGk)]
- Example 2 📹 [[Video](https://youtu.be/DPs8sBcIjs8)]

## Question 2

> Construct a pda P for the following langeage L = {...} where L = L(P) (acceptance bu final state. State on which side you write the top of the stack, left, or right. Hint: Put three markers on the stack for every 0.

$$
\text{Spring 2008, Summer 2013}\\quad
L = [0^i 1^{3i} \quad \text{|}\  i\geq 0]
$$

$$
\text{Summer 2000}\\quad
L = [0^{2i} 1^i \quad \text{|}\  i\geq 0]
$$

$$
\text{Summer 2012}\\quad
L = [0^i 1^{2i} \quad \text{|}\  i\geq 0]
$$

$$
\text{Summer 2012}\\quad
L = [0^i 1^{4i} \quad \text{|}\  i\geq 0]
$$


$$
\text{Summer 2015}\\quad
L = [0^{3i} 1^i \quad \text{|}\  i\geq 0]
$$

$$
\text{Summer 2017}\\quad
L = [0^{5i} 1^i \quad \text{|}\  i\geq 0]
$$

$$
\text{Summer 2022}\\quad
L = [10^{3i} 1^i \quad \text{|}\  i\geq 1]
$$

- LEISS on Right vs Left stack 12:28 18:10 - 📹 [[Video](https://www.youtube.com/watch?v=VVbsZKxvLM8)]

## Question 3

> Construct a pda P that accepts the following language by empty stack: L = L(G) where G = {...} with T = {...}, N = {...}, and P = {...}. State on which side you write the top of the stack, left, or right. Note: You must use the construction "cfg -> pda" given in class. Get G into GNF first!

- Refer to [Q2's](#question-2) videos

$$
\text{Summer 2009, 2010} \\quad
$$

$$
L = L(G) \\quad G = (T, N, P, E) \\quad T = (id, +, *, (, ))
$$

$$
N = {E} \\quad P = (E -> E + E | E*E | (E) | id)
$$

<br>

$$
\text{Summer 2012} \\quad
$$

$$
L = L(G) \\quad G = (T, N, P, E) \\quad T = (id, +, -, (, ))
$$

$$
N = {E} \\quad P = (E -> E + E | E-E | (E) | id)
$$

<br>

$$
\text{Summer 2013, 2015, 2017} \\quad
$$

$$
L = L(G) \\quad G = (T, N, P, E) \\quad T = (id, *, /, (, ))
$$

$$
N = {E} \\quad P = (E -> E*E | E/E | (E) | id)
$$

<br>

$$
\text{Summer 2022} \\quad
$$

$$
L = L(G) \\quad G = (T, N, P, S) \\quad T = (a,b,c,d)
$$

$$
N = {S, A} \\quad P = (S -> aSb| cAd | a, \\quad A -> aSb|SS)
$$

## Question 4

> Construct a grammar for L(G) for the language N(P): P = {...} where the move function delta is given by {...}. Here, the top of the stack is on the left.

$$
\text{Spring, Summer 2008} \\quad
$$

$$
P = ( (p, q), (a, b), (Z, X), δ, p, Z, Ø)
$$

$$
δ(p,a,Z) = {(p,XZ)} \\quad δ(p,ϵ,Z) = {(p, ϵ)} \\quad δ(p,a,X) = {(p, XX)}\\quad
$$

$$
δ(q,a,Z) = {(q,ϵ)} \\quad δ(p,b,X) = {(q, X)} \\quad δ(q,b,Z) = {(p,Z)}
$$

<br>

$$
\text{Summer 2009} \\quad
$$

$$
P = ( (p, q), (a, b), (Z, X), δ, p, Z, Ø)
$$

$$
δ(p,b,Z) = {(p,XZ)} \\quad δ(p,ϵ,Z) = {(q, ϵ)} \\quad δ(p,b,X) = {(p, XX)}\\quad
$$

$$
δ(q,b,Z) = {(p,XZ)} \\quad δ(p,a,X) = {(q, ϵ)} \\quad δ(p,a,X) = {(p,ϵ)}
$$

<br>

$$
\text{Summer 2009, 2010, 2012, 2013, 2015, 2017} \\quad
$$

$$
P = ( (p, q), (a, b), (Z, X), δ, p, Z, Ø)
$$

$$
δ(p,b,Z) = {(p,XZ)} \\quad δ(q,ϵ,Z) = {(q, ϵ)} \\quad δ(p,b,X) = {(p, XX)}\\quad
$$

$$
δ(q,b,Z) = {(p,XZ)} \\quad δ(q,a,X) = {(q, ϵ)} \\quad δ(p,a,X) = {(p,ϵ)}
$$

<br>

$$
\text{Summer 2022} \\quad
$$

$$
P = ( (p, q), (a, b), (Z, X), δ, p, Z, Ø)
$$

$$
δ(p,b,Z) = {(p,XZ)} \\quad δ(q,ϵ,Z) = {(q, ϵ)} \\quad δ(p,b,X) = {(p, XX)}\\quad
$$

$$
δ(q,b,Z) = {(p,XZ)} \\quad δ(q,a,X) = {(q, ϵ)} \\quad δ(p,a,X) = {(q,ϵ)}
$$

- Leiss Lecture 📹 [[Video](https://www.youtube.com/watch?v=aADmqDfpx-c)]

## Question 5

> Construct a Turing machine for the language in Question 1. L = {...}. Describe first in words what you are doing, then formulate the formal Turing machine.

$$
\text{Spring 2008}\\quad
L = [0^k 1^j 2^i \quad \text{|}\  i>j>k\geq 0]
$$

$$
\text{Summer 2008}\\quad
L = [0^k 1^j 2^i \quad \text{|}\  i>j>k\geq 1]
$$


$$
\text{Spring 2009}\\quad
L = [0^k 1^j 0^i \quad \text{|}\  i>j>k\geq 0]
$$

$$
\text{Summer 2010}\\quad
L = [a^k b^j a^i \quad \text{|}\  i>j>k\geq 1]
$$

$$
\text{Summer 2012, 2017}\\quad
L = [a^i b^j a^i \quad \text{|}\  j\geq i \geq 1]
$$

$$
\text{Summer 2013, 2015}\\quad
L = [a^i b^j a^i \quad \text{|}\  j > i \geq 1]
$$

$$
\text{Summer 2022}\\quad
L = [a^i b^i a^j \quad \text{|}\  j\geq i \geq 1]
$$

- LEISS (22:00 - 1:25:20) 📹 [[Video](https://www.youtube.com/watch?v=bqQ55-KM_7E)]
- Turing Machines - Leiss Lecturing 📹 [[Video](https://www.youtube.com/watch?v=bqQ55-KM_7E)]
- Turing Machines - Example 📹 [[Video](https://www.youtube.com/watch?v=Y0x9kmfjQTA)]
