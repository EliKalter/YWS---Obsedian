
>Def (permutations as tournaments):
>	Let $k \in \mathbb{N}$. For $\sigma \in S_k$ define $Y_\sigma \in T_k$ by, for $a,b \in [k]$ s.t. $a < b$, $Y_\sigma(\{a,b\}) := \mathbf{1}_{[\sigma(a)<\sigma(b)]}$ 
>	Note: we mean that $a$ won over $b$ when $a$ gets "placed" closer to the top of the list defined by a permutation $\sigma$.

^34bd27

>Lemma (permutations and tournament relations):
>	Let $k \in \mathbb{N}$. For $\sigma \in S_k$ and distinct $a,b \in [k]$, the following holds: $a \succ_{Y_\sigma} b \Leftrightarrow \sigma(a) < \sigma(b)$.
>	
>Proof:
>	If $a<b$ then $a \succ_{Y_\sigma} b$ iff $Y_\sigma(\{a,b\}) = 1$ iff $\sigma(a)<\sigma(b)$. Otherwise, if $a>b$ then $a \succ_{Y_\sigma} b$ iff $Y_\sigma(\{a,b\}) = 0$ iff $\neg\big(\sigma(b)<\sigma(a)\big)$, which since $\sigma$ is a bijection and $a \neq b$ is iff $\sigma(a)<\sigma(b)$.

^80f1be

>Theorem (permutations and tournaments):
>	Let $k \in \mathbb{N}$. The mapping $S_k \to L_k$, defined for all $\sigma \in S_k$, by $\sigma\mapsto Y_\sigma$, is a bijection.
>	
>Proof:
>	well-defined: Let $a,b,c \in [k]$. For $\sigma \in S_k$, if $a \succ_{Y_\sigma} b$ and $b \succ_{Y_\sigma} c$ then, by the above [[Permutations as Tournaments#^80f1be|lemma]], $\sigma(a) < \sigma(b) < \sigma(c)$, hence $\sigma(a) < \sigma(c)$, hence $a \succ_{Y_\sigma} c$. Thus $Y_\sigma \in L_k$. 
>	Injective: For $\sigma,\pi \in S_k$ such that $Y_\sigma = Y_\pi$, by the above [[Permutations as Tournaments#^80f1be|lemma]], $\sigma(a)<\sigma(b)$ iff $\pi(a)<\pi(b)$ for all distinct $a,b \in [k]$. Thus $\sigma = \pi$, giving injectivity. 
>	Surjective: let $Y \in L_k$. By [[Tournaments and Tournament Relations#^1f802c|proposition]], $\succ_Y$ is a strict total order on $[k]$. A finite nonempty totally ordered set has a maximum, so by induction $\succ_Y$ is a chain $c_1 \succ_Y \ldots \succ_Y c_k$. Define $\sigma : [k] \to [k]$ for all $i \in [k]$ by $\sigma(c_i) = i$. 
>	Note that $\sigma$ is a bijection with $\sigma(a)<\sigma(b)$ iff $a \succ_Y b$ for all $a,b \in [k]$. Thus, by the above [[Permutations as Tournaments#^80f1be|lemma]], $Y_\sigma = Y$, giving surjectivity.

^9898e8

