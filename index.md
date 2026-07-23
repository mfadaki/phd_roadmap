---
title: "PhD Journey"
layout: default
---


# PhD Roadmap to ADP

**Path:** Background → MDP / Exact DP → RL → ADP → Unified framework → Research

---

## PhD milestones (RMIT)

There are three milestones, and the details are as follows:

### Milestone 1: Confirmation of Candidature

First milestone; your candidature stays probationary until you pass. Submit documentation at least 15 days before you present to the panel and wider research community.

-  **Research proposal**: written documentation setting out the project, its aims, significance, and your theoretical or conceptual framework.
-  **Methodology and an initial review of literature and references**: how the project will be undertaken, plus a first literature review showing how your work relates to the existing body of knowledge.
-  **Research methods course and compulsory training**: evidence of being enrolled in, having completed, or being exempted from the research methods course, plus all compulsory training on your Canvas dashboard.
-  **Research data management plan**: how you will store and manage your research data.
-  **Statement of ethics and/or biosafety approval status**: evidence of approvals, or an explanation and timeline if not yet obtained, or an approved exemption, or confirmation that none is required with a rationale.
-  **Publication plan and a viable timeline to completion**: pending or completed outputs with timelines, and a clear schema for completing the degree from confirmation to submission.

### Milestone 2: Second Milestone Review (mid-candidature)

Mid-way point; shows you are on the way to finishing on time. Submit at least 15 days before you present.

-  **At least two draft thesis chapters, OR a draft dissertation**: this is what RMIT means by "a significant piece of work" (Schedule 1). At least two draft chapters of the thesis, or the equivalent in draft or published papers, or a portfolio that includes a draft of the dissertation. Which two chapters is set with your supervisor; in an OR or ADP thesis they are commonly the introduction and the literature review, or a first model and methodology chapter.
-  **Summary document**: an updated review of literature and references, and any changes to your candidature since confirmation.
-  **Maintained ethics/biosafety, data plan, and publication plan**: evidence approvals are obtained and maintained, an updated data management plan, and an updated publication plan.
-  **A detailed timeline from the mid-point to completion**: plus evidence of impact and stakeholder engagement where appropriate.

### Milestone 3: Third Milestone Review (final)

Final milestone; shows you are on track to submit. Submit at least 15 days before you present.

-  **At least two draft chapters OR a draft dissertation (advanced and coherent)**: an advanced draft giving a coherent account of the research that answers your research questions.
-  **iThenticate Summary Report for the current draft**: a similarity report for the current draft (or substantial written component), with demonstrated engagement with and understanding of it. A personal reflection may accompany it.
-  **Summary document**: an updated review of literature and references, and any changes to your candidature since the last milestone.
-  **A detailed path and timeline to submission**: how the thesis or project will be completed between this milestone and submission, plus maintained ethics/biosafety, data plan, publication plan, and stakeholder communication.

---

## The phases

### Phase 1: Background

#### General

-  Latex (Olverleaf)
-  Python (Vs Code + CPlex)

#### Mathematical background

**Goal.** Acquire only the mathematical tools the rest of the roadmap relies on: convex optimization, linear algebra, statistical learning, and probability.

-  **Prerequisite for convex optimization: linear algebra + multivariable calculus**: vectors and matrices, eigenvalues, norms, and gradients.
-  **[Boyd & Vandenberghe, Convex Optimization](https://web.stanford.edu/~boyd/cvxbook/)** (targeted, not cover to cover): Ch 2 to 3 (convex sets and functions), Ch 4 (LP and QP), Ch 5 (duality), then skim Ch 9 to 11 (gradient / Newton methods).
-  **[Stephen Boyd, Stanford EE364A Convex Optimization I (video lectures, 2023)](https://www.youtube.com/playlist?list=PLoROMvodv4rMJqxxviPa4AmDClvcbHi6h)**: the author's own lecture series, the video companion to the book.
-  **[James et al., An Introduction to Statistical Learning (ISL)](https://www.statlearning.com/)**
-  PAC (Probably Approximately Correct) Learning

$\lVert V^{alg} - V^* \rVert_{1,\nu} \le UB \; \;$ with probability of $1-\delta$


$\lVert V^{alg} - V^* \rVert_{1,\nu} = \mathbb{E}_\nu \lvert V^{alg} - V^*\rvert$

-  Markov chains 
-  Conditional expectation, the law of total expectation, approximating expectations.
-  Algorithm Design, Iterative algorithms, Algorithm Complexity (Big O, ...), Lower bound, Upper Bound for an algorithm.
-  Gradient Descent, Stochastic Gradient Descent, Mirror Descent
-  Lipschitz continuity
-  Kernel and Kernel Tricks
-  Uncertainty Modeling - Probability distributions, Ambiguity sets, etc.
-  Primal-Dual methods + Column Generation
-  Function Approximation
-  Regularization
-  Lagrangian
-  Norm ($1, 2, \infty, weighted$)
-  Famous Inequalities/Bounds: Markov, Hoeffding, Jensen, Chernoff, Chebyshev, Chernoff, McDiarmid, Cauchy-Schwartz, etc.
-  Stochastic Optimization + Decomposition (e.g.,  Advanced Optimization, lecture 8, 9, 10 [Jalal Kazempour](https://www.youtube.com/@jalalkazempour1429))


### Phase 2: MDP foundations

**Goal.** Build the rigorous theoretical core of MDPs: the Bellman equation, value and policy iteration, and conditions for optimality.

-  **[Puterman, Markov Decision Processes (Ch 1 to 6)](https://onlinelibrary.wiley.com/doi/book/10.1002/9780470316887)**: the rigorous MDP reference. Finite and infinite horizon, discounted and average reward, value/policy iteration, the LP formulation.
-  **[Sutton & Barto, Reinforcement Learning: An Introduction (2nd ed.)](http://incompleteideas.net/book/the-book-2nd.html)**: Ch 3 (Finite Markov Decision Processes) and Ch 4 (Dynamic Programming) for the MDP foundations.
-  **[David Silver RL Course, Lectures 1 to 3](https://www.youtube.com/playlist?list=PLqYmG7hTraZDM-OYHWgPebj2MfCFzFObQ)**: L1 Introduction to RL, L2 Markov Decision Processes, L3 Planning by Dynamic Programming.
-  **[Silver Lecture 2: Markov Decision Process (direct)](https://www.youtube.com/watch?v=lfHX2hHRMVQ)**: the single most useful lecture for this phase.

### Phase 3: Reinforcement learning core

**Goal.** Learn to act without knowing the model, through Monte Carlo, temporal-difference, Q-learning, function approximation.

-  **[Sutton & Barto, Reinforcement Learning: An Introduction (2nd ed.)](http://incompleteideas.net/book/the-book-2nd.html)**: the main text. Core: Ch 3 to 6, 7, and 9 to 13.
-  **[David Silver RL Course, Lectures 4 to 10](https://www.youtube.com/playlist?list=PLqYmG7hTraZDM-OYHWgPebj2MfCFzFObQ)**: L4 Model-Free Prediction, L5 Model-Free Control, L6 Value Function Approximation, L7 Policy Gradient, L8 Integrating Learning and Planning, L9 Exploration and Exploitation, L10 Case Study.
-  **[DeepMind x UCL RL Lecture Series (2021)](https://www.youtube.com/watch?v=TCCjZe0y4Qc)**: optional and modern, more depth on deep RL.

#### Solution Approaches.:

#### None-LP:

| Category                                           | Representative Algorithms                                    | Model Required?                |
| -------------------------------------------------- | ------------------------------------------------------------ | ------------------------------ |
| **Dynamic Programming (Exact)**                    | Value Iteration, Policy Iteration, Modified Policy Iteration, ==Linear Programming== | Yes                            |
| **Approximate Dynamic Programming (ADP)**          | Approximate Value Iteration, Approximate Policy Iteration, Rollout Algorithms, Neuro-Dynamic Programming | Usually Yes                    |
| **Monte Carlo Methods**                            | First-Visit Monte Carlo, Every-Visit Monte Carlo, Monte Carlo Control | No                             |
| **Temporal Difference (TD) Learning**              | TD(0), TD(λ), SARSA, Expected SARSA, Q-learning              | No                             |
| **Eligibility Trace Methods**                      | SARSA(λ), Q(λ), Watkins' Q(λ), TD(λ)                         | No                             |
| **Policy Gradient Methods**                        | REINFORCE, Vanilla Policy Gradient                           | No                             |
| **Actor-Critic Methods**                           | Advantage Actor-Critic (A2C), Asynchronous Advantage Actor-Critic (A3C), Deep Deterministic Policy Gradient (DDPG), Twin Delayed DDPG (TD3), Soft Actor-Critic (SAC) | No                             |
| **Trust Region / Constrained Policy Optimization** | Trust Region Policy Optimization (TRPO), Proximal Policy Optimization (PPO) | No                             |
| **Distributional Reinforcement Learning**          | C51, Quantile Regression DQN (QR-DQN), Implicit Quantile Networks (IQN) | No                             |
| **Deep Value-Based Methods**                       | Deep Q-Network (DQN), Double DQN, Dueling DQN, Rainbow DQN   | No                             |
| **Model-Based Reinforcement Learning**             | Dyna-Q, MuZero, Probabilistic Ensembles with Trajectory Sampling (PETS), Model-Based Policy Optimization (MBPO) | Learns or Uses a Model         |
| **Offline Reinforcement Learning**                 | Batch-Constrained Q-learning (BCQ), Conservative Q-Learning (CQL), Implicit Q-Learning (IQL) | No Interaction During Training |
| **Imitation Learning**                             | Behavior Cloning, Dataset Aggregation (DAgger), Inverse Reinforcement Learning (IRL), Generative Adversarial Imitation Learning (GAIL) | Demonstrations Required        |
| **Multi-Agent Reinforcement Learning**             | Independent Q-Learning, Multi-Agent DDPG (MADDPG), QMIX, Value Decomposition Networks (VDN) | Varies                         |
| **Hierarchical Reinforcement Learning**            | Options Framework, MAXQ, HIRO, FeUdal Networks               | No                             |
| **Evolutionary / Black-Box Optimization**          | Evolution Strategies (ES), Genetic Algorithms (GA), Covariance Matrix Adaptation Evolution Strategy (CMA-ES) | No                             |
| **Multi-Armed Bandit Methods**                     | ε-Greedy, Upper Confidence Bound (UCB), Thompson Sampling, Contextual Bandits | Stateless                      |

#### LP: Convert the Belmman equation to LP and then solve LP

### Phase 4: Approximate dynamic programming

**Goal.** Scale dynamic programming to real, high-dimensional problems, addressing the curses of dimensionality through value-function approximation.

-  **[Powell, Approximate Dynamic Programming (2nd ed., 2011)](https://castle.princeton.edu/approximate-dynamic-programming/)**: the dedicated ADP text. Core: Ch 4, 6, 8, 9 to 11.
-  **[Bertsekas, Reinforcement Learning and Optimal Control (2019)](https://www.mit.edu/~dimitrib/rlbook_athena.html)**: approximation in value/policy space, rollout, MPC, aggregation.
-  Dimitri Bertsekas, Neuro-Dynamic Programming
-  Powell, *Reinforcement Learning and Stochastic Optimization: A Unified Framework for Sequential Decisions*
-  Powell, *Approximate Dynamic Programming: Solving the Curses of Dimensionality*
-  Powell, *Algorithms for Sequential Decision Making*
-  Powell, *Optimal Learning*
-  Powell, Sequential Decision Analytics and Modeling: Modeling with Python
-  **[Powell, RLSO Ch 15 & 18: Backward ADP and convex VFAs](https://castle.princeton.edu/rlso/)**: backward ADP, piecewise-linear separable VFAs.
-  **[Powell (2019), A unified framework for stochastic optimization. EJOR, 275(3), 795 to 821.](https://doi.org/10.1016/j.ejor.2018.07.014)**: the journal-length statement of the framework; it shows RL and ADP are two faces of the same problem.

### Phase 5: Powell's unified framework

**Goal.** Tie everything together with Powell's five-element model and four policy classes (PFA, CFA, VFA, DLA), moving from algorithms to modeling then solving.

-  **[Powell, RLSO: full structured read](https://castle.princeton.edu/rlso/)**: Ch 1 to 2, 9 to 11, 12 (PFA), 13 (CFA), 19 (DLA), 20 (multiagent and POMDPs).
-  **[Powell, Sequential Decision Analytics and Modeling (2nd ed.)](https://castle.princeton.edu/sdamodeling/)**: the teach-by-example companion.

**Solution Approaches for ALP.**

-  **Column Generation**: Adelman 2007, Zhang and Adelman 2009
-  **Constraint Sampling**: de Farias and Van Roy 2004
-  **Constraint violation learning**: Lin et al. 2020
-  **Reformulation**: Tong and Topaloglu (2013) and Vossen and Zhang (2015)
-  **Aggregation**: Hugo P. Simão, Jeff Day, Abraham P. George, Ted Gifford, John Nienow, Warren B. Powell (2009)
-  Primal-Dual
-  Auto-generated basis function
-  ...

Phase XXX: Neural Network

---

## Learn and practice ADP

Tutorial-style reads to understand ADP (mostly Powell), then hands-on resources to build, run, and tune policies on small problems that have known optimal benchmarks.

-  **[Powell, W. B. (2009). What you should know about approximate dynamic programming. Naval Research Logistics, 56(3), 239 to 249.](https://doi.org/10.1002/nav.20347)**: the best short entry point; the major dimensions of an ADP algorithm and strategies for approximating value functions.
-  **[Powell, W. B. (2014). Clearing the jungle of stochastic optimization. INFORMS Tutorials in Operations Research, 109 to 137.](https://doi.org/10.1287/educ.2014.0128)**: the canonical five-part model and the four classes of policies (PFA, CFA, VFA, lookahead).
-  **[Powell, W. B. (2016). Perspectives of approximate dynamic programming. Annals of Operations Research, 241, 319 to 356.](https://doi.org/10.1007/s10479-012-1077-6)**: an overview of ADP, its history, and how the four policy classes fit together.
-  **[Powell, W. B., Simao, H. P. & Bouzaiene-Ayari, B. (2012). Approximate dynamic programming in transportation and logistics: a unified framework. EURO Journal on Transportation and Logistics, 1(3), 237 to 284.](https://doi.org/10.1007/s13676-012-0015-8)**: a step-by-step build from Bellman's equation to the four policies, illustrated on real applications.
-  **[George, A. P. & Powell, W. B. (2006). Adaptive stepsizes for recursive estimation with applications in approximate dynamic programming. Machine Learning, 65(1), 167 to 198.](https://doi.org/10.1007/s10994-006-8365-9)**: stepsize rules (including OSA); the wrong stepsize makes a correct algorithm look broken.
-  **[Jiang, D., Pham, T., Powell, W. B., Salas, D. & Scott, W. (2014). A comparison of approximate dynamic programming techniques on benchmark energy storage problems: does anything work? IEEE Symposium Series on Computational Intelligence (ADPRL).](https://ieeexplore.ieee.org/document/7010626/)**: which ADP methods actually work against optimal benchmarks; lookup table with structure beats generic value-function approximation.
-  **Powell, four-part unified-framework video tutorial (INFORMS, 2022)**: [Part I: introduction and the universal framework](https://tinyurl.com/SDAPartI), [Part II: an energy storage example and the four policy classes](https://tinyurl.com/SDAPartII), [Part III: PFAs, CFAs, and VFAs](https://tinyurl.com/SDAPartIII), [Part IV: DLAs and the jungle of stochastic optimization](https://tinyurl.com/SDAPartIV).
-  **[Powell, W. B. Sequential Decision Analytics and Modeling (2nd ed.).](https://castle.princeton.edu/sdamodeling/)**: a teach-by-example introduction where each chapter pairs a worked sequential decision problem with a Python module.
-  **[Sequential Decision Problem Modeling Library (Python, CASTLE Lab).](https://github.com/wbpowell328/stochastic-optimization)**: runnable models built as model / policy / driver: asset selling, energy storage, blood management, clinical trials, diabetes, stochastic shortest path, two newsvendors.
-  **[SDAM supplements (spreadsheets and datasets)](https://castle.princeton.edu/sdamodelingsupplements/)**: tune policy parameters in a spreadsheet before moving to code.

---

## Watch: the field up close

Optional but motivating. The human story behind the algorithms in this roadmap.

-  **[AlphaGo, The Movie (2017 documentary)](https://www.youtube.com/watch?v=WXuK6gekU1Y)**: the full DeepMind documentary on the AlphaGo vs Lee Sedol match. Free.
-  **[The Thinking Game (DeepMind documentary)](https://www.youtube.com/watch?v=d95J8yzvjbQ)**: five years inside DeepMind with Demis Hassabis, from AlphaGo to AlphaFold. Free.
-  **[David Silver: AlphaGo, AlphaZero, and Deep RL (Lex Fridman #86)](https://www.youtube.com/watch?v=uPUEq8d73JI)**: the lead researcher on how self-play learns superhuman policies.
-  **[Rich Sutton: the early days of reinforcement learning (with Michael Littman and Lex Fridman)](https://www.youtube.com/watch?v=2P1Ssas_PI0)**: the co-author of Sutton & Barto on where RL came from.

---

## Sources

- [Powell CASTLE Lab, RLSO](https://castle.princeton.edu/rlso/)
- [Powell, Sequential Decision Analytics (4-part tutorial)](https://castle.princeton.edu/sda/)
- [Sutton & Barto, free book](http://incompleteideas.net/book/the-book-2nd.html)
- [David Silver course](https://www.davidsilver.uk/teaching/)
- [Bertsekas, books and video lectures](https://www.mit.edu/~dimitrib/publ.html)
- [Boyd & Vandenberghe, Convex Optimization](https://web.stanford.edu/~boyd/cvxbook/)
- [RMIT milestone reviews](https://www.rmit.edu.au/students/my-course/research-students/milestones)
- [RMIT HDR Schedule 1, milestone submission requirements](https://policies.rmit.edu.au/document/view.php?id=237)
