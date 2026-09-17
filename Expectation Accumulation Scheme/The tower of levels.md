>Context (mainly for me):
>	Let $r<k\in\mathbb{N}$ and let $X_1,X_2,X_3$ be [[Accumulation Scheme#^1e5e30|the three levels]].
>	Recall that every $a$ in [[Natural way to select teams#^710c40|a set that yields a natural ordering of [k]]] carries [[Natural way to select teams#^3d9aa7|an ordering $\succ_a$ of [k]]], and that [[Natural way to select teams|the natural projection onto the r teams]] $\zeta_A:A\to\begin{pmatrix} [k] \\ r \end{pmatrix}$ sends $a \mapsto C_{\succ_a}$.

^70b1c0

>Lemma (orderings are permutations):
>	Let $k\in\mathbb{N}$ and let $\succ$ be a [[Ordering#^456f81|strict total ordering]] of $[k]$. Then there is exactly one $\sigma\in S_k$ with $\succ_\sigma=\succ$, where $\succ_\sigma$ is [[Natural way to select teams#^339310|the order represented by]] $\sigma$.
>
>Proof:
>	By [[Permutations as Tournaments#^80f1be|lemma]], $\succ_\sigma=\succ_{Y_\sigma}$ for every $\sigma \in S_k$. By [[Permutations as Tournaments#^9898e8|theorem]] the map $\sigma\mapsto Y_\sigma$ is a bijection $S_k\to L_k$, and by [[Tournaments and Tournament Relations#^1f802c|proposition(ii)]] the map $Y\mapsto\succ_Y$ is a bijection from $L_k$ onto the strict total orders on $[k]$. The composition $\sigma\mapsto\succ_\sigma$ is therefore a bijection from $S_k$ onto the strict total orders on $[k]$, which is exactly the claim. YAY

^5ab0e1

>Def (The ranking map):
>	Let $A$ be [[Natural way to select teams#^710c40|a set that yields a natural ordering]] of $[k]$. We define $\eta_A:A\to S_k$ by sending $a$ to the unique $\sigma\in S_k$ with $\succ_\sigma=\succ_a$, which exists and is unique by [[#^5ab0e1|the last lemma]].
>	We call $\eta_A(a)$ the ranking of $a$, and $\eta_A$ the natural projection of $A$ onto $S_k$.
>	Note: Sometimes we will just write $\eta$ without referencing $A$.

^e7a911

>Note:
>	>(1): $\eta_{S_k}=Id_{S_k}$, since $\succ_\sigma=\succ_\sigma$.
>	
>	>(2): For $x=(x_1,\dots,x_k)\in X_1$ the ranking is given explicitly by $$\eta(x)(i)=\left\vert \left\{ j\in[k] \mid x_j\ge x_i \right\} \right\vert$$ ya'ani $\eta(x)(i)$ is the place of the $i$'th candidate when the candidates are listed from the highest score down. (It is a bijection $[k]\to[k]$ precisely because $x$ has no ties, and it satisfies $\eta(x)(i)<\eta(x)(j)\iff x_i>x_j$, which by [[Natural way to select teams#^2cfff4|def]] says $\succ_{\eta(x)}=\succ_x$.)

^fc0d21

>Lemma (idk):
>	Let $A$ be [[Natural way to select teams#^710c40|a set that yields a natural ordering]] of $[k]$. Then$$\zeta_A=\zeta_{S_k}\circ\eta_A$$
>Proof:
>	Let $a\in A$. By [[#^e7a911|the definition of]] $\eta_A$ we have $\succ_{\eta_A(a)}=\succ_a$, hence $$\zeta_{S_k}(\eta_A(a))=C_{\succ_{\eta_A(a)}}=C_{\succ_a}=\zeta_A(a)$$ where both outer equalities are [[Natural way to select teams|the definition of the natural projection]]. The point is simply that $\zeta_A(a)$ depends on $a$ only through $\succ_a$.

^c04d13

>Def (The tower and its projections):
>	The tower is $$X_1\ \overset{p_1}{\longrightarrow}\ X_2\ \overset{p_2}{\longrightarrow}\ X_3$$ where $p_1:=\eta_{X_1}$ is [[#^e7a911|the ranking map]] and $p_2:=\zeta_{S_k}$ is [[Natural way to select teams|the natural projection onto the $r$ teams]].
>	For $1\le i\le j\le 3$ we denote $P_{i\to j}:=p_{j-1}\circ\cdots\circ p_i:X_i\to X_j$, with the convention $P_{i\to i}:=Id_{X_i}$.

^70e2b4

>Note:
>	$P_{1\to2}=\eta_{X_1}$ and $P_{2\to3}=\zeta_{S_k}$ by definition, and $P_{1\to3}=\zeta_{X_1}$ by [[#^c04d13|the lemma]]. So "rank first and then pick the top $r$" and "pick the top $r$ straight away" are the same map, and we may speak of *the* projection of $X_1$ onto level $j$ without saying which route we took.

>Note (why the tower loses information, and in which direction):
>	$\left\vert X_1 \right\vert=100\cdot99\cdots(100-k+1)$ (so we are always assuming $k\le100$), $\left\vert X_2 \right\vert=k!$ and $\left\vert X_3 \right\vert=\begin{pmatrix} k \\ r \end{pmatrix}$. Both $p_1$ and $p_2$ are onto. $p_1$ is never injective, and $p_2$ is not injective once $k\ge3$ (for $k=2,r=1$ it happens to be a bijection). Each step forgets: $p_1$ forgets the sizes of the scores and keeps only their order, $p_2$ forgets the order and keeps only who made the cut. This is the reason the scheme runs downwards only, [[potential something#^acc005|see remark]].
