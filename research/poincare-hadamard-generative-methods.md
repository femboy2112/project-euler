# Dossier IX — Poincaré and Hadamard as generators of mathematics

## Provenance and label mapping (read this before quoting)

Supplied by the Correspondent on 2026-07-16 as a compiled research report
(`Poincare_Hadamard_Generative_Methods.docx`), converted to markdown for the repository.
**Conversion note:** the report's inline equations did not survive text extraction — where a
formula is elided the surrounding prose states its content, and the original `.docx` remains
the authority for the symbols. Its tables were reconstructed as markdown tables, cell-faithful.

Unlike dossiers I–VIII, this one was researched outside the Academy. It ships as a dossier
because it carries its own three-level evidence discipline, which maps onto the house labels:

- **Level A — explicit testimony** (Poincaré's or Hadamard's own page-cited statements)
  ≈ house **PARAPHRASE-with-citation**: page cites are present but the report mostly
  paraphrases. Do **not** upgrade to VERBATIM when quoting from this dossier; for verbatim
  Poincaré, dossier VII's primary-printing citations are the quote authority.
- **Level B — practice reconstructed from the mathematical work** ≈ house **PARAPHRASE**
  with the reconstruction flag: historically constrained, stated in modern language.
- **Level C — prescriptive synthesis** (the numbered "laws," the protocol, the diagnostics)
  carries **no historical label at all**: the laws are the report's compression, not anything
  either man wrote. Quote them as this dossier's synthesis, never as Poincaré or Hadamard.

House rule unchanged: labels never upgrade, and consequences inherit the weakest label in
their chain. Division of authority: where this dossier and dossier VII
(`incubation-poincare-hadamard.md`) overlap on the creativity account, **VII is the quote
authority**; **IX is the method authority** — the P-laws, H-laws, two-operator loop, research
protocol, and failure diagnostics that power the `poincare` and `hadamard` agents and their
lenses in `skills/the-masters/`.

---

# Poincaré and Hadamard as Generators of Mathematics

## A rigorous reconstruction of their general methods of discovery, representation, proof, and research judgment

### Research report · 16 July 2026

Governing question. What must be internalized if one wants to generate Poincaré-like or Hadamard-like mathematical moves in an unfamiliar domain, without merely imitating the theorems for which they are famous?

## Executive thesis

The transferable lesson of Henri Poincaré and Jacques Hadamard is not a bag of tricks and not the slogan “intuition first, rigor later.” It is a discipline for constituting a problem so that the right mathematics becomes visible.

Both men treated mathematical invention as a severe selection problem. Possible formulas, definitions, examples, auxiliary constructions, and deductions are effectively inexhaustible. Research therefore cannot be exhaustive search. It succeeds by changing the search space until valuable combinations are preferentially generated and useless combinations rarely arise. Poincaré called discovery discernment and selection; Hadamard adopted the same view and tried to explain how preparation, nonconscious recombination, aesthetic judgment, and later conscious work cooperate.

Their common generative architecture is:

Constitute the problem. Decide what the actual object is, what counts as the same object, what must be preserved, and what kind of answer would have mathematical force.

Choose a representation that exposes relations. Replace coordinates, explicit solutions, or isolated cases by a phase space, group action, quotient, invariant, analytic encoding, functional, boundary-value problem, or lifted problem.

Find the structural skeleton. Study periodic orbits, singularities, zeros, boundaries, equality cases, extremals, characteristic surfaces, or other low-complexity carriers of global behavior.

Generate constrained variants. Perturb, continue, generalize, factor, quotient, lift, descend, or translate across an exact analogy while tracking what persists.

Select by prospective fertility. Prefer objects that unify distant facts, compress many deductions, reveal a law, survive transformations, or expose a sharp obstruction.

Separate invention from certification. Aesthetic fit and sudden conviction rank candidates. They do not prove them. Proof, counterexample search, stability analysis, and boundary testing decide truth.

Extract relay-results. Turn each verified intermediate result into a stable new starting point, then exhaust its consequences and allow it to reorganize the original problem.

Poincaré’s distinctive strength was global architectural vision: replacing “solve the equation” with “understand the organized space of possible motions”; replacing measurements with invariants; and moving between apparently distant subjects through form-preserving analogy. Hadamard’s distinctive strength was analytic and operational control: asking whether a proposed problem is even legitimate, turning global objects into zeros and growth, differentiating with respect to functions and shapes, and moving a problem to a dimension or representation where the solution mechanism becomes available.

The deepest shared law is this:

Do not begin by asking how to derive the desired statement. Ask what re-representation would make the statement a consequence of structure rather than an accident of calculation.

The rest of this report justifies that thesis historically, reconstructs the mathematical operations behind it, separates evidence from inference, and converts the reconstruction into a reusable research protocol.

# I. Methodological safeguards

## 1. Three truth levels

This report keeps three levels distinct.

Level A — Explicit testimony. Claims Poincaré or Hadamard themselves made about reasoning, discovery, signs, beauty, proof, or research direction. Their introspections are primary evidence about their own experience, not universal laws of cognition.

Level B — Practice reconstructed from mathematical work. Repeated operations visible across their theorems: quotienting by symmetries, replacing flows by return maps, factorizing entire functions by zeros, testing well-posedness, using descent, and so on. These reconstructions are historically constrained, but they use modern language and therefore involve interpretation.

Level C — Prescriptive synthesis. The “laws” formulated here for present research. These are explicit inferences. They are not quotations and should be judged by whether they faithfully compress the evidence and produce useful, falsifiable research moves.

The distinction matters because retrospective mythology is easy. A polished proof hides search, false starts, discarded representations, and the moment when the object of study changed. Conversely, an autobiographical story can overstate the suddenness of an insight and understate years of technical formation. Hadamard was unusually careful about this: the spectacular illumination is not self-sufficient; it requires preparation and is followed by verification and development.

## 2. What “internalize the laws” means

To internalize a theorem is to remember a result. To internalize a method is to recognize when a family of operations is admissible and potentially high-leverage. A generative law must therefore specify at least four things:

Trigger: what configuration or failure should make the law come to mind;

Operation: what transformation to perform;

Preservation obligation: what must remain equivalent, invariant, or recoverable;

Success signal: what observable result would show that the transformation improved the problem.

For example, “use topology” is not a method. A generative version is:

When coordinate formulas vary wildly while qualitative incidence or connectivity appears stable, define an equivalence relation that forgets metric detail, construct invariants under that equivalence, and test whether the target distinction factors through those invariants. The move succeeds only if the invariant separates cases relevant to the theorem or turns evolution into a finite or algebraic constraint.

This form can generate specifics on demand.

## 3. A formal vocabulary for research transformations

It is useful to model a research problem as a tuple

where:

 is the candidate object space;

 is the admissible data or hypotheses;

 is the equivalence relation declaring which descriptions count as the same object;

 is a family of transformations or symmetries;

 is the target claim;

 is the set of observables available for proof or computation.

A representation  is useful when it improves at least one of the following without losing the target:

visibility: relevant relations become explicit;

compressibility: many cases share one description;

stability: small changes have controllable effects;

decidability: an obstruction or certificate becomes checkable;

transportability: a theorem from another domain becomes applicable.

The preservation obligation is crucial. A heuristic representation may merely correlate with the target. A proof-bearing representation needs one of:

an equivalence ;

a sound implication ;

a contrapositive obstruction ;

a lift showing every relevant object in the reduced space comes from an admissible original object.

Poincaré and Hadamard were extraordinarily powerful partly because they could invent representations. Their occasional errors also show why the preservation obligation cannot be implicit.

# II. Poincaré’s generative method

## 4. The central act: select relations, not facts

Poincaré begins from scarcity of attention. Nature and mathematics contain more facts and possible combinations than a mind can examine. Method is therefore selection. In Science and Method, he measures the importance of a fact by its “return”: how much future thought it saves, how many other facts it predicts, and whether it reveals a general law. A lone calculation has little research value unless it exposes the resemblance and difference between a wider class of problems. A valuable result does not merely add one fact; it reorganizes old facts by showing their relation (Poincaré 1914, pp. 15–31).

This yields a first exact reconstruction.

### Poincaré Law P1 — Maximize structural return

Trigger: You can prove or compute many isolated statements, but they do not constrain one another.

Operation: Search for a common relation, invariant, transformation law, or classification parameter under which the statements become instances.

Preservation obligation: The abstraction must recover the distinctions needed by the original problems. Compression obtained by erasing the target is worthless.

Success signal: One new statement predicts several old results, identifies the possible generalizations, and shows which calculations are unnecessary.

This is not generic “generalize your theorem.” Poincaré’s standard is prospective force. A generalization is valuable when it changes what can be foreseen.

## 5. Research begins at nodal points

Poincaré distinguishes ordinary examples from facts situated at “nodal points” where several domains meet. Such facts have high return because information can propagate in multiple directions. His model scientist begins with regular facts to establish a rule, then deliberately seeks extreme exceptions where the rule is most likely to fail. Apparent discrepancies are especially valuable when they conceal similarity of form (Poincaré 1914, pp. 18–21 and 284–287).

The resulting search policy has two phases:

Regularity phase: establish the stable pattern on clean, representative cases.

Discrimination phase: move to boundaries, extremes, singularities, and exceptions that distinguish competing explanations.

### Poincaré Law P2 — Sample for discrimination, not coverage

Trigger: More examples keep confirming what is already believed.

Operation: Identify two or more plausible structural hypotheses and search where their predictions diverge most strongly.

Preservation obligation: The chosen stress cases must remain within the actual hypothesis class or explicitly test its boundary.

Success signal: A small number of cases eliminates an entire explanatory frame, exposes a missing variable, or forces a sharper invariant.

This anticipates a modern experimental-design principle: evidence is valuable in proportion to the hypotheses it discriminates, not the number of data points it adds.

## 6. Replace explicit solution by qualitative organization

Poincaré’s qualitative theory of differential equations is the clearest embodiment of his method. The inherited question was often: find a formula for the solution. Poincaré asked instead: what can be known about the total organization of solutions even when no formula exists?

For a differential equation

the object is not only a function . It is the flow  on a phase space: fixed points, periodic orbits, invariant manifolds, recurrence, limiting behavior, and the partition of initial conditions by qualitative fate. This reconstitution changes the attainable theorems. One can classify singular points, study limit cycles, identify separatrices, and prove qualitative impossibility without integrating the equation.

The key move is ontological: the “solution” becomes an organized space of motions. Formulas are coordinates on that object, not the object itself.

### Poincaré Law P3 — Promote the solution set to the object

Trigger: Individual trajectories or instances are hard to compute, unstable, or uninformative.

Operation: Construct the space of all admissible states or solutions and study its decomposition into invariant classes.

Preservation obligation: Prove how the target property of an individual solution is encoded by its class, orbit, stratum, or invariant set.

Success signal: Global restrictions become provable without pointwise solution, or the impossibility of a closed form becomes irrelevant.

This law applies far beyond differential equations. In number theory it suggests studying a space of orbits, encodings, or local realizations rather than a single integer trajectory. In combinatorics it suggests the moduli space of configurations. In proof search it suggests the geometry of all admissible witnesses.

## 7. Reduce continuous complexity to a return operator

For a flow, Poincaré introduced what is now called a Poincaré section and return map. Choose a transversal section . For , let  be the next return time and define

The continuous-time problem is converted into iteration of a lower-dimensional map. Periodic orbits become fixed or periodic points of ; stability becomes the behavior of derivatives of iterates; invariant manifolds become geometrically visible; recurrence becomes repeated return. The map is usually not explicitly computable, but its geometry and preservation laws still constrain it. Holmes emphasizes that this reduction captures crucial information even when the original equations cannot be integrated (Holmes 1990, pp. 144–150).

### Poincaré Law P4 — Search for a faithful event map

Trigger: The system evolves continuously or through a long chain, and most intermediate states are redundant.

Operation: Choose a recurrent event, boundary crossing, normalization, or canonical representative and record only successive returns.

Preservation obligation: Specify which properties of the original evolution are conjugate to, implied by, or reconstructible from the event map.

Success signal: Dimension or temporal complexity drops while periodicity, stability, recurrence, or obstruction becomes algebraic or geometric.

The subtlety is in the word faithful. Sampling every thousandth iterate is not automatically a Poincaré reduction. The section must be structurally tied to the dynamics, and return must be defined on the relevant domain.

## 8. Group action, fundamental domain, quotient

Across Poincaré’s work on automorphic functions, non-Euclidean geometry, and topology, a recurring architecture is:

A complicated infinite pattern becomes a fundamental domain plus gluing rules. An automorphic function is characterized by invariance under a transformation group. A surface can be represented by a polygon whose sides are identified. Loops and substitutions yield algebraic data. Modern expositions of Analysis Situs show how Poincaré’s work on Fuchsian groups supplied a guiding structure for the fundamental group and higher-dimensional topology (Poincaré, Papers on Topology, translator’s introduction, pp. 3–12; Bartocci, “Analogy and Invention,” pp. 9–13).

This is more than using symmetry to simplify a calculation. It divides description into:

coordinate redundancy, removed by the quotient;

local structure, stored in a fundamental piece;

global structure, stored in the gluing or group relations.

### Poincaré Law P5 — Separate local content from global gluing

Trigger: The same local pattern repeats, yet globally different objects occur.

Operation: Identify the transformation group generating repetitions, choose a fundamental domain, and encode global difference in boundary identifications or relations.

Preservation obligation: Show that the quotient or gluing data classify the equivalence relevant to the target, or identify what information they fail to retain.

Success signal: An infinite object is represented finitely, and global distinctions become algebraic.

This law generates fundamental domains, covering spaces, automata quotients, orbit spaces, residue-class models, and renormalization cells. It also warns against a common failure: local rules do not determine global structure unless the gluing is included.

## 9. Invent invariants when classification stalls

Poincaré did not treat invariants as a fixed menu. If existing invariants failed to distinguish objects, that failure was evidence that a new invariant was needed. Betti numbers did not classify three-manifolds, so he introduced a stronger noncommutative object, the fundamental group. The move was guided by analogy with Fuchsian group constructions, not by arbitrary symbol manufacture (Bartocci, pp. 9–13).

Let  act on . An invariant is a map  such that

But invariance alone is cheap: a constant map is invariant. A research invariant needs discriminating power. It should separate at least some inequivalent objects, constrain evolution, or obstruct a target configuration.

### Poincaré Law P6 — Let collisions design the next invariant

Trigger: Two objects agree on every current statistic but behave differently under the target property.

Operation: Examine the smallest witness of their difference, then construct a quantity or algebraic object preserved by the allowed equivalences but sensitive to that witness.

Preservation obligation: Prove invariance under every allowed move; test nontriviality on the collision pair.

Success signal: The new invariant separates the counterexample, explains why the old invariants collided, and scales beyond the motivating case.

This is a disciplined route to a new mathematical object: not “invent a clever quantity,” but “extract the conserved content of the minimal unresolved distinction.”

## 10. Perturb the solvable model and ask what survives

Poincaré repeatedly began with an integrable or otherwise tractable system, introduced a perturbation, and examined persistence. The central question is not merely whether a power series can be written, but which structures are stable when omitted terms return. In the three-body problem, stable and unstable manifolds that coincide in an integrable truncation can split and intersect transversely after perturbation. The resulting homoclinic tangle is not noise around the old solution; it is a new global structure obstructing additional analytic integrals (Holmes 1990, pp. 148–158).

This yields a hierarchy:

solve or classify a canonical model ;

introduce ;

identify invariant structures of ;

determine which persist, deform, split, or disappear;

treat the failure of persistence as positive information.

### Poincaré Law P7 — Make stability a theorem, not an assumption

Trigger: A simplified model gives a beautiful picture, and the argument informally assumes small neglected terms cannot change it.

Operation: Restore perturbations one class at a time and study structural persistence of the exact objects on which the proof depends.

Preservation obligation: Quantify the topology, norm, or equivalence in which “small” and “same qualitative structure” are meant.

Success signal: Either a persistence theorem validates the reduction, or the first failure identifies the true nonlinear mechanism.

This law is one of the strongest protections against false proofs built on accurate-looking asymptotics.

## 11. Singular, periodic, and extremal objects form the skeleton

Poincaré’s qualitative work privileges objects that organize nearby behavior:

fixed points and singularities;

periodic orbits;

stable and unstable manifolds;

separatrices and homoclinic intersections;

recurrent sets;

topological cycles and boundaries.

These are small subsets of phase space, but they control global decomposition. The research heuristic is not “special cases are easier.” It is “some special cases carry the incidence relations of the whole.”

### Poincaré Law P8 — Find the organizing minority

Trigger: The generic object space is too large for direct classification.

Operation: Identify configurations with enhanced recurrence, symmetry, singularity, extremality, or boundary status; determine how general objects attach to or move around them.

Preservation obligation: Prove the organizing relation—basin, foliation, deformation, index formula, density, or obstruction—rather than extrapolating from visual salience.

Success signal: A low-dimensional or exceptional subset partitions the ambient space or controls allowed transitions.

## 12. Analogy is transport of form, not resemblance of appearance

Poincaré’s highest-value discoveries often joined distant domains. But he explicitly warns that merely combining incongruous things mostly produces nonsense. Fruitful analogy identifies parallel relations or operations. In his words, analogous names should be given when things differ in matter but resemble one another in form and have parallel properties (Poincaré 1914, pp. 130–133).

A rigorous analogy should be represented as a dictionary:

| Source structure | Target structure | Obligation |
|---|---|---|
| Objects | Objects | Define the translation |
| Allowed maps | Allowed maps | Show composition is respected |
| Equivalence | Equivalence | Show equivalent sources map to equivalent targets |
| Invariants | Candidate invariants | Prove preservation or state failure |
| Obstruction | Target obstruction | Prove transfer direction |

### Poincaré Law P9 — Transfer a relation diagram

Trigger: Two domains display the same pattern of composition, invariance, boundary, or recurrence despite dissimilar objects.

Operation: Write an explicit object-map and operation-map. Determine which commutative diagrams or identities survive.

Preservation obligation: No theorem transfers until its hypotheses and conclusion are translated and the required diagram commutes.

Success signal: The target acquires a natural definition or invariant that was forced by the source relations, not merely suggested by vocabulary.

## 13. Mathematical beauty as a trained ranking functional

Poincaré’s “beauty” is often romanticized. His text gives it operational content. A beautiful mathematical combination exhibits harmony, symmetry, happy adjustment, unity of whole and parts, unexpected conjunction of previously separate objects, or striking simplicity relative to the problem. These features are valuable because they increase comprehension, expose analogy, and suggest a law. Beauty is therefore connected to economy of thought and future reuse (Poincaré 1914, pp. 29–31 and 58–59).

We can reconstruct a non-numerical scoring functional for a candidate :

This is a search heuristic, not a truth measure. Poincaré explicitly reports that a compelling illumination can fail verification, often because the false idea would have been elegant if true.

### Poincaré Law P10 — Beauty proposes; proof disposes

Trigger: Several technically possible constructions compete.

Operation: Rank them by structural compression, unification, invariance, and generativity.

Preservation obligation: Do not convert the ranking score into evidential confidence. Independently verify every proof-bearing step.

Success signal: The selected candidate yields shorter explanations and new consequences and survives adversarial proof.

## 14. The architecture of understanding

Poincaré distinguishes following each syllogism from grasping a proof. A long proof is not a heap of valid local steps. It is an ordered whole. Error can arise when the meaning of an intermediate proposition shifts between its introduction and reuse. The mathematician’s advantage is therefore not necessarily exceptional memory; it is a grasp of the “general trend” that gives each step its place (Poincaré 1914, pp. 46–50).

This has a rigorous modern reading. Let a proof be a dependency graph, not merely a line:

nodes are definitions, lemmas, constructions, and claims;

directed edges record exact dependency;

interfaces specify the meaning and type of each intermediate object;

global invariants state what remains unchanged along a chain.

### Poincaré Law P11 — Audit meaning across proof interfaces

Trigger: Every local inference appears valid, yet the argument feels opaque or fragile.

Operation: Draw the dependency graph and restate each intermediate object at every reuse. Check that no quantifier, domain, topology, branch, or equivalence relation has drifted.

Preservation obligation: Each edge must preserve both formal truth and intended semantic content.

Success signal: The proof can be reconstructed from its architecture; removing any lemma has an intelligible structural effect.

## 15. Definitions are engineered instruments

For Poincaré, a definition must be consistent, but consistency is not sufficient. A worthwhile definition should answer why its components were assembled, what need it fills, what reasoning it shortens, which rough examples motivated it, and how it differs from nearby objects. The definition should often be prepared by examples before its final exact statement (Poincaré 1914, pp. 130–133).

### Poincaré Law P12 — Make definitions earn their cost

Trigger: A new object has been named, but its role is unclear.

Operation: Supply its construction, nearest nonexamples, invariance class, characteristic use, and the theorem it compresses.

Preservation obligation: Prove nonemptiness or consistency and show that each clause is necessary for the intended discrimination.

Success signal: The definition becomes a reusable interface: it shortens arguments and makes a previously hidden relation stateable.

## 16. Conscious preparation, incubation, illumination, verification

Poincaré’s famous account of mathematical creation is often reduced to sudden insight. His actual sequence is stricter:

voluntary work activates a deliberately selected family of ideas;

unsuccessful combinations narrow and structure the search;

a break permits further recombination outside focal awareness;

a promising combination enters awareness with an aesthetic sense of fit;

conscious work derives consequences, orders the result, and verifies it.

He insists that inspiration is neither ready-made calculation nor proof. Nonconscious work provides points of departure. Detailed calculation and certification demand conscious attention. He also explicitly labels his psychological model hypothetical (Poincaré 1914, pp. 51–63).

The transferable law is not “take breaks and answers will arrive.” It is:

### Poincaré Law P13 — Seed incubation with a structured impasse

Trigger: Focused search has explored the obvious local moves and begun to repeat itself.

Operation: Before disengaging, state the target, active constraints, failed representations, and promising elements. Then switch to a genuinely different activity or problem.

Preservation obligation: On return, treat every illumination as an unverified candidate and reconstruct the missing derivation.

Success signal: The return produces a new relation or representation, not merely renewed effort on the same path.

Modern evidence supports a modest incubation effect whose magnitude depends on task type, preparation, and the intervening activity; it does not establish Poincaré’s particular mechanism (Sio & Ormerod 2009).

## 17. Error repair is a discovery operator

Poincaré’s history contains a decisive warning and a decisive opportunity. His prize memoir on the three-body problem contained a serious error concerning invariant manifolds. The correction did not simply patch the original picture; it exposed the transverse intersections and homoclinic structure that helped found modern dynamical-systems theory. The Institut Mittag-Leffler’s historical account explicitly links the correction to the tangled consequences of homoclinic points (Institut Mittag-Leffler, “Prize Competition”; see also Barrow-Green’s historical study).

His topology supplies a parallel case. Analysis Situs contained gaps and an incorrect early conjecture; criticism and successive supplements sharpened definitions, added torsion, repaired duality arguments, and produced the correct form of the Poincaré conjecture (Poincaré, Papers on Topology, pp. 8–12).

### Poincaré Law P14 — When a proof fails, preserve the counter-geometry

Trigger: A central equivalence, coincidence, or persistence claim fails.

Operation: Do not ask only how to restore the conclusion. Characterize the exact mode of failure as a new object: splitting, monodromy, torsion, instability, nonuniqueness, or obstruction.

Preservation obligation: Recheck all downstream claims under the corrected structure.

Success signal: The failure mechanism predicts new phenomena or defines the invariant the original proof lacked.

## 18. Poincaré’s method in one sentence

Replace exhaustive calculation by a global representation whose invariants, return structure, and exceptional skeleton make the high-return relations visible; use analogy and beauty to generate candidates, then force every candidate through proof, perturbation, and counterexample.

# III. Hadamard’s generative method

## 19. Hadamard does not merely inherit Poincaré

Hadamard’s Psychology of Invention in the Mathematical Field explicitly begins from Poincaré’s lecture, but Hadamard adds several critical elements:

a sharper role for conscious preparation;

a detailed account of later conscious work;

“relay-results” as intermediate platforms;

synthesis and nonverbal schemas;

the role of personal signs;

dangers of attention that is too narrow or too scattered;

the choice of research direction;

extensive comparison with testimony from other mathematicians.

His mathematical work supplies an even more important correction to the popular psychological portrait. Hadamard’s characteristic moves are not dreamy. They are technically exact transformations of the problem: discrete data to analytic functions, zeros to products, shapes to functionals, high dimension to low dimension, physical propagation to characteristic geometry, and informal solvability to existence–uniqueness–stability.

## 20. Begin by asking whether the problem is legitimate

Hadamard’s most durable methodological contribution is the concept of a well-posed problem. A problem with data  and solution  is well posed when:

a solution exists;

it is unique;

the solution depends continuously on the data.

The third condition means that small observational or numerical errors do not cause arbitrarily large solution errors in the chosen topologies. Formally, the solution operator  should be continuous. The exact spaces and norms matter.

This changes the order of research. Before deriving a formula, ask whether the requested output is determined and stable. A formula for an unstable inverse is not a solution in any operational sense.

### Hadamard Law H1 — Audit existence, uniqueness, and stability first

Trigger: A problem asks to reconstruct, predict, or infer an object from partial data.

Operation: Define the data space, solution space, topology or norm, and solution map. Test existence, uniqueness, and continuous dependence separately.

Preservation obligation: Do not hide instability by changing norms after seeing the counterexample. Justify the topology from the problem’s intended observables.

Success signal: Either the problem is certified well posed, or its precise failure suggests regularization, weaker recovery, additional data, or a different target.

This is not limited to PDE. It applies to inverse problems, statistical identification, computational conjecture, proof reconstruction, and mathematical definitions. A research question can be ill posed when several inequivalent objects produce the same observables.

## 21. Translate discrete structure into analytic structure

Hadamard’s work on entire functions and the prime number theorem exemplifies a general analytic strategy:

encode discrete or arithmetic information in a complex-analytic object;

use analytic continuation to enlarge the domain of control;

turn zeros and singularities into the decisive structural data;

obtain asymptotics for the original discrete problem by inversion or contour arguments.

For primes, the Euler product relates  to multiplicative structure; the logarithmic derivative packages prime powers; the absence of zeros on  removes the obstruction to the desired asymptotic. Hadamard’s earlier theory of entire functions of finite order helped provide the analytic tools. Historical accounts emphasize this pipeline and the role of the zero-free boundary line (Apostol, “A Centennial History of the Prime Number Theorem”; Cartwright 1965, pp. 732–734).

### Hadamard Law H2 — Encode irregular data in a rigid ambient category

Trigger: The original objects are discrete, locally erratic, or combinatorially unstructured.

Operation: Construct a generating function, transform, determinant, zeta function, kernel, or other analytic object whose algebra records the original data.

Preservation obligation: Prove the coefficient, zero, pole, trace, or inversion formula that returns the original information.

Success signal: A global analytic constraint—growth, continuation, zero-free region, convexity, positivity—implies a nontrivial theorem about the original objects.

The danger is ornamental encoding: writing a generating function that stores the data but adds no rigidity. The ambient category must contribute theorems unavailable in the original representation.

## 22. Reconstruct the whole from zeros, singularities, and growth

Hadamard factorization states, roughly, that an entire function of finite order can be represented by its zeros through a canonical product, multiplied by an exponential of a polynomial:

The exact theorem controls the genus, convergence factors, and degree of  using growth. Conceptually, the function’s global identity is decomposed into:

a zero at the origin;

its nonzero zero set with multiplicities;

a residual exponential factor constrained by growth.

This is a model of structural reconstruction: find the singular skeleton and the minimal residual freedom.

### Hadamard Law H3 — Decompose into skeleton plus controlled remainder

Trigger: A global object is difficult to handle directly, but a distinguished set of events—zeros, poles, jumps, critical points, prime factors, or singularities—is accessible.

Operation: Seek a representation in which those events become factors and all remaining ambiguity lies in a low-complexity correction term.

Preservation obligation: Prove convergence and completeness: the skeleton plus remainder must determine the original object in the claimed class.

Success signal: Global questions reduce to distribution of the skeleton and bounds on the residual term.

This law recurs in spectral theory, algebraic factorization, dynamical zeta functions, and decomposition of measures or representations.

## 23. Growth is not a nuisance; it is classification data

Hadamard’s theory of entire functions classifies objects not only by zeros but by order and growth. Growth controls which products converge and how large the residual polynomial may be. This suggests a general method: when exact values are uncontrollable, organize objects by rates.

Given a size functional , define a growth scale such as

The point is not this particular definition; it is the move from pointwise data to an asymptotic class that constrains representation.

### Hadamard Law H4 — Use growth to bound representational freedom

Trigger: Many objects share the same local or singular data.

Operation: Add a global growth, regularity, energy, or complexity class.

Preservation obligation: Prove that the chosen class is stable under the operations used and sharp enough to control the remainder.

Success signal: Previously nonunique reconstruction becomes finite-dimensional or unique.

## 24. Extremal principles expose exact equality structure

Hadamard’s determinant inequality is an exemplary extremal move. If the row vectors of a matrix are , the determinant is the volume of the parallelepiped they span, so

with equality exactly when the rows are mutually orthogonal. What looks like an algebraic bound becomes a geometric volume statement; the equality case reveals the optimal structure.

### Hadamard Law H5 — Ask what geometry saturates the bound

Trigger: The problem asks for a maximum, minimum, sharp inequality, or best constant.

Operation: Reinterpret the objective geometrically or variationally; identify local competing contributions; derive the bound and solve the equality conditions.

Preservation obligation: Prove both inequality and characterization of equality. A sharp number without its extremizers gives less structural information.

Success signal: The optimal configuration has a recognizable orthogonality, symmetry, independence, or concentration law that generalizes.

This is a powerful generator because equality conditions often define the previously missing object.

## 25. Promote finite variables to functions and shapes

Hadamard viewed the calculus of variations as an opening chapter of functional calculus. Instead of differentiating a function of finitely many coordinates, vary a function, curve, or domain. For a functional , consider

For shape dependence, vary the boundary and measure the induced change in a Green function or other solution. Cartwright’s obituary records Hadamard’s development of functional derivatives and his explicit recognition that functional continua require new analytic machinery because ordinary geometric intuition gives no simple picture (Cartwright 1965, pp. 735–737).

### Hadamard Law H6 — Differentiate the object class

Trigger: The unknown is itself a function, path, domain, measure, or operator, and finite-coordinate perturbations obscure the true degrees of freedom.

Operation: Define admissible variations, compute first and second variations, and identify stationarity, integrability, and boundary terms.

Preservation obligation: Specify the function space, regularity, boundary conditions, and topology. Formal variation without admissibility is not proof.

Success signal: The infinite-dimensional problem acquires a local differential calculus, and necessary or sufficient conditions become explicit.

## 26. Treat singularities as carriers of propagation

Hadamard’s wave and PDE work begins from physical discontinuity rather than smoothing it away. In wave propagation, a front separates regions already affected by a disturbance from regions not yet affected. Singular surfaces therefore encode causality, characteristic geometry, and compatibility conditions. Cartwright emphasizes that analytic or continuous approximations could misrepresent the physics and that Hadamard built a general classification of singular surfaces and compatibility levels (Cartwright 1965, pp. 737–741).

### Hadamard Law H7 — Preserve the singular support

Trigger: Approximation makes a problem smoother but appears to erase fronts, jumps, defects, or causal boundaries.

Operation: Identify the singular set and derive its evolution or compatibility law directly. Choose generalized objects if ordinary functions cannot retain it.

Preservation obligation: Show that approximation converges in a topology that preserves the target singular information, or explicitly track what is lost.

Success signal: Propagation speed, causal domain, shock structure, or obstruction is read from the singular geometry.

This is a general warning for computational research: a smoothed statistic can converge while the theorem-relevant exceptional set disappears.

## 27. Fundamental solutions turn operators into kernels

Hadamard sought elementary or fundamental solutions and used Green-type identities to express general solutions through boundary and source data. The method shifts attention from solving  separately for each  to constructing a kernel  with

Once the response to a point source is understood, superposition and integral identities organize the general problem. Singularities of the kernel are not defects; they are the precise local response needed to reconstruct solutions.

### Hadamard Law H8 — Solve the response to an atomic source

Trigger: A linear operator must be inverted for many inputs.

Operation: Find the response to a point mass, basis vector, irreducible representation, or other atomic input; then assemble general inputs by superposition or convolution.

Preservation obligation: Control singularities, boundary terms, and the function/distribution space in which inversion holds.

Success signal: One universal kernel replaces a family of unrelated solution procedures.

## 28. Change dimension to change difficulty

Hadamard’s method of descent solves a lower-dimensional PDE by embedding it in a higher-dimensional problem whose solution is known, often by taking the higher-dimensional solution to be independent of an extra coordinate. In schematic form, if  solves  and is independent of , then

solves the descended equation when the operators are compatible. Cartwright identifies the systematic use of descent as one of Hadamard’s principal PDE contributions (Cartwright 1965, pp. 739–742).

### Hadamard Law H9 — Lift to a category with stronger tools, then descend

Trigger: The native dimension or category lacks a formula, symmetry, factorization, or classification theorem.

Operation: Embed the problem in a richer space where the desired mechanism exists; impose a constraint or symmetry; restrict, average, trace, or quotient back.

Preservation obligation: Prove that the lift exists, that the higher-dimensional solution respects the constraint, and that descent returns every required property.

Success signal: The hard native problem becomes a special case of a tractable ambient problem.

The lift must add structure, not only coordinates. Otherwise it merely enlarges the problem.

## 29. Exact analogy and direct generalization

Hadamard repeatedly sought the appropriate generalization of a classical identity to a broader operator or variable-coefficient setting. His PDE work generalized Green formulas and elementary solutions from familiar elliptic cases to hyperbolic equations with variable coefficients. The method was not formal substitution. He identified the functional role of each component, then rebuilt that role when singularities changed character.

### Hadamard Law H10 — Generalize the role, not the formula

Trigger: A classical formula works in a canonical case but breaks under changed coefficients, dimension, geometry, or regularity.

Operation: Decompose the formula into jobs: inversion, boundary transfer, conservation, normalization, causality. Reconstruct each job in the new category.

Preservation obligation: Prove that the generalized object satisfies the defining identity, not merely that its syntax resembles the original.

Success signal: The new formula reduces to the classical one in the old regime and continues to perform the same structural function.

## 30. Preparation is search-space conditioning

Hadamard rejects the idea that rest alone produces solutions. Preparation activates and directs the elements that later recombine. In Poincaré’s metaphor, deliberate work sets selected “atoms” in motion. Hadamard compares effective preparation to aiming with an appropriate spread: attention that is too narrow misses adjacent connections; attention that is too diffuse fails to constrain search. He advises researchers not to confine themselves to one chapter of science and to leave a stuck problem provisionally with an intention to return (Hadamard 1945, pp. 43–56).

### Hadamard Law H11 — Control the bandwidth of preparation

Trigger: Search is either repetitive within one formalism or scattered across unrelated possibilities.

Operation: Define a core constraint set and an adjacent exploration band. Work deeply enough to create an impasse, while deliberately loading two or three structurally related external methods.

Preservation obligation: Record why each external method is adjacent—shared operator, invariant, asymptotic regime, or categorical structure.

Success signal: Incubation or later work combines target constraints with a genuinely external operation, without degenerating into free association.

## 31. Synthesis precedes linear exposition

Hadamard describes understanding as the ability to hold all elements of an argument together in a simultaneous schema. His own mental image could be vague: not a readable formula, but a ribbon darker where dominant terms lie. The image did not encode each logical link; it encoded how the links fit. He insists that such schemas remain vague enough not to deceive by false precision. Words may be absent during discovery and enter later for communication or to stabilize an intermediate result (Hadamard 1945, pp. 76–103).

This distinction is especially important:

synthetic schema: global dependency, salience, direction, expected scale;

analytic proof: exact definitions and local implications;

exposition: a linear path optimized for another mind.

### Hadamard Law H12 — Maintain a global schema and a local ledger

Trigger: Formal derivation grows but research direction becomes unclear, or a vivid global intuition lacks exact content.

Operation: Keep two synchronized artifacts: a one-page structural map and a line-by-line proof ledger.

Preservation obligation: Every arrow in the structural map must eventually point to a proved lemma or be labeled conjectural; every ledger step must state its role in the map.

Success signal: The schema guides search without substituting for proof, and proof development updates the schema when intuition was wrong.

## 32. Signs are tools, not the substance of thought

Hadamard’s survey found wide variation in whether mathematicians think in words, images, algebraic signs, or motor patterns. He treats signs as supports and labels. Creative thought often uses flexible personal signs, including ad hoc ones for a single problem; conventional language becomes more important during formulation and communication. The methodological law is representation pluralism, not a claim that all good mathematics is nonverbal.

### Hadamard Law H13 — Use the cheapest sign system that preserves structure

Trigger: Standard notation imposes excessive working-memory cost or forces premature precision.

Operation: Introduce temporary spatial, graphical, rhythmic, or symbolic markers for roles and relations; later translate them into public definitions.

Preservation obligation: Maintain a dictionary. Personal signs must not silently change meaning, and public proof must not depend on private imagery.

Success signal: The working representation increases simultaneous grasp and can be losslessly formalized when needed.

## 33. Relay-results are the units of cumulative research

Hadamard calls verified intermediate results “relay-results.” They stabilize progress, become new starting points, and should be used systematically and exhaustively. A relay-result may require incubation before it becomes integrated into the larger synthetic scheme. The term captures a neglected fact: a lemma is not merely a step toward a fixed theorem. Once proved, it can change the route and the destination (Hadamard 1945, pp. 59–83).

### Hadamard Law H14 — Promote every nontrivial lemma to an object

Trigger: An intermediate result has been proved and the work immediately rushes past it.

Operation: State its exact hypotheses, equality cases, converses, stability, functoriality, computational witnesses, and adjacent applications.

Preservation obligation: Separate proved consequences from conjectural extrapolation.

Success signal: The lemma either closes multiple branches or reveals a stronger reformulation of the main problem.

## 34. Narrow attention creates invisible consequences

Hadamard gives unusually candid examples of missing immediate consequences of his own formulas because attention was fixed on a famous target. He also describes missing conditions under which an extremum was reached—conditions that pointed toward later major developments. The methodological lesson is that discovery failure can occur after the decisive formula is already present (Hadamard 1945, pp. 49–55).

### Hadamard Law H15 — Re-read results without the original question

Trigger: A formula or lemma was derived for a specific purpose.

Operation: Temporarily remove the target. Ask what the result implies under every natural specialization, limit, extremal condition, dual interpretation, and equality case.

Preservation obligation: Do not infer importance from novelty alone; prove each consequence and compare with known results.

Success signal: An “obvious in retrospect” consequence appears that the target-focused search suppressed.

## 35. Choose research by fertile beauty, then test tractability

Hadamard agrees with Poincaré that scientific taste guides subject selection. The expected applications of a genuinely beautiful structure may be unknown, but fruitfulness often appears later. Yet his practice adds a tractability constraint: one should identify intermediate questions that can become relay-results.

### Hadamard Law H16 — Select a direction with both depth and handles

Trigger: Several important problems compete for attention.

Operation: Rank each by structural centrality, connection to other domains, availability of discriminating subproblems, and the chance of producing reusable intermediate results even without full solution.

Preservation obligation: Do not confuse prestige or difficulty with structural centrality.

Success signal: Failure to solve the headline problem still leaves a durable theory, obstruction, method, or classification.

## 36. Hadamard’s method in one sentence

First decide whether the problem and its data define a stable mathematical task; then translate it into a rigid analytic, variational, kernel, or higher-dimensional representation, build and digest relay-results, and alternate synthetic global control with exact verification until the representation yields the theorem.

# IV. Comparison: one research machine, two control systems

## 37. Shared core

Poincaré and Hadamard agree on the following substantive points:

| Shared principle | Poincaré’s emphasis | Hadamard’s emphasis |
|---|---|---|
| Discovery is selection | Useful combinations are a tiny minority | Preparation and aesthetic judgment condition selection |
| Global understanding exceeds local logic | The order and architecture of proof | Synthesis and simultaneous schema |
| Beauty is epistemically useful but fallible | Harmony predicts laws and generalizations | Scientific taste guides combinations and research direction |
| Unconscious work is prepared | Voluntary effort activates relevant elements | Preparation is indispensable and direction-setting |
| Verification is independent | Conviction can be false | Later conscious work verifies and “precises” |
| Breadth enables invention | Distant domains yield fruitful relations | Avoid confinement to one chapter of science |
| Definitions and signs are engineered | Names expose form and analogy | Personal signs support synthesis; public signs stabilize relay-results |
| Failure is informative | Exceptions and broken persistence reveal structure | Missed consequences diagnose over-narrow attention |

Neither man endorses unconstrained intuition. Their “intuition” is trained sensitivity to mathematical order after extensive preparation.

## 38. The difference in mathematical temperament

### Poincaré: global geometry of possibilities

Poincaré characteristically asks:

What is the space of all possible behaviors?

What equivalence forgets irrelevant detail?

What invariant survives the allowed transformations?

What periodic, singular, or recurrent structures organize the rest?

Can a flow be compressed to a return map?

What remains under perturbation?

Which distant domain has the same relational form?

His characteristic danger is fertile overreach: the global picture can outrun exact definitions or proof. His best corrective is to preserve the failed geometry and let counterexamples design the next invariant.

### Hadamard: analytic control of determination and transfer

Hadamard characteristically asks:

Is this problem well posed in the stated data and topology?

What analytic object encodes the data?

Can the whole be reconstructed from zeros, singularities, or an atomic response?

What growth class controls the remainder?

What equality structure saturates the bound?

Can I differentiate with respect to the function or domain?

Can I lift to a friendlier dimension and descend?

What verified intermediate result should become the next platform?

His characteristic danger is attention capture: a powerful formula can be viewed only through the target that produced it, hiding immediate consequences. His corrective is systematic re-reading and relay-result exploitation.

## 39. The complementary pair

The combined method alternates two operators.

Poincaré operator : structural reconstitution

It asks: What is the correct global object?

Hadamard operator : analytic legitimization

It asks: What exact structure determines that object and makes inference stable?

Applied iteratively:

The Poincaré step prevents local technical work from being trapped in the wrong ontology. The Hadamard step prevents a beautiful ontology from floating free of determinacy, analytic control, and proof.

# V. The extracted generative laws

## 40. Twenty laws worth internalizing

The following are the highest-level laws that survive changes of subject.

### Law 1 — The object is not given by the problem statement

The first formulation usually names data and a desired output, not the best mathematical object. Reconstitute the problem as a space, action, operator, functional, or solution map.

Test: Can you state what counts as two descriptions of the same object?

### Law 2 — Search is impossible until it is biased

The candidate space is too large. Preparation, constraints, invariants, and representation must make useful candidates statistically or structurally favored.

Test: Why should the desired object occur in the part of the space you are searching?

### Law 3 — Prefer structure that predicts, not notation that stores

An encoding is valuable only if its ambient mathematics yields restrictions or inversion mechanisms.

Test: What theorem becomes available after encoding that was unavailable before?

### Law 4 — Globalize before calculating locally

Identify the orbit space, moduli space, phase portrait, or dependency architecture before expanding formulas.

Test: What are the invariant strata or organizing subsets?

### Law 5 — Compress evolution by canonical events

Use return maps, renormalized states, boundary hits, or canonical representatives to eliminate redundant intermediate motion.

Test: Which target properties are faithfully represented after compression?

### Law 6 — Separate local content from gluing

Repeated local rules plus global identifications determine the object. Study them separately.

Test: Could two globally different objects share every local rule in your model?

### Law 7 — Let unresolved collisions generate invariants

When current statistics collide, inspect the minimal difference and algebraize it.

Test: Does the new invariant separate the motivating collision and remain preserved under all allowed moves?

### Law 8 — Treat boundaries and singularities as information channels

Zeros, poles, shocks, separatrices, equality cases, and degeneracies often carry the theorem.

Test: What is lost when the object is smoothed or restricted to the generic case?

### Law 9 — Reconstruct from a skeleton plus controlled remainder

Find distinguished events and bound the residual freedom by growth, regularity, energy, or dimension.

Test: Is the remainder genuinely controlled, or merely renamed?

### Law 10 — Make stability explicit

Every approximation, truncation, computation, or inverse inference depends on a topology and a stability claim.

Test: Can arbitrarily small input changes reverse the conclusion?

### Law 11 — Perturb the exact structure on which the proof depends

Do not test only numerical output. Test persistence of invariant manifolds, rank, injectivity, sign, spectral gap, or other proof-bearing structure.

Test: What is the first omitted term capable of destroying?

### Law 12 — Generalize roles, not formulas

Decompose a successful construction into jobs and rebuild those jobs in the new category.

Test: Does the generalized object satisfy the defining universal or operator identity?

### Law 13 — Lift only when the ambient space adds a theorem

Higher dimension or abstraction is useful when it adds symmetry, factorization, compactness, linearity, or a known classification.

Test: What becomes easier upstairs, and how is it recovered downstairs?

### Law 14 — Equality cases are latent definitions

Sharp bounds often reveal the canonical structure in their saturation conditions.

Test: Have you classified all extremizers, including degenerate ones?

### Law 15 — Beauty is a proposal distribution

Use unity, compression, unexpected fit, and low ad hoc complexity to rank candidates.

Test: What independent falsification would kill the beautiful idea?

### Law 16 — Keep synthesis and proof synchronized but distinct

Use a global schema to guide work and a local ledger to certify it.

Test: Which arrows in the schema are proved, computational, heuristic, or aspirational?

### Law 17 — Convert results into relay platforms

Every substantial lemma deserves a consequence audit before it is treated as a mere stepping stone.

Test: What changes if the original target is removed from view?

### Law 18 — Incubation requires a prepared impasse

A break is productive after relevant structures and failures have been loaded, not instead of work.

Test: Can you write the constraint set and the exhausted local moves before disengaging?

### Law 19 — Proof failure should enlarge the ontology

Characterize the mode of failure as a mathematical object.

Test: Does the counterexample reveal splitting, torsion, nonuniqueness, instability, or missing gluing data?

### Law 20 — A method is not mastered until its dominance boundary is known

Every representation has problems it clarifies and problems it conceals.

Test: State the class on which the method is complete, the class on which it is merely heuristic, and a counterexample outside its range.

# VI. A reusable Poincaré–Hadamard research protocol

## 41. Phase A — Constitute the problem

Write a one-page problem constitution with these fields:

Objects: What exactly ranges over the quantifiers?

Equivalence: Which differences are coordinate artifacts or irrelevant?

Target: Is the claim existence, classification, asymptotic behavior, obstruction, or recovery?

Observables: What data can actually be measured, computed, or proved?

Solution map: What input is supposed to determine what output?

Well-posedness: Is determination existent, unique, and stable?

Truth state: Which claims are proved, computationally observed, plausible, or refuted?

Exit criterion: The target cannot change meaning when translated into later representations.

## 42. Phase B — Build a representation atlas

Construct at least four views.

| View | Question | Typical objects |
|---|---|---|
| Native | What does the problem say literally? | equations, integers, graphs |
| Geometric/dynamic | What space and motion does it define? | phase space, flow, orbit, return map |
| Algebraic/invariant | What survives equivalence? | group, homology, spectrum, conserved quantity |
| Analytic/functional | What rigid ambient theory can encode it? | generating function, kernel, determinant, functional |
| Lifted/quotiented | What becomes simpler after adding or removing redundancy? | cover, quotient, higher dimension, fundamental domain |

For each representation, record:

forward map;

inverse or loss profile;

target translation;

available theorems;

known failure modes.

Exit criterion: At least one representation makes a previously informal obstruction exact.

## 43. Phase C — Identify the structural skeleton

Search systematically for:

fixed and periodic objects;

zeros, poles, and singular support;

extremizers and equality cases;

boundary and degenerate cases;

invariant manifolds or subspaces;

minimal counterexamples;

gluing relations;

growth exponents and dominant terms;

atomic responses or fundamental solutions.

Do not assume the most numerous objects are the most informative.

Exit criterion: You can state how the skeleton organizes or constrains generic objects.

## 44. Phase D — Run discriminating perturbations

For every proof-bearing feature , test:

parameter perturbation;

hypothesis deletion;

dimension change;

boundary degeneration;

adversarial example;

change of representation;

numerical precision or truncation change.

Record whether  persists exactly, approximately, statistically, or not at all.

Exit criterion: “Small perturbation” and “same structure” have explicit meanings.

## 45. Phase E — Alternate synthesis and verification

Maintain four ledgers:

| Ledger | Contents |
|---|---|
| Structural map | objects, transformations, invariants, desired bottleneck |
| Proof ledger | exact statements, dependencies, domains, quantifiers |
| Computation ledger | code version, range, precision, witnesses, failure logs |
| Counterexample ledger | failed claims, minimal witnesses, repaired statements |

Use the structural map for candidate generation. Use the other three to prevent the map from becoming mythology.

Exit criterion: Every structural arrow has an explicit truth label.

## 46. Phase F — Incubate deliberately

Before a break, write:

the exact impasse;

three exhausted moves;

two structural tensions;

one external method with an explicit analogy dictionary;

the condition a successful new representation must satisfy.

After the break, capture candidates immediately but do not edit the prior ledger. Then attempt reconstruction and falsification.

Exit criterion: New ideas are evaluated as hypotheses, not recollections of certainty.

## 47. Phase G — Extract relay-results

For each proved result , run this audit:

converse;

contrapositive;

equality case;

limiting case;

perturbative stability;

functoriality under maps;

interaction with every prior invariant;

minimal hypotheses;

computational certificate;

possible role as a definition.

Then decide whether  is:

a local lemma;

a bridge between representations;

an obstruction theorem;

a classification parameter;

a new central object.

Exit criterion: No important lemma remains trapped in the purpose for which it was first proved.

## 48. Phase H — State the dominance boundary

Conclude each research round with:

proven region: where the method is complete;

computational region: where evidence exists but proof does not;

heuristic region: where the representation is suggestive;

failure region: explicit counterexamples or loss of equivalence;

next discriminator: the smallest test separating the leading frames.

This is the operational form of rigor without intellectual paralysis.

# VII. Failure diagnostics

## 49. Symptoms that the current frame is wrong

### Symptom 1 — Calculations proliferate without reusable lemmas

Diagnosis: isolated-fact accumulation.

Poincaré move: search for analogy, return structure, or invariant.

Hadamard move: seek an encoding or kernel that packages the calculations.

### Symptom 2 — The model predicts data but cannot exclude countermodels

Diagnosis: ill-posed identification.

Poincaré move: strengthen the invariant using a collision pair.

Hadamard move: test uniqueness and stability of the recovery map.

### Symptom 3 — A truncation looks exact across all tested cases

Diagnosis: unproved structural persistence.

Poincaré move: restore the first term capable of splitting the invariant structure.

Hadamard move: bound the remainder in the topology relevant to the conclusion.

### Symptom 4 — The key object has many definitions and no decisive use

Diagnosis: definition without earned necessity.

Poincaré move: identify nearest nonexamples and the invariant distinction.

Hadamard move: state the solution or operator role the object performs.

### Symptom 5 — Intuition is vivid but cannot be written

Diagnosis: synthetic schema not yet translated.

Poincaré move: identify the global order and candidate relation.

Hadamard move: build a sign dictionary and relay-results until every arrow has content.

### Symptom 6 — Every local inference checks, but the theorem still feels wrong

Diagnosis: semantic drift or missing global hypothesis.

Poincaré move: audit the architecture and meaning at reuse points.

Hadamard move: test existence, uniqueness, boundary conditions, and stability of the constructed object.

### Symptom 7 — A beautiful conjecture survives only on regular examples

Diagnosis: aesthetic overfitting.

Poincaré move: search extreme exceptions and perturb the skeleton.

Hadamard move: inspect singular support, equality cases, and growth remainder.

### Symptom 8 — A strong lemma does not seem to advance the headline theorem

Diagnosis: target fixation.

Poincaré move: ask what new classification or invariant it suggests.

Hadamard move: remove the headline problem and exhaust the relay-result.

# VIII. Training the method rather than memorizing it

## 50. Exercises that build generative reflexes

### Exercise A — Five ontologies

Take one unsolved or difficult problem and formulate it as:

a state space and evolution;

a group action and quotient;

an invariant-classification problem;

an operator inversion or recovery problem;

an extremal or variational problem.

For each formulation, state exactly what is lost and gained. The purpose is not to keep all five. It is to learn that the first ontology is not compulsory.

### Exercise B — Collision-driven invariant design

Find two objects with identical current statistics but different target behavior. Identify the minimal witness of difference. Attempt to close that witness under the allowed transformations. The closure is a candidate invariant.

### Exercise C — Return-map compression

For a long evolution, define a canonical event and an induced map. Prove one property that transfers both ways and exhibit one that does not. This trains faithfulness analysis.

### Exercise D — Well-posedness autopsy

For a favored conjectural reconstruction, construct sequences of data . Determine whether candidate solutions converge, bifurcate, or diverge. State the topology. This trains Hadamard’s third condition.

### Exercise E — Skeleton and remainder

Choose an object with distinguished zeros, singularities, prime factors, critical points, or jumps. Ask what residual freedom remains when the skeleton is fixed. Find the weakest growth or regularity condition that controls it.

### Exercise F — Equality-first research

For an inequality used in a proof, derive all equality conditions before trying to sharpen the constant. Determine whether the extremizer defines a new canonical object.

### Exercise G — Prepared incubation

Work to a precisely recorded impasse, disengage, and log the first new representation that appears. Then measure whether it actually differs from the exhausted search. This removes mysticism from incubation.

### Exercise H — Relay-result day

Spend one research session forbidding work on the main theorem. Analyze only the strongest intermediate lemma using the ten-item relay audit. This counteracts attention capture.

## 51. What not to imitate

Do not imitate Poincaré’s speed, Hadamard’s personal imagery, their work schedules, or the surface style of their papers. Those are individual particulars.

Do not infer that:

a sudden idea is likely true;

beautiful mathematics is automatically important;

nonverbal thought is superior to symbolic thought;

breaks substitute for preparation;

broad analogy licenses theorem transfer;

qualitative understanding licenses missing estimates;

analytic encoding is useful merely because it is sophisticated;

a higher-dimensional lift is explanatory without a faithful descent;

a correct finite computation establishes stability or asymptotics.

The laws are the control conditions that make their boldness productive.

# IX. A compact operating card

## 52. Before attacking a hard problem

What is the actual object space?

What differences are inessential?

Is the desired output determined by the stated data?

What are the organizing singular, periodic, extremal, or boundary objects?

Which representation adds the strongest external theorem?

What must be preserved under reduction, quotient, lift, or encoding?

## 53. When stuck

Replace individual solutions by the space of solutions.

Search for a return map or canonical event.

Find two current-invariant collisions.

Inspect the first perturbation that can destroy the picture.

Translate the problem into zeros/growth, kernels, or a functional.

Lift to a category with a real advantage, then prove descent.

Re-read the strongest lemma without the original target.

Record a structured impasse and incubate.

## 54. Before believing a result

Does every representation step have a proved preservation statement?

Are existence, uniqueness, and stability separately established?

Have singular, boundary, equality, and degenerate cases been tested?

Is the conclusion robust to the first omitted term?

Has a counterexample search targeted the exact invariant used?

Is aesthetic conviction being mistaken for evidence?

Can the proof architecture be reconstructed from relay-results?

Is the dominance boundary stated?

# X. Final synthesis

Poincaré and Hadamard should not be internalized as collections of celebrated outputs. Their deepest contribution to research practice is a theory of where mathematical necessity comes from.

For Poincaré, necessity becomes visible when we pass from isolated computations to the global architecture of relations: phase spaces instead of trajectories, return maps instead of continuous detail, group actions and quotients instead of redundant coordinates, invariants instead of appearances, and perturbative skeletons instead of unjustified exact pictures. His intuition is sensitivity to order in this architecture. His beauty is a trained detector of compression and latent law. His errors show why architecture must remain answerable to exact proof and adversarial examples.

For Hadamard, necessity becomes usable when the problem is constituted as a legitimate transformation from data to solution and then moved into a rigid domain: an analytic function determined by zeros and growth, a functional differentiated by admissible variations, a kernel responding to an atomic source, a singular surface carrying propagation, or a higher-dimensional problem from which the native solution descends. His psychology of invention is the control cycle that permits these transformations to be found: prepared attention, constrained recombination, synthetic insight, verification, and the accumulation of relay-results.

Their combined research ethic is neither formalist passivity nor intuitive license. It is high-agency structural exploration under exact preservation obligations:

Change the object until the theorem becomes structural. Change the representation until the structure becomes controllable. Change neither without proving what survives.

That is the law capable of generating the specifics on the fly.

# Appendix A. Evidence map

## A1. Primary sources

Henri Poincaré, Science and Method, English translation, 1914. Especially “The Selection of Facts,” “The Future of Mathematics,” “Mathematical Discovery,” and “Mathematical Definitions and Education.” Full scan.

Henri Poincaré, The Foundations of Science: Science and Hypothesis, The Value of Science, Science and Method, 1913. Internet Archive edition.

Henri Poincaré, Papers on Topology: Analysis Situs and Its Five Supplements, trans. John Stillwell, 2009. Manuscript/scan.

Jacques Hadamard, An Essay on the Psychology of Invention in the Mathematical Field, 1945. Full scan.

## A2. Historical and mathematical studies

M. L. Cartwright, “Jacques Hadamard,” Journal of the London Mathematical Society 40 (1965), 722–748. PDF.

Philip Holmes, “Poincaré, Celestial Mechanics, Dynamical-Systems Theory and ‘Chaos’,” Physics Reports 193 (1990), 137–163. PDF.

Claudio Bartocci, “Analogy and Invention: Poincaré and Mathematical Creation.” PDF.

June Barrow-Green, Poincaré and the Three Body Problem, historical study/dissertation version. PDF.

Tom M. Apostol, “A Centennial History of the Prime Number Theorem.” PDF.

“Henri Poincaré,” Stanford Encyclopedia of Philosophy, revised 2026. Entry.

MacTutor History of Mathematics, “Jacques Hadamard’s Mathematician’s Mind.” Entry.

Institut Mittag-Leffler, “Prize Competition.” Historical note.

## A3. Modern cognitive qualification

Ut Na Sio and Thomas C. Ormerod, “Does Incubation Enhance Problem Solving? A Meta-Analytic Review,” Psychological Bulletin 135 (2009), 94–120. PubMed record.

# Appendix B. Historiographic cautions

Poincaré’s and Hadamard’s introspections are unusually valuable but remain reports by elite practitioners about their own experience.

Modern terms such as “search-space conditioning,” “representation atlas,” “solution operator,” and “proposal distribution” are reconstructive language used to expose transferable structure; they are not period vocabulary.

Poincaré’s claims about logic, induction, and foundations are historically important but not accepted wholesale in contemporary logic or philosophy of mathematics. The present report extracts their methodological content rather than endorsing every foundational thesis.

“Mathematical beauty” is treated here as an expert heuristic correlated with compression, unity, and generativity. It is neither necessary nor sufficient for truth.

The four-stage sequence is a useful model, not a mandatory chronology. Discovery can be gradual, collaborative, or repeatedly cyclic.

Poincaré’s topology and celestial mechanics demonstrate both extraordinary structural insight and real proof gaps. They are evidence for coupling bold invention to aggressive correction, not for relaxing rigor.

Hadamard well-posedness depends on chosen spaces and topologies. A problem may be ill posed in one setting and well posed in another; changing the setting must be mathematically and operationally justified.
