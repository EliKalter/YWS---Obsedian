
>Def (digraph of a tournament):
>	let $k \in \mathbb{N}$. For $Y \in T_k$ define $G_Y := ([k], \succ_Y)$. For $\sigma \in S_k$ write $G_\sigma := G_{Y_\sigma}$.

^e7a17b

>Def (vertex relabelling):
>	let $k \in \mathbb{N}$. For $\pi \in S_k$ and a digraph $G = ([k], A)$, set $\pi G := ([k], \pi A)$ where $\pi A := \{(\pi(u),\pi(v)) : (u,v) \in A\}$.

^f16132

>Lemma (relabelling action):
>	let $k \in \mathbb{N}$. $\pi \mapsto (G \mapsto \pi G)$ is a left action of $S_k$ on the digraphs on $[k]$. Moreover, for $\pi \in S_k$ and $u,v \in [k]$, it holds that $(u,v) \in \pi A$ iff $\big(\pi^{-1}(u), \pi^{-1}(v)\big) \in A$.
>	
>Proof:
>	$\mathrm{Id}A = A$ is clear, and for $\pi,\rho \in S_k$ it holds that: $(\pi\rho)A = \big\{\big((\pi\rho)(u),(\pi\rho)(v)\big) : (u,v) \in A\big\} = \big\{\big(\pi(\rho(u)),\pi(\rho(v))\big) : (u,v) \in A\big\} = \big\{(\pi(u),\pi(v)) : (u,v) \in \rho A\big\} = \pi(\rho A)$. For the last claim, substitute $u' := \pi^{-1}(u)$, $v' := \pi^{-1}(v)$; as $(u',v')$ ranges over $[k]^2$ so does $(u,v)$.

^da1df9

>Note:
>	We note that our choice of represnting tournaments as weakly connected orientations of the clique on $[k]$, denoted $K_k$, was arbitrary - conversely, a different equivalent choice could have been: reprenting tournaments as undirected subgraphs of $K_k$; where the existence of an edge $\left\{a,b\right\}$, written with $a<b$, represents that $a$ beat $b$.

>Proposition (tournaments and digraphs):
>	Let $k\in\mathbb{N}$.
>	(i) $Y\mapsto G_Y$ is a bijection from $T_k$ onto the set of digraphs on $[k]$ whose edges are a tournament relation on $[k]$.
>	(ii) $Y\mapsto G_Y$ restricts to a bijection from $L_k$ onto the set of digraphs on $[k]$ whose edges are a strict total order on $[k]$.

^f84109

>Proof:
>	A digraph on the fixed vertex set $[k]$ is determined by its edges set: $A\mapsto ([k],A)$ is a bijection from the power set of $[k]^2$ onto the digraphs on $[k]$, with inverse $([k],A)\mapsto A$. Composing it with [[Tournaments and Tournament Relations#^1f802c|proposition(i)]] gives (i), and with [[Tournaments and Tournament Relations#^1f802c|proposition(ii)]] gives (ii).

>Theorem (characteriation of left multiplication):
>	Let $k\in \mathbb{N}$. For all $\sigma,\tau\in S_k$  it holds that $G_{\sigma\tau}=\tau^{-1}G_\sigma$.
>
>Proof:
>	Both $G_{\sigma\tau}$ and $\tau^{-1}G_\sigma$ have vertex set $[k]$, so it suffices to show that their edges agree. Let $a,b\in [k]$. If $a=b$ then neither set of edges contains $(a,b)$, since $\succ_Y$ holds only between distinct elemnts. Otherwise $a\ne b$, and by [[Permutations as Tournaments#^80f1be|lemma]], $(a,b)\in \succ_{Y_{\sigma\tau}}$ iff $(\sigma\tau)(a)<(\sigma\tau)(b)$, that is iff $\sigma(\tau(a))<\sigma(\tau(b))$, which by [[Permutations as Tournaments#^80f1be|lemma]] again is iff $(\tau(a),\tau(b))\in\succ_{Y_{\sigma}}$. By [[Tournaments as Graphs#^da1df9|lemma]] applied to $\pi:=\tau^{-1}$, this holds iff $(a,b)\in\tau^{-1}\succ_{Y_{\sigma}}$. Hence $\succ_{Y_{\sigma\tau}}=\tau^{-1}\succ_{Y_{\sigma}}$ and $G_{\sigma\tau}=\tau^{-1}G_\sigma$.

^cbd7d7

>Corollary (relabelling is simply transitive):
>	Let $k\in \mathbb{N}$. The action of $S_k$ by vertex relabelling on $\left\{G_\sigma :\sigma\in S_k \right\}$ is simply transitive. That is, for all $\sigma,\tau\in S_k$ there exists a unique $\rho\in S_k$ with $\rho G_\sigma=G_\pi$, namely $\rho:=\pi^{-1}\sigma$.
>
>Proof:
>	By [[Tournaments as Graphs#^cbd7d7|theorem]] applied to $\tau:=\rho^{-1}$ we have $\rho G_\sigma=G_{\sigma\rho^{-1}}$. Hence $\rho G_\sigma=G_\pi$ iff $G_{\sigma\rho^{-1}}=G_\pi$, iff $Y_{\sigma\rho^{-1}}=Y_\pi$ by [[Tournaments as Graphs#^f84109|proposition(ii)]], iff $\sigma\rho^{-1}=\pi$ by [[Permutations as Tournaments#^9898e8|theorem]], iff $\rho=\pi^{-1}\sigma$.

>Corollary (useful identities):
>	Let $k\in\mathbb{N}$ and $\sigma,\tau\in S_k$. Then: $G_{\sigma\tau}=\tau^{-1} G_\sigma$ , $G_{\tau\sigma}=(\sigma^{-1}\tau^{-1}\sigma)G_\sigma$ , $G_{\tau\sigma\tau^{-1}}=(\tau\sigma^{-1}\tau^{-1}\sigma)G_\sigma$ , $G_\sigma=\sigma^{-1}G_{Id}$.
>
>Proof:
>	TODO

^3af7f7

