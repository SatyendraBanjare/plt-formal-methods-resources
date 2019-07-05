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
- [BLogs](#blogs)
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

- **[Logic and Proof - CMU | Lean introduction](https://leanprover.github.io/logic_and_proof/)** ![Tool Used](https://img.shields.io/badge/Lean-based-green.svg) : This is course designed at CMU and it also serves as a introductory material for theorem proving in Lean 

## Blogs
- https://www.eeweb.com/profile/adarbari/articles/getting-started-with-formal-verification 

## MOOCs
- **[Formal Software Verification - edX](https://www.edx.org/course/formal-software-verification-0)**
- **[Quantitative Model Checking -  Coursera](https://www.coursera.org/learn/quantitative-model-checking)**

## Tools

### Proof Assistants

- [coq](https://coq.inria.fr/) 
  + [![Community](https://img.shields.io/badge/Community-green.svg)](https://shields.io/) 
- [Nuprl](http://www.nuprl.org/)
  + [![Community](https://img.shields.io/badge/Community-green.svg)](https://shields.io/) 
- [Isabelle](https://isabelle.in.tum.de/)
  + [![Community](https://img.shields.io/badge/Community-green.svg)](https://shields.io/) 
- [lean](https://leanprover.github.io/)
  + [![Community](https://img.shields.io/badge/Community-green.svg)](https://shields.io/) 
- [Agda](https://github.com/agda/agda)
  + [![Community](https://img.shields.io/badge/Community-green.svg)](https://shields.io/) 

It is now also possible to extract the proofs into a ML code. Coq does it beautifully.

### SAT/SMT/SMC solvers

SAT Solvers :
- [MiniSat](https://github.com/niklasso/minisat).

SMT Solvers :
- [Z3](https://github.com/Z3Prover/z3)
  + [![Community](https://img.shields.io/badge/Community-green.svg)](https://shields.io/) 
- [MathSAT5](http://mathsat.fbk.eu/)
  + [![Community](https://img.shields.io/badge/Community-green.svg)](https://shields.io/) 
- [SMTInterpol](https://ultimate.informatik.uni-freiburg.de/smtinterpol/)
  + [![Community](https://img.shields.io/badge/Community-green.svg)](https://shields.io/) 
- [Princess](http://www.philipp.ruemmer.org/princess.shtml)
  + [![Community](https://img.shields.io/badge/Community-green.svg)](https://shields.io/) 
- [CVC4](https://github.com/CVC4/CVC4)
  + [![Community](https://img.shields.io/badge/Community-green.svg)](https://shields.io/) 

SMC Solvers :
- [Publication](https://people.eecs.berkeley.edu/~sseshia/pubdir/hscc17-smc.pdf)

### Hybrid Solvers
Proof Assitants have very strong implmentations of program logics. Sometimes it may not be tactically possible to carry out complex proofs only by using them. Therefore Current research combines this principle of strong logic based reasoning with powerful SMT and SMC solvers to ease the proof development. Some examples are here below :

- **[Fstar(F*)](https://github.com/FStarLang/FStar)**
  + It is possible to extract F* code to C using [KreMLin](https://github.com/FStarLang/kremlin).
  + [![Community](https://img.shields.io/badge/Community-green.svg)](https://shields.io/) 
- **[SMTCoq](https://github.com/smtcoq/smtcoq)**

## Projects
- [DeepSpec](https://deepspec.org/main) is an umbrella project that focuses on building verified software systems. Follwoing major sub-projects are actively worked upon : 
  + [Compcert](https://github.com/AbsInt/CompCert)
  + [Verified LLVM (VeLLVM)](https://github.com/vellvm/vellvm)
  + [Verified Software ToolChain (VST)](https://github.com/PrincetonUniversity/VST)
  
- [ikos](https://github.com/NASA-SW-VnV/ikos) is a reliable **bug-free** C compiler based on the theory of abstract interpretation.
- [Project Everest](https://github.com/project-everest) is research project that aims at creating secure and verified HTTPS ecosystem.
- [CertiCrypt](http://certicrypt.gforge.inria.fr/) is a project focuse on modelling public key cryptography using coq proof assistant.

## Upcoming Challenges 
- **Software Security**
  + Readings
    * aplha
    * beta
  + Videos 
- **Differential Privacy**
  + Readings
  + Videos
- **Applications in BLock Chain Security**
  + Readings
  + Videos
- **Challenges in making AI secure**
  + Readings
  + Videos
- **Development of Quantum Programming Language**
  + Readings
  + Videos
- **Languages Refinement using formal methods**
  + Readings
  + Videos
- **Create secure CyberPhysical Systems**
  + Readings
  + Videos
 - **Applications in securing Databases**
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

