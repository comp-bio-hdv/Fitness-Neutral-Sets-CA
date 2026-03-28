**1. inverse_ca_neutral_networks.nb**

Wolfram Mathematica code that implements an inverse cellular automata algorithm via random walks on adaptive mutation chains.

<details>
<summary>More info</summary>

***User-entered Parameters***

*Target Lifetime:* lifetime to which an adaptive mutation chain should reach<br>
*Rule Bucket Size:* number of adaptive mutation chain iterations<br>
*Max Mutation Attempts* per iteration<br>

***Successful Scenario of an Adaptive Mutation Chain***

Lifetime reached = Target lifetime<br>
Rule progression is plotted<br>
Iterations per lifetime table is printed<br>

***Failed Scenarios of an Adaptive Mutation Chain***

Lifetime reached > Target lifetime<br>
Lifetime reached < Target lifetime after all unique point mutations fail<br>
Maximum mutation attempts per iteration exceeded<br>

</details>

**2. WWS26_Essay_RZ_Edits_addendum_2.pdf**

Wolfram Mathematica code that explores neutral networks (also known as fitness-neutral sets) in adaptive mutation chains in the aspect of percolation in the multidimensional rule space.

<details>
<summary>More info</summary>

The terms ***fitness-neutral set*** and ***percolation*** and its metrics ***average local neutrality*** and ***network diameter*** are first defined followed by an introduction to cellular automata riles in (k=3, r=1).

A sample random walk is then shown which demonstrates these metrics, thereafter the issue of percolation is examined via further metrics, namely ***radius of gyration*** and ***average inter-point distance*** and their visualizations.

</details>

**3. Schemata with Neutrality.nb**

Wolfram Mathematica code that builds on **inverse_ca_neutral_networks.nb** adapted to (k=2, r=2) with a focus on the identifaction of schemata in a collection of phenotypes with a similar lifetime.

<details>
<summary>More info</summary>

Random walks with 1–3 bit mutations per step are performed accepting mutations that reduce the distance to a user-specified target lifetime (26 is used here). The search includes random restarts to escape local optima. Upon convergence, the program outputs the genotype (32-entry lookup table) and phenotype (space-time diagram) of the matched rule.

Building block schemata variants using a 5×5 sliding window are examined on the run results in order to identify patterns shared across genotypically distinct but phenotypically equivalent cellular automaton rulesacross all phenotypes. Similar binary patterns (Hamming distance ≤ 8) are clustered, and each cluster was collapsed into a ternary schema: 0 (stable white across all variants), 1 (stable black), and * (wildcard, varies between genotypes).

</details>
