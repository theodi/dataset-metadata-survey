# Dataset Metadata Survey

This repo is the result of the ODI tech team's investigations into the different metadata standards in use to describe datasets. It is made up of three parts:

* Looking into the [types and methods of metadata publishing](https://github.com/theodi/dataset-metadata-survey/blob/master/metadata_survey.md)
* [Finding commanalities in each method and matching them with questions in the Open Data Certificate](https://github.com/theodi/dataset-metadata-survey/blob/master/metadata.csv)
* Seeing [what datastores use what schema, and how the metadata can be reached](https://github.com/theodi/dataset-metadata-survey/blob/master/datastores.csv)

We found that if a datastore uses DCAT, we could potentially match:

* 6/18 requirements for basic level
* 5/26 requirements for pilot level
* 3/24 requirements for standard level
* 2/16 requirements for exemplar level

However, some questions, such as if a dataset is machine readable or not, can be gleaned from things such as the format of the data.

We also found that very few of datastores we surveyed contained much usable metadata, although [data.gov.uk](http://data.gov.uk), [the Beta Ordnance Survey Open Data Linked Data Platform](http://beta.data.ordnancesurvey.co.uk) and [Open Data Communities](http://opendatacommunities.org/) have a good chunk of metadata available for analysis.