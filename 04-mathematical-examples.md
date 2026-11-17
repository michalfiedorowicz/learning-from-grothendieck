# Mathematical examples

[Contents](README.md) · [Previous: structural lessons](03-structural-lessons.md) · [Next: inquiry practice](05-inquiry-practice.md)

Some entries explain historical mathematical mechanisms; others are elementary illustrations developed to clarify their methodological consequences. The latter are not attributed as Grothendieck's own examples. The arguments are ordinary mathematics, not a claim of new theorem-prover verification.

## Nilpotents and the limits of ordinary values

In the field $\mathbb F_3$, the equation $x^2=0$ has only the solution $x=0$. Now consider the ring of dual numbers

$$
A=\mathbb F_3[\varepsilon]/(\varepsilon^2).
$$

Every element is uniquely $a+b\varepsilon$, with $a,b\in\mathbb F_3$, and

$$
(a+b\varepsilon)^2=a^2+2ab\varepsilon.
$$

If this square is zero, then $a^2=0$ in the field, so $a=0$. Every value of $b$ then works. The roots are exactly $0$, $\varepsilon$, and $2\varepsilon$.

The nonzero element $\varepsilon$ is nilpotent: its square vanishes although it does not. Restricting attention to field-valued solutions hides this behavior. The broader setting contains structure that the earlier observation could not express.

This is an elementary illustration of the mechanism discussed in [D, §1] and [M, pp. 18-19]. It does not imply that more detailed models are always better. It identifies a particular distinction and the kind of question for which that distinction matters.

## Generalized points distinguish what field points miss

Let $k$ be a field. In the category of $k$-schemes, compare

$$
P=\operatorname{Spec}(k),\qquad
D=\operatorname{Spec}(k[\varepsilon]/(\varepsilon^2)).
$$

Each has one underlying topological point. For every extension field $K/k$, each also has exactly one $K$-valued point as a $k$-scheme. A $k$-algebra map

$$
k[\varepsilon]/(\varepsilon^2)\longrightarrow K
$$

must send $\varepsilon$ to a square-zero element of a field, hence to zero. Even all extension-field probes fail to distinguish these two schemes.

Now use $D$ itself as a probe. There is exactly one $k$-morphism $D\to P$, since $P$ is terminal among $k$-schemes. There are at least two distinct $k$-morphisms $D\to D$: on coordinate rings, send $\varepsilon$ to zero or to $\varepsilon$. Both preserve $\varepsilon^2=0$.

The enlarged probe class sees a distinction that the narrower class cannot see. Completeness within an inadequate class of observations is not completeness for the object.

For an object $X$ of a locally small category, its representable functor is

$$
h_X(T)=\operatorname{Hom}(T,X).
$$

For a map $u:T'\to T$, the induced map $h_X(T)\to h_X(T')$ is precomposition by $u$. This compatibility is part of the information. Under the usual size conventions, Yoneda gives

$$
\operatorname{Nat}(h_X,h_Y)\cong\operatorname{Hom}(X,Y).
$$

Thus the full representable functor identifies its representing object up to isomorphism. It does not say that every proposed functor is representable or that an arbitrary finite feature vector determines an object. [Y; G]

## Relative objects and base change

Let $p:X\to S$ be a scheme over a base $S$, and let $f:S'\to S$ be a change of base. The fiber product has maps

$$
p_X:X\times_S S'\to X,\qquad
p_{S'}:X\times_S S'\to S'
$$

such that $p\circ p_X=f\circ p_{S'}$.

Its defining property is this: for any scheme $T$ with maps $a:T\to X$ and $b:T\to S'$ satisfying $p\circ a=f\circ b$, there is a unique $u:T\to X\times_S S'$ with $p_X\circ u=a$ and $p_{S'}\circ u=b$.

For affine schemes, ring maps $R\to A$ and $R\to B$ give

$$
\operatorname{Spec}(A)\times_{\operatorname{Spec}(R)}\operatorname{Spec}(B)
\cong\operatorname{Spec}(A\otimes_R B).
$$

The common base is part of the construction. This is not an unqualified Cartesian product of underlying point sets. The relative viewpoint treats extension of the base and variation in a family through a common language while retaining the differences between bases. [D, §1; M, pp. 20-21; F]

The transferable discipline is to preserve agreement conditions when changing context. Its mathematical conclusion requires the actual categorical setting; a metaphorical base does not supply it.

## Why an isomorphism class may forget too much

*Esquisse* objects to the loss of automorphism groups in coarse moduli for the problem being considered. It also discusses fundamental groupoids and suitable families of base points as ways to retain relevant symmetry. [E, §2, PDF pp. 5-6]

An elementary abstract illustration separates a groupoid from its set of isomorphism classes. A one-object groupoid with a trivial automorphism group and a one-object groupoid with a nontrivial automorphism group both have a singleton set of isomorphism classes. The class set alone cannot recover the automorphism group.

The example does not establish that every quotient is inadequate. If only the class is needed, the quotient may be sufficient. If the next operation concerns symmetry or ways of identification, the discarded data matters. A representation should be judged against those operations, not against a universal preference for smallness.

## Cohomology through a common construction

McLarty describes categorical exactness and injective resolutions as a way to organize cohomological constructions that had required separate foundations. [M, pp. 7-11]

One must retain the hypotheses. A Grothendieck abelian category, with the relevant coproducts, exact filtered colimits (AB5), and a generator, has enough injectives. "AB5 alone" and "every abelian category" are not the statement being used. [A; I]

For a sheaf of abelian groups $\mathcal F$ on a topological space $X$, choose an injective resolution

$$
0\longrightarrow\mathcal F\longrightarrow I^0\longrightarrow I^1
\longrightarrow\cdots.
$$

Apply global sections to obtain a complex. The sheaf cohomology groups are

$$
H^n(X,\mathcal F)=H^n(\Gamma(X,I^\bullet)).
$$

The existence theorem, the construction, and an efficient calculation are different matters. Suitable acyclic or other special resolutions can remain useful computational tools. The common framework explains their relationship rather than requiring every calculation to use the same concrete presentation.

This account is a mechanism sketch with modern precision references, not a replacement for a treatment of derived functors or a claim about sole historical authorship.

## Gluing and descent do not mean arbitrary assembly

For a sheaf of sets $\mathcal F$ on a topological space, let $U=\bigcup_i U_i$. If sections $s_i\in\mathcal F(U_i)$ agree after restriction to every overlap $U_i\cap U_j$, the sheaf condition gives a unique section $s\in\mathcal F(U)$ restricting to all the $s_i$.

Agreement is substantive. Independently chosen local sections need not agree, and a presheaf need not satisfy this gluing condition. General descent also distinguishes properties, morphisms, and objects; effectiveness of object descent requires the applicable hypotheses. [D, §2; M, pp. 14, 16-17]

The useful methodological analogy is that local validity does not establish compatible composition. It does not imply that every set of research reports is a sheaf or that every proposed collection of local data has a global realization.

## A richer idea of locality and of space

A topology determines what counts as a local test and a covering. Deligne's discussion of étale topology explains a change in the allowable morphisms and covers, extending local geometric reasoning beyond ordinary open subsets. [D, §2]

Grothendieck's account in [P, §§12-13] further distinguishes studying spaces through sheaves from taking the category of set-valued sheaves as the carrier of spatial structure, and then considering more general categories with appropriate properties. The reconstruction of an old topological space has qualifications: the cited discussion uses sobriety, including Hausdorff spaces, rather than asserting recovery of every space.

This is a guide to the conceptual move, not a complete axiomatization of topoi. More views of an old object, a change in its representation, and admission of genuinely new objects are distinct steps.

## A precise correspondence across mathematical domains

In *Esquisse*, finite maps embedded in surfaces, suitable ramified coverings of the projective line, and algebraic curves over number fields are connected through a mathematical dictionary. Grothendieck explicitly credits Belyi's result. [E, §3, PDF pp. 10-13]

The methodological significance is the construction of a productive correspondence: operations and arithmetic information become accessible through a combinatorial presentation. This is stronger than noticing that two diagrams look alike.

The account here identifies the historical example without attempting the full theorem or a current survey of its consequences. A correspondence between mathematical domains does not itself validate a proposed transfer between empirical domains.

## Re-expression can simplify without forgetting

Consider the idealized recurrences

$$
T_{n+1}=T_a+r(T_n-T_a),\qquad
V_{n+1}=rV_n+u.
$$

Assume fixed parameters and $|r|<1$. Their equilibria are $T_a$ and $V_*=u/(1-r)$. For fixed nonzero scales $s_T,s_V$ in their respective units, define

$$
z_T=(T-T_a)/s_T,\qquad z_V=(V-V_*)/s_V.
$$

Both satisfy $z_{n+1}=rz_n$, hence $z_n=r^nz_0$ by induction. Bounds on $z_n$ return to the original quantities through their respective scales. The coordinate changes are invertible; no state information has been discarded.

With $r=1/2$, $T_a=20$, $u=3$, unit scales, and initial states $28$ and $14$, both deviations begin at $8$ and follow

$$
8,4,2,1,1/2,1/4,1/8,1/16,1/32.
$$

Three failures show what the shared syntax does not establish:

- For $r=3/2$, deviations starting at $8$ grow as $8,12,18,27,81/2$. Stability depends on its hypothesis.
- The summary $\alpha(x)=|x|$ merges $-1$ and $1$. After $x\mapsto x+1$, their magnitudes become $0$ and $2$. A current observation can be insufficient for a later use.
- The laws $f(z)=z/2$ and $g(z)=z/2+z(z-1)(z-2)$ agree at $0,1,2$ but return $3/2$ and $15/2$ at $3$. A finite fit did not identify the governing law.

These are supplied mathematical models. They neither establish that a real cooling device obeys the recurrence nor show that an adequate representation can be discovered automatically.

## A relational obstruction that local counts miss

Suppose each of three simultaneous jobs needs one resource, each resource can serve at most one job, and compatibility is known. An assignment must be injective and respect the allowed pairs.

| Job | Feasible instance | Infeasible instance |
| --- | --- | --- |
| 1 | $\{r_1\}$ | $\{r_1\}$ |
| 2 | $\{r_2\}$ | $\{r_1\}$ |
| 3 | $\{r_1,r_3\}$ | $\{r_2,r_3\}$ |

Both have job option counts $(1,1,2)$ and resource incidence counts $(2,1,1)$. The left instance admits $1\mapsto r_1$, $2\mapsto r_2$, $3\mapsto r_3$. The right cannot assign distinct resources to jobs 1 and 2.

For any set of jobs $S$, a necessary condition is $|N(S)|\ge |S|$, where $N(S)$ is the union of their compatible resources. Distinct assigned resources must all lie in that union. The right instance fails for $S=\{1,2\}$.

The useful representation changes the question from whether every job has an option to which sets compete for insufficient joint capacity. That is a concrete form of fertility. The correspondence fails if sequential scheduling, non-unit capacity, durations, or preferences rather than permissions are decisive. A method applicable to two instances does not make their outcomes identical.

[Source details](SOURCES.md) · [Concept index](INDEX.md)
