# Data Matching software

This is a list of (Fuzzy) Data Matching software. The software in this list is open source and/or freely available.

The term data matching is used to indicate the procedure of bringing together information from two or more records that are believed to belong to the same entity. Data matching has two applications: (1) to match data across multiple datasets and (2) to match data within a dataset. See the [Wikipedia page](https://en.wikipedia.org/wiki/Record_linkage) about data matching for more information. 

*Similar terms:* record linkage, data matching, deduplication, fuzzy matching, entity resolution

This list is licensed under [CC-BY-SA 3.0](http://creativecommons.org/licenses/by-sa/3.0/).

| Software                                                        | API    | GUI | License            |
|:----------------------------------------------------------------|:-------|:----|:-------------------|
| [Dedupe](#dedupe)                                               | Python | No  | MIT                |
| [fastLink](#fastlink)                                           | R      | No  | GPL-3.0            |
| [FEBRL](#febrl)                                                 | Python | Yes | ANUOS-1.3          |
| [FRIL](#fril)                                                   | Java   | Yes | MIT                |
| [FuzzyMatcher](#fuzzymatcher)                                   | Python | No  | MIT                |
| [JedAI](#jedai)                                                 | Java   | Yes | Apache License 2.0 |
| [PRIL](#pril)                                                   | SQLPL  | No  | MIT                |
| [Python Record Linkage Toolkit](#python-record-linkage-toolkit) | Python | No  | GPL-3.0            |
| [RecordLinkage (R)](#recordlinkage-r)                           | R      | No  |                    |
| [RELAIS](#relais)                                               | Java   | Yes | EUPL-1.1           |
| [The Link King](#the-link-king)                                 | SAS    | Yes |                    |


## Software

- [Dedupe](https://github.com/dedupeio/dedupe) - Dedupe is a python library for fuzzy matching, deduplication and entity resolution on structured data. The library makes use of active learning to match record pairs. Active learning is useful in cases without training data. Dedupe has a side-product for deduplicating CSV files, [csvdedupe](https://github.com/dedupeio/csvdedupe), through the command line. Dedupeio also offers commercial products for data matching.  [[source code]](https://github.com/dedupeio/dedupe) `MIT` `Python`

- [fastLink](https://cran.r-project.org/web/packages/fastLink/index.html) - Implements a Fellegi-Sunter probabilistic record linkage model that allows for missing data and the inclusion of auxiliary information. This includes functionalities to conduct a merge of two datasets under the Fellegi-Sunter model using the Expectation-Maximization algorithm. fastLink is a programming API written in R. ([Enamorado, Fifield & Imai, 2017](http://imai.princeton.edu/research/files/linkage.pdf))  [[source code]](https://github.com/kosukeimai/fastLink) `GPL-3.0` `R`

- [FEBRL](https://sourceforge.net/projects/febrl/) - Febrl (Freely Extensible Biomedical Record Linkage) is a training tool suitable for users to learn and experiment with record linkage techniques, as well as for practitioners to conduct linkages with data sets containing up to several hundred thousand records. Febrl is a data matching tool with a large number of algorithms implemented and offers a Python programming interface as well as simple GUI. Febrl doesn't offer unsupervised and active learning algorithms. The software is now longer actively maintained. ([Christen, 2008](http://crpit.com/confpapers/CRPITV80Christen.pdf)) [[source code]](https://sourceforge.net/projects/febrl/) `Python`

- [FRIL](http://fril.sourceforge.net/) - FRIL (Fine-grained Records Integration and Linkage tool) is free tool that enables record linkage through a GUI. The tool implements automatic weights estimation through the EM-algorithm and offers serveral techniques to make record pairs. FRIL was developed by the Emory University and is not longer maintained. [[source code]](http://fril.sourceforge.net/download.html) `Java`

- [FuzzyMatcher](https://pypi.python.org/pypi/fuzzymatcher) - A Python package that allows the user to fuzzy match two pandas dataframes based on one or more fields in common. The functionality is limited at the moment. `MIT` `Python`

- [JedAI](http://jedai.scify.org/) Java gEneric DAta Integration (JedAI) Toolkit is a Entity Resolution Tool developed by a group of univeristies. JedAI offers a Graphical User Interface. [[source code]](https://github.com/scify/JedAIToolkit) `Apache License 2.0` `Java` 

- [PRIL](https://github.com/LSHTM-ALPHAnetwork/PIRL_RecordLinkageSoftware) - PRIL (Point-of-contact Interactive Record Linkage) is a record linkage program with a GUI. PRIL can be used to link datasets about individuals. ([Rentsch CT, Kabudula CW, Catlett J et al., 2017](https://gatesopenresearch.org/articles/1-8/v1)) [[source code]](https://github.com/LSHTM-ALPHAnetwork/PIRL_RecordLinkageSoftware) `MIT` `SQLPL`

- [Python Record Linkage Toolkit](https://github.com/J535D165/recordlinkage) - The Python Record Linkage Toolkit is a library to link records in or between data sources. The toolkit provides most of the tools needed for record linkage and deduplication. The package is developed for research and the linking of small or medium sized files. [[source code]](https://github.com/J535D165/recordlinkage) `GPL-3.0` `Python`

- [RecordLinkage (R)](https://cran.r-project.org/web/packages/RecordLinkage/index.html) - Package written in R that provides functions for linking and de-duplicating data sets. Both supervised and unsupervised classification algorithms are available. Record pairs can be compared with a limited set of algorithms. The package is published on CRAN. `GPL-3.0` `R`

- [RELAIS](http://www.istat.it/en/tools/methods-and-it-tools/processing-tools/relais) - RELAIS (REcord Linkage At IStat) is a toolkit providing a set of techniques for dealing with record linkage projects. IStat is the main producer of official statistics in Italy. `EUPL-1.1` `R/Java`

- [The Link King](http://www.the-link-king.com/) - The Link King’s graphical user interface (GUI) makes record linkage and unduplication easy for beginning and advanced users. The software requires a SAS license. `SAS`

## Outdated/ no longer available

- BigMatch (by USA census) - A record linkage tool for use in matching a very large file against a moderate size file developed by the USA Census Bureau. There are several papers available about this program [(BigMatch, 2007)](https://www.census.gov/srd/papers/pdf/rrc2007-01.pdf) 
