# LinkedBooksMonographs: Citations Dataset

A dataset of citations extracted from monographs about the history of Venice, created in the context of the [LinkedBooks project](http://dhlab.epfl.ch/page-127959-en.html). 

The creation of the dataset and its characteristics are discussed in the article: Colavizza, G., Romanello, M. and Kaplan, F. "The References of References: A Method to Enrich Humanities Library Catalogs with Citation Data." in *International Journal on Digital Libraries*, Springer (forthcoming 2017).

## Provenance
TBD describe the dataset extraction, main results from the article

## Contents

* `LICENCE` MIT
* `README.md` this file
* `Plots.ipynb` a Python notebook to replicate figures 3 and 6 from the article
* `dataset/`
    * [citation_data.json](dataset/citation_data.json) the citation dataset among monographs on the history of Venice
    * [data_description.md](dataset/data_description.md) describes in detail the contents of `citation_data.json`
    * [directed_edges.csv](dataset/directed_edges.csv) the edgelist of the directed citation network. Sep. `;`, Quote `"`. Columns: `"Source";"Target";"Type";"Year"`
    * [directed_nodes.csv](dataset/directed_nodes.csv) the nodelist of the directed citation network. Sep. `;`, Quote `"`. Columns: `"Id";"Bid";"Title";"Author";"LB";"Year";"Consultation"`
    * [node_stats.csv](dataset/node_stats.csv) the in and outdegree distribution of each node in the network. Sep. `;`, Quote `"`. Columns: `"id";"bid";"title";"author";"lb";"year";"consultation";"indegree";"outdegree";"degree"`
    * [territorio.csv](dataset/territorio.csv) basic information about all libraries in the Italian Library System (e.g. library code, coordinates. etc.). This data is openly available at <http://opendata.anagrafe.iccu.sbn.it/territorio.zip>.

## Running the notebook

Assuming that Python is already installed (tested with version 3.5.0), the following depencies need to be installed as well (it will take a moment):

    pip install seaborn
    pip install jupyter

Then launch the notebook server with

    jupyter notebook

A new browser/tab will open pointing at Jupyter's starting page.

## Linked Books Team at EPFL, DHLAB
Giovanni Colavizza, Matteo Romanello, Martina Babetto, Silvia Ferronato.

## Acknowledgements
This work would not have been possible without the help of several Italian institutions of culture. 
In alphabetical order we thank: the Ca’Foscari University Library System and the Ca’Foscari University Humanities Library (BAUM), the Central Institute for the Union Catalogue of Italian Libraries and Bibliographic Information (ICCU), the European Library of Information and Culture (BEIC), the Istituto Veneto di Scienze Lettere ed Arti, the Marciana Library, the State Archive of Venice.

The project is supported by the Swiss National Fund, with grants 205121_159961 and P1ELP2_168489.

## Please cite as

Matteo Romanello, & Giovanni Colavizza. (2017). dhlab-epfl/LinkedBooksMonographs: LinkedBooksMonographs (version 1.0) [Data set]. Zenodo. http://doi.org/10.5281/zenodo.266889

    @misc{matteo_romanello_2017_266889,
      author       = {Matteo Romanello and
                      Giovanni Colavizza},
      title        = {{dhlab-epfl/LinkedBooksMonographs: 
                       LinkedBooksMonographs (version 1.0)}},
      month        = feb,
      year         = 2017,
      doi          = {10.5281/zenodo.266889},
      url          = {https://doi.org/10.5281/zenodo.266889}
    }