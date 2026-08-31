>Def (Neutral function on symetreis):
>	Let $f:S_k \to S_k$. We say that $f$ is neutral when for all $\tau,\sigma \in S_k$ $f(\tau\circ\sigma\circ\tau^{-1}) = \tau\circ f(\sigma) \circ \tau^{-1}$

>Def ($n$ - dimensional conjugation):
>	Let $\tau \in S_k$ and $\sigma = \begin{pmatrix} \sigma_1 \\ \sigma_2 \\ \vdots \\ \sigma_n \end{pmatrix} \in S_k^n$. We denote $\tau\circ\sigma\circ\tau^{-1} := \left( \tau \circ \sigma_i \circ \tau^{-1} \right)_{i = 1}^n$.

^f5dcf4

>Def (Applying a $1$ - dimensional $\varphi$ to a $n$ - dimensional vector):
>	Let $S, R$ be sets. And $\varphi:S \to R$. Then we define $\varphi_n:S^n \to R^n$ by $\left( s_i \right)_{i = 1}^n \mapsto \left( \varphi(s_i) \right)_{i = 1}^n$.

^7740ad

>Note:
>	[[#^f5dcf4|n - dim conj]] is just [[#^7740ad|applying 1 - d dim function of n - dim vector]] for $\varphi:S_k \to S_k$ given by $\sigma \mapsto \tau \circ \sigma \circ \tau^{-1}$.

>Def ($n$ - dimensional neutrality):
>	Let $f:S_k^n \to S_k$. We say that $f$ is neutral when for all $\tau \in S_k$ and  $\sigma = \begin{pmatrix} \sigma_1 \\ \sigma_2 \\ \vdots \\ \sigma_n \end{pmatrix} \in S_k^n$ we have that $f(\tau\circ\sigma\circ\tau^{-1}) = \tau\circ f(\sigma) \circ \tau^{-1}$
>Where $\tau\circ\sigma\circ\tau^{-1}$ is defined according to [[#^f5dcf4|n - dim conjugation]] and $\tau\circ f(\sigma) \circ \tau^{-1}$ is normal conjugation.