
>Def (Atomic natural projection):
>	Let $A,B$ be sets. We say that there is an atomic natural projection from $A$ into $B$ when there is a function in the [[The list of atomic natural projections#^937368|list of atomic natural projections]] call it $\zeta$ s.t. $Dom(\zeta) = A \wedge Range(\zeta) = B$.
>	In that case we will denote $\zeta_{B,A}:=\zeta$.

^62832b

>Def (Natural projection):
>	Let $A,B$ be sets. We say that there is an a natural projection from $A$ into $B$ when there is a series $(C_0,\dots , C_l)$ $l \in \mathbb{N}$ with $C_0 = A \wedge C_l = B$ s.t. $\forall i \in [l]$ there is [[#^62832b|an atomic natural projection]] from $C_{i-1}$ into $C_i$.
>	In that case we denote (recursivaly): $$\zeta_{B,A} := \begin{cases} \zeta_{B,A} & l=1 \\ \zeta_{B,C_{l-1}} \circ \zeta_{C_{l-1},A} & l > 1 \end{cases}$$
>	Where $\zeta_{C_{l-1},A}$ is defined by the same rule.

