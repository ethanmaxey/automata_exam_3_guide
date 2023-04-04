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


- Pumping Lemma (For CFL) 📹 [[Video](https://www.youtube.com/watch?v=jRhqx1_KcCk)]
- Example 1 📹 [[Video](https://youtu.be/eQ0XkUk3qGk)]
- Example 2 📹 [[Video](https://youtu.be/DPs8sBcIjs8)]

## Question 2

> Construct a pda P for the following langeage L = {...} where L = L(P) (acceptance bu final state. State on which side you write the top of the stack, left, or right. Hint: Put three markers on the stack for every 0.

- Intro to Pushdown Automata 📹 [[Video](https://youtu.be/4ejIAmp_Atw)]
- Formal Definition of Pushdown Automata 📹 [[Video](https://youtu.be/JtRyd7Svlew)]
- Pushdown Automata - Graphical Notation 📹 [[Video](https://youtu.be/eY7fwj5jvC4)]
- Example 1 - Part 1 📹 [[Video](https://youtu.be/TEQcJybMMFU)]
- Example 1 - Part 2 📹 [[Video](https://youtu.be/BxA-aI2dyRo)]
- Example 1 - Part 3 📹 [[Video](https://youtu.be/xHj2WI1Rrl4)]

## Question 3

> Construct a pda P that accepts the following language by empty stack: L = L(G) where G = {...} with T = {...}, N = {...}, and P = {...}. State on which side you write the top of the stack, left, or right. Note: You must use the construction "cfg -> pda" given in class. Get G into GNF first!

- Refer to [Q2's](#question-2) videos

## Question 4

> Construct a grammar for L(G) for the language N(P): P = {...} where the move function delta is given by {...}. Here, the top of the stack is on the left.

- Equivalance of CFG and PDA - Part 1 📹 [[Video](https://youtu.be/FjGrU7vczyg)]
- Equivalance of CFG and PDA - Part 2a 📹 [[Video](https://youtu.be/kyvLetfjOhc)]
- Equivalance of CFG and PDA - Part 2b 📹 [[Video](https://youtu.be/DjbukiTf-48)]

## Question 5

> Construct a Turing machine for the language in Question 1. L = {...}. Describe first in words what you are doing, then formulate the formal Turing machine.

- Turing Machines - Intro Part 1 📹 [[Video](https://youtu.be/FjGrU7vczyg)]
- Turing Machines - Intro Part 2 📹 [[Video](https://youtu.be/GPSk9tRsK2I)]
- Turing Machines (Formal Definition) 📹 [[Video](https://youtu.be/yFEdBR-rP9g)]
- Example 1 📹 [[Video](https://youtu.be/D9eF_B8URnw)]
- Example 2 📹 [[Video](https://youtu.be/cR4Re0YfoOo)]
- The Church-Turing Thesis 📹 [[Video](https://youtu.be/0D7yInuKvKs)]
- Turing Machine for Even Palindromes 📹 [[Video](https://youtu.be/KW9md3j4_cU)]
- Turing Machines Programming Techniques Part 1 📹 [[Video](https://youtu.be/BKhQJP4sa_8)]
- Turing Machines Programming Techniques Part 2 📹 [[Video](https://youtu.be/23vQEJWXc-k)]
- Turing Machines Programming Techniques Part 3 📹 [[Video](https://youtu.be/CyB3aQhH9u4)]
- Multitape Turing Machine 📹 [[Video](https://youtu.be/CLLutxGVDY4)]
- Nondeterministic Turing Machine - Part 1 📹 [[Video](https://youtu.be/gQnPM6sydkk)]
- Nondeterministic Turing Machine - Part 2 📹 [[Video](https://youtu.be/9Bk11XgiC1E)]
- Turing Machine as Problem Solvers  📹 [[Video](https://youtu.be/f_1GptvagSw)]
- Universal Turing Machine 📹 [[Video](https://youtu.be/eKCX-4_jzck)]
