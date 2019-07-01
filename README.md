# Programming Language Theory & Formal Methods - Resources

Formal methods are mathematical techniques that are used for design, verification and specifications of software and hardware problems. These are essentially a subset of **Programming Language Theory research** that are being used to study complex computer science problems.

Analysis by Formal Methods basically involves these steps :
1. `Formal Specification`  
2. `Formal Proofs` 
3. `Model Checking` 
4. `Abstraction` 

The formal proof development and model checking are primarily done using interactive theorem provers often called as proof Assistants. Abstraction is creating structurally sound relations between parts of models. 

Here is my attempt to curate a list of useful reading materials and tools accompanied by some upcoming challenges in the field.

**[Note]** : The reader is expected to have some basic knowledge of type theory.

## Contents

- [Books & Lectures](#books--lectures)
- [BLogs](#blogs)
- [Tools](#tools)
- [Projects](#projects)
- [Upcoming Challenges](#upcoming-challenges)
- [Related Industries & Startups](#related-industries--startups)

## Books & Lectures

- **Software Foundations** https://softwarefoundations.cis.upenn.edu/ : I highly advice this as a starting material for diving deep into this field. The book is very helpful in building basic concepts and serves as a very sound introduction to the research field.

- **Interactive Theorem Proving - Adam Chlipala**

- **Abstract Interpretation - Patrick Cousot**

## Blogs
- https://www.eeweb.com/profile/adarbari/articles/getting-started-with-formal-verification 

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

## Upcoming Challenges 
- **Software Security**
  + Readings
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

## License
[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

