# Data Matching software

- [Overview](#overview)
- [Software](#software)
- [Outdated](#outdated-no-longer-available)
- [Contributing](#contributing)

This is a list of (Fuzzy) Data Matching software. The software in this list is
FOSS (Free and open-source software).

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
| [hlink](#hlink)                                                 | PySpark|        :x:         | :white_check_mark: |  :grey_question:   |            :x:            |            :x:              |          :x:          |
| [JedAI](#jedai)                                                 | Java   | :white_check_mark: | :white_check_mark: |  :grey_question:   |    :white_check_mark:     |       :grey_question:       |    :grey_question:    |
| [PRIL](#pril)                                                   | SQL    |        :x:         | :white_check_mark: |  :grey_question:   |      :grey_question:      |       :grey_question:       |    :grey_question:    |
| [Python Record Linkage Toolkit](#python-record-linkage-toolkit) | Python |        :x:         | :white_check_mark: | :white_check_mark: |    :white_check_mark:     |     :white_check_mark:      |          :x:          |
| [RecordLinkage (R)](#recordlinkage-r)                           | R      |        :x:         | :white_check_mark: | :white_check_mark: |    :white_check_mark:     |     :white_check_mark:      |          :x:          |
| [Reclin2](#reclin2)                           | R      |        :x:         | :white_check_mark: | :white_check_mark: |    :white_check_mark:     |     :x:      |          :x:          |
| [RELAIS](#relais)                                               | :x:    | :white_check_mark: | :white_check_mark: |  :grey_question:   |      :grey_question:      |     :white_check_mark:      |          :x:          |
| [ReMaDDer](#remadder)                                           | :x:    | :white_check_mark: | :white_check_mark: | :white_check_mark: |            :x:            |     :white_check_mark:      |          :x:          |
| [RLTK](#rltk) | Python |        :x:         | :white_check_mark: | :white_check_mark: |    :white_check_mark:     |     :x:      |          :x:          |
| [Splink](#splink)                                               | Python |        :x:         | :white_check_mark: | :white_check_mark: |    :white_check_mark:     |     :white_check_mark:      |          :x:          |
| [Zingg](#zingg)                                               | Python|        :x:         | :white_check_mark: | :white_check_mark: |            :white_check_mark:            |      :x:     |          :x:          |
| [dirty-cat](#dirty-cat)                                               | Python|        :x:         | :white_check_mark: | :white_check_mark: |            :white_check_mark:            |      :white_check_mark:     |          :x:          |

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
diverse epidemiological research studies. 

|  |  |
|---|---| 
| License | ![GitHub](https://img.shields.io/github/license/pierrepita/atyimo) |
| Language | `Python` `Spark` | 
| Latest release | NA |
| Downloads per month |  |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/pierrepita/atyimo.svg?style=social&label=Star)](https://github.com/pierrepita/atyimo) |

#### [Dedupe](https://github.com/dedupeio/dedupe)

Dedupe is a python library for fuzzy matching, deduplication and entity
resolution on structured data. The library makes use of active learning to
match record pairs. Active learning is useful in cases without training data.
Dedupe has a side-product for deduplicating CSV files,
[csvdedupe](https://github.com/dedupeio/csvdedupe), through the command line.
Dedupeio also offers commercial products for data matching.  

|  |  |
|---|---| 
| License | ![PyPI - License](https://img.shields.io/pypi/l/dedupe) |
| Language | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dedupe) | 
| Latest release | [![PyPI](https://img.shields.io/pypi/v/dedupe.svg)](https://pypi.python.org/pypi/dedupe/) |
| Downloads per month | ![PyPI - Downloads](https://img.shields.io/pypi/dm/dedupe) |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/dedupeio/dedupe.svg?style=social&label=Star)](https://github.com/dedupeio/dedupe) |

#### [fastLink](https://cran.r-project.org/web/packages/fastLink/index.html)

Implements a Fellegi-Sunter probabilistic record linkage model that allows for
missing data and the inclusion of auxiliary information. This includes
functionalities to conduct a merge of two datasets under the Fellegi-Sunter
model using the Expectation-Maximization algorithm. fastLink is a programming
API written in R. ([Enamorado, Fifield & Imai,
2017](http://imai.princeton.edu/research/files/linkage.pdf))  [[source
code]](https://github.com/kosukeimai/fastLink) 

|  |  |
|---|---| 
| License | ![CRAN/METACRAN](https://img.shields.io/cran/l/fastLink) |
| Language | `R`  | 
| Latest release | [![CRAN](https://img.shields.io/cran/v/fastLink.svg)](https://cran.r-project.org/web/packages/fastLink/index.html) |
| Downloads per month | [![metacran downloads](https://cranlogs.r-pkg.org/badges/last-month/fastLink)](https://cran.r-project.org/package=fastLink) |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/kosukeimai/fastLink.svg?style=social&label=Star)](https://github.com/kosukeimai/fastLink) |

#### [FEBRL](https://sourceforge.net/projects/febrl/)

Febrl (Freely Extensible Biomedical Record Linkage) is a training tool
suitable for users to learn and experiment with record linkage techniques, as
well as for practitioners to conduct linkages with data sets containing up to
several hundred thousand records. Febrl is a data matching tool with a large
number of algorithms implemented and offers a Python programming interface as
well as simple GUI. Febrl doesn't offer unsupervised and active learning
algorithms. The software is no longer actively maintained. ([Christen,
2008](http://crpit.com/confpapers/CRPITV80Christen.pdf)) [[source
code]](https://sourceforge.net/projects/febrl/)

|  |  |
|---|---| 
| License | Custom |
| Language | `Python` | 
| Latest release |  |
| Downloads per month |  |
| GitHub stars |  |

#### [FRIL](http://fril.sourceforge.net/)

FRIL (Fine-grained Records Integration and Linkage tool) is free tool that
enables record linkage through a GUI. The tool implements automatic weights
estimation through the EM-algorithm and offers serveral techniques to make
record pairs. FRIL was developed by the Emory University and is not longer
maintained. [[source code]](http://fril.sourceforge.net/download.html)

|  |  |
|---|---| 
| License | Custom |
| Language | `Java` | 
| Latest release |  |
| Downloads per month |  |
| GitHub stars |  |

#### [FuzzyMatcher](https://pypi.python.org/pypi/fuzzymatcher) 

A Python package that allows the user to fuzzy match two pandas dataframes
based on one or more fields in common. The functionality is limited at the
moment. [[source code]](https://github.com/RobinL/fuzzymatcher) 

|  |  |
|---|---| 
| License | ![PyPI - License](https://img.shields.io/pypi/l/fuzzymatcher) |
| Language | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fuzzymatcher) | 
| Latest release | [![PyPI](https://img.shields.io/pypi/v/fuzzymatcher.svg)](https://pypi.python.org/pypi/fuzzymatcher/) |
| Downloads per month | ![PyPI - Downloads](https://img.shields.io/pypi/dm/fuzzymatcher) |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/RobinL/fuzzymatcher.svg?style=social&label=Star)](https://github.com/RobinL/fuzzymatcher) |


#### [hlink](https://pypi.python.org/pypi/hlink) 

A Python package designed to link two datasets. The primary use case was for linking demographics in the Household -> Person hierarchical structure, however it can be used to link generic datasets as well by skipping household linking tasks. It allows for probabilistic and deterministic record linkage. [[source_code]](https://github.com/ipums/hlink)

|  |  |
|---|---| 
| License | ![PyPI - License](https://img.shields.io/pypi/l/hlink) |
| Language | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hlink) | 
| Latest release | [![PyPI](https://img.shields.io/pypi/v/hlink.svg)](https://pypi.python.org/pypi/hlink/) |
| Downloads per month | ![PyPI - Downloads](https://img.shields.io/pypi/dm/hlink) |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/ipums/hlink?style=social&label=Star)](https://github.com/ipums/hlink) |


#### [JedAI](http://jedai.scify.org/) 

Java gEneric DAta Integration (JedAI) Toolkit is a Entity Resolution Tool
developed by a group of univeristies. JedAI offers a Graphical User Interface.
[[source code]](https://github.com/scify/JedAIToolkit) 

|  |  |
|---|---| 
| License | ![GitHub](https://img.shields.io/github/license/scify/JedAIToolkit) |
| Language | `Java` | 
| Latest release |  |
| Downloads per month |  |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/scify/JedAIToolkit.svg?style=social&label=Star)](https://github.com/scify/JedAIToolkit) |

#### [PRIL](https://github.com/LSHTM-ALPHAnetwork/PIRL_RecordLinkageSoftware) 

PRIL (Point-of-contact Interactive Record Linkage) is a record linkage program
with a GUI. PRIL can be used to link datasets about individuals. ([Rentsch CT,
Kabudula CW, Catlett J et al.,
2017](https://gatesopenresearch.org/articles/1-8/v1)) [[source
code]](https://github.com/LSHTM-ALPHAnetwork/PIRL_RecordLinkageSoftware)

|  |  |
|---|---| 
| License | ![GitHub](https://img.shields.io/github/license/LSHTM-ALPHAnetwork/PIRL_RecordLinkageSoftware) |
| Language | `SQLPL` | 
| Latest release |  |
| Downloads per month |  |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/LSHTM-ALPHAnetwork/PIRL_RecordLinkageSoftware.svg?style=social&label=Star)](https://github.com/LSHTM-ALPHAnetwork/PIRL_RecordLinkageSoftware) |

#### [Python Record Linkage Toolkit](https://github.com/J535D165/recordlinkage) 

The Python Record Linkage Toolkit is a library to link records in or between
data sources. The toolkit provides most of the tools needed for record linkage
and deduplication. The package is developed for research and the linking of
small or medium sized files. 

|  |  |
|---|---| 
| License | ![PyPI - License](https://img.shields.io/pypi/l/recordlinkage) |
| Language | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/recordlinkage) | 
| Latest release | [![PyPI](https://img.shields.io/pypi/v/recordlinkage.svg)](https://pypi.python.org/pypi/recordlinkage/) |
| Downloads per month | ![PyPI - Downloads](https://img.shields.io/pypi/dm/recordlinkage) |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/J535D165/recordlinkage.svg?style=social&label=Star)](https://github.com/J535D165/recordlinkage) |

#### [RecordLinkage (R)](https://cran.r-project.org/web/packages/RecordLinkage/index.html) 

Package written in R that provides functions for linking and de-duplicating
data sets. Both supervised and unsupervised classification algorithms are
available. Record pairs can be compared with a limited set of algorithms. The
package is published on CRAN. 

|  |  |
|---|---| 
| License | ![CRAN/METACRAN](https://img.shields.io/cran/l/RecordLinkage) |
| Language | `R` | 
| Latest release | [![CRAN](https://img.shields.io/cran/v/RecordLinkage.svg)](https://cran.r-project.org/web/packages/RecordLinkage/index.html) |
| Downloads per month | [![metacran downloads](https://cranlogs.r-pkg.org/badges/last-month/RecordLinkage)](https://cran.r-project.org/package=RecordLinkage) |
| GitHub stars |  |


#### [Reclin2](https://github.com/djvanderlaan/reclin2)

Package written in R that provides functions for linking data sets. The framework offers
the option to compute the weigths of the Fellegi-Sunter model. It doesn't implement an
undersupervised algorithms to predict the cutoff. The
package is published on CRAN. Formerly https://github.com/djvanderlaan/reclin. 

|  |  |
|---|---| 
| License | ![CRAN/METACRAN](https://img.shields.io/cran/l/reclin2) |
| Language | `R` | 
| Latest release | [![CRAN](https://img.shields.io/cran/v/reclin2.svg)](https://cran.r-project.org/web/packages/reclin2/index.html) |
| Downloads per month | [![metacran downloads](https://cranlogs.r-pkg.org/badges/last-month/reclin2)](https://cran.r-project.org/package=reclin2) |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/djvanderlaan/reclin2.svg?style=social&label=Star)](https://github.com/djvanderlaan/reclin2) |

#### [RELAIS](https://www.istat.it/en/methods-and-tools/methods-and-it-tools/process/processing-tools/relais)

RELAIS (REcord Linkage At IStat) is a toolkit providing a set of techniques
for dealing with record linkage projects. IStat is the main producer of
official statistics in Italy.

|  |  |
|---|---| 
| License | `EUPL-1.1` |
| Language | `R/Java` | 
| Latest release |  |
| Downloads per month |  |
| GitHub stars |  |

#### [ReMaDDer](http://remadder.findmysoft.com/)

ReMaDDer is unsupervised free fuzzy data matching software with a GUI.
ReMaDDer is capable to perform fully automatic fuzzy record matching without
human expert intervention, while attaining accuracy of human clerical review.
NOTE: The software is free, but not open source and requires an internet
connection to work.

|  |  |
|---|---| 
| License |  |
| Language |  | 
| Latest release |  |
| Downloads per month |  |
| GitHub stars |  |

#### [RLTK](https://github.com/usc-isi-i2/rltk)

The Record Linkage ToolKit (RLTK) is a general-purpose open-source record
linkage package. The toolkit provides a full pipeline needed for record linkage
and deduplication. 

|  |  |
|---|---| 
| License | ![PyPI - License](https://img.shields.io/pypi/l/rltk) |
| Language | `Python` | 
| Latest release | [![PyPI](https://img.shields.io/pypi/v/rltk.svg)](https://pypi.python.org/pypi/rltk/) |
| Downloads per month | ![PyPI - Downloads](https://img.shields.io/pypi/dm/rltk) |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/usc-isi-i2/rltk.svg?style=social&label=Star)](https://github.com/usc-isi-i2/rltk) |

#### [Splink](https://github.com/moj-analytical-services/splink)

Splink is a Python package for probabilistic record linkage at scale.
It supports multiple backends to execute linkage jobs, including DuckDB
Apache Spark and AWS Athena. It is able to perform linking and deduplication of very large datasets
of tens of millions of records with runtimes of less than an hour, including 
the clustering of results using connected components. It includes interactive tools
to support the lifecycle of a linking project, from exploratory analysis through to
diagnostics and quality assurance.[[source
code]](https://github.com/moj-analytical-services/splink)

|  |  |
|---|---| 
| License | ![PyPI - License](https://img.shields.io/pypi/l/splink) |
| Language | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/splink) | 
| Latest release | [![PyPI](https://img.shields.io/pypi/v/splink.svg)](https://pypi.python.org/pypi/splink/) |
| Downloads per month | ![PyPI - Downloads](https://img.shields.io/pypi/dm/splink) |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/moj-analytical-services/splink.svg?style=social&label=Star)](https://github.com/moj-analytical-services/splink) |

#### [Zingg](https://github.com/zinggAI/zingg)

[Zingg](https://zingg.ai) is an open-source ML based tool for entity resolution with which analytics engineer and the data scientist can quickly integrate data silos and build unified views at scale. Zingg has the ability to connect to disparate data source, local and cloud file systems in any format, enterprise applications and relational, NoSQL and cloud databases and warehouses. It scales to large volume of data and you can define domain specific functions to improve matching.
Not only Zingg support English as well as Chinese, Thai, Japanese, Hindi and other languages, it also has a very active [slack community](https://join.slack.com/t/zinggai/shared_invite/zt-w7zlcnol-vEuqU9m~Q56kLLUVxRgpOA) where people around the globe come and help and share their views.

|  |  |
|---|---| 
| License | ![PyPI - License](https://img.shields.io/pypi/l/zingg) |
| Language | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zingg) `Spark` | 
| Latest release | [![PyPI](https://img.shields.io/pypi/v/zingg.svg)](https://pypi.python.org/pypi/zingg/) |
| Downloads per month | ![PyPI - Downloads](https://img.shields.io/pypi/dm/zingg) |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/zinggAI/zingg.svg?style=social&label=Star)](https://github.com/zinggAI) |

#### [dirty-cat](https://github.com/dirty-cat/dirty_cat)

[dirty-cat](https://dirty-cat.github.io/) is an open-source Python package that facilitates machine-learning with with dirty data: robust to morphological variants, such as typos. Some of the currently supported features are: fuzzy joining tables on dirty numerical, string or mixed type columns, deduplicating and encoding dirty categorical variables for ML. [This example](https://dirty-cat.github.io/stable/auto_examples/01_dirty_categories.html) illustrates why to use dirty-cat encoders rather than OneHotEncoder on dirty data and [this one](https://dirty-cat.github.io/stable/auto_examples/04_fuzzy_joining_and_FeatureAugmenter.html) shows how to join multiple dirty tables for ML.
The transfomers ([TableVectorizer](https://dirty-cat.github.io/stable/generated/dirty_cat.TableVectorizer.html), [FeatureAugmenter](https://dirty-cat.github.io/stable/generated/dirty_cat.FeatureAugmenter.html)) are scikit-learn compatible, and easily introduced into ML pipelines.

|  |  |
|---|---| 
| License | ![PyPI - License](https://img.shields.io/pypi/l/zingg) |
| Language | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zingg) `Spark` | 
| Latest release | [![PyPI](https://img.shields.io/pypi/v/zingg.svg)](https://pypi.python.org/pypi/zingg/) |
| Downloads per month | ![PyPI - Downloads](https://img.shields.io/pypi/dm/zingg) |
| GitHub stars | [![GitHub stars](https://img.shields.io/github/stars/zinggAI/zingg.svg?style=social&label=Star)](https://github.com/zinggAI) |

## Outdated/ no longer available

#### BigMatch (by USA census)

A record linkage tool for use in matching a very large file against a moderate
size file developed by the USA Census Bureau. There are several papers
available about this program [(BigMatch,
2007)](https://www.census.gov/srd/papers/pdf/rrc2007-01.pdf)

#### [The Link King](http://the-link-king.party/) 

The Link King’s graphical user interface (GUI) makes record linkage and
unduplication easy for beginning and advanced users. The software requires a
SAS license. `SAS`

## Contributing

Do you know an open source and/or free data matching tool? Please open an
issue or do a Pull Request. The same holds for missing or incomplete
information.

This project is initiated by the author of the [Python Record Linkage
Toolkit](https://github.com/J535D165/recordlinkage) @J535D165. The aim is to
get a list and comparison of data matching software. 

This list is licensed under [CC-BY-SA 3.0](http://creativecommons.org/licenses/by-sa/3.0/). 
