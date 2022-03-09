# Mathematical Physics for Aging Discovery

Aging is a process that manifests itself at all levels of organization in a living organism [1]. Understanding the key molecular factors that are the drivers of the reorganization of the human body over time would allow us to develop methods of influencing them and thereby create a therapy for old age.

More than ten thousand articles on aging are published yearly. However, there has been no significant progress in prolonging human life so far. This situation can be changed by models that use state-of-the-art mathematical physics methods and are built on experimental biological data.

## The human body is a complex network of networks.
Conceptually, one can consider a human (or any other) organism as an evolving complex network - a radically reduced description, where the full system is described by an interaction network, whose vertices represent distinct physiological subsystems, and whose edges represent time-dependent interactions between them based on observations. Likewise, vertices may represent networks on smaller spatial scales leading to a complex mixture of interacting homogeneous and inhomogeneous networks of networks[2]. The development of mathematics over the last two decades has demonstrated that the network paradigm can fundamentally advance our understanding of natural and artificial complex dynamical systems.

## Equations that describe the dynamics of aging for interacting organism's physiological units

It is shown in [3,4,5] that the dynamics of aging for interacting degrees of freedom, or physiological units of the organism - genes, metabolites, immune system, etc., can be described by the following deterministic differential equation,

![eq1](https://latex.codecogs.com/svg.latex?\frac{d\vec{x}}{dt}=-A(t)\vec{x}+\vec{f}(t)+\delta\vec{f}(t),\hspace{100pt}(1))

where ![x](https://latex.codecogs.com/svg.latex?\vec{x}=(x_1,x_2,...x_n)) is a vector with components corresponding to the values of interacting physiological units, for example, gene expression levels and concentrations of metabolites; ![A](https://latex.codecogs.com/svg.latex?A(t)) a slowly changing matrix describing the interaction between physiological units; ![f](https://latex.codecogs.com/svg.latex?\vec{f}(t)) are vector fields associated with average environmental stress and the signaling or control processes in the body, which are considered as changing slowly; ![df](https://latex.codecogs.com/svg.latex?\delta\vec{f}(t)) random rapidly fluctuating force.

For short-lived organisms, aging can be described by the dynamics of a single variable following the Langevin equation, meaning that such variable can be a biomarker of aging,

![eq2](https://latex.codecogs.com/svg.latex?\frac{d\vec{y}}{dt}=-\alpha\vec{y}+\vec{f}'(t)+\delta\vec{f}'(t),\hspace{100pt}(2)) 

where ![alpha](https://latex.codecogs.com/svg.latex?\alpha) is, up to multiplication by a negative constant, the smallest (largest negative) eigenvalue of the matrix ![A](https://latex.codecogs.com/svg.latex?A(t)).

However, for human and long-lived organisms, such behavior (eq. 2) takes place only at a specific moment, namely, at the end of life or in the case of several chronic diseases [4, 5, 9].

## Equations for a limited number of degrees of freedom

In a biological system, interactions of degrees of freedom are highly complex. Given the size of such a system, it is almost impossible to take into account all interactions (moreover, it is physically impossible to obtain this type of data). So, we must use approximate models. For instance, in the works [5, 10], the authors used the transcriptomic profiles and the panel of blood parameters, respectively, and got the same results. Due to the limited data and complexity, we can only consider the dynamics of a separate set of degrees of freedom or physiological units, the so-called "truncated" models. Nevertheless, as mentioned earlier, even this approach gives good results. Moreover, these results indicate that the dropped degrees of freedom do not lead to a strong distortion of the overall picture and can probably be treated as some minor corrections.

## Universality

The beauty of this theory (equation 1) is that calculated  appears to be the same within the margin of error regardless of the type of data (that is, regardless of the selected physiological units) chosen for vector  for a particular species. This is an argument for universal behavior (inherent in systems operating in near-critical mode) taking place: independently of the microscopic structure, the behavior of two systems differing in the choice of so-called physiological units is described by the same quantities (among which the mentioned ).

**We assume that the following setup can shed light on the interconnection between gene expressions and aging and identify genes that determine aging dynamics, whose editing would radically increase lifespan.**

One should obtain time series of gene expression levels for several species and then find cross-correlation between time series for each type of organism. It is a rough approximation of gene-gene expression correlators, but it can be used to get measures of the interactions between genes.
The resulting matrices will reflect interconnections between genes and their change with time and are associated with the matrix  from equation (1), which determines the dynamics of aging itself. Having obtained them, we will next apply network theory and statistical mechanics to uncover underlying causes of aging.

To begin with, we will conduct our analysis on open cross-sectional and longitudinal transcriptomic datasets from databases such as GEO (https://www.ncbi.nlm.nih.gov/geo/) or UK Biobank (https://www.ukbiobank.ac.uk/). We plan to obtain our dataset of longitudinal transcriptomes for human blood or skin cells in the future. Also, we plan to obtain data on changes in expression profiles in response to various interventions, which will allow us to understand the change in the parameters of matrix  in response to various longevity interventions and develop a strategy for combinatorial therapy against aging.

## Dynamics of gene regulatory network in the process of aging: Project aims

Measures of gene expression rates can be a powerful tool to study aging in the context of the dynamics of a gene regulatory network (GRN). The regulation of gene expression involves a complex network of interacting elements. The regulation of gene expression involves a complicated network of interacting elements. At the core of this network are promoters, transcription factor complexes, enhancers, and inhibitors, which all regulate the transcription of genes.

## Methods and theory we are going to apply to the obtained data

**First of all**, analysis of matrix eigenvalues can give us a representation of GRN structure (clustering, existence of cliques, hubsn and other patterns). We can analyze how gene-gene correlations change in time and try to determine possible conservation laws and then interpret our results from a biological point of view. An evolution of matrix structure in time can indirectly describe aging.

**Secondly**, we can speak about chaotic behavior and bifurcations in GRN dynamics by analyzing level spacing distribution. Based on work [5], we assume that this analysis is strongly related to aging. It is a well-known fact that GRN works near criticality [6,7]. We believe it is possible to develop a more rigorous and comprehensive aging model based on the analysis of GRN dynamics and its spectral properties. Our beliefs are supported by the fact that spectral analysis was successfully used for connectome studies and it produced several outstanding results:
The comparative analysis, based on structural connectomes for several organisms - *C. elegans*, macaque, and human, has demonstrated that the human connectome differs from the other connectomes. This difference can be described quantitatively by graph spectra [11].
It was shown that the human connectome operates near criticality, and properties of this network can be captured by the quite simple mathematical model (Kuramoto model) [12].
From these works (and many other works in the field of theoretical neuroscience), it seems pretty clear that complicated dynamics of connectome can be described in terms of relatively simple models whose predictions can be experimentally verified. We should emphasize that all the progress is based only on a few things: 1) existence of appropriate data, 2) correct choice of model degrees of freedom. 

In addition, we believe that the renormalization group method (RG approach) may be helpful. This method has found wide application in statistical physics. It allows us to explore the neighborhood of a critical point and extract information about critical indexes. Critical indexes are a set of values that exhaustively describe the statistical properties of a system near a critical point. For example, in [5], one of the key results is the correlator of time fluctuations. The analysis of the properties of this correlator carried out in the mentioned article is very similar to the classical approach of the renormalization group for phase transitions.

The renormalization group method has already found application in a wide range of condensed matter physics problems (for example, the analysis of phase transitions from a magnetic phase to a non-magnetic one) and soft matter physics (various phase transitions in polymers, including peptides). The ideas of the renormalization group approach go back to dynamic systems, which strengthens our expectation that this approach will be useful for aging models.

It is worth noting that we will not analyze only the time series of transcriptomes. We will also apply our models to blood test datasets, methylomes, proteomes, and metabolomes to check for the property of universality and search for the most accurate and cheap strategy for calculating the biomarker of aging. Also, such omics data as lipidome is very interesting. Technically, such an analysis has become available only recently. The lipid network is interesting for its somewhat isolation from other networks (transcriptome, metabolome, proteome) and greater predictive power concerning certain diseases.

## What issues can be solved by investigating the properties of matrix A (equation 1)?

1. Biomarker of aging for resilient organisms. Groups of genes that determine parameters of stable states and transitions between stable states of long-lived organisms.
2. There are inspiring organisms, such as the naked mole-rat (Heterocephalus glaber), whose cause of death has not yet been identified, and the arctic sea sponge (Anoxycalyx joubini), which belongs to the animal kingdom and lives about 15000 years (Figure 2). The peculiarity of the sponge is the absence of actual tissues and organs; different functions in its organism are performed by various individual cells and cellular layers. What does this mean within the framework of network theory? Does this mean that the genetic regulatory network of the sponge has specific conservation laws? Is the presence of organs - the appearance of another level of organization - a decisive factor that significantly affects the aging process and changes the interaction laws, as happens in particle physics [13]?
3. Selection of combinatorial therapy against aging. In other words, how to theoretically predict changes in the properties of matrix  in response to gene therapy, drug therapy, or other interventions. Is it possible to change the sign of the smallest eigenvalue of matrix  by any intervention, thereby transforming an unstable organism into a stable one? Will we achieve a synergistic effect by selecting a group of drugs that changes distinct eigenvalues of matrix ? How to apply anti-aging interventions correctly in time - is pulse therapy the better strategy?

## The grant money will be spent on:

- Salaries for physicists, bioinformaticians, data scientists
- Experiments (transcriptomic analyses)

