# Structural lessons

[Contents](README.md) · [Previous: conceptual moves](02-conceptual-moves.md) · [Next: mathematical examples](04-mathematical-examples.md)

The lessons below interpret documented mathematical mechanisms. Each has a general methodological use, but the use outside mathematics must earn its own evidence. A suggestive resemblance does not supply the definitions or hypotheses of a theorem.

## Find a language adequate to the work

An adequate language makes the relevant relations expressible and supports the operations the subject requires. It may bring formerly separate constructions under common laws, while keeping their particular realizations available.

In *Esquisse*, Grothendieck recalls seeking a general language adequate to algebraic geometry and also describes returning to elementary surfaces and curves. That combination rules out a simple instruction to maximize generality. [E, §2, PDF p. 4] McLarty's account of cohomology explains how categorical properties and derived functors supplied common foundations for constructions previously treated separately. [M, pp. 5-11]

The test is consequential: what becomes answerable or constructible in the new language? A shorter description is not sufficient. Neither is a more imposing vocabulary. A useful language can increase the size of the representation while reducing the complexity of the argument.

A general theory can also make the place of specialized tools clearer. A common construction of cohomology does not prohibit choosing an appropriate special resolution for a calculation. Generality and concrete efficiency need not compete at every step.

## Generality must support a needed operation

One reason to enlarge a setting is that the old one repeatedly fails to contain the results of a necessary operation. Deligne describes admitting affine schemes associated with arbitrary commutative unital rings, not only geometrically comfortable ones. The enlarged category supports fiber products. [D, §1, printed pp. 12-13]

The generalization has two obligations:

1. It must admit the cases or constructions that motivated the enlargement.
2. It must preserve the old distinctions, intuitions, and results that still matter, with any additional hypotheses stated explicitly.

A setting can be too narrow because an operation breaks it. It can also be too broad because the useful conclusions no longer hold. [P, §14] State the operation, the old obstruction, the newly admitted cases, and the preservation conditions together.

Translation can precede extension. Re-expressing a familiar kind of object through its structural properties can expose which restrictions were accidental; other objects satisfying those properties may then become candidates. That is still not a proof that every desired object exists or that all older theorems transfer. The topos discussion distinguishes spaces, their categories of sheaves, and more general settings rather than treating these as interchangeable names. [P, §§12-13]

## Study the object relative to its conditions

The relative viewpoint studies a morphism $X\to S$, retaining the base as part of the situation. A change $S'\to S$ leads to the fiber product $X\times_S S'\to S'$. This unifies being defined over a base and varying in a family without declaring the bases identical. [D, §1; M, pp. 20-21]

The general lesson is to make dependence explicit. A claim about performance may depend on workload, baseline, units, resources, and the allowed kind of change. A result can be invariant under renaming while remaining conditional on a physical regime or an institutional arrangement.

Ask what remains true, what changes predictably, and what needs new evidence when the context changes. Copying a successful description into a different context is not yet transfer. Calling a context a base does not create a category or prove a base-change law.

## Understand through probes and their relations

A probe is a way of asking a structured question of an object. Generalized points of a scheme are maps into it from varying test schemes. The information includes how answers change when one probe maps to another. It is not just an unordered list of responses. [D, §1, printed p. 14; Y; G]

The methodological question is which observations and transformations reveal the distinctions needed for the inquiry. An isolated label may say much less than an object's behavior under changed conditions, exceptions, or interactions.

Two cautions are essential. First, more observations of an inadequate kind may never reveal the missing structure. Second, finitely many responses, prompts, measurements, or interviews do not acquire a reconstruction theorem by being called a profile. The full mathematical result concerns the appropriate functor, including compatibility across probes. The [generalized-point example](04-mathematical-examples.md#generalized-points-distinguish-what-field-points-miss) makes this boundary precise.

## Preserve structure the coarse picture cannot see

A quotient, aggregate, or normalization can erase exactly what the next question needs. Relevant losses include symmetries, multiple ways of identifying an object, dependence on context, and infinitesimal structure.

*Esquisse* criticizes coarse moduli for losing automorphism groups in the setting under discussion. It also advocates suitable families of base points and fundamental groupoids when a single base point obscures symmetry. [E, §2, PDF pp. 5-6] These are objections to particular losses, not a universal prohibition on quotients or simplification.

The response is not to retain every imaginable detail. Identify a difference capable of changing a consequence. Sometimes a richer representation is easier to reason with because it retains the relations that explain why special cases behave differently.

The [nilpotent example](04-mathematical-examples.md#nilpotents-and-the-limits-of-ordinary-values) shows how something invisible to ordinary field-valued observation can remain mathematically consequential.

## A specification is not its realization

A moduli problem can be expressed as a functor before a representing object has been constructed. Representability is then a mathematical question, not something granted by a good definition. Deligne stresses the need for methods of proving representability and credits Artin's further work. [D, §1, printed p. 14]

This supports a broader distinction between:

- formulating a coherent desired behavior;
- establishing that something with that behavior exists;
- constructing it effectively;
- making it tractable in the intended setting;
- showing that it answers the original question.

A specification can be an advance even when realization is open. Conversely, a definition that says to find the useful representation does not constitute a discovery method. Existence and uniqueness alone do not imply an efficient algorithm.

## Local progress requires compatible recombination

A local solution belongs to a whole only through the relevant compatibility conditions. Descent distinguishes questions about properties, morphisms, and objects; gluing requires agreement on overlaps and the hypotheses of the chosen setting. [D, §2, printed pp. 15-16]

Outside mathematics, the corresponding discipline is to inspect the assumptions where partial results meet. Two analyses may each be valid but concern different populations, time windows, standards, or resource limits. Combining their conclusions without reconciling those assumptions produces no single valid account.

A contradiction on an overlap should return to the premise that generated it. Averaging the conclusions does not repair incompatible meanings. A collection of completed reports is not automatically a synthesis, and a matching serialized type does not prove semantic compatibility.

The analogy with descent remains an analogy unless the objects, maps, covers, data, and effectiveness conditions have actually been supplied. It is useful without pretending that an organizational practice is a theorem.

## Change what counts as a local view

Sometimes the chosen observation cannot disclose the relevant property, however much more of it is collected. Étale topology changes the class of morphisms and coverings available for local geometric reasoning. Deligne presents this in relation to earlier Galois descent and Serre's work. [D, §2]

The general proposal is to choose a view because it can resolve a named uncertainty. Interaction counts may not reveal off-platform checking or work avoided. A full task episode may answer a question that a survey of preferences cannot. A different mathematical test object may reveal structure that every probe in a narrower class misses.

Views are not equally informative. They can be noisy, correlated, or incapable of identifying the property at issue. The choice requires a correspondence between what is observed and what is being claimed, as well as any necessary authority to obtain the observation.

## Seek unity through diverse realizations

A shared structure can explain why different constructions belong together without making their proofs or implementations interchangeable. Deligne's six-operation discussion describes a common formalism across cohomological settings with different proofs. His discussion of motives concerns an ambition to explain the family resemblance more deeply. [D, §§3-4]

The relevant unity preserves diversity rather than removing it. [R, Part III, opening of note 124] A common law is useful because it organizes comparison and reuse. It does not establish that all concrete instances have identical behavior, evidence, or realization costs.

This also prevents a false demand for a single canonical viewpoint. Complementary accounts may expose different structure. Their relationship can be more informative than forcing both into one flattened language.

## Generality must return to examples and comparison

A theory earns confidence through its consequences and failure boundaries. In *Esquisse*, proposed tame axioms are explicitly temporary; comparison theorems and specific examples are tests of the proposal. [E, §5, PDF pp. 24-26]

Carry a normal case through the definitions. Then carry a case that stresses them. Compare the result with another adequate account. If a distinction disappears, determine whether that loss is harmless for the declared use or defeats the construction.

A good example does more than decorate a principle. It lets the reader see what the representation enables, where it fails, and which assumption bears the load. The next chapter provides such examples without presenting finite calculations as proofs of universal discovery capability.

[Source details](SOURCES.md) · [Concept index](INDEX.md)
