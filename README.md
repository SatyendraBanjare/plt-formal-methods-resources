# Programming Language Theory & Formal Methods - Resources

![FORSYTE group pics](http://forsyte.at/wp-content/uploads/wordle.png)
**Image Courtsey : [Forsyte group](https://forsyte.at/)**

Formal methods are mathematical techniques that are used for design, verification and specifications of software and hardware problems. These are essentially a subset of **Programming Language Theory research** that are being used to study complex computer science problems.

Analysis by Formal Methods basically involves these steps :
1. `Formal Specification`  
2. `Formal Proofs` 
3. `Model Checking` 
4. `Abstraction` 

The formal proof development and model checking are primarily done using interactive theorem provers often called as proof Assistants. Abstraction is creating structurally sound relations between parts of models. 

Here is my attempt to curate a list of useful reading materials, videos and tools accompanied by some upcoming challenges in the field. 

### NOTE :
1. I have tried to make the content more focused on current research and industrial application. People looking for purely academic collection must refer [Formal Methods in Education - Jeremy Avigad](https://avigad.github.io/formal_methods_in_education/).

2. The reader is expected to have some basic knowledge of **[Type Theory](https://en.wikipedia.org/wiki/Type_theory)**. A more academic insight can be found here [learn-tt](https://github.com/jozefg/learn-tt).  

## Contents

- [Books & Lectures](#books--lectures)
- [Blogs](#blogs)
- [MOOCs](#moocs)
- [Tools](#tools)
- [Projects](#projects)
- [Upcoming Challenges](#upcoming-challenges)
- [Related Industries & Startups](#related-industries--startups)

## Books & Lectures

- **[Software Foundations](https://softwarefoundations.cis.upenn.edu/)** ![Tool Used](https://img.shields.io/badge/Coq-based-green.svg) : I highly advice this as a starting material for diving deep into this field. The book is very helpful in building basic concepts and serves as a very sound introduction to the field. Beautifully illustrated concepts with examples to practice are provided all throughout making interactive theorem proving learning fun. 

- **[FRAP - Adam Chlipala](http://adam.chlipala.net/frap/)** ![Tool Used](https://img.shields.io/badge/Coq-based-green.svg) : A book that helps you understand and reason formal correctness of programs. Imperative language (**C**) inspired examples of data structures and algorithms helps immensely to begin thinking about their formal verification.

- **[Certified Programming with Dependent Types - Adam Chlipala](http://adam.chlipala.net/cpdt/)** ![Tool Used](https://img.shields.io/badge/Coq-based-green.svg)  : One of the best `theoretical books` to learn theorem proving using coq.

- **[Formal Verification - Jacques Fleuriot](http://www.inf.ed.ac.uk/teaching/courses/fv/)** : This a course that involves theorem proving using some more developed tools like [SAT](https://en.wikipedia.org/wiki/Boolean_satisfiability_problem) and [SMT](https://en.wikipedia.org/wiki/Satisfiability_modulo_theories) solvers.

- **[Abstract Interpretation - Patrick Cousot](http://web.mit.edu/16.399/www/)** The best available material on the theory of Abstract Interpretation. It gives a complete and pure mathematical analysis of program mutations. The Program behaviour as a continuously modifying relation between different abstract mathematical structures is explained and proved!!.  

- **[Logic and Proof - CMU & Lean introduction](https://leanprover.github.io/logic_and_proof/)** ![Tool Used](https://img.shields.io/badge/Lean-based-green.svg) : This is course designed at CMU and it also serves as a introductory material for theorem proving in Lean 

If you feel you need more theoretical insights, please refer [Note](#note-) above.

## Blogs
- https://www.eeweb.com/profile/adarbari/articles/getting-started-with-formal-verification 

## MOOCs
- **[Formal Software Verification - edX](https://www.edx.org/course/formal-software-verification-0)**
- **[Quantitative Model Checking -  Coursera](https://www.coursera.org/learn/quantitative-model-checking)**

## Tools

### Proof Assistants

- [coq](https://coq.inria.fr/): The most popular and widely used theorem prover. It supports a lot of features including ML-extraction, Project packaging (Project and Makefile creation). There are plenty of `how-to` material available that use coq for formalization. Anyone might find this very interesting [100 Theorems in Coq](https://github.com/coq/coq/wiki/Top100MathematicalTheoremsInCoq).
- [lean](https://leanprover.github.io/): A fairly new Theorem Prover by **Microsoft Research**. Has a nice interactive tutorial, is easy to get started with.
- [PRISM model checker](https://www.prismmodelchecker.org/) : It is model checker developed by University of Oxford.
- [Nuprl](http://www.nuprl.org/) : Theorem Prover by **Cornell** under Proof Refinement Logic Project.
- [Agda](https://github.com/agda/agda): A quite Mature Proof Assistant. Has features similar to Coq. easy to learn after some experience in coq.
- [Isabelle](https://isabelle.in.tum.de/): It is an old theorem Prover. Has nice implementation of core logic but lacks other UX related features.

### SAT/SMT/SMC solvers

#### SAT Solvers :
- [MiniSat](https://github.com/niklasso/minisat).

#### SMT Solvers :
- [Z3](https://github.com/Z3Prover/z3)
- [CVC4](https://github.com/CVC4/CVC4)
- [MathSAT5](http://mathsat.fbk.eu/)
- [SMTInterpol](https://ultimate.informatik.uni-freiburg.de/smtinterpol/)
- [Princess](http://www.philipp.ruemmer.org/princess.shtml)

#### SMC Solvers :
- [Publication](https://people.eecs.berkeley.edu/~sseshia/pubdir/hscc17-smc.pdf)

### Hybrid Solvers
Proof Assitants have very strong implmentations of program logics. Sometimes it may not be tactically possible to carry out complex proofs only by using them. Therefore Current research combines this principle of strong logic based reasoning with powerful SMT and SMC solvers to ease the proof development. Some examples are here below :

- **[Fstar(F*)](https://github.com/FStarLang/FStar)**
  + It is possible to extract F* code to C using [KreMLin](https://github.com/FStarLang/kremlin).
- **[SMTCoq](https://github.com/smtcoq/smtcoq)**

## Projects

Most of the projects are more or less development of the respective theorem provers or SAT/SMT/SMC/ solvers and hence can be looked up there. These are some of other projects actively developed.

- [DeepSpec](https://deepspec.org/main) is an umbrella project that focuses on building verified software systems. Follwoing major sub-projects are actively worked upon : 
  + [Compcert](https://github.com/AbsInt/CompCert)
  + [Verified LLVM (VeLLVM)](https://github.com/vellvm/vellvm)
  + [Verified Software ToolChain (VST)](https://github.com/PrincetonUniversity/VST)
  
- [ikos](https://github.com/NASA-SW-VnV/ikos) is a reliable **bug-free** C compiler based on the theory of abstract interpretation.
- [Project Everest](https://github.com/project-everest): It is research project that aims at creating secure and verified HTTPS ecosystem.
- [CertiCrypt](http://certicrypt.gforge.inria.fr/): It is a project focuse on modelling public key cryptography using coq proof assistant.
- [Iris](https://iris-project.org/): Iris is a Higher-Order Concurrent Separation Logic Framework implemented and verified in the proof assistant Coq.

## Upcoming Challenges 

### Security Related
- ### Software Security
  + Readings
    * [Formal Methods for Security, NSF workshop](https://arxiv.org/pdf/1608.00678.pdf)
    * [Symbolic Relationship between Formal Methods and Security](http://www.cs.cmu.edu/~wing/publications/Wing98.pdf)
    * [Project-Everest Research Papers](https://project-everest.github.io/papers/)
    * [Formal Methods in Software Security](http://projects.laas.fr/IFSE/FMF/J7/slides/P01_TJensen.pdf)
    * [Formal Methods for Safe and Secure Computers Systems](https://github.com/SatyendraBanjare/plt-formal-methods-resources/blob/master/books_and_articles/formal_methods_security.pdf)
    * [The Computational Soundness of Formal Encryption](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.20.2584&rep=rep1&type=pdf)
    * [Security Structures using Formal Methods](http://diyhpl.us/~nmz787/pdf/Security%20Architectures%20Using%20Formal%20Methods.pdf)
    * [Verification of Cryptographic Primitive](https://www.cs.princeton.edu/~appel/papers/verif-sha.pdf)
    * [Formal Certification of Game based Cryptographic proofs ](https://pastel.archives-ouvertes.fr/pastel-00584350/document)
    * [Formal certification of code-based cryptographic proofs](https://dl.acm.org/citation.cfm?id=1480894)
  + Videos 
    * [DSL for Verified Secure Multiparty Computations in F*](https://youtu.be/pEBp-BoSDE8)
    * [Using Formal Methods for development of Highly Secure Systems](https://youtu.be/2OG-TQhVJRc)
    * [Security through FOrmal Methods and Secure Architecture (CERIAS - Purdue University)](https://youtu.be/XsBUKCgIH7g)
    * [Language based techniques for Cryptography and Privacy](https://www.youtube.com/watch?v=4GAaum1VM_I)
- ### Differential Privacy
  + Readings
    * [Formal Verification of Differential Privacy for Interactive Systems](https://arxiv.org/abs/1101.2819)
    * [Formal Methods for Privacy](https://apps.dtic.mil/dtic/tr/fulltext/u2/a507044.pdf)
    * [LightDP - Towards automating Differential Privacy Proofs](http://www.cse.psu.edu/~dbz5017/pub/popl17.pdf)
    * [EasyCrypt - Verified Computational Differential Privacy with Applications to Smart Meter](http://www0.cs.ucl.ac.uk/staff/G.Danezis/papers/easypriv.pdf)
    * [Proving Differential Privacy in Hoare Logic](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6957126)
    * [Differentially Private Bayesian Programming](https://dl.acm.org/citation.cfm?id=2978371)
    * [Advanced Probabilistic Coupling for Differential Privacy](https://dl.acm.org/citation.cfm?id=2978391)
  + Videos
    * [Formal Methods and proofs of privacy properties - 1](https://simons.berkeley.edu/talks/formal-methods-and-proofs-privacy-properties)
    * [Formal Methods and proofs of privacy properties - 2](https://simons.berkeley.edu/talks/formal-methods-and-proofs-privacy-properties-part-ii)
    * [Formal Methods and proofs of privacy properties - 3](https://simons.berkeley.edu/talks/formal-methods-and-proofs-privacy-properties-part-iii)
- ### Applications in Block Chain Security
  + Readings
  + Videos
- ### Challenges in making AI secure
  + Readings
  + Videos
- ### Create secure CyberPhysical Systems
  + Readings
  + Videos

### Programming Language Research related
- ### Probabilistic Programming
  + Readings
    * [Probabilistic Logic Programming and Bayesian Networks](https://www.seas.upenn.edu/~cis700dr/Spring19/localpapers/haddawy2.pdf)
     * [probabilistic Functions and Cryptographic Oracles in Higher Order Logic - Andreas Lochbihler](https://www7.in.tum.de/~schulzef/2016-06-03-Andreas-Lochbihler.pdf)
     * [Probabilistic Relational Verification of Cryptographic implementations](https://dl.acm.org/citation.cfm?id=2535847)
     * [Coupling Proofs are Probabilistic product programs](https://dl.acm.org/citation.cfm?id=3009896)
     * [Advanced Probabilistic Coupling for Differential Privacy](https://dl.acm.org/citation.cfm?id=2978391)
  + Videos
- ### Development of Quantum Programming Language 
  + Readings
  + Videos
- ### Languages Refinement using formal methods
  + Readings
  + Videos
  


## Related Industries & Startups
- **[Galois Inc](https://galois.com/)**
- **[Synthetic Minds](https://synthetic-minds.com/)**
- **[Nomadic Labs](https://www.nomadic-labs.com/)**
- **[Tezos](https://tezos.com/)**
- **[JaneStreet](https://www.janestreet.com/technology/)**
- **[Systerel](http://www.systerel.fr/en/expertise/formal-methods/)**

## License
[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

Any suggestions are welcome. Please do consider submitting a pull request if you feel like !!
