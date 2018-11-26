# Lattes-data-mining
Script in Python to mine CV Lattes Brazilian information from researchers and then compare it with the Qualis Score

## How it works?
### Lattes info Data Mining
First it gets a list of CV Lattes links from an excel spreadsheet called listalattes.xlsx\
Then, for every line, it performs a Beautiful Soup HTML search\
It them gets the whole list of 'Artigos Completos Publicados em Periódicos'\
By each 'Artigo' if finds:
* Year that was published
* ISSN of the Journal that was published\
### Sucupira QUALIS Score
For each ISSN of 'Artigo' extracted it then compares to the ISSN of the downloaded spreadsheet of all CAPES QUALIS Score\
**You have to insert the specific score guidelines from the CAPES Research Area that you are interested in the dictionary of the code**
### The Output
It outputs a spreadsheet called prod_cis.xlsx with all the information for all of the links in listalattes.xlsx

## Example
In this repository there is an example from the whole faculty of the Master in Smart Cities at Universidade Nove de Julho - UNINOVE, Sao Paulo - Brazil\
There are 14 professor, so there's 14 lines in the listalattes.xlsx\
The QUALIS scoring dictionary and scoring ISSNs are from the *Planejamento Urbano Regional e Demografia* CAPES Area\
The output is a spreadsheet for the Journal Production of the Smart Cities Faculty named prod_cis.xlsx
