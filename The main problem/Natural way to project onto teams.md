
>Def ($r$ team/selection out of $k$ candidates):
>	Let $r < k \in \mathbb{N}$. An element $A \in \begin{pmatrix} [k] \\ r \end{pmatrix}$ is called "an $r$ team out of the $k$ candidates"

^67c8f8

>Def (The $r$ teams):
>	[[#^67c8f8|In the same context]] we call $\begin{pmatrix} [k] \\ r \end{pmatrix}$ "The $r$ teams" or "All the $r$ teams".

>Def (Natural $r$ selection given order):
>	Let $\succ$ be some [[Ordering#^456f81|strict total ordering]] of $[k]$. (I want the best/top ones to come first so using $\succ$ and not $\prec$).
>	Denote $C_\succ \in \begin{pmatrix} [k] \\ r \end{pmatrix}$ the $r$ team that holds $\forall i \in C_\succ, j \in [k] \setminus C_\succ: i \succ j$ (Why it exists? and who is it?)
>	We call $C_\succ$ the natural $r$ team under $\succ$.

^e84282

>Def (The order on $[k]$ encripted in a permutation):
>	Let $\sigma \in S_k$. We call the only order on $[k]$ $\succ$ that has $i \succ j \iff \sigma(i) < \sigma(j)$ the order on $[k]$ represented by $\sigma$.

^339310

>Def (The order on $[k]$ encripted in an element of $[0,1]^k$ (Without ties)):
>	Let $x = (x_1, \dots, x_k) \in [0,1]^k \text{(Without ties)}$. We call the only order on $[k]$ $\succ$ that has $i \succ j \iff x_i > x_j$ the order on $[k]$ represented by $x$.

^2615f8

>Def (The order on $[k]$ encripted in an element of $[100]^k$ (Without ties)):
>	Let $x = (x_1, \dots, x_k) \in [100]^k \text{(Without ties)}$. We call the only order on $[k]$ $\succ$ that has $i \succ j \iff x_i > x_j$ the order on $[k]$ represented by $x$.

^2cfff4

>Def (A set that yields a natural ordering of $[k]$):
>	Denote:
>	
>	>(1): $A_1:=S_k$
>	
>	>(2): $A_2:=[0,1]^k$ (Without ties)
>	
>	>(3): $A_3:=[100]^k$ (Without ties)
>	
>	$\mathcal{A}:=\left\{ A_i \right\}_{i=1}^3$
>	
>	Given a set $A$ we say that $A$ yields a natural ordering of $[k]$ iff $A\in \mathcal{A}$

^710c40

>Note: By [[#^339310|Def 1]], [[#^2615f8|Def 2]] and [[#^2cfff4|Def 3]], we get that for any $A \in \mathcal{A}$ and any $a \in A$ we have an ordering of $[k]$ obtained. We can denote it $\succ_a$.

^3d9aa7

>Def (Natural projection onto the $r$ teams):
>	Let $A$ be [[#^710c40|a set that yields a natural ordering]] on $[k]$. And let $a \in A$. [[#^3d9aa7|Then we have]] $\succ_a$ and thus by [[#^e84282|the natural selection given order]] we have $C_{\succ_a}$.
>	Denote $C_a:=C_{\succ_a}$
>	 And we get $\zeta_A:A\to\begin{pmatrix} [k] \\ r \end{pmatrix}$ given by $a\mapsto C_a$.
>	 Note: Sometimes we will just write $\zeta$ without referencing $A$.
>	 We will call $\zeta(a)$ the natural selection given $a$. And $\zeta$ itself is the natural projection of $A$ onto $\begin{pmatrix} [k] \\ r \end{pmatrix}$.