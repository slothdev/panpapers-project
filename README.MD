# README - PP Exercise
### 6 Apr 2016
### SPS

> Updates

13 Apr 2016: Pls refer to http://www.unicornriot.ninja/?p=5357 for a detailed description of the nature of the leak (it is the CMS portal belonging to the law firm which they used to store/manage their clients' entities' documents, as well as allowing their clients to access them.) Presumably, the ICIJ datasets released as graph info are built upon processing of the raw documents found in this document store.

***

> Introduction

The repo contains datasets collected from the following sources, organised into the folders as follows:

    Folder Name       | Summary                                     | Source
    ------------------|---------------------------------------------|------------
    rawSrc1           | Direct dl from ICIJ containing old/new info | [link](http://icij-uploads.s3-website-us-east-1.amazonaws.com/2013/10/offshore/csv.zip)
    rawSrc2           | Slightly different set with only node/edge files | [link](http://www.thereportertimes.com/panama-papers-icij-offshore-leaks-database-documents/23489/)
    rawSrcAmaboura    | Amaboura's github repo for metadata extracted from ICIJ site visualizations | [link](https://github.com/amaboura/panama-papers-dataset-2016)
    rawSummaryGraphs  | K-V pairs for the ICIJ [summary graphs](https://panamapapers.icij.org/graphs/) | [link](http://pastebin.com/pern5JRF)

Documents pertaining to the datasets background:

    Folder Name   | Summary                                       | Source
    --------------|-----------------------------------------------|------------
    docEmailNYT   | Alleged email exchange between leaker and NYT | [link](http://pastebin.com/rnhwJ7nN)
    N.A.    | Documentcloud of 150+ raw documents released  | [link](https://www.documentcloud.org/public/search/Source:%20%22Internal%20documents%20from%20Mossack%20Fonseca%20%28Panama%20Papers%29%22/p4)

This project only focuses on rawSrc1 as those files were directly obtained from the ICIJ source comprising both older and newer information. There are four files which generally have the following relationships:

countriesNW.csv:country_id ===1:n===>  node_countriesNW.csv:NODEID1 ===n:1===> nodesNW.csv:Unique_ID ===1:n===> edges_1DNW.csv:Unique_ID

A more detailed description of the ETL for rawSrc1 is currently stored in the [project folder](https://github.com/slothdev/panpapers-project/etl/)

The "papers" themselves appeared to have been taken through the law firm's Drupal CMS [see link in French](https://reflets.info/panamapapers-how-shit-happens)

> Disclaimer

The veracity of the information from the ICIJ-processed source is neither claimed nor disavowed. Any interpretation remains within the readers' discretion.

***
