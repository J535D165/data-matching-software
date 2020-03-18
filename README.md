# Data Matching software

- [Overview](#overview)
- [Software](#software)
- [Outdated](#outdated-no-longer-available)
- [Contributing](#contributing)

This is a list of (Fuzzy) Data Matching software. The software in this list is
open source and/or freely available.

The term data matching is used to indicate the procedure of bringing together
information from two or more records that are believed to belong to the same
entity. Data matching has two applications: (1) to match data across multiple
datasets (linkage) and (2) to match data within a dataset (deduplication).
See the [Wikipedia page](https://en.wikipedia.org/wiki/Record_linkage) about
data matching for more information.

*Similar terms:* record linkage, data matching, deduplication, fuzzy matching,
    entity resolution

## Overview

The table below gives a dense overview of data matching software properties.
The properties evaluated are [Application Programming Interface
(API)](https://en.wikipedia.org/wiki/Application_programming_interface),
[Graphical User Interface
(GUI)](https://en.wikipedia.org/wiki/Graphical_user_interface), Linking,
Deduplication, [Supervised
Learning](https://en.wikipedia.org/wiki/Supervised_learning), [Unsupervised
Learning](https://en.wikipedia.org/wiki/Unsupervised_learning) and [Active
Learning](https://en.wikipedia.org/wiki/Active_learning_(machine_learning)).

| Software                                                        | API    |        GUI         |        Link        |       Dedup        | Supervised <br/> Learning | Unsupervised <br/> Learning | Active <br/> Learning |
|:----------------------------------------------------------------|:-------|:------------------:|:------------------:|:------------------:|:-------------------------:|:---------------------------:|:---------------------:|
| [AtyImo](#atyimo)		                                  | PySpark|         :x:	| :white_check_mark: | :white_check_mark: |            :x:            |             :x:               |          :x:          |
| [Dedupe](#dedupe)                                               | Python |        :x:         | :white_check_mark: | :white_check_mark: |    :white_check_mark:     |             :x:             |  :white_check_mark:   |
| [fastLink](#fastlink)                                           | R      |        :x:         | :white_check_mark: |  :grey_question:   |            :x:            |     :white_check_mark:      |          :x:          |
| [FEBRL](#febrl)                                                 | Python | :white_check_mark: | :white_check_mark: | :white_check_mark: |            :x:            |             :x:             |          :x:          |
| [FRIL](#fril)                                                   | Java   | :white_check_mark: | :white_check_mark: |        :x:         |      :grey_question:      |     :white_check_mark:      |          :x:          |
| [FuzzyMatcher](#fuzzymatcher)                                   | Python |        :x:         | :white_check_mark: |        :x:         |            :x:            |     :white_check_mark:      |          :x:          |
| [JedAI](#jedai)                                                 | Java   | :white_check_mark: | :white_check_mark: |  :grey_question:   |    :white_check_mark:     |       :grey_question:       |    :grey_question:    |
| [PRIL](#pril)                                                   | SQL    |        :x:         | :white_check_mark: |  :grey_question:   |      :grey_question:      |       :grey_question:       |    :grey_question:    |
| [Python Record Linkage Toolkit](#python-record-linkage-toolkit) | Python |        :x:         | :white_check_mark: | :white_check_mark: |    :white_check_mark:     |     :white_check_mark:      |          :x:          |
| [RecordLinkage (R)](#recordlinkage-r)                           | R      |        :x:         | :white_check_mark: | :white_check_mark: |    :white_check_mark:     |     :white_check_mark:      |          :x:          |
| [RELAIS](#relais)                                               | :x:    | :white_check_mark: | :white_check_mark: |  :grey_question:   |      :grey_question:      |     :white_check_mark:      |          :x:          |
| [ReMaDDer](#remadder)                                           | :x:    | :white_check_mark: | :white_check_mark: | :white_check_mark: |            :x:            |     :white_check_mark:      |          :x:          |
| [Splink](#splink)                                               | PySpark|        :x:         | :white_check_mark: | :white_check_mark: |            :x:            |     :white_check_mark:      |          :x:          |
| [The Link King](#the-link-king)                                 | :x:    | :white_check_mark: | :white_check_mark: | :white_check_mark: |      :grey_question:      |     :white_check_mark:      |          :x:          |


:white_check_mark: Yes/Implemented
:x: No/Not implemented
:grey_question: Unknown

## Software

This section describes **data matching** software. The software is
alphabetically ordered.

#### [AtyImo](https://github.com/pierrepita/atyimo)
AtyImo implements a mixture of deterministic and probabilistic routines for data
linkage. Initially developed in 2013 to serve as a linkage tool supporting a joint
Brazil–U.K. project aiming at building a large population-based cohort with data
from more than 100 million participants and producing disease-specific data to facilitate
diverse epidemiological research studies. `MIT` `Python` `Spark`
[![GitHub stars](https://img.shields.io/github/stars/pierrepita/atyimo.svg?style=social&label=Star)](https://github.com/pierrepita/atyimo)

#### [Dedupe](https://github.com/dedupeio/dedupe)

Dedupe is a python library for fuzzy matching, deduplication and entity
resolution on structured data. The library makes use of active learning to
match record pairs. Active learning is useful in cases without training data.
Dedupe has a side-product for deduplicating CSV files,
[csvdedupe](https://github.com/dedupeio/csvdedupe), through the command line.
Dedupeio also offers commercial products for data matching.  [[source
code]](https://github.com/dedupeio/dedupe) `MIT` `Python`
[![GitHub stars](https://img.shields.io/github/stars/dedupeio/dedupe.svg?style=social&label=Star)](https://github.com/dedupeio/dedupe)
[![PyPI](https://img.shields.io/pypi/v/dedupe.svg)](https://pypi.python.org/pypi/dedupe/)

#### [fastLink](https://cran.r-project.org/web/packages/fastLink/index.html)

Implements a Fellegi-Sunter probabilistic record linkage model that allows for
missing data and the inclusion of auxiliary information. This includes
functionalities to conduct a merge of two datasets under the Fellegi-Sunter
model using the Expectation-Maximization algorithm. fastLink is a programming
API written in R. ([Enamorado, Fifield & Imai,
2017](http://imai.princeton.edu/research/files/linkage.pdf))  [[source
code]](https://github.com/kosukeimai/fastLink) `GPL-3.0` `R`
[![GitHub stars](https://img.shields.io/github/stars/kosukeimai/fastLink.svg?style=social&label=Star)](https://github.com/kosukeimai/fastLink)
[![CRAN](https://img.shields.io/cran/v/fastLink.svg)](https://cran.r-project.org/web/packages/fastLink/index.html)

#### [FEBRL](https://sourceforge.net/projects/febrl/)

Febrl (Freely Extensible Biomedical Record Linkage) is a training tool
suitable for users to learn and experiment with record linkage techniques, as
well as for practitioners to conduct linkages with data sets containing up to
several hundred thousand records. Febrl is a data matching tool with a large
number of algorithms implemented and offers a Python programming interface as
well as simple GUI. Febrl doesn't offer unsupervised and active learning
algorithms. The software is no longer actively maintained. ([Christen,
2008](http://crpit.com/confpapers/CRPITV80Christen.pdf)) [[source
code]](https://sourceforge.net/projects/febrl/) `Python`

#### [FRIL](http://fril.sourceforge.net/)

FRIL (Fine-grained Records Integration and Linkage tool) is free tool that
enables record linkage through a GUI. The tool implements automatic weights
estimation through the EM-algorithm and offers serveral techniques to make
record pairs. FRIL was developed by the Emory University and is not longer
maintained. [[source code]](http://fril.sourceforge.net/download.html) `Java`

#### [FuzzyMatcher](https://pypi.python.org/pypi/fuzzymatcher)

A Python package that allows the user to fuzzy match two pandas dataframes
based on one or more fields in common. The functionality is limited at the
moment. [[source code]](https://github.com/RobinL/fuzzymatcher) `MIT` `Python`
[![GitHub stars](https://img.shields.io/github/stars/RobinL/fuzzymatcher.svg?style=social&label=Star)](https://github.com/RobinL/fuzzymatcher)
[![PyPI](https://img.shields.io/pypi/v/fuzzymatcher.svg)](https://pypi.python.org/pypi/fuzzymatcher/)

#### [JedAI](http://jedai.scify.org/)

Java gEneric DAta Integration (JedAI) Toolkit is a Entity Resolution Tool
developed by a group of univeristies. JedAI offers a Graphical User Interface.
[[source code]](https://github.com/scify/JedAIToolkit) `Apache License 2.0`
`Java`

#### [PRIL](https://github.com/LSHTM-ALPHAnetwork/PIRL_RecordLinkageSoftware)

PRIL (Point-of-contact Interactive Record Linkage) is a record linkage program
with a GUI. PRIL can be used to link datasets about individuals. ([Rentsch CT,
Kabudula CW, Catlett J et al.,
2017](https://gatesopenresearch.org/articles/1-8/v1)) [[source
code]](https://github.com/LSHTM-ALPHAnetwork/PIRL_RecordLinkageSoftware) `MIT`
`SQLPL`
[![GitHub stars](https://img.shields.io/github/stars/LSHTM-ALPHAnetwork/PIRL_RecordLinkageSoftware.svg?style=social&label=Star)](https://github.com/LSHTM-ALPHAnetwork/PIRL_RecordLinkageSoftware)


#### [Python Record Linkage Toolkit](https://github.com/J535D165/recordlinkage)

The Python Record Linkage Toolkit is a library to link records in or between
data sources. The toolkit provides most of the tools needed for record linkage
and deduplication. The package is developed for research and the linking of
small or medium sized files. [[source
code]](https://github.com/J535D165/recordlinkage) `GPL-3.0` `Python`
[![GitHub stars](https://img.shields.io/github/stars/J535D165/recordlinkage.svg?style=social&label=Star)](https://github.com/J535D165/recordlinkage)
[![PyPI](https://img.shields.io/pypi/v/recordlinkage.svg)](https://pypi.python.org/pypi/recordlinkage/)


#### [RecordLinkage (R)](https://cran.r-project.org/web/packages/RecordLinkage/index.html)

Package written in R that provides functions for linking and de-duplicating
data sets. Both supervised and unsupervised classification algorithms are
available. Record pairs can be compared with a limited set of algorithms. The
package is published on CRAN. `GPL-3.0` `R`
[![CRAN](https://img.shields.io/cran/v/RecordLinkage.svg)](https://cran.r-project.org/web/packages/RecordLinkage/index.html)

#### [RELAIS](https://www.istat.it/en/methods-and-tools/methods-and-it-tools/process/processing-tools/relais)

RELAIS (REcord Linkage At IStat) is a toolkit providing a set of techniques
for dealing with record linkage projects. IStat is the main producer of
official statistics in Italy. `EUPL-1.1` `R/Java`

#### [ReMaDDer](http://remadder.findmysoft.com/)

ReMaDDer is unsupervised free fuzzy data matching software with a GUI.
ReMaDDer is capable to perform fully automatic fuzzy record matching without
human expert intervention, while attaining accuracy of human clerical review.
NOTE: The software is free, but not open source and requires an internet
connection to work.

#### [Splink](https://github.com/moj-analytical-services/splink)

Splink is a Python/PySpark package that implements Fellegi-Sunter's canonical model of
record linkage in Apache Spark. It uses the Expectation Maximisation algorithm to estimate
parameters of the model. It is able to perform linking and deduplication of very large datasets
of tens of millions of records with runtimes of less than an hour. [[source
code]](https://github.com/moj-analytical-services/splink) `MIT` `Python` `Spark`
[![GitHub stars](https://img.shields.io/github/stars/moj-analytical-services/splink.svg?style=social&label=Star)](https://github.com/moj-analytical-services/splink)
[![PyPI](https://img.shields.io/pypi/v/splink.svg)](https://pypi.python.org/pypi/splink/)

#### [The Link King](http://www.the-link-king.com/)

The Link King’s graphical user interface (GUI) makes record linkage and
unduplication easy for beginning and advanced users. The software requires a
SAS license. `SAS`

## Outdated/ no longer available

#### BigMatch (by USA census)

A record linkage tool for use in matching a very large file against a moderate
size file developed by the USA Census Bureau. There are several papers
available about this program [(BigMatch,
2007)](https://www.census.gov/srd/papers/pdf/rrc2007-01.pdf)

## Contributing

Do you know an open source and/or free data matching tool? Please open an
issue or do a Pull Request. The same holds for missing or incomplete
information.

This project is initiated by the author of the [Python Record Linkage
Toolkit](https://github.com/J535D165/recordlinkage) @J535D165. The aim is to
get a list and comparison of data matching software.

This list is licensed under [CC-BY-SA 3.0](http://creativecommons.org/licenses/by-sa/3.0/).
