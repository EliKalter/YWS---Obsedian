>Def (A pseudo - matric):
>	Let $X$ be a set. And $d:X^2\to\mathbb{R}$.
>	We say that $d$ is a pseudo - matric on $X$ when:

^3a1a19

>	>(1): $d$ is symetric. Meaning that $\forall x,y \in X: d(x,y) = d(y,x)$.

>	>(2): $d$ is positive. Meaning that $\forall x,y \in X: d(x,y) \geq 0 \vee d(x,x) = 0$.

^6222e1

>	>(3): Triangle inequality ($\triangle ie$). Meaning that $\forall x,y,z \in X: d(x,z) \leq d(x,y) + d(y,z)$.

^967160

>Note:
>	For $d$ to be [[#^967160|a pseudo matric]] on $X$, it has to have the same requirements as [[Metric space#^344d53|a matric]] on $X$ except for the "[[Metric space#^6067ad|fully positive]]" requirement that is weakend to just "[[#^6222e1|positive]]".

>Def (Equivalency under a pseudo matric):
>	Let $X$ be a set. And $d$ [[#^3a1a19|a pseudo - matric]] on $X$.
>	We define $\equiv_{d}:= \left\{ (x,y) \in X^2 \mid d(x,y) = 0 \right\}$.

>Proposition:
>	Let $X$ be a set. And $d$ [[#^3a1a19|a pseudo - matric]] on $X$.
>	Then $\equiv_{d}$ is [[Equivalence|an equivalence relation]] on $X$.
>Proof:
>	>[[Symetric]]: Obvious.
>	
>	>[[Reflexive]]: Obvious.
>	
>	>[[Transitive]]: Let $x,y,z \in X$ s.t. $x \equiv_d y \vee y \equiv_d z$. We need to show that $x \equiv_d z$.
>	>	By definition we get that $d(x,y) = d(y,z) = 0$. And because $d$ is a pseudo - matric, [[#^967160|it has the]] $\triangle ie$. Thus $d(x,z) \leq d(x,y) + d(y,z) = 0 + 0 = 0$ and therefor, by definition $x \equiv_d z$.

>Def (The equivalency classes induced by a pseudo matric):
>	Let $X$ be a set. And $d$ [[#^3a1a19|a pseudo - matric]] on $X$.
>	We will define $$X':=X\big / {\equiv_d}$$ (using the )