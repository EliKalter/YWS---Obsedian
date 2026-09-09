Given some (k) candidates we want to choose a subset of them (r) who will be picked.

The candidates can be represented as a score, either in [0,1] (continous) or in [100] (descrete).

They can maybe be represented as a vector of scores (l), each representing their score in one aspect.

We call the scores that represent the candidates "The truth" or "The objective truth".

We have interviewers (n). We think of an interviewer as someone who gives their opinion about the candidates. And we can talk about how good that opinion is, in the lense of how "close" the opinion is to the truth.

Then we can make a final desicion based on the opinions the interviewers gave for the candidates. And our job is to come up with a method of making that final desicion, in a way that will yield good results, meaning that we will make decisions that align well with the objective truth.
Obviously the quality of the final decision might depand on the quality of the interviewers, so we  want to construct a way of measuring the quality of a final desition method, relative to the quality of the interviewers.

>A candidate:
>	We represent a candidate as $D^l$
>	For $D \in \left\{ [0,1], [100] \right\}$ the way we represent the input scores
>	And $l$ is the amount of different criteria we take as input (Maybe one is average grade of the candidate, and another is their level of English)


>An interviewer: 
>	We represent an interviewer as $f:(D^l)^k \to R^{l'}$
>	For $R \in \left\{ [0,1]^k, [100]^k, S_k, \begin{pmatrix} [k] \\ r \end{pmatrix} \right\}$  is the way the interviewer expresses their opinio
>	And $l'$ allows for a multy dimensional answer, maybe the opinion is one score for social skils and another for academic ability. It is usually 1.

>Our candidates:
>	We fix some $x = (x_1, \dots, x_k) \in D^k$ and call it "our candidates".
>	(Because we want to model a situation where we don't have controll over who the candidates will be.)

>The distrebution of the candidates:
>	Later.

>A fixed collection of interviewers:
>	Denote $$\mathcal{F}:=(R^{l'})^{(D^l)^k}$$ the set of all interviewers.
>	(It might look like $([0,1]^k)^{[0,1]^k}$ for the case where $l,l' = 1, D=[0,1], R=[0,1]^k$.)

>Our interviewers:
>	For $n\in \mathbb{N}$ we fix $\left( f_i \right)_{i=1}^n \subseteq \mathcal{F}$, and call it "our interviewers".
>	(Because we want to model a situation where we don't have controll over who the interviewers will be.)

>The quality of our interviewers:
>	Later.

>A method for making final decisions:
>	We represent such a decision method as $\delta: (R^{l'})^n \to \begin{pmatrix} [k] \\ r \end{pmatrix}$.
>	Which will take the output of our interveiwers, and give a final verdict on which candidates are chosen.

>Our verdict method:
>	We fix one $\delta: (R^{l'})^n \to \begin{pmatrix} [k] \\ r \end{pmatrix}$ and call it "our verdict method"

>Remark:
>	In the case where $\delta = \zeta_A \circ \psi$ for some $\psi: R^{l'} \to A$ for $A$ [[Natural way to project onto teams#^710c40|a set that yields order on k]] , we will call that $\psi$ "our choice of verdict system" instead/along with $\delta$.

>Quality:
>	We will want to be able to quantify the quality of verdict methods and give a quality score to our verdict method