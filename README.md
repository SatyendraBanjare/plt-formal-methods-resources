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
  + [Security Related](#security-related)
    * [Software Security](#software-security)
    * [Differential Privacy](#differential-privacy)
    * [Applications in Block Chain Security](#applications-in-block-chain-security)
    * [Challenges in Making AI secure](#challenges-in-making-ai-secure)
    * [Create Secure CyberPhysical Systems](#create-secure-cyberphysical-systems)
  + [Programming Language research related](#programming-language-research-related)
    * [Probabilistic Programming](#probabilistic-programming)
    * [Development of Quantum Programming Language](#development-of-quantum-programming-language)
    * [Language Refinement using formal methods](#languages-refinement-using-formal-methods)
  + [Abstract Interpretation focused](#abstract-interpretation-focused)
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

- [Getting Started with formal methods](https://www.eeweb.com/profile/adarbari/articles/getting-started-with-formal-verification)
- [K Framework & efforts of Formal verification in Blockchain](https://medium.com/epicenterpodcast/the-k-framework-formal-verification-efforts-in-the-blockchain-space-1651b789e5d4)
- [Pact Formal Verification for Blockchain smart contracts](https://medium.com/kadena-io/pact-formal-verification-for-blockchain-smart-contracts-done-right-889058bd8c3f) : Awesome short blog explaining the **Pact FV's** methodology with a small introduction to formal verification by first principles.
- [Towards Robust and Verified AI: Specification Testing, Robust Training, and Formal Verification - **DeepMind**](https://deepmind.com/blog/robust-and-verified-ai/)
- [The challenge of verification and testing of machine learning - **Ian GoodFellow & Nicolas Papernot**](http://www.cleverhans.io/security/privacy/ml/2017/06/14/verification.html)

## MOOCs

- **[Formal Software Verification - edX](https://www.edx.org/course/formal-software-verification-0)**
- **[Quantitative Model Checking -  Coursera](https://www.coursera.org/learn/quantitative-model-checking)**
- **[Cyber Physical Systems](https://www.edx.org/course/cyber-physical-systems)** : Course by UC Berkeley, focused in using verification methods for modelling Cyper Physical systems (CPS).

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
- [VeriDeep - Safety Verification of Deep Neural Networks](https://github.com/VeriDeep/DLV)
- [VeHICal](https://vehical.org/) : Project focused on developing the foundations of verified co-design of interfaces and control for human cyber-physical systems.

## Upcoming Challenges 

### Security Related

- #### Software Security
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
    * [Deep Specification for Dropbox](https://www.youtube.com/watch?v=Y2jQe8DFzUM)
    * [DSL for Verified Secure Multiparty Computations in F*](https://youtu.be/pEBp-BoSDE8)
    * [Using Formal Methods for development of Highly Secure Systems](https://youtu.be/2OG-TQhVJRc)
    * [Security through FOrmal Methods and Secure Architecture (CERIAS - Purdue University)](https://youtu.be/XsBUKCgIH7g)
    * [Language based techniques for Cryptography and Privacy](https://www.youtube.com/watch?v=4GAaum1VM_I)

- #### Differential Privacy
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
    * [Proving Differential privacy using Relational Types](https://simons.berkeley.edu/talks/tba-42)

- #### Applications in Block Chain Security

  **[Formal Methods for Block Chains](https://sites.google.com/view/fmbc/)** : This is first ever workshop focused on using formal methods in Block Chain technology. It will be on _11th October 2019_.
  
  **[CertiK](https://certik.org/)** : It is a startup focused on using formal methods to make blockchains verifialbly secure.
  
  + Readings
    * [How Formal Analysis and Verification Add Security to Blockchain-based Systems - Tutorial @ MIT](https://pdfs.semanticscholar.org/aef7/0c6c305eec9df96e2b58a593bd60ba66c16a.pdf)
    * [Smart contracts and oppurtunities for formal methods](https://pdfs.semanticscholar.org/409b/a537907855706f64daf3cb2e3e344a971ffb.pdf)
    * [K Framework & efforts of Formal verification in Blockchain](https://medium.com/epicenterpodcast/the-k-framework-formal-verification-efforts-in-the-blockchain-space-1651b789e5d4) an Awesome collection of explainatory material on K framework and its application in verifying Blockchain systems.
    * [Pact Formal Verification for Blockchain smart contracts](https://medium.com/kadena-io/pact-formal-verification-for-blockchain-smart-contracts-done-right-889058bd8c3f) : Awesome short blog explaining the **Pact FV's** methodology with a small introduction to formal verification by first principles.
    * [Temoporal Blockchains - a formal analysis](https://researchportal.port.ac.uk/portal/files/5324699/A_temporal_blockchain_A_formal_analysis.pdf)
    * [Validation of Decentralised Smart Contracts through Game Theory and Formal Methods](https://dspace.stir.ac.uk/bitstream/1893/23914/1/bHalo_Degano2015.pdf)
  + Videos
    * [Formal Design, Implementation and Verification of BlockChain Languages](https://testnet.iohkdev.io/iele/about/formal-verification/)
    * [CertiK - Smart contract formal verification platform (review)](https://www.youtube.com/watch?v=pLOR_WuoPaY)
    * [Simplicity - A new Language for blockchains](https://blockstream.com/2018/02/08/en-simplicity-a-new-language-for-blockchains-bpase/)

- #### Challenges in making AI secure
  **[FLoC 2018- Summit of Machine Learning meets formal methods](https://www.floc2018.org/summit-on-machine-learning/)**
  **[Verified Machine Learning - Radboud University Nijmegen](https://www.sws.cs.ru.nl/Teaching/VerifiedMachineLearning)** : University course on using verification methods in Machine Learning.
  **[Formal Methods meets Machine Learning - RWTH Aachen University](https://moves.rwth-aachen.de/teaching/ss-18/fvmml/)** : 2018's seminar on advancements in Verifiably Secure Machine Learning using formal methods.
  
  + Readings
    * [Towards Verified Artificial Intelligence - S. Seshia](https://arxiv.org/pdf/1606.08514.pdf)
    * [Towards Robust and Verified AI: Specification Testing, Robust Training, and Formal Verification - **DeepMind**](https://deepmind.com/blog/robust-and-verified-ai/)
    * [Developing BugFree Machine Learning Systems with Formal Mathematics](https://arxiv.org/pdf/1706.08605.pdf)
    * [Mixing Formal methods, Machine Learning & Human Computer Interaction](https://www.aaai.org/ocs/index.php/FSS/FSS16/paper/viewPDFInterstitial/14127/13686)
    * [Machine Learning in Formal Methods](http://www.cs.utexas.edu/users/hunt/FMCAD/FMCAD16/slides/tutorial1.pdf)
    * [Machine Learning and Formal Methods](http://drops.dagstuhl.de/opus/volltexte/2018/8430/pdf/dagrep_v007_i008_p055_17351.pdf)
    * [Algorithms for Verifying Deep Neural Networks](https://arxiv.org/pdf/1903.06758.pdf)
    * [Safety Verification of Deep Neural Networks](http://qav.comlab.ox.ac.uk/papers/hkww17.pdf)
    * [The challenge of verification and testing of machine learning - **Ian GoodFellow & Nicolas Papernot**](http://www.cleverhans.io/security/privacy/ml/2017/06/14/verification.html)
    * [Verifying Properties of Binarized Deep Neural Networks](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/download/16898/16241)
    * [Reluplex: An Efficient SMT Solver for Verifying Deep Neural Networks](https://arxiv.org/pdf/1702.01135.pdf)
    * [Verification of Piecewise Linear Feed Forward Networks](https://arxiv.org/pdf/1705.01320.pdf)
    * [Challenges in Verification of Reinforcement Learning Algorithms](https://ntrs.nasa.gov/archive/nasa/casi.ntrs.nasa.gov/20170007190.pdf)
    * [Applying Formal Methods in Reinforcement Learning - Galois Inc.](https://galois.com/wp-content/uploads/2017/10/galois-formal-methods-reinforcement-learning.pdf)
    * [Towards Proving the Adversarial Robustness of Deep Neural Networks](https://arxiv.org/pdf/1709.02802.pdf)
    
  + Videos
    * [Safety Verification for Deep Neural Networks -ICST 2018](https://www.youtube.com/watch?v=OTXEzJnzUV0)
    * [Safety Verification for Deep Neural Networks - Marta Kwiatkowska - CAV 2017](https://www.youtube.com/watch?v=XHdVnGxQBfQ)
    * [Safety Verification for Deep Neural Networks -INRIA ](https://www.canal-u.tv/video/inria/safety_verification_of_deep_neural_networks.25215)
    * [Rules of Machine Learning Verification, from data driven bugs to explainable AI](https://www.oreilly.com/library/view/oreilly-artificial-intelligence/9781491976289/video311845.html)
    * [Verification of Machine Learning Programs](https://www.youtube.com/watch?v=Reo5REo71GU)
    * [Reluplex: An Efficient SMT Solver for Verifying Deep Neural Networks - Conference Video](https://www.youtube.com/watch?v=KiKS_zaPb64)
    * [Developing Bug-Free Machine Learning models using Certigrad - Daniel Selsam](https://www.youtube.com/watch?v=-A1tVNTHUFw)
    
    

- #### Create secure CyberPhysical Systems

  **[VeHICal](https://vehical.org/)** : Project focused on developing the foundations of verified co-design of interfaces and control for human cyber-physical systems.
  + Readings
  + Videos

### Programming Language Research related
- #### Probabilistic Programming
  + Readings
    * [Probabilistic Logic Programming and Bayesian Networks](https://www.seas.upenn.edu/~cis700dr/Spring19/localpapers/haddawy2.pdf)
     * [probabilistic Functions and Cryptographic Oracles in Higher Order Logic - Andreas Lochbihler](https://www7.in.tum.de/~schulzef/2016-06-03-Andreas-Lochbihler.pdf)
     * [Probabilistic Relational Verification of Cryptographic implementations](https://dl.acm.org/citation.cfm?id=2535847)
     * [Coupling Proofs are Probabilistic product programs](https://dl.acm.org/citation.cfm?id=3009896)
     * [Advanced Probabilistic Coupling for Differential Privacy](https://dl.acm.org/citation.cfm?id=2978391)
     * [Formal Methods for probabilistic Programming](https://pps2018.sice.indiana.edu/files/2017/12/dselsam_pps_2018.pdf)
  + Videos
- #### Development of Quantum Programming Language 
  + Readings
  + Videos
- #### Languages Refinement using formal methods
  + Readings
  + Videos
    * [Algorithmic Software Verification](https://youtu.be/DM1G__Limmo)
 
 ### Abstract Interpretation focused
 
- [Fast and Effective Robustness Certification](https://www.sri.inf.ethz.ch/publications/singh2018effective) : project DeepZ - for certifying neural network robustness based on abstract interpretation.
- [AI2 : Safety and Robustness Certification of Neural Networks with Abstract Interpretation](https://files.sri.inf.ethz.ch/website/papers/sp2018.pdf)
- [Boosting Robustness Certification of Neural Networks](https://files.sri.inf.ethz.ch/website/papers/RefineZono.pdf) : Uses Abstract Interpretation in its methodology.


## Related Industries & Startups
- **[CertiK](https://certik.org/)**
- **[Galois Inc](https://galois.com/)**
- **[Synthetic Minds](https://synthetic-minds.com/)**
- **[Nomadic Labs](https://www.nomadic-labs.com/)**
- **[Tezos](https://tezos.com/)**
- **[JaneStreet](https://www.janestreet.com/technology/)**
- **[Systerel](http://www.systerel.fr/en/expertise/formal-methods/)**

## License
[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

Any suggestions are welcome. Please do consider submitting a pull request if you feel like !!
