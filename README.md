# MSMP+-B

This research is an extension on the MSMP+, where we include the brand names in the process of the binary vectorization and a more thorough data cleaning procedure.

## MSMP+:
An LSH-Based Model-Words-Driven Product Duplicate Detection Method
Aron Hartveld, Max van Keulen, Diederik Mathol, Thomas van Noort Thomas Plaatsman, Flavius Frasincar, and Kim Schouten

## How to run
In order to run the code, open the python script and run the code blocks in the order they are in. Once you run the code in the main, the results will start computing. Make sure to upload your file path in the environment if you run this via google colab.

## Summary of the code
First we download and import the necessary packages. 
After this we have the functions related to the cleaning of the json file. Via this way we obtain a cleand json file. In this cleaning we extended the MSMP+ by cleaning more units
Then we compute the binary represenation of the data using a binary vectorization of the dictionaries of the tvs. Our main extension is being done here, by including the brand names in the dictionaries.
Using this binary matrix we then compute the signature matrix in the minhashing code block
We then perform LSH on this signature matrix.
In the baseline code block we have the functions used to compute the MSMP+ results.
The MSM code block contains all the functions related to the MSM. Beware that these functions may contain mistakes as we did not manage to get optimal results.
In the metrics code block we compute the PQ, PC, F1star and F1
In the bootstrapping code block we compute the functions putting all the above code together. You should run these to get the PC, PQ, F1star and F1 results.
Afterwards we have the functions to plot the results.
At last we have the main, which you should run if you want to obtain all the results and graphs.
