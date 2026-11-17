# The operations called abstraction

[Contents](README.md) · [Previous: paradigm](01-paradigm.md) · [Next: structural lessons](03-structural-lessons.md)

"Be more abstract" is incomplete advice. Different moves change different things and preserve different consequences. This chapter gives a working vocabulary for recognizing those moves. It is an explanatory synthesis, not terminology attributed to Grothendieck.

## Keep representation, interpretation, and subject distinct

A representation can be a sentence, diagram, equation, measurement, or program. Interpretation concerns what that representation says in a context: its units, conventions, assumptions, provenance, and intended use. The subject is what the interpretation concerns. None of these is automatically recoverable from either of the others.

An abstraction is a way of exposing selected structure for some work. A correspondence relates representations or situations; it does not automatically establish identity, causality, or permission to substitute. A return interprets or realizes an abstract result in a particular situation. That return may require additional information and need not be an inverse of the abstraction.

Evidence supports a particular claim at a particular strength. A proof establishes a consequence of its assumptions. An observation bears on a model's relation to the situation. A similarity score can suggest a candidate correspondence. These are different jobs.

## A vocabulary of moves

| Move | What changes | What would justify it? | Typical loss or confusion |
| --- | --- | --- | --- |
| Re-expression | Coordinates, notation, or representational form | A relation or operation becomes accessible while the needed content remains available | Treating a shorter notation as a stronger explanation |
| Re-description | The primitives and relations used to characterize the situation | The new account distinguishes consequential cases or exposes a hidden dependency | Renaming without changing any consequence |
| Parameterization | Fixed choices become explicit parameters | One argument works over a declared family of choices | Suppressing the dependence on parameters |
| Generalization | Restrictions are weakened so more cases are admitted | A useful result survives, perhaps under explicit additional hypotheses | Assuming all old conclusions survive automatically |
| Extension | New objects, relations, or operations are admitted | A necessary construction becomes possible or the setting becomes stable under it | Admitting possibilities without showing they exist or are usable |
| Forgetting | Distinctions are deliberately removed | The retained information suffices for declared questions and uses | Losing a distinction needed by a later operation |
| Idealization | Properties are omitted or simplified to obtain a tractable model | The omission is controlled relative to the conclusion | Confusing a result in the model with adequacy of the model |
| Factorization | Roles, dependencies, or operations are separated | Independent variation becomes visible and recombination can be justified | Mistaking a decomposition into parts for a completed whole |
| Interface extraction | Only the laws or assumptions needed by an argument are retained | The argument can be reused without importing unnecessary structure | Matching notation or data types while meanings differ |
| Unification | A common organization relates different constructions | Common laws and comparison rules explain the relationship | Flattening differing realizations into one supposed object |
| Canonicalization | A representative is selected for a declared equivalence | Stable comparison is needed and the equivalence is appropriate | Treating proximity or resemblance as equivalence |
| Alignment and transport | A correspondence is established and a result is moved through it | The relevant assumptions, operations, and conclusions survive | Assuming symmetry, an inverse, or target applicability |
| Vocabulary revision | Primitives, distinctions, or construction rules change | An old obstruction becomes expressible or a useful new question emerges | Calling a new name a discovered concept |

These moves can cooperate. Translating a dynamical model into deviations from equilibrium is re-expression; stating the argument for every admissible decay parameter is parameterization; discarding the sign of a deviation is forgetting. They have different preservation obligations even if all three are casually called abstraction.

## Generality has several dimensions

A method can apply to more input formats without answering more questions. It can cover more domains while requiring stronger assumptions in each. A richer language may describe more situations without making any additional problem tractable. A wider class of allowed interventions may require retaining distinctions that were irrelevant to passive observation.

Specify which dimension is changing:

- admissible objects or cases;
- questions and outputs;
- operations or interventions;
- applicability assumptions;
- representation language;
- contexts in which the result is claimed.

There is no universal rule that more generality must reduce accuracy or increase cost. A better formulation can improve several properties together. Conversely, a shared label does not show that a wider family has been understood.

The [two-sided preservation test](03-structural-lessons.md#generality-must-support-a-needed-operation) asks what a larger setting admits and what survives inside it.

## Classifying a move differs from understanding its composition

Saying that a construction is an idealization does not identify its components. Listing its components does not show whether it is a generalization, an approximation, or an exact change of coordinates.

Classify the claim by its preservation strength, content, reach, and degree of automation. Separately inspect how interpretation, representation, abstract operation, and return fit together. A heuristic analogy and an exact transfer can share a search procedure while supporting very different conclusions.

The distinctions matter when combining work. One component may provide a prediction while the next requires a causal effect. One may prove a result for a model while the next assumes the model describes the observed situation. A common data format does not bridge that gap.

## Relations that support different kinds of reuse

| Relation | What it can support | What does not follow by itself |
| --- | --- | --- |
| Surface or statistical similarity | Retrieval, candidate generation, a question worth testing | Interchangeability or shared mechanism |
| A shared parameterized law | Reuse of a conditional method across instances | Equal trajectories or satisfied hypotheses |
| Equivalence for declared uses | Substitution for those questions and operations | Equality for all purposes or future contexts |
| Directed abstraction or simulation | Consequences preserved in the specified direction | A converse, symmetric transfer, or full reconstruction |
| Approximation | A bounded claim under a stated error model | Exact identity or safe repeated composition |
| Problem reduction | Solving an encoded task and reconstructing a solution | Cheap encoding, easy reconstruction, or automatic discovery |
| Causal correspondence | Claims about specified interventions under adequate assumptions | Causation inferred from ordinary resemblance |
| Compositional compatibility | Using one result as input to another under compatible conditions | Compatibility from matching names or types alone |

Keeping weak relations weak is useful. A promising analogy can remain a lead without pretending to be a theorem. Removing it because it lacks proof can impoverish exploration; using it as if it had proof can corrupt the conclusion.

## Discovery has several forms

Selecting an existing method and establishing its applicability can be a substantive discovery. So can composing familiar primitives into a useful representation, introducing a new distinction, or finding a better question. None requires every constituent to be historically unprecedented.

Describe what was supplied and what was found. A library containing a method is different from an input that already supplies the resolved correspondence. Retrieving an indexed answer is different from constructing the representation that makes the answer available. A newly named primitive may be definable in an older language and still improve access to a difficult operation, but that improvement needs demonstration.

These forms are not a mandatory ladder. A narrow reformulation can be sufficient. Several incompatible abstractions can remain useful for different purposes, without a single greatest common parent or a universal normal form.

[Source details](SOURCES.md) · [Concept index](INDEX.md)
