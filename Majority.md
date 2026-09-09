For $t \in \mathbb{N}$ and $n := 2t + 1$. Assume $x = (x_1,\dots,x_n) \in \mathbb{Z}_2^n$. We will define the majority of $x$ to be the value that is found more in $x$. Formaly we mean $majority(x):= \begin{cases} 1 & \sum\limits_{i=1}^{n} x_i > \frac{n-1}{2} \\ 0 & \sum\limits_{i=1}^{n} x_i < \frac{n-1}{2} \end{cases}$
So now we have:
>Def (majority):
>	Let $t \in \mathbb{N}$ and $n := 2t + 1$.
>	$majority: \mathbb{Z}_2^n \to \mathbb{Z}_2$ is given by $(x_1,\dots,x_n) \mapsto \begin{cases} 1 & \sum\limits_{i=1}^{n} x_i > \frac{n-1}{2} \\ 0 & \sum\limits_{i=1}^{n} x_i < \frac{n-1}{2} \end{cases}$

>Majority on a coordinate:
	Let $t \in \mathbb{N}$ denote $n := 2t + 1$, and let $m \in \mathbb{N}$. Assume we have some $x_1 = (x_1^1,\dots,c_1^m),\dots,x_n = (x_n^1,\dots,x_n^m)$. Then for a coordinate $i_0 \in [m]$ we can look at $(x_{j}^{i_0})_{j=1}^n \in \mathbb{Z}_2^n$ the vector of the entries of the $x_i$'s at the $i_0$'th coordinate, denote $coor_{i_0}((x_j)_{j=1}^n)$. And we can look at $majority(coor_{i_0}((x_j)_{j=1}^n))$ as the value majority of the $x_i$'s gave the $i_0$'th coordinate.

>Majority on all coordinates at once. (Majority coordinate wise vs Majority per each vec by itself)

Let $k,t \in \mathbb{N}$. Denote $m:=\begin{pmatrix} k \\ 2 \end{pmatrix}, n:=2t+1$ And assume $\omega: S_k \to z_2^m$. (Here I come from the prespective of having $\omega$ that maps a permutation $\sigma$ to an element $\omega(\sigma) \in z_2^m$ s.t. both represent the same [[Tournaments and Tournament Relations#^f2bd52|tournament]] . Such bijections we have seen [[Tournamnets as Binary Vectors#^2a692b|here]] for example). Then for some  $\sigma = (\sigma_1,\dots,\sigma_n) \in S_k^n$ we can define "the majority permutation" to be the permutation that is obtained by looking at the elments of $z_2^m$ that are the images of the $\sigma_i$'s under $\omega$, for which we take the majority of each coordinate, and finaly we go back with $\omega^{-1}$ and get a permutation. Formally: Define $majority(\sigma):= \omega^{-1}\left( majority(coor_1( (\omega(\sigma_i))_{i=1}^n )), \dots,majority(coor_m( (\omega(\sigma_i))_{i=1}^n ))  \right)$ ^e5f668

TODO
Note: It is unclear why would $majority(coor_1( (\omega(\sigma_i))_{i=1}^n )), \dots,majority(coor_m( (\omega(\sigma_i))_{i=1}^n ))$ be transitive (We have examples where it isn't...). And when it isn't, it would not make sense to apply $\omega^{-1}$... We need to check under what conditions does it make sense to define it in this way. ^f38740

TODO
Note: We need to pay attention to the fact that $\omega$ is used in the definiton. We have to check under what conditions on $\omega$ this is well defined.