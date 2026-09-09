
>General context:
>	Let $A_1,\dots,A_n, B$ be sets.
>	Denote $\mathcal{A}:= \bigtimes\limits_{i=1}^{n} A_i$
>	And let $f:\mathcal{A} \to B$.

^97eb0f

>Note:
>	Often we will look at simplified versions:

>	>(1): $A_1 = \cdots = A_n = A$ for some set $A$. i.e. $\mathcal{A} = A^n$
^93691a

>	>(2): $B = \mathcal{A}$

>	>(3): [[#^93691a|(1)]] and  $B = A$.

>Def (Does entry matter to $f$):
>	[[#^97eb0f|In the general context]]
>	Let $i_0 \in [n]$. We say that $i_0$ matters to $f$ when there exists $p = \begin{pmatrix} p_1 \\ p_2 \\ \vdots \\ p_n \end{pmatrix},p' = \begin{pmatrix} p'_1 \\ p'_2 \\ \vdots \\ p'_n \end{pmatrix} \in \mathcal{A}$ s.t. $\forall j \in [n]: j \neq i_0 \implies p_{j} = p'_{j}$ and $f(p) \neq f(p')$. That is to say, that there exists some point $p$ where changing only the value at  the $i_0$'th entry of $p$ changes the value of $f$.

^328625

>Def (The matters func):
>	[[#^97eb0f|In the general context]]
>	We define $matters_f:[n] \to \mathbb{Z}_2$ by $i \mapsto \begin{cases} 1 & i_0 \text{ matters to } f \\ 0 & Otherwise \end{cases}$ 

>Def (The infulence of an entry):
>	[[#^97eb0f|In the general context]]
>	Let $i_0 \in [n]$. We denote $\Delta_{i_0}:= \left\{ \begin{pmatrix} x_1 \\ x_2 \\ \vdots \\ x_n \end{pmatrix} \in \mathcal{A} \Big\vert \exists x'_{i_0} \in A_{i_0} : f\begin{pmatrix} x_1 \\ x_2 \\ \vdots \\ x_n \end{pmatrix} \neq f\begin{pmatrix} x_1 \\ x_2 \\ \vdots \\ x'_{i_0} \\ \vdots \\ x_n \end{pmatrix} \right\}$ . 
>	We define the infulence of $i_0$ on $f$ to be $\frac{\left\vert \Delta_{i_0} \right\vert}{\left\vert \mathcal{A} \right\vert}$.

^ab104f

>Def (The influ func):
	[[#^97eb0f|In the general context]]
>	We define $influ_f:[n] \to \mathbb{R}_{+}$ by $$i \mapsto \frac{\left\vert \Delta_{i} \right\vert}{\left\vert \mathcal{A} \right\vert}$$

>Note:
>	(1): $matter_f(i_0) = \begin{cases} 1 & influ_f(i_0) \neq 0 \\ 0 & influ_f(i_0) = 0 \end{cases}$
>	(2): $influ_f(i_0) = \mathbb{P}_{\mathcal{A}}(\Delta_{i_0})$

>Def (Dictatorship):

^f80738

	[[#^97eb0f|In the general context]], we say that $f$ is a dictatorship when there is $i_0 \in [n]$ s.t. for all $p = \begin{pmatrix} p_1 \\ p_2 \\ \vdots \\ p_n \end{pmatrix},p' = \begin{pmatrix} p'_1 \\ p'_2 \\ \vdots \\ p'_n \end{pmatrix} \in \mathcal{A}$ we have that if $p_{i_0} = p'_{i_0}$ then $f(p) = f(p')$. That is to say, that a change in any entry except for the $i_0$'th entry, does not change the value of $f$

^f38582

>Note:
>	If $f$ is constant, then $f$ is a dictatorship, because for any $i \in [n]$ we will have the required property.

>Def (Real vs Trivial dictatorship):
>	[[#^97eb0f|In the general context]], and assume $f$ [[#^f38582|is a dictatorship]]. If $f$ is constant we say that $f$ is a trivial dictatorship, and when $\left\vert \text{Image } (f) \right\vert > 1$ we say that $f$ is a real dictatorship.

^79d24a

>Lemma:
>	[[#^97eb0f|In the general context]], and assume $f$ is a real dictatorship. Then $\exists ! i \in [n]$ s.t. $i$ matters to $f$.
>Proof:
>	When we have the time.

^c9806a

>Def (The dictator of a function):
>	[[#^97eb0f|In the general context]], and assume $f$ [[#^79d24a|is a real dictatorship]] . We call that unique $i_0 \in [n]$ [[#^c9806a|from the lemma]], the dictator of $f$.

>Lemma (Dictatorship iff at most one entry matters):
>	[[#^97eb0f|In the general context]] $f$ is a dictatorship $\iff$ $\exists i_0 \in [n]$ s.t. $\forall i_0 \neq j \in [n]: matter_f(j) = 0$.
>Proof:
>	In the pictures. Need time to type.

^0379b7

>Def (Equal influence):
>	[[#^97eb0f|In the general context]] we say that $f$ has eqaul influence when $\forall i,j \in [n]: influ_f(i) = iflu_f(j)$

^471bf9

>Def (Everyone have influence):
>	[[#^97eb0f|In the general context]] we say that everyone has influence over $f$ when $\forall i \in [n]: matters_f(i) = 1$

^cfc15d

