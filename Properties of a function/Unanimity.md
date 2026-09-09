

>Def (r-unanimity):
>	Let $k,n \in \mathbb{N}$ and $r \in [k]$.
>	Let $f:S_k^n \to S_k$. We say that $f$ is $r$ - unanimous, or that $f$ respects unanimous voting for the $r$'th place when for all $\sigma = \begin{pmatrix} \sigma_1 \\ \sigma_2 \\ \vdots \\ \sigma_n \end{pmatrix} \in S_k^n$, if $\sigma_i^{-1}(r) = \sigma_j^{-1}(r) \forall i,j \in [n]$ then $f\left(\sigma\right)^{-1}(r) = \sigma_1^{-1}(r)$.
>	That is to say that if all the voters agree on who should be the $r$'th ranked candidate, then $f(\sigma)$ agrees and sends that candidate to $r$.

^29ad08

>Def (Unanimous function):

^e845f4

	In the same context as [[#^29ad08|the last definition]], we say that $f$ is unanimous when it is $1$ - unanimous.
	That is to say that if all the voters agree on who is the best candidate, then $f(\sigma)$ agrees and sends that candidate to $1$.


>Def (all-unanimity):
>	[[#^29ad08|In the same context]], we say that $f$ is all-unanimous when $\forall r \in [k]$ $f$ is $r$ - unanimous.

^156ba1

Other variations:
	$f$ respects $r$ agreements

>Them:
>	Unan + IIA $\implies$ all-unanimity