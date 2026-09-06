
>Def (tournament):
>	Let $k \in \mathbb{N}$. Define $E_k := \{\{a,b\} \subseteq [k] : a \neq b\}$. A tournament is a function $Y : E_k \to \mathbb{F}_2$. Define $T_k := \mathbb{F}_2^{E_k}$, the set of all tournaments.

>Def (tournament relation):
>	Let $X$ be a set. Say $R \subseteq X^2$ is a tournament relation if it is asymmetric and semiconnex.

>Def ($\mathbf{1}_{[\cdot R\cdot]}$):
>	Let $X$ be a set. For a binary relation $R \subseteq X^2$ and $x,y \in X$, define $\mathbf{1}_{[xRy]} := 𝟙_R\big((x,y)\big)$ where $𝟙_R : X^2 \to \mathbb{F}_2$ is the indicator of $R$.

>Def ($\succ_Y$):
>	Let $k \in \mathbb{N}$. For $Y \in T_k$ and distinct $a,b \in [k]$, say $a$ beats $b$, and denote $a \succ_Y b$, if $Y(\{a,b\}) = \mathbf{1}_{[a<b]}$, that is if $a<b$ and $Y(\{a,b\}) = 1$, or $a>b$ and $Y(\{a,b\}) = 0$.

>Def (transitive tournament):
>	Let $k \in \mathbb{N}$. Say $Y \in T_k$ is transitive if for all distinct $a,b,c \in [k]$, $a \succ_Y b \wedge b \succ_Y c \Rightarrow a \succ_Y c$. Denote by $L_k \subseteq T_k$ the subset of all transitive tournaments.

>Proposition 1:
>	let $k\in\mathbb{N}$. 
>	(i) $Y \mapsto\, \succ_Y$ is a bijection from $T_k$ onto the set of tournament relations on $[k]$.
>	(ii) For $Y \in T_k$, it holds that $Y \in L_k$ iff $\succ_Y$ is a strict total order on $[k]$. Hence $Y \mapsto\, \succ_Y$ restricts to a bijection from $L_k$ onto the set of strict total orders on $[k]$.
>	
>Proof:
>	(i) well-defined: for all distinct $a,b \in [k]$, $\mathbf{1}_{[a<b]}$ and $\mathbf{1}_{[b<a]}$ are the two distinct elements $0$ and $1$ of $\mathbb{F}_2$. So, the value $Y(\{a,b\})$ equals exactly one of them, giving both asymmetry and semiconnexity. Thus $\succ_Y$ is a tournament relation on $[k]$. 
>	Injective: let $Y,Y' \in T_k$ such that $\succ_Y\, =\, \succ_{Y'}$. For each $a,b \in [k]$ such that $a<b$, $Y(\{a,b\}) = \mathbf{1}_{[a \succ_Y b]} = \mathbf{1}_{[a \succ_{Y'} b]} = Y'(\{a,b\})$. Thus $Y = Y'$ giving injectivity. 
>	Surjective: let $R \subseteq [k]^2$ be a tournament relation. Define $Y : E_k \to \mathbb{F}_2$, for all $a,b \in [k]$ such that $a<b$, by $Y(\{a,b\}) = \mathbf{1}_{[aRb]}$. Let $a,b \in [k]$. If $a<b$, then by the definition of $\succ_Y$, $a \succ_Y b$ iff $Y(\{a,b\}) = \mathbf{1}_{[a<b]} = 1$, which, by the definition of $Y$, is iff $\mathbf{1}_{[aRb]} = 1$ iff $(a,b) \in R$. On the other hand, if $a>b$ then $a \succ_Y b$ iff $Y(\{a,b\}) = \mathbf{1}_{[a<b]} = 0$ which is iff $\mathbf{1}_{[bRa]} = 0$ iff $(a,b) \notin R$, which, by semiconnecity of $R$, is iff $(b,a) \in R$. In either case, it holds that $a \succ_Y b$ iff $(a,b) \in R$. Hence $\succ_Y\, = R$, giving surjectivity. 
>	(ii) By definition, $Y \in L_k$ mean $\succ_Y$ is transitive on distinct triples, and by (i) it is a tournament relation; so $\succ_Y$ is a strict total order. Conversely, a strict total order is in particular transitive.

>Def (permutation to tournament translation):
>	Let $k \in \mathbb{N}$. For $\sigma \in S_k$ define $Y_\sigma \in T_k$ by, for $\{a,b\} \in E_k$ written with $a<b$, $Y_\sigma(\{a,b\}) = \mathbf{1}_{[\sigma(a)<\sigma(b)]}$

>Lemma 2:
>	Let $k \in \mathbb{N}$. For $\sigma \in S_k$ and distinct $a,b \in [k]$, the following holds: $a \succ_{Y_\sigma} b \Leftrightarrow \sigma(a) < \sigma(b)$.
>	
>Proof:
>	If $a<b$ then $a \succ_{Y_\sigma} b$ iff $Y_\sigma(\{a,b\}) = 1$ iff $\sigma(a)<\sigma(b)$. Otherwise, if $a>b$ then $a \succ_{Y_\sigma} b$ iff $Y_\sigma(\{a,b\}) = 0$ iff $\neg\big(\sigma(b)<\sigma(a)\big)$, which since $\sigma$ is a bijection and $a \neq b$ is iff $\sigma(a)<\sigma(b)$.

>Theorem 3:
>	Let $k \in \mathbb{N}$. The mapping $\eta :S_k \to L_k$, defined for all $\sigma \in S_k$, by $\eta(\sigma) = Y_\sigma$, is a bijection.
>	
>Proof:
>	well-defined: Let $a,b,c \in [k]$. For $\sigma \in S_k$, if $a \succ_{Y_\sigma} b$ and $b \succ_{Y_\sigma} c$ then, by lemma 2, $\sigma(a) < \sigma(b) < \sigma(c)$, hence $\sigma(a) < \sigma(c)$, hence $a \succ_{Y_\sigma} c$. Thus $\eta(\sigma) = Y_\sigma \in L_k$. 
>	Injective: For $\sigma,\pi \in S_k$ such that $Y_\sigma = Y_\pi$, by lemma 2, $\sigma(a)<\sigma(b)$ iff $\pi(a)<\pi(b)$ for all distinct $a,b \in [k]$. Thus $\sigma = \pi$, giving injectivity. 
>	Surjective: let $Y \in L_k$. By proposition 1(ii), $\succ_Y$ is a strict total order on $[k]$. A finite nonempty totally ordered set has a maximum, so by induction $\succ_Y$ is a chain $c_1 \succ_Y \ldots \succ_Y c_k$. Define $\sigma : [k] \to [k]$ for all $i \in [k]$ by $\sigma(c_i) = i$. 
>	Note that $\sigma$ is a bijection with $\sigma(a)<\sigma(b)$ iff $a \succ_Y b$ for all $a,b \in [k]$. Thus, by lemma 2, $Y_\sigma = Y$, giving surjectivity.

>Def (digraph of a tournament):
>	let $k \in \mathbb{N}$. For $Y \in T_k$ define $G_Y := ([k], \succ_Y)$. For $\sigma \in S_k$ write $G_\sigma := G_{Y_\sigma}$.

>Def (vertex relabelling):
>	let $k \in \mathbb{N}$. For $\pi \in S_k$ and a digraph $G = ([k], A)$, set $\pi G := ([k], \pi A)$ where $\pi A := \{(\pi(u),\pi(v)) : (u,v) \in A\}$.

>Lemma 4:
>	let $k \in \mathbb{N}$. $\pi \mapsto (G \mapsto \pi G)$ is a left action of $S_k$ on the digraphs on $[k]$. Moreover, for $\pi \in S_k$ and $u,v \in [k]$, it holds that $(u,v) \in \pi A$ iff $\big(\pi^{-1}(u), \pi^{-1}(v)\big) \in A$.
>	
>Proof:
>	$\mathrm{Id}A = A$ is clear, and for $\pi,\rho \in S_k$ it holds that: $(\pi\rho)A = \big\{\big((\pi\rho)(u),(\pi\rho)(v)\big) : (u,v) \in A\big\} = \big\{\big(\pi(\rho(u)),\pi(\rho(v))\big) : (u,v) \in A\big\} = \big\{(\pi(u),\pi(v)) : (u,v) \in \rho A\big\} = \pi(\rho A)$. For the last claim, substitute $u' := \pi^{-1}(u)$, $v' := \pi^{-1}(v)$; as $(u',v')$ ranges over $[k]^2$ so does $(u,v)$.

>Proposition 5:
>	Let $k\in\mathbb{N}$.
>	(i) $Y\mapsto G_Y$ is a bijection from $T_k$ onto the set of digraphs on $[k]$ whose edges are a tournament relation on $[k]$.
>	(ii) $Y\mapsto G_Y$ restricts to a bijection from $L_k$ onto the set of digraphs on $[k]$ whose edges are a strict total order on [k]$.
>
>Proof:
>	A digraph on the fixed vertex set $[k]$ is determined by its edges set: $A\mapsto ([k],A)$ is a bijection from the power set of $[k]^2$ onto the digraphs on $[k]$, with inverse $([k],A)\mapsto A$. Composing it with proposition 1(i) gives (i), and with proposition 1(ii) gives (ii).

>Theorem 6:
>	Let $k\in \mathbb{N}$. For all $\sigma,\tau\in S_k$  it holds that $G_{\sigma\tau}=\tau^{-1}G_\sigma$.
>
>Proof:
>	Both $G_{\sigma\tau}$ and $\tau^{-1}G_\sigma$ have vertex set $[k]$, so it suffices to show that their edges agree. Let $a,b\in [k]$. If $a=b$ then neither set of edges contains $(a,b)$, since $\succ_Y$ holds only between distinct elemnts. Otherwise $a\ne b$, and by lemma 2, $(a,b)\in \succ_{Y_{\sigma\tau}}$ iff $(\sigma\tau)(a)<(\sigma\tau)(b)$, that is iff $\sigma(\tau(a))<\sigma(\tau(b))$, which by lemma 2 again is iff $(\tau(a),\tau(b))\in\succ_{Y_{\sigma}}$. By lemma 4 applied to $\pi:=\tau^{-1}$, this holds iff $(a,b)\in\tau^{-1}\succ_{Y_{\sigma}}$. Hence $\succ_{Y_{\sigma\tau}}=\tau^{-1}\succ_{Y_{\sigma}}$ and $G_{\sigma\tau}=\tau^{-1}G_\sigma$.

>Corollary 7:
>	Let $k\in \mathbb{N}$. The action of $S_k$ by vertex relabelling on ${G_{\sigma}:\sigma\in S_k}$ is simply transitive. That is, for akk $\sigma,\tau\in S_k$ there exists a unique $\rho\in S_k$ with $\rho G_\sigma=G_\pi$, namely $\rho:=\pi^{-1}\sigma$.
>
>Proof:
>	By therorem 6 applied to $\tau:=\rho^{-1}$ we have $\rho G_\sigma=G_{\sigma\rho^{-1}}$. Hence $\rho G_\sigma=G_\pi$ iff $G_{\sigma\rho^{-1}}=G_\pi$, iff $Y_{\sigma\rho^{-1}}=Y_\pi$ by proposition 5(ii), iff $\sigma\rho^{-1}=\pi$ by theorem 3, iff $\rho=\pi^{-1}\sigma$.

>Corollary 8:
>	Let $k\in\mathbb{N}$ and $\sigma,\tau\in S_k$. Then: $G_{\sigma\tau}=\tau^{-1} G_\sigma$ , $G_{\tau\sigma}=(\sigma^{-1}\tau^{-1}\sigma)G_\sigma$ , $G_{\tau\sigma\tau^{-1}}=(\tau\sigma^{-1}\tau^{-1}\sigma)G_\sigma$ , $G_\sigma=\sigma^{-1}G_{Id}$.
>
>Proof:
>	By corollary 7, 

>Proposition 9:
>	Let $k\ge 3$ and $\tau\in S_k$. If $\pi\in S_k$ satisfies $G_{\tau\sigma}=\pi G_\sigma$ for all $\sigma\in S_k$, then $\tau=\pi=Id$.
>
>Proof:
>	By corollary 8, $G_{\tau\sigma}=(\sigma^{-1}\tau^{-1}\sigma)G_\sigma$, so by the uniqueness in corollary 7, $\pi=\sigma^{-1}\tau^{-1}\sigma$ for all $\sigma\in S_k$. Taking $\sigma:=Id$ gives $\pi=\tau^{-1}$, and substituting back, $\sigma^{-1}\tau^{-1}\sigma=\tau^{-1}$ for all $\sigma\in S_k$, that is $\tau^{-1}\in Z(S_k)$. Since $Z(S_k)={Id}$ for $k\ge 3$, we get $\tau=\pi=Id$.