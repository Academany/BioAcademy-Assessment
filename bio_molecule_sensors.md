# Bio Molecule Sensors

The objective of the homework is to run the Rosetta protein structure prediction simulations and analyze the results.The idea is to get an understanding of how computational protein modeling works, looking at protein structures using a viewer (PyMol or Chimera or Rasmol) and making sense of the squiggles and wiggles. You'll also hopefully appreciate the computing power needed for biomolecular simulations. You'll pick one of the five test cases in the homework folder and run structure prediction calculations. The native structure of all the five test cases has already been solved. So, you can compare your output against the correct answer.

Description of the folder contents The homework/structure_prediction has seven subfolders: 1S12, 1TTZ, 1WHZ, 2HFQ, 2HJJ, database and executable The executable folder contains two executables one each for Mac and Linux. There is no executable for Windows machine. You have to run the calculations on a Mac or Linux terminal. The database folder has a ton of precomputed database files that Rosetta uses for the simulation. The remaining five folders are the test cases. You'll pick one for your homework (feel free to pick more than one). The name of the folder is the PDB (www.rcsb.org) code of the native structure.

Contents of the test case folders (1S12,1TTZ, 1WHZ, 2HFQ, 2HJJ): In each folder you'll find six files. 'XXXX' corresponds to any one of the above PDB codes.

XXXX.200.3mers and XXXX.200.9mers: these are database of short fragments that Rosetta uses to assemble 3D structure customized for this protein.

XXXX.fasta: this is the protein sequence.

XXXX.pdb: this is the experimentally solved native structure.

XXXX.psipred.ss2: this contains the secondary structure propensity at every position.

abrelax_flags: instructions for the Rosetta code and paths to database.

The only file you may have to modify is abrelax_flags. You won't have to touch any of the other files.

Running the calculations Pick one test case. You can look at the native structure topology and size, and may be even function and decide on which one to pick. On a linux or mac terminal, navigate your way to the homework folder. Go to the specific folder of your test case. Open abrelax_flags in your favorite editor. Check to see if the following line is as shown. -database ../database If it says anything else besides ../database change it to ../database

The line -nstruct 100 tells the code to generate a 100 models. The more models you generate, the accurate your result is likely to be. But running more models requires more computing time. So you'll have balance that. The first time see how many hours it takes to generate a hundred models. If you have more free computer time, change the nstruct 100 to a larger number and rerun the calculations.

To the run program, type the following command inside your specific test case folder. If you type this anywhere else the program will not run because its looking for specific files in that folder.

../executable/AbinitioRelax.static.macosclangrelease @abrelax_flags

That should start the program, and it will keep running till it generates a 100 models. If you turn off your computer or close the terminal screen, the job will end. If you are bit linux savvy, you can use the 'nohup' command and free the terminal.

After about 10-15 mins, you should additional files appear in that directory. score.fsc S_000001.pdb, S_000002.pdb etc

The S_ files are the models. The score.fsc file contains energy (in the 'score' column) and distance to native (in the 'rms' column).

Deliverables for homework assignment

#### 1. Plot the score (or energy) vs rms plot. Rms stands for root mean square deviation. These are two columns in the score.fsc file. Compare that with the energy vs rms plots I showed in my slides.

#### 2. Pick the lowest energy model and structurally compare it to the native. How close is it to the native? If its different, what parts did the computer program get wrong? You'll have to compare the structures using a Viewer like pymol or chimera or rasmol.

#### 3. Pick the lowest rms model and structurally compare it to the native. How close is it to the native? If its different, how is it different? Remember that in a blind case, we will not have the benefit of an rms column.
