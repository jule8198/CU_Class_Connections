# CU_Class_Connections
Web scraping University of Colorado course catalogue for class information and description.
Completed as final project for CSCI 4022 Advanced Data Science for Spring 2022 under Dr. Zach Mullen
The workflow for data collection and HITS is in the courses_nb notebook.

## Web Scraper
Uses Beautifulsoup package to scrape course information for each department.
Store urls to each department in course_urls.txt
Dictionary stored in course_info.json

## Analysis
### HITS
Creates directed graph of required and recommended prerequsites and equivalent classes.
dfdrop.pkl is pandas dataframe of adjacency matrix, dfdrop is dataframe that excludes classes with no edges.
Ran HITS algorithm. Eigenvalue and eigenvectors stored in auts.npy and hubs.npy
Graph rendered through networkx package shown [here](output.png).


### TF-IDF
Ran TF-IDF vectorization through sklearn. Used cosine similarity for distance between courses.
Workflow stored in course_sim.


### Results
See the [presentation](Class%20Connections.pdf) for the findings.
