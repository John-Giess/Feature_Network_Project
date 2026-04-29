# Feature_Network_Project
Network Project for ORF 387

Data file are missing "hot100.csv" and "mbz_feature_edges_billboard_only.csv" as they were too large for github
First run the main.ipynb file. This file  pulls artists from the hot100.csv and fuzzy matches them to musicbrainz aritst names. It then pulls the features for these artists and appends them to a csv. Reports are made to show which artists could not be efectively lined up and so were missed. Other csvs of artists could be used instead of the billboard list. 

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