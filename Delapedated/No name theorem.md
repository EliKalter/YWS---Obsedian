>Weak version (Proved 200 years ago):
>	If f is always transitive than f is a dictatorship

>Strong version (Proved on the year 2000 $\pm$ 2 by gil of huji):
>	If f is almost always transitive, then f is almost a dictatorship.
>	Denote S the set of all inputs that f gives a transitive result for.

I don't understand the exact setup of the theorems, but that was the spirit.

>Proposed basic theorem:
>	Let $f:\left( \mathbb{Z}_2^3 \right)^3\to \mathbb{Z}_2^3$ be a transitive function (need the definition). Then $f$ [[Influence of an entry on a function#^f38582|is a dictatorship]].

^e256fd

>Counter example:
>	$\left( \mathbb{Z}_2^3 \right)^3$ is isomorphic to $\mathbb{Z}_2^9$. We will show $T:\mathbb{Z}_2^9 \to \mathbb{Z}_2^3$ a linear map that is transitive and is not a dictatorship.

^829045

>	>We can define such $T$ by choosing the $T(e_i)$'s. We will choose $T(e_1) = e_1$, $T(e_2) = e_2 + e_3$, and $\forall i \geq 3: T(e_i):=(0,0,0)$.
^4f1f77

>	>$T$ is transitive: For all $v = (v_i)_{i = 1}^9 \in \mathbb{Z}_2^9$ $T(v) = (v_1, v_2, v_2)$. And that is allways a transitive element of $\mathbb{Z}_2^3$ (Check manually).
>	
>	>$T$ is not a dictatorship: By [[Linear dictatorship characterization#^b75cf5]]

>General approach for proving such themed thoerems.
>	When we have a theorem that looks like "When $f$ has $X$ properties (Where $X$ is a set of properties) then $f$ is a dictatorship". One approach of trying to prove that, might be spliting the work into two stages:
>	
>	>(1): Shoing that if that $f$ is linear, then it has to be a dictatorship (Could be easyer then the general case thanks to [[Linear dictatorship characterization#^b75cf5]]).
>	
>	>(2): Showing that such $f$ mush be linear.
>	
>	Not sure how general is this general method, in what situations does it actually work. Under what assumpsions every dictatorship is linear? And under what assumpsions we can show that f is linear, even if not every dictatorship has to be linear?

^61dc7f
