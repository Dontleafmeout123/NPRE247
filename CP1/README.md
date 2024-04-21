# NPRE247

Computational Project 1 deals with a three-component decay chain. The CodeOutput program reads the input file, labeled Sample Input File.txt, and creates an output file with all of the relevant data, in the JSON format. The CodeGraph program then reads the output JSON file and graphs it. The input file will have the data all listed out, and to change the parameters, just open the file and change the relevant numbers. The sample parameters include the word stable for the decay of element C, which represents the fact that C does not decay. The words after the numbers are for human understanding of units, not for the program, so changing them will not do anything. There will be two programs one for generating the output file and one for generating the plots. Initially, you can run the two programs with the example data to generate the output file and associated graphs.

The CodeOutput jupyter notebook is responsible for taking the input parameters and generating data sets for the output JSON file that can then easily be converted into graphs. It does so by reading in the data using "with open". It then gets the decay constants from the half-lives. Using the input parameters and the decay constants all of the datasets are generated for the three graphs. This includes the numerical solutions and scatter plot information for the Maximum Time graphs. The data for each graph is organized into its own dictionary and all of the information for all of the graphs is dumped into a JSON file. 

The output file is organized into a lot of dictionaries which is nice as dictionaries allow the array of data points to be preceded by a label, that explains what the data is for. This organization is cleaner and simpler. 

Finally, the CodeGraph jupyter notebook reads the output file and creates the graphs, it also saves them to the imgs folder present in this repository. The graphs it creates are interactive, so the user can move the graph around and zoom into the important parts should they require it. The tile can be changed near the bottom of each section to save different graphs effectively

(The ipynb_checkpoints are autogenerated)
