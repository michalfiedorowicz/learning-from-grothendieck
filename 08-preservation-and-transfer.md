# Preservation and transfer

[Contents](README.md) · [Previous: limits](07-limits.md) · [Sources](SOURCES.md)

This optional appendix develops a restricted mathematical account of several distinctions used in the collection. It assumes an interpretation has already been supplied. It does not solve interpretation, define all meaning, or provide an algorithm for discovering the right abstraction. The arguments are explanatory constructions, not historical claims about Grothendieck's notation or research programme.

## Interpretation is a separate obligation

Let $R$ be a set of representations and $M_\Gamma$ a set of situations or models in a context $\Gamma$. Even a partial interpretation

$$
I_\Gamma:R\rightharpoonup M_\Gamma
$$

requires justification. Ambiguous evidence may call for several candidate interpretations or a probabilistic model instead of a single map.

Fixing one interpretation allows subsequent mathematics to proceed. It does not prove that the interpretation was identified from the original material. The distinction between missing evidence, lossy representation, and computational difficulty remains in force.

## Exact adequacy relative to questions and continuations

Take a set $M$, a family of questions $q:M\to Y_q$ indexed by $Q$, and a family $\mathcal C$ of total allowed continuations $c:M\to M$ containing the identity. Write $U=(Q,\mathcal C)$ and define

$$
x\sim_U y
\quad\Longleftrightarrow\quad
\forall q\in Q,\ c\in\mathcal C,\quad q(c(x))=q(c(y)).
$$

This is an equivalence relation. It identifies situations that cannot be distinguished by the declared questions after any declared continuation.

An abstraction $\alpha:M\to A$ is exactly adequate for these uses when

$$
\alpha(x)=\alpha(y)\quad\Longrightarrow\quad x\sim_U y.
$$

It may retain more distinctions than the use requires. It may not merge two situations that require different answers under an allowed use.

This explains why the future operations matter. With $\alpha(x)=|x|$, the states $-1$ and $1$ have the same summary. If the question is current magnitude, that summary suffices. If continuation by $x\mapsto x+1$ is allowed, the resulting magnitudes $0$ and $2$ disagree.

## Factorization makes the preservation claim exact

Adequacy holds if and only if every $q\circ c$ has a unique factor

$$
\bar q_c:\operatorname{im}\alpha\to Y_q
$$

satisfying

$$
q\circ c=\bar q_c\circ\alpha,
$$

where $\alpha$ is corestricted to its image.

For the forward direction, define $\bar q_c(\alpha(x))=q(c(x))$. Adequacy says that this does not depend on the representative $x$. For the reverse direction, the factorization makes equal abstract values give equal answers. Uniqueness follows because every point of the image has a representative.

Using the image avoids making an arbitrary choice of answers for abstract values that never arise. This is a statement about lawful forgetting after interpretation, not a characterization of every useful change of viewpoint.

If $\mathcal C$ is closed under composition, the equivalence is stable under allowed continuations. To compare $c(x)$ with $c(y)$, any further test $q\circ d$ is the original test $q\circ(d\circ c)$, which is allowed. Adding questions or continuations can only refine the equivalence on a fixed $M$.

## A finite information limit

Suppose $M$ is finite and nonempty, with $N=|M/{\sim_U}|$. Exact adequacy implies

$$
|\operatorname{im}\alpha|\ge N.
$$

Indeed, map each abstract value $\alpha(x)$ to the equivalence class of $x$. Adequacy makes this well-defined, and every class occurs. The map is therefore onto.

If the abstract state has at most $2^b$ distinguishable encodings, then

$$
b\ge\lceil\log_2N\rceil.
$$

This is an information-capacity bound. It is not a runtime lower bound or proof that an optimal computable representation exists. Keeping the original material in an accessible store can preserve the missing distinctions, but that store and its access costs are then part of the system. A small summary plus a large retained source is not a contradiction of the bound.

Lossless encoding, invertible re-expression, narrower uses, approximation, and several complementary views remain possible. Their claims need to state which of these alternatives is being used.

## Shared dynamics support conditional reuse

Suppose two state spaces $M_S,M_T$ map to a common space $A$ by $\alpha_S,\alpha_T$. Let $F_S,F_T,F_A$ be total transitions and assume

$$
\alpha_i\circ F_i=F_A\circ\alpha_i,
\qquad i\in\{S,T\}.
$$

Induction gives

$$
\alpha_i(F_i^n(x))=F_A^n(\alpha_i(x)).
$$

If the question in each domain factors as $q_i=\bar q\circ\alpha_i$, then

$$
q_i(F_i^n(x))=\bar q(F_A^n(\alpha_i(x))).
$$

The shared structure is useful because it preserves an operation and an answer, not because both spaces happen to map to it. Every pair of sets maps to a singleton; that observation alone provides no discriminating consequence.

The cooling and accumulator example gives invertible coordinate changes satisfying this relationship for supplied parameters. Identifying the law and parameters from observations is additional work.

## A reduction needs reconstruction

For problem families with instances $X,Z$ and solution sets $\operatorname{Sol}_P(x)$ and $\operatorname{Sol}_K(z)$, a usable reduction needs an instance map

$$
a:X\to Z
$$

and, for each $x$, a reconstruction

$$
b_x:\operatorname{Sol}_K(a(x))\to\operatorname{Sol}_P(x).
$$

No inverse $a^{-1}$ is required. But reconstruction cannot be treated as free when it conceals the original problem. Its existence, computability, resource use, and adequacy for the desired output may each need attention.

Reconstructing an answer also need not reconstruct every desired evidence object. A result may require a witness, explanation, provenance, or authority that is not carried by the answer alone.

## Composition needs an intermediate contract

Suppose step one establishes $P_1(x)\Rightarrow Q_1(f(x))$ and step two establishes $P_2(y)\Rightarrow Q_2(g(y))$. Using those contracts to justify the composition requires that the relevant output of the first step satisfies $P_2$.

One sufficient bridge is $Q_1(y)\Rightarrow P_2(y)$ on the relevant outputs. A separately established stronger condition can also suffice. Type compatibility alone is not this implication.

This applies to physical units, currencies, time windows, object identity, observation scope, and proof assumptions. A claim about all currently visible records does not become a claim about all records that ever existed merely because another component accepts the same record format.

## Approximate composition

Let ideal maps $f_i:X_{i-1}\to X_i$ and approximations $\widetilde f_i$ act between metric spaces. Assume, on all relevant intermediate states, that $f_i$ is $L_i$-Lipschitz and

$$
d_i(\widetilde f_i(z),f_i(z))\le\varepsilon_i.
$$

Starting from the same initial state, let $E_i$ be the distance between approximate and ideal trajectories after stage $i$. The triangle inequality gives

$$
E_i\le\varepsilon_i+L_iE_{i-1},\qquad E_0=0.
$$

Induction yields

$$
E_n\le\sum_{i=1}^n\varepsilon_i\prod_{j=i+1}^nL_j.
$$

Both trajectories must stay in the domains where the assumptions hold. A first-stage error of $1/100$ followed by an exact multiplication by $100$ produces final error $1$. An exact later component can amplify an earlier error; a contraction can attenuate it.

The bound does not apply automatically to semantic similarity, uncalibrated confidence, arbitrary causal transfer, or discontinuous decisions. Those uses need an appropriate relation and their own argument.

## A shared language does not make interface work disappear

For $n$ domains, storing every ordered pairwise route can require $n(n-1)$ routes. A common representation with an inward and outward interface for each domain uses up to $2n$ routes under that organization.

This is a count of interfaces, not a complexity theorem for discovery. The common model or adapters may conceal the difficult pair-specific work. Compare total costs of finding the structure, building interfaces, checking target applicability, and revising them against the best actual alternative, not an artificially exhaustive set of bridges.

## Boundaries of this fragment

The exact account uses supplied interpretations, total deterministic continuations, and equality of answers. Probability, partial actions, nondeterminism, proof-sensitive evidence, and open-world change require their own adequacy conditions. Approximation does not inherit an exact guarantee by changing a symbol.

A representation may also suffice for a decision while leaving exact facts unresolved. Question formation can change the use itself. Both are legitimate, but success under a revised use must not be reported as though the original question and criterion were unchanged.

[Concept index](INDEX.md)
