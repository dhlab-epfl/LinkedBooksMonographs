# linked_books_citations_monographs_dataset
A dataset of citations among monographs on the history of Venice. The creation of the dataset and its characteristics are discussed in the article: Colavizza, G., Romanello, M. and Kaplan, F. "The References of References: A Method to Enrich Humanities Library Catalogs with Citation Data." Forthcoming in 2017.

# Contents
* `LICENCE` MIT
* `README.md` this file
* `Plots.ipynb` a Python notebook to replicate figures 3 and 6 from the article
* `dataset/`
    * `citation_data.json` the citation dataset among monographs on the history of Venice
    * `data_description.md` describes in detail the contents of `citation_data.json`
    * `directed_edges.csv` the edgelist of the directed citation network. Sep. `;`, Quote `"`. Columns: `"Source";"Target";"Type";"Year"`
    * `directed_nodes.csv` the nodelist of the directed citation network. Sep. `;`, Quote `"`. Columns: `"Id";"Bid";"Title";"Author";"LB";"Year";"Consultation"`
    * `node_stats.csv` the in and outdegree distribution of each node in the network. Sep. `;`, Quote `"`. Columns: `"id";"bid";"title";"author";"lb";"year";"consultation";"indegree";"outdegree";"degree"`

# Provenance
TBD describe the dataset extraction, main results from the article

# Dependencies
Python 3.5

Seaborn

# Linked Books Team at EPFL, DHLAB
Giovanni Colavizza, Matteo Romanello, Martina Babetto, Silvia Ferronato.

# Acknowledgements
This work would not have been possible without the help of several Italian institutions of culture. 
In alphabetical order we thank: the Ca’Foscari University Library System and the Ca’Foscari University Humanities Library (BAUM), the Central Institute for the Union Catalogue of Italian Libraries and Bibliographic Information (ICCU), the European Library of Information and Culture (BEIC), the Istituto Veneto di Scienze Lettere ed Arti, the Marciana Library, the State Archive of Venice.

The project is supported by the Swiss National Fund, with grants 205121_159961 and P1ELP2_168489.

# Please cite as
TBD