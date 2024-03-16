---
title: "Notes for Probability and Stochastic Process"
excerpt: "This is my notes for the lecture Probability and Stochastic Process"
collection: portfolio
---

# 			Notes for Probability and Stochastic Process

<center> &copy;Author: Zhan Cheng 
    E-Mail: zhanc113003@gmail.com
    Textbook: ISBN 978-7-5635-4537-7


------

[TOC]

# Chapter 1:Events and Their Probabilities

## 1.1 Experiment, Sample Space and Random Event

***

### 1.1.1 Basic Definations

​	***Random experiment*** has three characteristics: Reapeatability, Predictability, Uncertainty. And it can be denoted by $E$ , here is an example:
$$
E_{1}: \text{Determintation of the sex of a newborn child.}
$$
​	Each possible outcome is called an ***sample point*** or ***elementary event*** $\omega$ . The set of all possible outcomes of $E$ is known as the ***sample space*** $\Omega$ . Here is an example about $\Omega_{1}$ corresponding to $E_{1}$:
$$
\text{For } E_{1}\text{: }\Omega_{1}=\left\{g,b\right\}\text{, where the outcome }g\text{ means that the child is a girl and }b\text{ that it is a }\text{boy}
$$
​	Any subset of the $\Omega$ is known as an ***random event*** or ***event*** $A,B,C,···$. We say that $A$ occurs when the outcome of the experiment lies in $A$. Those events must occur in the experiment are called the ***inevitable events*** $S$. Those could not happen anytime are said to be ***impossible events*** $\emptyset$.

***

### 1.1.2 Events as Sets

​	The relationships and operations between random events could be described in term of ***set theory***.

​	Let $\Omega$ be the sample space of the random experiment $E$ and $A,B,A_{i}(i=1,2,···)$ be the random events of $E$.

1. $A\subset B:\text{if event A occurs, then B occurs}$
2. $A\cup B: \text{either A or B occurs}$
3. $A\cap B\text{ or }AB:\text{both A and B occur}$
4. $A-B:\text{A occurs but B does not occur}$

​	Common operations of the events are not listed, but there are two important formulas to remember:
$$
A-B=A-AB=A\overline{B}\\
A\cup B=A\cup \overline{A}B
$$

## 1.2 Probabilities Defined on Events

***

### 1.2.1 Classical Probability

​	A random experiment $E$ is ***classical*** if:

​	(i) : $E$ contains only different limited basic events.

​	(ii) : all outcomes are equally likely to occur.

​	$\text{If }\Omega=\left\{\omega_{1},\omega_{2},···,\omega_{n}\right\}\text{, we define the probability of event A as}\\$
$$
P(A)={{\#A}\over{\#\Omega}}
$$
​	$\text{where \#A means the number of all possible outcomes of event A, \#}\Omega\text{ means the number of all possible outcomes of sample space }\Omega$

$\text{and }P(\O)=0$

​	For classical random experiment $E$, the probability has the following properties:

​		$(1)\text{ for every event }A, P(A)\ge0,$

​		$(2)P(\Omega)=1,$

​		$(3)\text{for every finite sequence of n disjoint events }A_{1},A_{2},\cdots,A_{n},$
$$
P(\bigcup_{i=1}^{n}A_{i} )=\sum_{i=1}^{n} P(A_{i}).
$$
​	We just skip that proof.

***

### 1.2.2 Geometric Probability

​	A random experiment $E$ is ***geometric*** if:

​		(i) : the sample space is a measurable region, i.e. $0<L(\Omega)<\infin$, and

​		(ii) : the probability of every event has nothing to do with its position and shape.

​	In this case, we define the probability of event A as
$$
P(A)={{L(A)}\over{L(\Omega)}}
$$
$\text{and }P(\O)=0$

​	For geometrical random experiment $E$, the probability has the following properties:

​		$(1)\text{ for every event }A, P(A)\ge0,$

​		$(2)P(\Omega)=1,$

​		$(3)\text{for every finite sequence of n disjoint events }A_{1},A_{2},\cdots,A_{n},$
$$
P(\bigcup_{i=1}^{n}A_{i} )=\sum_{i=1}^{n} P(A_{i}).
$$
​	We skip that proof as well.

***

### 1.2.3 The Frequency Interpretation of Probability

​	Let $f_{n}(A)$ be the times that $A$ occurs. The ration
$$
F_{n}(A)={f_{n}(A)\over{n}}
$$
​	is said to be the ***frequency*** of event $A$ in the n trials.

​	$\text{If }n\text{ is large enough, the probability of event }A\text{ will be approximated by }F_{n}(A)$

​	For a random experiment $E$, the frequency has the following properties:

​		$(1)\text{ for every event }A, F_{n}(A)\ge0,$

​		$(2)F_{n}(\Omega)=1,$

​		$(3)\text{for every finite sequence of n disjoint events }A_{1},A_{2},\cdots,A_{n},$
$$
F_{n}(\bigcup_{i=1}^{n}A_{i} )=\sum_{i=1}^{n} F_{n}(A_{i}).
$$
​	We skip the part of $\sigma\text{-algebra}$ because it is too hard😢

## 1.3 Conditional Probabilities

### 1.3.1 The Defination of Conditional Probability

​	Given two events $A$ and $B$ with $P(B)>0$, the ***conditional probability of*** $A$ ***given*** $B$ is 
$$
P(A|B)={P(AB)\over{P(B)}}
$$
​	$\text{If }P(B)>0,\text{ then }P(A|B)\text{ is also a probability, that is}$

​		$(1)\text{ for every event }A, P(A|B)\ge0,$

​		$(2)P(\Omega|B)=1,$

​		$(3)\text{for every finite sequence of countable disjoint events }A_{1},A_{2},\cdots,A_{n},$
$$
P(\bigcup_{i=1}^{\infin}A_{i}|B )=\sum_{i=1}^{\infin} P(A_{i}|B).
$$
​	Some fomulas:
$$
P(\overline{A}|B)=1-P(A|B)\\
\text{if }A\sub B\text{, then }P(C-A|B)=P(C|B)-P(A|B)\text{ and }P(A|B)\le P(C|B)\\
P(A\cup C|B)=P{(A|B)}+P(C|B)-P(AC|B)
$$

***

### 1.3.2 The Multiplication Rule

​	Assume that $P(B)>0$. Then
$$
P(AB)=P(B)\cdot P(A|B)
$$
​	Or if $P(A)>0$, Then
$$
P(AB)=P(A)\cdot P(B|A)
$$
​	Suppose that $A_{1},A_{2},\cdot\cdot\cdot,A_{n}$ are events satisfying $P(A_{1}A_{2}\cdot\cdot\cdot A_{n-1})>0$.Then
$$
P(A_{1}A_{2}\cdot\cdot\cdot A_{n})=P(A_{1})P(A_{2}|A_{1})P(A_{3}|A_{1}A_{2})\cdots P(A_{n}|A_{1}A_{2}\cdot\cdot\cdot A_{n-1})
$$

***

### 1.3.3 Total Probability Formula

​	Let $\Omega$ denote the sample space of some experiment. n events $P(B_{1}B_{2}\cdot\cdot\cdot B_{n})$ are said to form a ***partition*** of $\Omega$ if these events satisfy:

​	$(1)B_{1},B_{2},\cdots,B_{n}\text{ are disjoint and}$

​	$(2)\bigcup_{i=1}^{n}B_{i}=\Omega$

​	Suppose that the events $B_{1},B_{2},\cdot\cdot\cdot, B_{n}$ form a partition of the sample space $\Omega$ and $P(B_{i})>0$ for $i=1,2,\cdots,n$. Then, for every event $A$ in $\Omega$
$$
P(A)=\sum_{i=1}^{n}P(B_{i}) P(A|B_{i})
$$

***

### 1.3.4 Baye's Theorem

​	Let the events $B_{1},B_{2},\cdot\cdot\cdot, B_{n}$ form a partition of the sample space $\Omega$ such that $P(B_{i})>0$ for $i=1,2,\cdots,n$, and let $A$ be an event such that $P(A)>0$. Then for $i=1,2,\cdots,n$,
$$
P(B_{i}|A)={P(B_{i})P(A|B_{i})\over{\sum_{j=1}^{n}P(B_{j}) P(A|B_{j})}}
$$

## 1.4 Independence of Two Events

### 1.4.1 Independence of Two Events and Several Events

​	Two events $A$ and $B$ are ***independent*** if
$$
P(AB)=P(A)P(B)
$$
​	Three events $A,B$ and $C$ in the sample space $S$ of a random experiment are said to be ***mutually independent*** if
$$
P(AB)=P(A)P(B)\\
P(BC)=P(B)P(C)\\
P(AC)=P(A)P(C)\\
P(ABC)=P(A)P(B)P(C)
$$
​	Events $A,B$ and $C$ are said to be ***pairwise independent*** if the first three equations hold.

***

### 1.4.2 Bernoulli Trials

​	A ***Bernoulli experiment*** $E$ is such kind of random experiment, the outcome of which can be classified in but one of two mutually exclusive and exhaustive ways, mainly, *success* and *failure*

​	***A sequence of Bernoulli trials*** $E_{n}$ occurs when a Bernoulli experiment is *performed serveral independent times so that the probability of success, say, p, remains the same from trial to trial*

​	The outcomes of $E_{n}$ are the $2^n$ sequences of lenth n. The number of outcomes of $E_{n}$ that contain a exactly $k$ times is given by the binomial coefficient
$$
\binom{n}{k}={n!\over{k!(n-k)!}}
$$
​	The probability that the outcome of an experiment that consists of n Bernoulli trials has $k$ success and $n-k$ failures is given by:
$$
P_{n}(k)= \binom{n}{k}p^kq^{n-k}
$$
