# Feature_Network_Project
Network Project for ORF 387

The data file that are missing are "hot100.csv" and "mbz_feature_edges_billboard_only.csv" as they were too large for github. Feel free to use any csv with artist names for the hot100.csv file. The main code will output the mbz_feature_edges_billboard_only.csv but depending on the size of the input csv, it can take a few hours to run.

First run the main.ipynb file. This file  pulls artists from the hot100.csv and fuzzy matches them to musicbrainz aritst names. It then pulls the features for these artists and appends them to a csv. Reports are made to show which artists could not be efectively lined up and so were missed.

The edge csv is then used for the genre analysis and then the spectral clustering (network analysis file) in that order. These files first use the genres json file to match artists up with their respective genres and then perform a range of analysis. They look at individual artists rankings and construct various graphs both all of the artists and genre specific graphs. It outputs a range of files that can be visualized using the Gephi tool. 

We used the following packages:
difflib
json
musicbrainzngs
networkx
os
pandas
re
time
unicodedata
matplotlib.pyplot
