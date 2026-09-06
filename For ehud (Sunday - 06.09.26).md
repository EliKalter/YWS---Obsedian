
>Introduction:
>	This file contains a summary of what we worked on over the past week. It consists of four parts:
>	(1): The conditions appearing in Arrow's theorem, which we tried to define carefully;
>	(2): an attempt to understand neutrality by representing tournaments graphically;
>	(3): our attempt to reconstruct the theorem Ehud presented in the last meeting;
>	(4) a first model of an interview process.
>	Each item links to the note where the definition or claim is written out in full, and where something is still missing or only sketched we say so.

>1) Arrows conditions
>	>(1) We defined [[Unanimity#^e845f4|unanimity]] [[Unanimity#^29ad08|k-unanimity]] and [[Unanimity#^156ba1|all-unanimity]].
>	
>	>(2): Neutrality: We tried two variants of an attribute that could be called "neutrality", "[[Neutrality#^41bc65|Conjucation neutrality]]" and "[[Our discusion about neutrality#^021854|Composition neutrality]]"  [[Our discusion about neutrality#^23f405|and checked for some concrete examples]], which satisfy which property, [[Our discusion about neutrality#^bfa273|see table]].
>	
>	>(3): We carefully defined [[IIA - אב"ק|IIA]]

>2) Neutrality and Tournaments
>	We felt we don't understand the neutality property as presented by Ehud in our meeting, and wanted to see if we could give it a grphical representation, so that we can hopefully characterize neutral functions in terms of that visual representation.
>	
>	>(1): We defined tournaments (of k contestents) in a few natural ways to represent them.
>	>	a) [[Tournaments and Tournament Relations#^f2bd52|A set of inequalities]];
>	>	b) [[Tournaments as Graphs#^e7a17b|a graph in k nodes]];
>	>	c) [[Tournamnets as Binary Vectors#^2a692b|an element from]] $\mathbb{Z}_2^{C(k,2)}$ [[Tournamnets as Binary Vectors#^2a692b|(requires an arbitrary choice of order);]]
>	>	d) [[Permutations as Tournaments#^34bd27|a permutation (only for transitive tournaments)]].
>
>	>(2): We defined an [[Tournaments as Graphs#^f16132|action]] of $S_k$ on the graphs (in k nodes), for which we can easily find the graph representing $\sigma \circ \tau$ given the graph representing one of them, [[Tournaments as Graphs#^3af7f7||see corollary for useful identities]].
>
>	>(3): We are yet to determine whether this entire graph representation approach is useful for understanding neutrality. On the one hand it might not be useful because of the fact that there is no embedding $S_3 \to \mathbb{Z}_2^3$ (by Lagrange's theorem), and on the other hand, it might be useful because of (2).

^60f9c4

>3) No name theorem
>	In our previous meeting, Ehud presented some theorem that had tow versions, a basic one, and one that expands on the first in an $\varepsilon$ manner. We did not remember the exact formulation.
>	>(1): We suggested one potential proposition that we thought could be the basic theorem. And after some work we found a counter example to that suggestion.
>	
>	>(2): We carefully defined a dictator function, an index that matters to f, the ammound of influence of an index on f, and found some connections between them. For example, the characterization of f as a dictator in terms of having at most one index that matters.
>	
>	>(3): We suggested an approach for proving theorems of the form "if f has this properties then f is a dictatorship":
>	>	a) Prove that f is linear
>	>	b) Show that such linear f is a dictatorship 

>4) interview processes
>	>We tried to model the problem of a screening process of potential candidates, and quickly realized that there is too much room there for many choices to be made, and that we should look at some specific variation of the problem and model them in more detail.
>	
>	>(1): We decided to look at a two step process where there are $n$ [[Model#^993617|interviewers]] in the first stage which comprise an [[Model#^dfad6e|interview process]], and then a final [[Model#^1a8ab6|decision]] is made based on the "opinions" of the interviewers.
>	
>	>(2): We tried to come up with a [[Model#^b2fb6f|method of quantifying the "quality"]] of such screening systems. Given a list of simple criteria that intuitively comprise the "fairness" such systems,  the quality of the system will be some function of those criteria, [[Model#^727e39|see discussion]].
