# README - PanamaPapers Exercise
6 Apr 2016

***

> Introduction

The repo contains datasets collected from the following sources, organised into the folders as follows:

    Folder Name  | Summary | Source Link
    -------------|---------|------------
    rawSrc1      | Direct dl from ICIJ | [source](http://icij-uploads.s3-website-us-east-1.amazonaws.com/2013/10/offshore/csv.zip)
    rawSrc2      | Links integer labels to each activity name. Total of 6 activities.

* rawSrc1:
* rawSrc2: [source](http://www.thereportertimes.com/panama-papers-icij-offshore-leaks-database-documents/23489/)
* rawSrcAmaboura: [Amaboura's github repo for metadata extracted from ICIJ site visualizations](https://github.com/amaboura/panama-papers-dataset-2016)
* rawSummaryGraphs: K-V pairs for the ICIJ [summary graphs](https://panamapapers.icij.org/graphs/) [extracted source](http://pastebin.com/pern5JRF)

Documents pertaining to the datasets background:
* allegedLeakerMailToNYT: [source](http://pastebin.com/rnhwJ7nN)
* [150+ raw documents that were released: [Documentcloud link](https://www.documentcloud.org/public/search/Source:%20%22Internal%20documents%20from%20Mossack%20Fonseca%20%28Panama%20Papers%29%22/p4)

A description of the ETL for rawSrc1 is currently stored in the [project folder](https://github.com/slothdev/panpapers-project/project/)

This project itself focuses on rawSrc1 as those files were directly obtained from the ICIJ source comprising both older and newer information. There are four files which generally have the following relationships:
countriesNW.csv:country_id ===1:n===>  node_countriesNW.csv:NODEID1 ===n:1===> nodesNW.csv:Unique_ID ===1:n===> edges_1DNW.csv:Unique_ID

> Disclaimer

The veracity of the information from the ICIJ-processed source is neither claimed nor disavowed. Any interpretation remains within the readers' discretion.

***
