# LBCC
source code
python#################################################################################################################
1.Software version:

The Python code is written for Python 2.7.

2.The information of files:

complex.txt: the information of protein complexes of Saccharomyces cerevisiae.
deg.txt: the essential proteins of Saccharomyces cerevisiae.
input.txt: the input file(PPI networks)
output.txt: the output file. 
PPI data: the folder contains four input files of PPI networks. 

3.Usage

Running LBCC from command line:

python centrality_cpu.py

If you want to change the input data, please copy the contents of PPI networks into the file "input.txt".

4.Steps to reproduce the analysis

(1) ranking proteins in descending order based on their LBCC values 
(2) selecting the top 100, 200, 300, 400, 500, and 600 proteins as candidate essential proteins
(3) the number of true essential proteins is determined according to attribute ESS in file "output.txt"


c++#######################################################################################################

1.Experimental environment:
Ubuntu 14.04.4 LTS
Linux version 4.2.0-27-generic
gcc version 4.8.2


2.
complex.txt: the information of protein complexes.
deg.txt: the essential proteins.
input.txt: the input file(PPI networks), format(proteinname	proteinname	).
output.txt: the output file. 


3.Usage
Running LBCC from command line:

(1) g++ centrality-cpu.cpp fheap.cpp graph.cpp -o out
(2) ./out

If you want to change the input data, please copy the contents of PPI networks into the file "input.txt".

4.Steps to reproduce the analysis

(1) ranking proteins in descending order based on their LBCC values 
(2) selecting the top 100, 200, 300, 400, 500, and 600 proteins as candidate essential proteins
(3) the number of true essential proteins is determined according to attribute ESS in file "output.txt"
