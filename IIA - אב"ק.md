Independent of irrelevant (advantage?)
אי-תלות בבלתי קשורים

>Def ($\equiv_{a,b}^<$):
>	Let $k \in \mathbb{N}$ and $a,b \in [k]$ s.t. $a \neq b$.
>	$\equiv_{a,b}^<:= \left\{ \left( \tau, \tau' \right) \in S_k^2 \mid \tau(a) < \tau(b) \iff \tau'(a) < \tau'(b) \right\}$

>Def ($\equiv_{a,b}^<$ for the $n$ - dimensional case):
>	Let $k,n \in \mathbb{N}$ and $a,b \in [k]$ s.t. $a \neq b$.
>	$\equiv_{a,b}^<:= \left\{ \left( \tau = \begin{pmatrix} \tau_1 \\ \tau_2 \\ \vdots \\ \tau_n \end{pmatrix}, \begin{pmatrix} \tau'_1 \\ \tau'_2 \\ \vdots \\ \tau'_n \end{pmatrix} \right) \in (S_k^n)^2 \mid \forall i \in [n]:  \tau_i \equiv_{a,b}^< \tau'_i \right\}$
>Note:
>	We use the symbol $\equiv_{a,b}^<$ both for $\tau \in S_k$ and for $\tau \in S_k^n$ interchangeably

>Def ($a,b$ - IIA):
>	Let $f: S_k^n \to S_k$, and $a,b \in [k]$ ($a \neq b$).
>	$f$ is called "$a,b$ - IIA", when for all $\sigma, \sigma' \in S_k^n$: $\sigma \equiv_{a,b}^< \sigma' \implies f(\sigma) \equiv_{a,b}^< f(\sigma')$.

>Def (IIA):
>	Let $f: S_k^n \to S_k$. We say that $f$ is IIA when for all $a,b \in [k]$ $f$ is $a,b$ - IIA.