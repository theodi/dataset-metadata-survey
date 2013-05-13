# Metadata survey

## [CKAN API](http://docs.ckan.org/en/latest/api.html)

* Easy to parse JSON representation
* Licence given with URI and identifier
* Each resource has URIs, file size, and last updated fields
* Tags
* Temporal and Geographic granularity

* Difficult to 'follow your nose' (at least on data.gov.uk), as there is no link header, or machine readable way to get to the API representation from the website


### Examples of usage:

* [www.data.gov.uk](http://www.data.gov.uk)
* [www.datagm.org.uk](http://www.datagm.org.uk/)

## Link Header

* Works well in combination with an API
* Returns a license with `rel=licence` in the HTTP header
* We could sniff for this on requests, but is more generally given with the actual data, rather than information about the data

### Examples of usage:

* [beta.data.ordnancesurvey.co.uk](http://beta.data.ordnancesurvey.co.uk)

## HTTP Link Rel Header

* Easy to sniff
* Uses widely recognised standards

* No guarantee on the format you'll get out

### Examples of usage

* [www.data.gov.uk](http://www.data.gov.uk) - Gives RDF in DCAT format

## RDFa

* Using the [DCAT schema](https://dvcs.w3.org/hg/gld/raw-file/default/dcat/index.html) to describe datasets within the HTML
* No redirects involved, the page about the data describes the data without headers
* Can be easily interrogated

No current examples of usage, but data.gov.uk planning to

## Microdata / Schema.org

* As above, but using the [schema.org Dataset schema](http://www.w3.org/wiki/WebSchemas/Datasets)
* Same advantages as above, but not quite as in depth as DCAT (things like licence and more advanced RDF stuff are missing)

No current examples of usage, but data.gov.uk planning to

## [Datapackages](http://www.dataprotocols.org/en/latest/data-packages.html)

* Simple metadata standard, designed to be packaged with a CSV file
* Based on DSPL
* Simple, evolving standard
* Can be applied to web pages, Git repositories - anything on the web

## [DSPL](https://developers.google.com/public-data/)

* Designed to allow data to be uploaded to the Google Public Data repository
* Allows CSV fields to be mapped to concepts
* Powerful, but seems to be related to one aim, and designed just for uploading to Google's servers in a ZIP file.