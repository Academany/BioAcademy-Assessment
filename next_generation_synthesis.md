# Next Generation Synthesis

### Homework Assignment #1: Primer design to linearize plasmid backbone  

* Theory: Use NuPack to help select 18 bp priming sites that amplify a ~2.25 kb region of pUC19 (NEB) immediately upstream of the plac promoter and downstream of the start of lacZalpha. The resulting amplicon excludes the plac promoter and n-terminus of lacZalpha, which enables you to swap in a gene of interest under the control of a promoter of interest using Gibson Assembly later on in your workflow. Design one pair of oligos that prime optimally and another that prime poorly. Describe the PCR thermocycling program that uses Phusion polymerase (NEB) for these pairs. Crucially, determine annealing temperatures and extension times.  

Helpful readings:  
* PCR intro
* Primer Design  

### Nupack task check list:  
* Number of strand species >= 2 for combinations of primers and ~50bp regions from pUC19 containing their reverse compliment
* Sizes of complexes >= 2 to check self-hybridization, hybrid primer dimers and annealing to target  
* Primer and DNA concentrations are in a range suitable for PCR rx mixture
* Melt range includes several points in Phusion's annealing temperature range
* Experiment: PCR amplification using combinations of optimal/poor priming sites and exo+/- DNA polymerase. Readout with agarose gel andSanger sequencing (GeneWiz).  

#### Extra Credit: Identify sequences elsewhere on pUC19 that most closely match your primers. Use Nupack to assess the likelihood of off-target amplicons.


### Homework Assignment #2: Build a gene from shorter gene synthesis fragments  
* Theory: Recode a fluorescent reporter and use NuPack to help design 200-300 bp IDT gBlocks for building the reporter with Gibson Assembly. Check that your 15-30 bp overlaps do not fold into undesirable secondary structure during the isothermal reaction.  

Helpful readings:  
* Codon Table  
* Gibson Assembly  
* Linear backbone usage  
* Experiment: Assemble and amplify gene to readout on gel.  

####Extra Credit: Assemble into linearized pUC19 with a promoter plus RBS to express in E coli.  
Pass = design assignment from homework 1 and 2, experiments etc. are optional (but recommended)
