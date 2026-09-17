>Context:
>	[[The tower of levels#^70b1c0|In the context of the tower]], with [[Error of an interviewer#^17f0bb|an interviewer]] $f$, [[Error of an interviewer#^d15701|a distribution of the candidates]] $\mu$, and [[Accumulation Scheme#^dc3a91|a discrepency]] $d_j$ chosen on each level.
>	Everything below is the same one line argument: a pointwise inequality between errors, followed by the monotonicity and linearity of the expectation. The content is entirely in the hypothesis, which is [[Compatibility and contraction#^cc0b17|compatibility]].

>Theorem (Accumulation):
>	Let $X_1\overset{p_1}{\to}X_2\overset{p_2}{\to}\cdots\overset{p_{m-1}}{\to}X_m$ be a tower of sets, let $d_j$ be a discrepency on $X_j$ for each $j\in[m]$, and assume that for each $j$ the map $p_j$ is $C_j$-[[Compatibility and contraction#^cc0b17|contracting]] from $d_j$ to $d_{j+1}$.
>	Let $f:X_1\to X_i$ be [[Error of an interviewer#^17f0bb|an interviewer at level i]] and let $i\le j\le m$. Then:
>	>(1) (pointwise- hellll yeah): $\forall x\in X_1:\ Err^{(j)}_{f}(x)\ \le\ \left( \prod\limits_{l=i}^{j-1}C_l \right)\cdot Err^{(i)}_{f}(x)$
>	
>	>(2) (in expectation): $\mathfrak{E}_{j}(f)\ \le\ \left( \prod\limits_{l=i}^{j-1}C_l \right)\cdot\mathfrak{E}_{i}(f)$
>	
>	In particular, if $f$ is $\varepsilon$[[Error of an interviewer#^ec00d5|-good at level i]] then $f$ is $\left( \prod\limits_{l=i}^{j-1}C_l \right)\varepsilon$ - good at level $j$.
>
>Proof:
>	(1) By induction on $j-i$. For $j=i$ the empty product is $1$ and the claim is an equality. Assume it for $j$ and let $x\in X_1$. By [[The tower of levels#^70e2b4|the definition of the projections]], $P_{i\to j+1}=p_j\circ P_{i\to j}$ and $P_{1\to j+1}=p_j\circ P_{1\to j}$, so by [[Error of an interviewer#^e4401f|the definition of the error]] and the $C_j$-contraction of $p_j$ applied to the two points $P_{i\to j}(f(x)),P_{1\to j}(x)\in X_j$: $$Err^{(j+1)}_{f}(x)=d_{j+1}\Big( p_j\big( P_{i\to j}(f(x)) \big),p_j\big( P_{1\to j}(x) \big) \Big)\le C_j\cdot d_j\Big( P_{i\to j}(f(x)),P_{1\to j}(x) \Big)=C_j\cdot Err^{(j)}_{f}(x)$$ and the induction hypothesis finishes it. :)
>	(2) Apply $\mathbb{E}_{x\sim\mu}$ to (1), using that the expectation is monotone and homogeneous.

^acc001

>Note:
>	The theorem holds for every $\mu$ at once, since (1) is pointwise. So it is a statement about the interviewer and the discrepencies, and not about the population of candidates. The population enters only when one wants to *interpret* $\mathfrak{E}_i(f)$.


^acc002


^acc003


^acc004



^acc005

^acc006

>TODO:
>	>(1): Run the same scheme on a whole interview system, i.e. on $\delta\circ(f_1,\dots,f_n)$ for [[The main problem#^4870b0|a verdict method]] $\delta$. The pointwise step is identical; what is new is that the input error is now a vector of errors $\big( Err_{f_i} \big)_{i=1}^n$, and the question becomes which $\delta$ contract it and by how much. That is the quantitative form of [[Qaulity]].
>	
>	>(2): Lower bounds. The theorem says a good interviewer cannot produce a bad team. It says nothing about how good an interviewer has to be,  we have no converse of the form "if $\mathfrak{E}_1(f)\ge\varepsilon$ then $\mathfrak{E}_3(f)\ge\psi(\varepsilon)$" and maybe no such converse exists without further assumptions on $f$. Which assumptions?
