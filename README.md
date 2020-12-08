# A Reading List of System Configuration Management

## Introduction

## Motivation
* [Fail at Scale: Reliability in the face of rapid change](https://queue.acm.org/detail.cfm?id=2839461) (CACM, 2015)

## Practices

* [Configuration Design and Best Practices](https://sre.google/workbook/configuration-design/) (The Site Reliability Workbook, 2018) - Google recommended practices.

* [Configuration Specifics](https://sre.google/workbook/configuration-specifics/) (The Site Reliability Workbook, 2018) - Google recommended practices.

* [Holistic Configuration Management at Facebook](http://sigops.org/s/conferences/sosp/2015/current/2015-Monterey/printable/008-tang.pdf) (SOSP, 2015) - Facebook Configerator

* [STRIDER: A Black-box, State-based Approach to Change and Configuration Management and Support](https://www.usenix.org/legacy/publications/library/proceedings/lisa03/tech/wang/wang.pdf) (LISA, 2003) - Microsoft CCMS

## Testing and Validation

* [Testing Configuration Changes in Context to Prevent Production Failures](https://tianyin.github.io/pub/ctest.pdf) (OSDI, 2020) - Connecting production system configurations to software tests

* [Usable Declarative Configuration Specification and Validation for Applications, Systems, and Cloud](https://dl.acm.org/doi/abs/10.1145/3154448.3154453) (Middleware, 2017) -- IBM ConfigValidator

* [Holistic Configuration Management at Facebook](http://sigops.org/s/conferences/sosp/2015/current/2015-Monterey/printable/008-tang.pdf) (SOSP, 2015) - Facebook Configerator

* [ConfValley: A Systematic Configuration Validation Framework for Cloud Services](https://www.cs.jhu.edu/~huang/paper/confvalley-eurosys15.pdf) (EuroSys, 2015) - A declarative framework for writing configuration validation code 


## Detection

* [Rex: Preventing Bugs and Misconfiguration in Large Services Using Correlated Change Analysis](https://www.usenix.org/system/files/nsdi20-paper-mehta.pdf) (NSDI, 2020) - Correlated-change analysis for Microsoft Office 365 and Azure

* [EnCore: Exploiting System Environment and Correlation Information for Misconfiguration Detection](https://tianyin.github.io/pub/encore.pdf) (ASPLOS, 2014) - Checking correlations between configuration values and the deployment environment (VM images)

## Resilience and Diagnosability

* [Proactive Detection of Inadequate Diagnostic Messages for Software Configuration Errors](https://homes.cs.washington.edu/~mernst/pubs/inadequate-diagnostics-issta2015-abstract.html) (ISSTA, 2015) - Uses NLP to evaluate log message quality

* [Do Not Blame Users for Misconfigurations](https://tianyin.github.io/pub/spex.pdf) (SOSP, 2013) - Generates misconfigurations based on constraints inferred from source code

* [ConfErr: A Tool for Assessing Resilience to Human Configuration Errors](https://dslab.epfl.ch/research/conferr/) (DSN, 2010) - Generates misconfigurations based on human error model

## Troubleshooting

* [Automated Diagnosis of Software Configuration Errors](https://homes.cs.washington.edu/~mernst/pubs/configuration-errors-icse2013.pdf) (ICSE, 2013) - Identify behavior deviation caused by misconfiguration

* [X-ray: Automating Root-Cause Diagnosis of Performance Anomalies in Production Software](https://www.usenix.org/conference/osdi12/technical-sessions/presentation/attariyan) (OSDI, 2012) - Inferring causality between performance anomalies and configuration values

* [Automating configuration troubleshooting with dynamic information flow analysis](https://www.usenix.org/legacy/events/osdi10/tech/full_papers/Attariyan.pdf) (OSDI, 2010) - Inferring causality between failures and configuration values

* [Configuration Debugging as Search: Finding the Needle in the Haystack](https://www.usenix.org/legacy/publications/library/proceedings/osdi04/tech/full_papers/whitaker/whitaker.pdf) (OSDI, 2004) - Debugging by time traveling

* [Automatic Misconfiguration Troubleshooting with PeerPressure](https://www.usenix.org/legacy/events/osdi04/tech/full_papers/wang/wang.pdf) (OSDI, 2004) - Integrated in Windows troubleshooting toolkit for Windows registry

## Specificatons and Comprehension

* [Understanding and Discovering Software Configuration Dependencies in Cloud and Datacenter Systems](https://tianyin.github.io/pub/cdep.pdf) (ESEC/FSE, 2020) - Configuration dependency analysis

* [Probabilistic Automated Language Learning for Configuration Files](http://www.cs.yale.edu/homes/piskac/papers/2016SantolucitoETALConfigC.pdf) (CAV, 2016) - Learning a language model of configuration

* [ConfSeer: Leveraging Customer Support Knowledge Bases for Automated Misconfiguration Detection](http://www.vldb.org/pvldb/vol8/p1828-potharaju.pdf) (VLDB, 2015) - Using NLP to learn best practices from KB articles; Integrated in Microsoft Operations Management Suite

## Configuration Auto-tuning

## Datasets

## Surveys
