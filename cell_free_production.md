# cell free production

Design an useful synthetic minimal cell.
Design a system that can perform a function (biosensor, biomanufacturing, research - or any other purpose).
Design all the steps of building and deploying the system: define function, pick components, describe results.

Example solution to the SMC assignment, based on: Lentini, R. et al., 2014. Integrating artificial with natural cells to translate chemical messages that direct E. coli behaviour. Nature communications, 5(May), p.4012.
This paper is among the files I put in this folder: google drive
The example answers are given in italic. To complete the homework, answer all underlined questions.

#### 1. Pick a function.

1A What would your synthetic cell do? What is the input and what is the output.
Expand the sensing capacity of bacteria. Input: theophylline (inert to bacteria). Output of the SMC: IPTG. Output of the whole system: GFP produced in bacteria.
Theophyline Aptamer reference: Martini, L. & Mansy, S.S., 2011. Cell-like systems with riboswitch controlled gene expression. Chemical Communications, 47(38), p.10734.

1B Could this function be realized by cell free Tx/Tl alone, without encapsulation?
No. If the IPTG was not encapsulated, it would go into the bacteria without the need of theophylline-induced membrane channel synthesis, thus the synthetic cell actuator would not exist.

1C Could this function be realized by genetically modified natural cell?
Yes, in this particular case: the theophylline aptamer could be incorporated into transformed gene. This lacks the generality though – it is easier to make SMC than modify bacteria, so in this system single bacteria reporter can be used to detect various small molecules.

1D Describe the desired outcome of your synthetic cell operation. \\ In presence of SMC, bacteria sense theophylline.

#### 2. Design all components that would need to be part of your synthetic cell.   

2A What would be the membrane made of?
Phospholipids + cholesterol.
2B What would you encapsulate inside? Enzymes, small molecules.
Cell free Tx/Tl system, IPTG, gene for membrane transporter under the control of theophylline aptamer
2C Which organism your tx/tl system will come from? is bacterial OK, or do you need mammalian system for some reason? (hint: for example, if you want to use small molecule modulated promotors, like Tet-ON, you need mammalian system.
Bacterial, because of the theophylline riboswitch used as SMC input.
2D How will your synthetic cell communicate with the environment? (hints: are substrates permeable? or do you need to express membrane channel?
The membrane is permeable to the input molecule (theophylline), the output is IPTG that will cross the membrane via the membrane pore created after theophyline-initiated gene expression.   


#### 3. Experimental details
3A List all lipids and genes (bonus: find the specific genes; for example, instead of just saying “small molecule membrane channel” pick actual gene)
Lipids: POPC, cholesterol
Enzymes: bacterial cell free tx/tl
Genes: a-hemolysin (aHL) to encapsulate in SMC,
Biological cells: E.coli transformed with GFP under T7 promoter and a lac operator
3B How will you measure the function of your system?
Measure GFP output of the cells, via flow cytomertry. Alternatively, use enzymatic reporter, like luciferase, and measure bulk output of the enzyme.
Scheme (bonus)
“A picture is worth a thousand words”. The entire homework could be done in one, detailed and annotated scheme showing all the components of your synthetic cell in desired operation.
If possible, please include references (not only original papers, websites are OK too).
Edit
