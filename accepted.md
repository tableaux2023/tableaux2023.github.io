
FroCoS 2021 Accepted Papers with Abstracts
==========================================


[Martin Suda](http://people.ciirc.cvut.cz/~sudamar2/). Vampire With a Brain Is a Good ITP Hammer

**Abstract:** Vampire has been for a long time the strongest first-order automatic  
theorem prover, widely used for hammer-style proof automation in ITPs  
such as Mizar, Isabelle, HOL, and Coq. In this work, we considerably  
improve the performance of Vampire in hammering over the full Mizar  
library by enhancing its saturation procedure with efficient neural  
guidance. In particular, we employ a recently proposed recursive neural network  
classifying the generated clauses based only on their derivation  
history. Compared to previous neural methods based on considering the  
logical content of the clauses, our architecture makes evaluating a single clause  
much less time consuming. The resulting system shows good learning  
capability and improves on the state-of-the-art performance on the Mizar  
library, while proving many theorems that the related ENIGMA system  
could not prove in a similar hammering evaluation.

[Zarathustra Goertzel](https://zarathustra.gitlab.io/), Karel Chvalovský, Jan Jakubuv, Miroslav Olšák and [Josef Urban](http://www.ciirc.cvut.cz/~urbanjo3/). Fast and Slow Enigmas and Parental Guidance

**Abstract:** We describe several additions to the ENIGMA system that guides clause selection in the E automated theorem prover. First, we significantly speed up its neural guidance by adding server-based GPU evaluation. The second addition is motivated by fast weight-based rejection filters that are currently used in systems like E and Prover9. Such systems can be made more intelligent by instead training fast versions of ENIGMA that implement more intelligent pre-filtering. This results in combinations of trainable fast and slow thinking that improves over both the fast-only and slow-only methods. The third addition is based on "judging the children by their parents", i.e., possibly rejecting an inference before it finishes producing a clause. This saves time by not evaluating all clauses by more expensive methods and provides a complementary view of the generated clauses. The methods are evaluated on a large benchmark coming from the Mizar Mathematical Library.

Qingxiang Wang and [Cezary Kaliszyk](http://cl-informatik.uibk.ac.at/cek/). JEFL: Joint Embedding of Formal Proof Libraries

**Abstract:** The heterogeneous nature of the logical foundations used in different interactive proof assistant libraries has rendered discovery of similar mathematical concepts among them difficult.  
In this paper, we compare the previously developed algorithms for matching concepts across libraries with a proposed and developed unsupervised embedding approach that can help us retrieve similar concepts.  
Our approach is based on the fasttext implementation of Word2Vec, on top of which a tree traversal module is added to adapt its algorithm to the representation format of our data export pipeline.  
We compare the explainability, customizability, and online-servability of the approaches  
and argue that the neural embedding approach has more potential to be integrated into an interactive proof assistant.

[Martin Bromberger](http://people.mpi-inf.mpg.de/~mbromber/), Irina Dragoste, Rasha Faqeh, Christof Fetzer, [Markus Krötzsch](https://kbs.inf.tu-dresden.de/mak/) and [Christoph Weidenbach](http://www.mpi-inf.mpg.de/~weidenb/). A Datalog Hammer for Supervisor Verification Conditions Modulo Simple Linear Arithmetic

**Abstract:** The Bernays-Schönfinkel first-order logic fragment over simple linear  
real arithmetic  
constraints BS(SLR) is known to be decidable.  
We prove that BS(SLR) clause sets with both  
universally and existentially quantified verification  
conditions (conjectures) can be translated into BS(SLR) clause  
sets over a finite set of first-order constants. For the Horn case,  
we provide a  
Datalog hammer preserving validity and satisfiability.  
A toolchain from the BS(LRA) prover SPASS-SPL  
to the Datalog reasoner VLog establishes an effective  
way of deciding verification  
conditions in the Horn fragment. This is exemplified by the verification of supervisor code for a lane change  
assistant in a car and an electronic control unit for a supercharged combustion engine.

Filippo Bigarella, [Alessandro Cimatti](http://es.fbk.eu/people/cimatti/), [Alberto Griggio](http://es.fbk.eu/people/griggio/), [Ahmed Irfan](https://ahmed-irfan.github.io), Martin Jonas, Marco Roveri, [Roberto Sebastiani](http://disi.unitn.it/rseba/) and [Patrick Trentin](http://www.patricktrentin.com). Optimization Modulo Non-Linear Arithmetic via Incremental Linearization

**Abstract:** Incremental linearization is a conceptually simple, yet effective, technique that we have recently proposed for solving SMT problems on the theories of nonlinear arithmetic over the reals and the integers. Optimization Modulo Theories (OMT) is an important extension of SMT which allows for finding models that optimize given objective functions.  
In this paper, we show how incremental linearization can be extended to OMT in a simple way, producing an incomplete though effective OMT procedure. We describe the main ideas and algorithms, we provide an implementation within the OptiMathSAT OMT solver, and perform an empirical evaluation. The results support the effectiveness of the approach.  

[Franz Baader](http://lat.inf.tu-dresden.de/~baader/index-en.html), [Oliver Fernandez Gil](https://lat.inf.tu-dresden.de/~fernandez/) and Maryam Rostamigiv. Restricted Unification in the Description Logic FL0

**Abstract:** Unification in the Description Logic (DL) FL0 is known to be ExpTime-complete, and of unification type zero. We investigate in this paper whether a lower complexity of the unification problem can be achieved by either syntactically restricting the role depth of concepts or semantically restricting the length of role paths in interpretations. We show that the answer to this question depends on whether the number formulating such a restriction is encoded in unary or binary: for unary coding, the complexity drops from ExpTime to PSpace. As an auxiliary result, we prove a PSpace-completeness result for a depth-restricted version of the intersection emptiness problem for deterministic root-to-frontier tree automata. Finally, we also show that the unification type of FL0 improves from type zero to unitary (finitary) for unification without (with) constants.

Mostafa Sakr and Renate A. Schmidt. Semantic Forgetting in Expressive Description Logics

**Abstract:** Forgetting is an important ontology extraction tool, often required in applications such as reuse, construction, debugging and querying of ontologies.  
We study the notion of semantic forgetting which preserves all second order consequences of the original ontology.  
In the context of expressive description logics such as ALC, a major problem is that the extracted ontology is not in general representable in the language of the original ontology.  
We study different alternatives, in particular, representing the extracted ontology in a more complex logic, and extending the vocabulary of the extracted ontology with helper concept symbols.  
Our findings show that the latter alternative is preferable.  
Based on this representation, we develop and evaluate a terminating semantic forgetting method that preserves the structure of the original ontology.

Hai Lin, Christopher Lynch, Andrew M. Marshall, Catherine Meadows, Paliath Narendran, Veena Ravishankar and Brandon Rozek. Algorithmic Problems in the Symbolic Approach to the Verification of Automatically Synthesized Cryptosystems

**Abstract:** In this paper, we study several algorithmic problems arising from the verification of automatically synthesized cryptosystems built from block ciphers, in a theory that includes $ACUN$ symbols $\\oplus$ and $0$, as well as a symbol $f$ standing for the block cipher. One of these is static equivalence to an algorithm that produces a sequence of random terms. This is equivalent to there being no subsequence of ciphertext blocks that $\\oplus$-sums to $0$. The other is invertibility, the problem of determining whether, given a cryptosystem built from block ciphers, and the ability to compute $f$ and $f^{-1}$, it is always possible to compute the original plaintext from the ciphertext. We show that static equivalence to random in this theory is undecidable in general. In addition, we identify a reasonable special case for which there is a decidable condition implying security, along with an algorithm for verifying it. For invertibility, we identify a reasonable class of cryptosystems for which invertibility is equivalent to a simple syntactic condition that can be easily verified.

Antoine Defourné. Improving Automation for Higher-order Proof Steps

**Abstract:** We have extended the TLA+ proof system TLAPS with a new backend to improve the automation of proof steps that involve higher-order reasoning. The current support for such steps is poor, requiring the user to break down proofs into unnecessarily small steps. We defined a translation from TLA+ to THF, the TPTP dialect for higher-order logic, and integrated Zipperposition into TLAPS. We evaluate Zipperposition on proofs from the standard library of TLA+ and demonstrate that the new backend is able to handle much coarser proof steps than the other strategies provided by TLAPS, reducing the amount of necessary user interactions to write the proofs.

Hai Lin and Christopher Lynch. Formal Analysis of Symbolic Authenticity

**Abstract:** Authenticated encryption schemes are ways of encrypting messages which simultaneously assure the confidentiality and authenticity of data. Designing authenticated encryption schemes can be error-prone. In this paper, we are interested in the authenticity of authenticated encryption schemes. We introduce the notion of symbolic authenticity, and present two inference systems for verifying symbolic authenticity. The first inference system works for authenticated encryption schemes for messages of fixed length. It is sound, complete and terminating. The second one works for authenticated encryption schemes for messages of arbitrary length. It is sound, terminating, and complete under some condition. These inference systems can be used to automatically synthesize authenticated encryption schemes.

[Pascal Fontaine](http://www.montefiore.ulg.ac.be/~pfontain/) and [Hans-Jörg Schurr](https://schurr.io). Quantifier Simplification by Unification in SMT

**Abstract:** Quantifier reasoning in SMT solvers relies on instantiation: ground  
instances are generated heuristically from the quantified formulas until  
a contradiction is reached at the ground level. Current instantiation  
heuristics, however, often fail in presence of nested quantifiers.  
To address this issue we introduce a unification-based method that  
augments the problem with shallow quantified formulas obtained from  
assertions with nested quantifiers. These new formulas help unlocking the  
regular instantiation techniques, but parsimony is necessary since they  
might also be misguiding. To mitigate this, we identify some effective  
restricting conditions. The method is implemented in the veriT solver,  
and tested on benchmarks from the SMT-LIB. It allows the solver to  
prove more formulas, faster.

Serdar Erbatur, [Andrew M. Marshall](https://www.marshallandrew.net/) and [Christophe Ringeissen](http://www.loria.fr/~ringeiss/). Non-Disjoint Combined Unification and Closure by Equational Paramodulation

**Abstract:** Closure properties such as forward closure and closure via  
paramodulation have proven to be very useful in equational  
logic, especially for the formal analysis of security  
protocols. In this paper, we consider the non-disjoint  
unification problem in conjunction with these closure  
properties. Given a base theory $E$, we consider classes of  
theory extensions of $E$ admitting a unification algorithm  
built in a hierarchical way. In this context, a hierarchical  
unification procedure is obtained by extending an  
$E$-unification algorithm with some additional inference rules  
to take into account the rest of the theory. We look at  
hierarchical unification procedures by investigating an  
appropriate notion of $E$-constructed theory, defined in terms  
of $E$-paramodulation. We show that any $E$-constructed  
theory with a finite closure by $E$-paramodulation admits a  
terminating hierarchical unification procedure. We present  
modularity results for the unification problem modulo the  
union of $E$-constructed theories sharing only symbols in $E$.  
Finally, we also give sufficient conditions for obtaining  
terminating (combined) hierarchical unification procedures in  
the case of regular and collapse-free $E$-constructed  
theories.

[K. Subramani](http://www.csee.wvu.edu/~ksmani), Piotr Wojciechowski and Alvaro Velasquez. On the copy complexity of width~$3$ Horn constraint systems

**Abstract:** In this paper, we analyze the copy complexity of unsatisfiable width~$3$ Horn  
constraint systems, under the ADD refutation system. Recall that a  
linear constraint of the form $\\sum\_{i=1}^{n} a\_{i}\\cdot x\_{i} \\ge  
b$, is said to be a Horn constraint if all the $a\_{i} \\in \\{0,1,-1\\}$  
and at most one of the $a\_{i}$s is positive. A conjunction of such  
constraints is called a Horn constraint system (HCS). An HCS is said to  
have width~$3$, if there are at most $3$ variables with non-zero  
coefficients per constraint. Horn  
constraints arise in a number of domains including but not limited to  
program verification, power systems, econometrics, and operations  
research. The ADD refutation system is both {\\bf sound} and {\\bf  
complete}. Additionally, it is the simplest and most natural  
refutation system for refuting the feasibility of a system of linear  
constraints. The copy complexity of an infeasible linear constraint system (not  
necessarily Horn) in a refutation system is the minimum number of times each  
constraint  
needs to be replicated, in order to obtain a read-once refutation. We  
show that for an HCS with $n$ variables and $m$ constraints, the copy  
complexity is at most $2^{n-1}$, in the ADD refutation system. Additionally, we  
analyze  
width~$3$ HCSs from the perspective of copy complexity.  

Laine Rumreich and [Paolo A. G. Sivilotti](http://www.cse.ohio-state.edu/~paolo). Formal Verification of a Java Component Using the RESOLVE Framework

**Abstract:** A Binary Decision Diagram (BDD) is an efficient representation of a boolean formula with many applications in model checking, SAT solving, and networking. Recently, BDDs have also been used for solving problems in artificial intelligence, including the mining of frequent subsequences in higher-dimensional datasets. This paper uses the RESOLVE specification and reasoning framework to formally verify the functional correctness of a Java implementation of a BDD component. RESOLVE uses rich mathematical abstractions and clean value-based semantics for modular reasoning of assertive code. Java, on the other hand, includes many language features that are inconsistent with this notion of clean semantics and modular reasoning. Aliases, in particular, are easily created via assignment, parameter passing, and iterators, so reference-based semantics and points-to analysis are usually necessary when reasoning about Java code. This paper demonstrates the combination of these two paradigms. The implementation uses Java, but in a disciplined way and layered on a component catalog expressly designed to support modular reasoning. The assertional aspects of the code use RESOLVE, but are tailored to Java syntax and language constructs. In the development of the correctness proof for the BDD component, several errors in the original Java implementation were discovered and corrected. These errors were present despite the implementation passing an extensive test suite, exhibiting the value of the proof. The verification also exposed a limitation in the more general component design pattern related to unreachable code.

[Peter Baumgartner](http://users.rsise.anu.edu.au/~baumgart/). Combining Event Calculus and Description Logic Reasoning via Logic Programming

**Abstract:** The paper introduces a knowledge representation language that combines Kowalski's event calculus with description logic in a logic programming framework. The purpose is to provide the user with an expressive language for modelling and analysing systems that evolve over time. The description logic component is intended for modelling structural properties, the event calculus for actions and their consequences, and the logic programming rules for their integration and other aspects, such as diagnosis. By means of an elaborated example, the paper demonstrate the interplay of these three components for computing possible models as plausible explanations of the current state of the modelled system. The approach is prototypically implemented in our logic programming system Fusemate. The paper first extends Fusemate's rule language with a weakly DL-safe interface to the description logic ALCIF (which is implemented in Fusemate itself). It then embeds a suitable version of the event calculus, and provides rules as the "glue" between these components.

[Dennis Peuter](https://userpages.uni-koblenz.de/~dpeuter/) and [Viorica Sofronie-Stokkermans](http://userpages.uni-koblenz.de/~sofronie/). Symbol Elimination and Applications to Parametric Entailment Problems

**Abstract:** The main motivation for this work is the study of models for graph classes occurring in wireless network research. The properties of some functions and predicates used for the descriptions of such classes can be underspecified - we refer to such symbols as parameters.  
We are interested in finding conditions on such "parameters'' under which the graph classes are consistent resp. under which containedness or equality between graph classes holds.  
Such problems are non-trivial: For testing containedness between graph classes described using transformations we need to check entailment of second-order formulae.  
  
In this paper we combine two symbol elimination methods for solving such problems:  
(i) general symbol elimination - which we use for eliminating existentially quantified predicates and  
(ii) property-directed symbol elimination - which we use for obtaining conditions on parameters under which formulae are satisfiable or entailment holds.  
  
For general second-order quantifier elimination we use a specialization of the hierarchical superposition calculus. We analyze possibilities of obtaining weakest constraints on parameters which guarantee satisfiability (using a method we proposed in previous work, based on locality of suitable theories, instantiation and hierarchical reduction to quantifier elimination in a base theory).  
We identify situations in which entailment between formulae (possibly expressed using second order quantification) can be effectively checked, and - if entailent does not hold - possibilities of deriving additional constraints on parameters under which entailment can be guaranteed.
