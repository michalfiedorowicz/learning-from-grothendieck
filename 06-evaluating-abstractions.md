# Judging an abstraction

[Contents](README.md) · [Previous: inquiry practice](05-inquiry-practice.md) · [Next: limits](07-limits.md)

The following seven properties are proposed questions for judgment. They are not a scoring formula, a theorem about successful discovery, or a checklist that every early intuition must already satisfy.

## Faithfulness

Which differences can change the conclusion, and does the representation retain them? Faithfulness is relative to questions, operations, contexts, and evidence strength. It is not the retention of every available detail.

An abstraction fails when it merges situations that require different answers, or when it promotes predictive agreement into a causal claim. A proof can be faithful to a formal model while the interpretation of that model remains unsupported.

The generalized-point example shows that even all observations of an inadequate kind can miss structure. The preservation appendix states an exact version of the criterion for a supplied interpretation.

## Leverage

What becomes answerable, constructible, or materially easier because the representation was introduced? A new vocabulary, graph, or normal form has not yet shown leverage if the same work remains hidden in interpretation or reconstruction.

The gain may be a simpler argument, a diagnosis of impossibility, a reusable method, or access to a question that previously could not be stated. Returning the result to the actual situation is part of the achievement.

## Reach

Across which cases and contexts does the result apply, and under which conditions? Reach concerns warranted applicability, not the number of examples stored or the breadth of the vocabulary.

Weakening hypotheses does not preserve a theorem by default. Strengthening them may support a stronger conclusion while narrowing the family. That does not imply a universal inverse law between generality and correctness: a better representation can sometimes improve both.

Different instances may share a method while producing different results. The allocation example has the same local counts in a feasible and an infeasible instance. Reach of a method is not identity of its inputs or outputs.

## Fertility

Which further questions, distinctions, or constructions become possible? A representation can be fertile before it yields a numerical improvement on an existing task.

The allocation example changes the question from whether each job has an option to which sets of jobs compete for too little joint capacity. The new question exposes a real obstruction. Retrospectively renaming a supplied answer would not have done that.

Fertility is not permission to count every generated question as useful. A new question needs follow-through: what does it discriminate or make possible? A better question remains distinct from a completed answer to the old one.

## Composability

Can the result of one operation be used by another without losing its assumptions or guarantee? Types, units, identities, observation contracts, time windows, and uncertainty must line up.

For contracts $P_1(x)\Rightarrow Q_1(f(x))$ and $P_2(y)\Rightarrow Q_2(g(y))$, composition needs the intermediate result to meet $P_2$. A matching data format is not that argument. An adapter can supply the missing bridge, but its work belongs in the construction.

Approximate composition has an additional burden: later operations can amplify small errors. The [precise bound](08-preservation-and-transfer.md#approximate-composition) requires domains and Lipschitz assumptions; it does not apply automatically to arbitrary semantic similarity or confidence scores.

## Economy

Does the whole explanatory or operational burden earn its place across the motivating family? Count interpretation, construction, failed candidates, checking, reconstruction, learning, and maintenance. A cheap abstract solver can conceal expensive preparation.

A larger theory may reduce the total work by removing duplicated foundations. A short description may merely hide dependencies. Conversely, a reusable abstraction can be too expensive to justify for a one-off task.

For comparable outcomes and costs measured in consistent units, one useful accounting model is

$$
\Delta_N=\sum_{i=1}^N(B_i-R_i)-C_{\mathrm{setup}}-C_{\mathrm{maintenance}},
$$

where $B_i$ is the relevant alternative's whole cost and $R_i$ is the whole reuse cost on case $i$. Positive $\Delta_N$ means savings under those supplied assumptions. It is not empirical evidence that the assumed costs hold.

With constant illustrative values $B=10$, $R=6$, setup $100$, and no additional maintenance, strict savings start at $N=26$. If $B\le R$, repetition alone cannot recover positive setup cost under that model. When quality or achievable outcomes differ, a cost-only comparison is inadequate.

## Correctability

Can a false interpretation, changed premise, or lost distinction be located and revised? A representation is brittle if every contrary case is classified as impure, or if every result must be discarded because its dependencies were never retained.

Retain enough context to distinguish what has failed from what remains valid. A conditional theorem can remain true while its application no longer has support. A changed source can require re-examination without invalidating every conclusion derived from an earlier version.

Correctability can require more state and maintenance, but keeping everything is not the answer. Preserve dependencies capable of changing a consequential conclusion.

## Understand the coupling before declaring a tradeoff

| Coupling | Why it can occur | What can change it |
| --- | --- | --- |
| Richer representation and access cost | More structure may require more storage or more elaborate interfaces | Better coordinates, indexes, or selective views can simplify the needed operation |
| Broad reach and applicability work | Heterogeneous cases can need different assumptions and return maps | A genuinely common law or clearer partition of cases can reduce both difficulties |
| Stronger checking and latency | Some claims are expensive to verify | Cheap falsification, exact certificates, staged evidence, or a narrower claim can help |
| New vocabulary and existing tools | New primitives may lose familiar operations or libraries | A justified interpretation or adapter can preserve useful older constructions |
| Stable reuse and revision | Changing premises can make an old application stale | Conditional claims and explicit dependencies support selective correction |
| Broad candidate generation and review effort | A larger search can produce many misleading connections | Better questions, selection, and separation of proposal from acceptance can help |

These are conditional engineering possibilities, not universal mathematical laws. Measurements should include the whole task and a competent alternative.

## A small base-rate warning

A plausible-looking shortlist can contain mostly false candidates even with apparently favorable classification rates. Suppose a synthetic population has 10 valid and 10,000 invalid candidates. A procedure accepts 9 valid and 100 invalid ones. Its true-positive rate is 90%, its false-positive rate is 1%, but its accepted set has precision $9/109$, about 8.26%.

The general conditional-count identity is

$$
\Pr(\mathrm{valid}\mid\mathrm{accepted})
=\frac{\pi t}{\pi t+(1-\pi)f},
$$

when the denominator is positive, where $\pi$ is prevalence, $t$ the true-positive rate, and $f$ the false-positive rate on the specified population. No independent-error assumption is needed for this identity. The numbers are illustrative, not measured performance.

The lesson is to include rejected and misleading candidates in the economy of discovery rather than evaluating only successful examples.

## Do not add unlike properties into an invented score

Fertility, milliseconds, uncertainty, and explanatory reach are not interchangeable units. There is no justified universal sum of their scores. A particular use may impose hard constraints and then compare the remaining alternatives. Its preferences still need to be stated.

A technically elegant result also does not establish usefulness to someone, lawful access, adoption, or comparative value. Those questions need their own evidence. Novelty is not a substitute for benefit, and an ordinary method can be the best realization.

[Source details](SOURCES.md) · [Concept index](INDEX.md)
