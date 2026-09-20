
>	"A good interviewer gives a good opinion as to the marking of the candidates".

>The plan in one breath :) : 
>	An interviewer is judged by how far its opinion is from [[The main problem|the objective truth]]. "how far" is measured by a [[#^dc3a91|discrepency]]. The truth and the opinion both start in $X_1$ and are pushed down [[The tower of levels#^70e2b4|the tower]] (or a part of it) $X_1 \to X_2 \to X_3$ by the natural projections.

>Def (discrepency):
>	Let $Y$ be a set. A discrpency on $Y$ is a function $d:Y\times Y\to[0,\infty)$ satisfying $d(y,y)=0$ for all $y\in Y$.

^dc3a91

>Def (The three levels):
>	Let $r<k \in \mathbb{N}$.
>	$X_1:=[100]^k_{\ne}$, the vectors in $[100]^k$ without ties (injective maps $[k]\to[100]$).
>	$X_2:=S_k$
>	$X_3:=\begin{pmatrix} [k] \\ r \end{pmatrix}$, [[Natural way to select teams#^67c8f8|the r teams]].

^1e5e30

>Note (the maps between the levels):
>	The passage $X_2 \to X_3$ is [[Natural way to select teams|the natural projection onto the r teams]] $\zeta$. The passage $X_1 \to X_2$ is [[The tower of levels#^e7a911|the ranking map]].

>The notes of the scheme:
>	>(1): [[The tower of levels]]: the two projections $X_1 \to X_2 \to X_3$, and the fact that going down step by step is the same as going down at once.

>	
>	>(3): [[Error of an interviewer]]: $Err_f$, its level $j$ versions, the expected error $\mathfrak{E}_j(f)$, and what "$f$ is $\varepsilon$ - good" means.
>	
>	>(4): [[Compatibility and contraction]]: the one property a pair of discrepencies must have for an error bound to survive a projection, and the concrete constants along our tower.
>	
>	>(5): [[The accumulation theorem]] -- the transfer statement itself, its corollaries, and why it only runs downwards.

>Summary of 16.09.26:
>	>(1): We fixed the informal target ("a good interviewer marks well") and decided that the object to quantify is the *error of an interviewer at a level*, [[Error of an interviewer#^e4401f|see def]].
>	
>	>(2): We isolated the exact hypothesis that makes the transfer work: the projection must be [[Compatibility and contraction#^cc0b17|contracting from the upper discrepency to the lower one]]. Everything else is linearity and monotonicity of the expectation.
>	
>	>(3): We computed the two constants of our own tower: [[Compatibility and contraction#^ab12c3|$k-1$ from Hamming to Kendall]] and [[Compatibility and contraction#^bc23d4|$1$ from Kendall to the $r$ teams]].
>	
>	>(4): We found that the sup discrepency on $X_1$ does *not* transfer on its own, [[Compatibility and contraction#^ae56f1|see obstruction]], and that what repairs it is a margin assumption on the truth, [[Compatibility and contraction#^af67e2|see margin bound]].
>	
>	>(5): We noticed the chain is strictly one directional, [[potential something#^acc005|see remark]]: accuracy at $X_1$ is genuinely stronger than accuracy at $X_3$, which is exactly why it is worth assuming upstairs.

>
>	>(1): Sharp constants. Is $k-1$ [[Compatibility and contraction#^ab12c3|here]] attained? The refined count in that proof suggests $\begin{pmatrix} k \\ 2 \end{pmatrix} - \begin{pmatrix} k-s \\ 2 \end{pmatrix}$ is the truth.
>	
>	>(2): Which discrepencies on $S_k$ are the "right" ones? A natural demand is invariance under relabelling of the candidates, which is the same flavour as [[Neutrality#^41bc65|neutrality]]. Worth checking which of [[Discrepencies on the levels#^d20b7e|our level $2$ discrepencies]] are invariant, and whether invariance alone pins one down.
>	
>	>(3): The whole scheme is stated for one interviewer. The verdict method $\delta$ of [[The main problem#^4870b0|the main problem]] is a map out of $(R^{l'})^n$, so to speak about *systems* we should run the same argument on $\delta\circ(f_1,\dots,f_n)$ and ask how the errors of the $f_i$'s accumulate into the error of $\delta$. This is the bridge to [[Quality]].
>	
>	>(4): [[Error of an interviewer#^d15701|The distribution of the candidates]] is still a free parameter. Which $\mu$ is the honest one?
