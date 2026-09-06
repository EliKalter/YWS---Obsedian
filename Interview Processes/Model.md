
>Model context:
>	Let $k,n\in\mathbb{N}$. We look at interview processes consisting of $n$ interviewers and $k$ candidates, represented by the set $[k]$ - each interviewer decides one of two option with respect ot each candidate: "accepted", represented by the binary 1; or "rejected", represented by te binary 0. After the indiviual interviews have been done by each of the $n$ interviewers to each of the $k$ candidates, a final decision is reached for each candidate in the interview process with repect to an interview decision protocol.

>Def (interviewer): 
>	Let $k\in\mathbb{N}$. An interviewer is a mapping $f:[k]\to\mathbb{F}_2$. Define $\mathcal{F}_k:=\mathbb{F}_2^{[k]}$, the set of all interviewers (over $k$ candidates).

^993617

>Def (unordered finite collections):
>	Let $X$ be a set. Define $[X]_n$ to be the set of all unordered collections of $X$ of size $n$.

>Def (inteview stage):
> 	An interview process is a collection $\left\{f_i\right\}_{i=1}^n\in[\mathcal{F}_k]_n$.

^dfad6e

>Def (interview decision protocol):
>	An interview decision protocol a is a function $\Phi:[\mathcal{F}_k]_n\to\mathcal{F}_k$. Define $\mathcal{P}_{(k, n)}:=\mathcal{F}_k^{[\mathcal{F}_k]_n}$, the set of all interview processes (consisting of $n$ interviewers and $k$ candidates).

^1a8ab6

>Def (decision quality benchmark):
>	A decision quality benchmark is a function $B:\mathcal{P}_{(k,n)}\to D$ where $D\in\left\{\mathbb{R},\mathbb{R^+},[0,1],\mathbb{N},...\right\}$.

^b2fb6f

>Discussion:
>	We had the idea of definining evaluation functions of interview decision protocols $v_i:\mathcal{P}_{(k,n)}\to[0,1]$ for each "goodness/fairness" property $1\le i\le m$ that we want a protocol to satisfy. Then we would the option of defining $B:\mathcal{P}_{(k,n)}\to[0,1]$ for all $\Phi\in\mathcal{P}_{(k,n)}$ by $B(\Phi)=1-\sum_{i\in[m]}(w_i\cdot v_i(\Phi))$ for some non-negative $w_i$'s which sum up to $1$.
>	A "good" interview decision protocol is one that maximizes $B$; meaning the set of "good" interview decision protocols with respect to a decision qaulity benchmark $B$ is $Argmax_{\Phi\in\mathcal{P}_{(k,n)}} B(\Phi)\subseteq\mathcal{P}_{(k,n)}$.

^727e39

