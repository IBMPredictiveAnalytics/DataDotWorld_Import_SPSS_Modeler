# DataDotWorld_Import_SPSS_Modeler

This extension allows you to import datasets from [Data.World](https://data.world/) onto SPSS Modeler stream.

## Requirements

This extension requires the following
* IBM SPSS Modeler v18.1.1 or later
* IBM SPSS Modeler "Integration Plug-In for R"
* R v3.3.3

## Installation Instructions

This extension can be downloaded from the [Extension Hub](https://ibmpredictiveanalytics.github.io/)

## R packages used

This plugin will install the following R packages : 

* [Data.World](https://CRAN.R-project.org/package=data.world)
* [dwapi](https://CRAN.R-project.org/package=dwapi)
* [Properties](https://CRAN.R-project.org/package=properties)
* [stringr](https://CRAN.R-project.org/package=stringr)
* [httr](https://CRAN.R-project.org/package=httr)


## Other Requirements

This extension requires a Data.World Authentication Token. This token can be obtained from [here](https://data.world/settings/advanced)

## Steps

1. Download the extension from the Extension Hub

2. Click on the File Menu -> New Stream to create a new SPSS Modeler stream.

3. From the "Sources" node palette, drag drop "ImportDataDotWorld" onto the new stream. Configure the Data.World import node with the following settings :<br>
    a. Data.World [authentication token](https://data.world/settings/advanced). This needs to be entered only the first time the extension is used.<br>
    b. Data.World Dataset URL - https://data.world/zika-virus-data/census<br>
    c. Data.World SQL - select * from poverty_median_income_2014<br>
![Image 1](/Resources/SPSS_Image_1.png)

4. From the "Output" node palette, drag drop "Table" node onto the new stream. Select the "ImportDataDotWorld" node, click F2 and connect it to the "Table" node.<br>
![Image 2](/Resources/SPSS_Image_2.png)

5. Execute the stream by clicking on the green play button<br>
![Image 3](/Resources/SPSS_Image_3.png)    
    
 ## Authors
 
* Deepak Rangarao
* Amod Upadhye

## Contact Information
For any issues while using this extension, please raise an issue on GitHub or send us an <a href="mailto:h6u9j3n4w2n7k6i7@ibm-analytics.slack.com">Email</a>
