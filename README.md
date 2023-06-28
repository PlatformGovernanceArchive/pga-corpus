# PGA v1 Dataset

This is the original PGA dataset. Data has been collected retrospectively by a combination of automated and manual approaches., building on Internet Archive’s [Wayback Machine](https://web.archive.org/). It includes policies by four major platforms ranging back to their founding years. 

**Platforms:** Facebook, Instagram, Twitter, YouTube

**Time Frame:** 2005-2021

**Project Website:** [http://platformgovernancearchive.uni-bremen.de](http://platformgovernancearchive.uni-bremen.de)

### Using the Data

We are more than happy if you want to use our dataset in your research, reporting, and explorations. If you do:

1. Consult the respective data documentation;
2. reference this project and the actual dataset;
3. send us a note so that we include you in our research and output page. 

PGA v1 is made available under the [Open Data Commons Attribution License](http://opendatacommons.org/licenses/by/1.0/) (that means what we say above: use it, but reference us).

**Cite the Dataset**

Katzenbach, C., Kopps, A., Magalhaes, J. C., Redeker. D., Sühr, T. (2023). Platform Governance Archive (PGA) v1. [data set]. DOI: [10.17605/OSF.IO/XSBPT](https://doi.org/10.17605/OSF.IO/XSBPT). URL: http://platformgovernancearchive.uni-bremen.de/data/dataset-pga-v1-historical-dataset/.

**Cite a Single Document (recommended)**

Name of platform. (Date of version). *Name of policy*. Platform Governance Archive. Direct URL. 

### Documentation

#### Data Paper

The full documentation is available as a data paper: 

Katzenbach, C., Kopps, A., Magalhaes, J. C., Redeker. D., Sühr, T., Wunderlich, L. (2023). *The Platform Governance Archive v1 – A longitudinal dataset to study the governance of communication and interactions by platforms and the historical evolution of platform policies*. Centre for Media, Communication and Information Research (ZeMKI), University of Bremen. https://doi.org/10.17605/OSF.IO/XSBPT.

#### The dataset on Github

The Github repositories of the Platform Governance Archive provide detailed access to the PGA corpus as well as to research data and instruments that we used in the process, including the URL list, scripts and the datasets before the data cleaning processes.

This part of the archive consists of two repositories: 

- **[/pga-corpus](https://github.com/PlatformGovernanceArchive/pga-corpus)** (the final corpus of all identified policy versions)
- **[/pga-workbench](https://github.com/PlatformGovernanceArchive/pga-workbench)** (providing tools, and data that we used in the research process)

The generic naming convention for files is that filename bears the timestamp of the documents. This timestamp denotes the point in time when they were registered by the system. This does not necessarily match the exact date of when they were published or became effective. As the scraping was limited to a maximum of one new version per week, there are often a few days in between the actual publishing date and the date of registration by the system. This means that a document can mention a date of effectiveness that comes before the date in the name of the file. 

#### **/pga-corpus** 

The [/pga-corpus repository](https://github.com/PlatformGovernanceArchive/pga-corpus) is structured as followed: 

| **Folder**                                                   | **Description**                                              | **Format**                                 | **Units** | **Potential Use Cases**                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------ | --------- | ------------------------------------------------------------ |
| [pga-corpus/Versions](https://github.com/PlatformGovernanceArchive/pga-corpus/tree/main/Versions) | Final dataset containing all identified historical policy versions | PDF (individual & merged), HTML & Markdown | 1,071     | Analysis of the historical evolution of platform policies; analysis of the evolution of specific policy sections/provisions |

In addition to the individual versions, we also provide an overall PDF file for each policy which contains all historical versions of a policy in one file. 

#### **/pga-workbench**

In [/pga-workbench](https://github.com/PlatformGovernanceArchive/pga-workbench) we provide the following data and tools: 

| **Folder**                                                   | **Description**                                              | **Format**           | **Units** | **Potential Use Cases**                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ | -------------------- | --------- | ------------------------------------------------------------ |
| [pga-workbench/URL List ](https://github.com/PlatformGovernanceArchive/pga-workbench/tree/main/URL List ) | List of all the URLs at which the policies where stored over time which served as the basis for scraping the WBM | CSV                  | 1         | Reproducing our data collection process; investigating URL changes |
| [pga-workbench/Snapshots](https://github.com/PlatformGovernanceArchive/pga-workbench/tree/main/Snapshots) | All policy snapshots that were scraped from the WBM as part of the first data collection step (4.2) | PDF, HTML & Markdown | 15,039    | Reproducing our data cleaning process, Applying a different document filtering process; investigating the visual appearance of past platform policies |
| [pga-workbench/Diffcheck](https://github.com/PlatformGovernanceArchive/pga-workbench/tree/main/Diffcheck ) | Comparison view of the automated diff-check                  | HTML & Markdown      | 9,636     | Reproducing our data cleaning process, Applying a different document filtering process |
| [pga-workbench/Scripts ](https://github.com/PlatformGovernanceArchive/pga-workbench/tree/main/Scripts) | Scripts that were used for the automated scraping (miner), the creation of document types & automated diffchecking (convert versions) and for the creation of the plots (plots) in chapter 6 | IPYNB                | 3         | Reproducing and further understanding our data collection process |
| [pga-workbench/Plots](https://github.com/PlatformGovernanceArchive/pga-workbench/tree/main/Plots) | Heatmaps and graphs about the development of the change frequency and wordcount of the overall PGA corpus, as well as by platform & policy type | SVG & PNG            | 35        | Analysis and visualisation of the overall development of the PGA corpus; identification of general trends; comparative analysis between policy types/platforms |
