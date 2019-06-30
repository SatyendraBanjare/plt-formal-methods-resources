# Programming Language Theory & Formal Methods - Resources

Formal methods are mathematical techniques that are used for design, verification and specifications of software and hardware problems. These are essentially a subset of **Programming Language Theory research** that are being used to study complex computer science problems.

Analysis by Formal Methods basically involves these steps :
1. `Formal Specification`  
2. `Formal Proofs` 
3. `Model Checking` 
4. `Abstraction` 

The formal proof development and model checking are primarily done using interactive theorem provers often called as proof Assistants. Abstraction is creating structurally sound relations between parts of models. 

Here is my attempt to curate a list of useful reading materials and tools accompanied by some upcoming challenges in the field.

**Note** : The reader is expected to have some basic knowledge of type theory. I highly encourage going through resources mentioned in here [learn-tt](https://github.com/jozefg/learn-tt).


## Books & Lectures

- **Software Foundations** https://softwarefoundations.cis.upenn.edu/ : I highly advice this as a starting material for diving deep into this field. The book is very helpful in building basic concepts and serves as a very sound introduction to the research field.

- **Interactive Theorem Proving - Adam Chlipala**

- **Abstract Interpretation - Patrick Cousot**

## Blogs
- https://www.eeweb.com/profile/adarbari/articles/getting-started-with-formal-verification 

## Tools

### Proof Assistants

- coq
- Nuprl
- Isabelle
- lean

It is now also possible to extract the proofs into a ML code. Coq does it beautifully.

### SAT/SMT/SMC solvers

- z3


### Hybrid Solvers
Proof Assitants have very strong implmentations of program logics. Sometimes it may not be tactically possible to carry out complex proofs only by using them. Therefore Current research combines this principle of strong logic based reasoning with powerful SMT and SMC solvers to ease the proof development. Some examples are here below :

- **[Fstar(F*)](https://github.com/FStarLang/FStar)**
  + It is possible to extract F* code to C using KreMLin.

## Projects
- Compcert
- 

## Upcoming Challenges 
- challenges in making AI secure

## Related Industries & Startups
- **[Galois Inc](https://galois.com/)**
- **[Synthetic Minds](https://synthetic-minds.com/)**
- **[Nomadic Labs](https://www.nomadic-labs.com/)**
- **[Tezos](https://tezos.com/)**
- **[JaneStreet](https://www.janestreet.com/technology/)**



