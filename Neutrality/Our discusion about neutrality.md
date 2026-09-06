There is [[Neutrality#^41bc65|the definition of neutrality]] as Ehud defined it, here we will call it "Conjunction neutrality" or "Respects conjunction".

We considered the following property:

>Def ($n$ - dimensional Composition neutrality / Respects composition):
>	Let $f:S_k^n \to S_k$. We say that $f$ is neutral when for all $\tau \in S_k$ and  $\sigma = \begin{pmatrix} \sigma_1 \\ \sigma_2 \\ \vdots \\ \sigma_n \end{pmatrix} \in S_k^n$ we have that $f(\tau\circ\sigma) = \tau\circ f(\sigma)$
>	
>	Where $\tau\circ\sigma$ is defined according to [[Neutrality#^7740ad|applying 1 dim func to an n dim vector]] for the "composition by $\tau$ function" ($\sigma \mapsto \tau\circ\sigma$).

^021854

And we wanted to check for some concrete $f$ examples, whether or not it is "Conjunction neutral", and whether or not it is "Composition neutral".
We checked the folowing examples: ^23f405
>Looking at $f_i:S_3 \to S_3$ given by:
>	(1): $\sigma \overset{f_1}{\mapsto} \sigma^2$
>	(2): $\sigma \overset{f_2}{\mapsto} \sigma^{-1}$
>	(3): $\sigma \overset{f_3}{\mapsto} \alpha\circ\sigma$  for a fixed $\alpha \in S_3$
>	(4): $\sigma \overset{f_4}{\mapsto} \alpha\circ\sigma\circ\alpha^{-1}$  for a fixed $\alpha \in S_3$

We got that:

|       | Conjunction | Composition |
| ----- | ----------- | ----------- |
| $f_1$ | [V]         | [X]         |
| $f_2$ | [V]         | [X]         |
| $f_3$ | [X]         | [X]         |
| $f_4$ | [X]         | [X]         |

^bfa273

Here we realized that this does not help a lot with intuition and moved on to [[For ehud (Sunday - 06.09.26)#^60f9c4|trying the visual approach]]
