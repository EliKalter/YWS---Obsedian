>Model context (for me):
>	[[The tower of levels#^70b1c0|In the context of the tower]], and inside [[The main problem|the main problem]] with $l=l'=1$ and $D=[100]$, as in [[The striped down problem|the striped down version]].
>	We fix one $x\in X_1$ and read it as [[The main problem|the objective truth]] about the $k$ candidates: $x_i$ is the true worth of candidate $i$. We assume throughout, as agreed, that $[100]^k$ is taken without ties, both for the truth and for the opinions, ya'ani $[100]^k_{\ne}$.

^17e0aa

>Def (An interviewer at level $i$):
>	Let $i\in\left\{ 1,2,3 \right\}$. An interviewer at level $i$ is a map $f:X_1\to X_i$.
>	That is, $f$ reads the candidates and answers in the currency of level $i$: a marking ($i=1$), a ranking ($i=2$), or a team ($i=3$). This is [[The main problem|the interviewer of the main problem]] with $R$ taken to be $[100]^k,S_k$ or $\begin{pmatrix} [k] \\ r \end{pmatrix}$ respectively, [[Axes of complexity|which is one of the axes of complexity]].
>	Unless said otherwise "interviewer" means an interviewer at level $1$.

^17f0bb

>Def (The error of an interviewer at a level):
>	Let $f:X_1\to X_i$ be an interviewer at level $i$, let $i\le j\le3$, and let $d_j$ be [[Accumulation Scheme#^dc3a91|a discrepency]] on $X_j$. We define $Err^{(j)}_f:X_1\to[0,\infty]$ by $$Err^{(j)}_{f}(x):=d_j\Big( P_{i\to j}\big( f(x) \big)\ ,\ P_{1\to j}(x) \Big)$$ with [[The tower of levels#^70e2b4|the projections of the tower]].
>	In words: push the opinion and the truth down to level $j$, and measure how far apart they landed.

^e4401f

>Note:
>	>(1): For an interviewer at level $1$ the three errors read $$Err^{(1)}_{f}(x)=d_1\big( f(x),x \big)\qquad Err^{(2)}_{f}(x)=d_2\big( \eta(f(x)),\eta(x) \big)\qquad Err^{(3)}_{f}(x)=d_3\big( \zeta(f(x)),\zeta(x) \big)$$ so $Err^{(1)}_f$ is the plain $Err_f=d(f(x),x)$ we started from, and the other two are the same thing read after the projection.
>	
>	>(2): $Err^{(j)}_f(x)=0$ whenever $f(x)$ and $x$ agree at level $j$, even if they disagree wildly at level $1$. The error is a property of the pair (interviewer, level), never of the interviewer alone.
>	
>	>(3): An interviewer at level $3$ has only $Err^{(3)}_f$; there is nothing above its answer to compare.

>Def (The distribution of the candidates):
>	A distribution of the candidates is a probability measure $\mu$ on the finite set $X_1$. 
>	For simplicity, unless said otherwise $\mu$ is the uniform one.
>	(This is the slot left open in [[The main problem|the main problem]] under "The distrebution of the candidates: Later". Everything below holds for an arbitrary $\mu$.)

^d15701

>Def (The expected error / the inaccuracy of $f$ at level $j$):
>	[[#^e4401f|In the context of the error]], and given [[#^d15701|a distribution of the candidates]] $\mu$, we define $$\mathfrak{E}^{\mu}_{j}(f):=\mathbb{E}_{x\sim\mu}\left[ Err^{(j)}_{f}(x) \right]=\sum\limits_{x\in X_1}\mu(x)\cdot Err^{(j)}_{f}(x)$$
>	Note: Sometimes we will just write $\mathfrak{E}_j(f)$ without referencing $\mu$.

^e8f0c2

>Def ($\varepsilon$-good at level $j$):
>	[[#^e8f0c2|In the same context]] and for $\varepsilon\ge0$, we say that $f$ is $\varepsilon$-good at level $j$ (with respect to $d_j$ and $\mu$) when $\mathfrak{E}_j(f)\le\varepsilon$.
>	We say that $f$ is exact at level $j$ when $\mathfrak{E}_j(f)=0$.


^ec00d5

