
>Def (tournament):
>	Let $k \in \mathbb{N}$. Define $E_k := \{\{a,b\} \subseteq [k] : a \neq b\}$. A tournament is a mapping $E_k \to \mathbb{F}_2$. Define $T_k := \mathbb{F}_2^{E_k}$, the set of all tournaments.

^f2bd52

>Def (tournament relation):
>	Let $X$ be a set. Say $R \subseteq X^2$ is a tournament relation if it is asymmetric and semiconnex: menaing .

>Def ($\mathbf{1}_{[\cdot R\cdot]}$):
>	Let $X$ be a set. For a binary relation $R \subseteq X^2$ and $x,y \in X$, define $\mathbf{1}_{[xRy]} := 𝟙_R\big((x,y)\big)$ where $𝟙_R : X^2 \to \mathbb{F}_2$ is the indicator of $R$.

>Def ($\succ_Y$):
>	Let $k \in \mathbb{N}$. For $Y \in T_k$ and distinct $a,b \in [k]$, say $a$ beats $b$, and denote $a \succ_Y b$, if $Y(\{a,b\}) = \mathbf{1}_{[a<b]}$, that is if $a<b$ and $Y(\{a,b\}) = 1$, or $a>b$ and $Y(\{a,b\}) = 0$.

>Def (transitive tournament):
>	Let $k \in \mathbb{N}$. For $Y \in T_k$, say $Y$ is transitive if for all distinct $a,b,c \in [k]$, $a \succ_Y b \wedge b \succ_Y c \Rightarrow a \succ_Y c$. Denote by $L_k \subseteq T_k$ the subset of all transitive tournaments.

>Proposition (tournaments and tournament relations):
>	Let $k\in\mathbb{N}$. 
>	(i) $Y \mapsto\, \succ_Y$ is a bijection from $T_k$ onto the set of tournament relations on $[k]$.
>	(ii) For $Y \in T_k$, it holds that $Y \in L_k$ iff $\succ_Y$ is a strict total order on $[k]$. Hence $Y \mapsto\, \succ_Y$ restricts to a bijection from $L_k$ onto the set of strict total orders on $[k]$.
>	
>Proof:
>	(i) well-defined: for all distinct $a,b \in [k]$, $\mathbf{1}_{[a<b]}$ and $\mathbf{1}_{[b<a]}$ are the two distinct elements $0$ and $1$ of $\mathbb{F}_2$. So, the value $Y(\{a,b\})$ equals exactly one of them, giving both asymmetry and semiconnexity. Thus $\succ_Y$ is a tournament relation on $[k]$. 
>	Injective: let $Y,Y' \in T_k$ such that $\succ_Y\, =\, \succ_{Y'}$. For each $a,b \in [k]$ such that $a<b$, $Y(\{a,b\}) = \mathbf{1}_{[a \succ_Y b]} = \mathbf{1}_{[a \succ_{Y'} b]} = Y'(\{a,b\})$. Thus $Y = Y'$ giving injectivity. 
>	Surjective: let $R \subseteq [k]^2$ be a tournament relation. Define $Y : E_k \to \mathbb{F}_2$, for all $a,b \in [k]$ such that $a<b$, by $Y(\{a,b\}) = \mathbf{1}_{[aRb]}$. Let $a,b \in [k]$. If $a<b$, then by the definition of $\succ_Y$, $a \succ_Y b$ iff $Y(\{a,b\}) = \mathbf{1}_{[a<b]} = 1$, which, by the definition of $Y$, is iff $\mathbf{1}_{[aRb]} = 1$ iff $(a,b) \in R$. On the other hand, if $a>b$ then $a \succ_Y b$ iff $Y(\{a,b\}) = \mathbf{1}_{[a<b]} = 0$ which is iff $\mathbf{1}_{[bRa]} = 0$ iff $(a,b) \notin R$, which, by semiconnecity of $R$, is iff $(b,a) \in R$. In either case, it holds that $a \succ_Y b$ iff $(a,b) \in R$. Hence $\succ_Y\, = R$, giving surjectivity. 
>	
>	(ii) By definition, $Y \in L_k$ mean $\succ_Y$ is transitive on distinct triples, and by (i) it is a tournament relation; so $\succ_Y$ is a strict total order. Conversely, a strict total order is in particular transitive.

^1f802c
