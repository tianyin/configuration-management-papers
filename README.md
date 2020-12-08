# A Reading List of System Configuration Management

## Introduction

This is a list of materials and resources on configuration management for cloud and Internet systems. Some of the early work did not exactly target modern cloud systems, but I find the ideas relevant and inspiring. 

The list does not intend to include other forms of configuration, such as network device configuration, [feature flags](https://www.cs.cmu.edu/~ckaestne/pdf/icseseip20.pdf), or user preferences (fonts and background themes).

## Motivation

* [Fail at Scale: Reliability in the face of rapid change](https://queue.acm.org/detail.cfm?id=2839461) (CACM, 2015)

* [What I wish systems researchers would work on](http://matt-welsh.blogspot.com/2013/05/what-i-wish-systems-researchers-would.html)

* [How Hadoop clusters break](https://ieeexplore.ieee.org/document/6216347) (IEEE Software, 2013)

* [What Takes Us Down?](https://www.usenix.org/system/files/login/articles/login1210_kendrick.pdf) (;login:, 2012)

* [An Empirical Study on Configuration Errors in Commercial and Open Source Systems](http://opera.ucsd.edu/paper/sosp11-yin.pdf) (SOSP, 2011)

* [Why do Internet services fail, and what can be done about it?](http://roc.cs.berkeley.edu/papers/usits03.pdf) (USITS, 2003)


## Practices

* [Configuration Design and Best Practices](https://sre.google/workbook/configuration-design/) (The Site Reliability Workbook, 2018)

* [Configuration Specifics](https://sre.google/workbook/configuration-specifics/) (The Site Reliability Workbook, 2018)

* [Holistic Configuration Management at Facebook](http://sigops.org/s/conferences/sosp/2015/current/2015-Monterey/printable/008-tang.pdf) (SOSP, 2015)

* [ACMS: The Akamai Configuration Management System](https://www.usenix.org/legacy/publications/library/proceedings/nsdi05/tech/full_papers/sherman/sherman.pdf) (NSDI, 2005)

* [STRIDER: A Black-box, State-based Approach to Change and Configuration Management and Support](https://www.usenix.org/legacy/publications/library/proceedings/lisa03/tech/wang/wang.pdf) (LISA, 2003) - Microsoft CCMS


## Testing and Validation

* [Testing Configuration Changes in Context to Prevent Production Failures](https://tianyin.github.io/pub/ctest.pdf) (OSDI, 2020) - Connecting production system configurations to software tests

* [Usable Declarative Configuration Specification and Validation for Applications, Systems, and Cloud](https://dl.acm.org/doi/abs/10.1145/3154448.3154453) (Middleware, 2017) -- IBM ConfigValidator

* [Early Detection of Configuration Errors to Reduce Failure Damage](https://tianyin.github.io/pub/pcheck.pdf) (OSDI, 2016) - Generating configuration checks

* [ConfValley: A Systematic Configuration Validation Framework for Cloud Services](https://www.cs.jhu.edu/~huang/paper/confvalley-eurosys15.pdf) (EuroSys, 2015) - A declarative framework for writing configuration validation code 


## Detection

* [Automated Reasoning and Detection of Specious Configuration in Large Systems with Symbolic Execution](https://www.usenix.org/system/files/osdi20-hu.pdf) (OSDI, 2020)

* [Rex: Preventing Bugs and Misconfiguration in Large Services Using Correlated Change Analysis](https://www.usenix.org/system/files/nsdi20-paper-mehta.pdf) (NSDI, 2020) - Correlated-change analysis for Microsoft Office 365 and Azure

* [PracExtractor: Extracting Configuration Good Practices from Manuals to Detect Server Misconfigurations](https://www.usenix.org/conference/atc20/presentation/xiang) (USENIX ATC, 2020) - Using NLP to learn good practices and detect bad practices

* [EnCore: Exploiting System Environment and Correlation Information for Misconfiguration Detection](https://tianyin.github.io/pub/encore.pdf) (ASPLOS, 2014) - Checking correlations between configuration values and the deployment environment (VM images)

* [Context-based Online Configuration-Error Detection](https://www.usenix.org/legacy/event/atc11/tech/final_files/Yuan.pdf) (USENIX ATC, 2011) - Detecting abnormal configuration event sequences


## Resilience and Diagnosability

* [Proactive Detection of Inadequate Diagnostic Messages for Software Configuration Errors](https://homes.cs.washington.edu/~mernst/pubs/inadequate-diagnostics-issta2015-abstract.html) (ISSTA, 2015) - Uses NLP to evaluate log message quality

* [Do Not Blame Users for Misconfigurations](https://tianyin.github.io/pub/spex.pdf) (SOSP, 2013) - Generating misconfigurations based on constraints inferred from source code

* [ConfErr: A Tool for Assessing Resilience to Human Configuration Errors](https://dslab.epfl.ch/research/conferr/) (DSN, 2010) - Generating misconfigurations based on human error model


## Troubleshooting

* [Automated Diagnosis of Software Configuration Errors](https://homes.cs.washington.edu/~mernst/pubs/configuration-errors-icse2013.pdf) (ICSE, 2013) - Identify behavior deviation caused by misconfiguration

* [X-ray: Automating Root-Cause Diagnosis of Performance Anomalies in Production Software](https://www.usenix.org/conference/osdi12/technical-sessions/presentation/attariyan) (OSDI, 2012) - Inferring causality between performance anomalies and configuration values

* [Precomputing Possible Configuration Error Diagnoses](https://asrabkin.bitbucket.io/papers/ase11.pdf) (ASE, 2011)

* [Automating configuration troubleshooting with dynamic information flow analysis](https://www.usenix.org/legacy/events/osdi10/tech/full_papers/Attariyan.pdf) (OSDI, 2010) - Inferring causality between failures and configuration values

* [Configuration Debugging as Search: Finding the Needle in the Haystack](https://www.usenix.org/legacy/publications/library/proceedings/osdi04/tech/full_papers/whitaker/whitaker.pdf) (OSDI, 2004) - Debugging by time traveling

* [Automatic Misconfiguration Troubleshooting with PeerPressure](https://www.usenix.org/legacy/events/osdi04/tech/full_papers/wang/wang.pdf) (OSDI, 2004) - Integrated in Windows troubleshooting toolkit for Windows registry


## Specification and Comprehension

* [Understanding and Discovering Software Configuration Dependencies in Cloud and Datacenter Systems](https://tianyin.github.io/pub/cdep.pdf) (ESEC/FSE, 2020) - Configuration dependency analysis

* [Statically Inferring Performance Properties of Software Configurations](https://dl.acm.org/doi/abs/10.1145/3342195.3387520) (EuroSys, 2020)

* [Synthesizing Configuration File Specifications with Association Rule Learning](https://ennanzhai.github.io/pub/configv-oopsla17.pdf) (OOPSLA, 2017) - Synthesizing configuration specifications

* [Probabilistic Automated Language Learning for Configuration Files](http://www.cs.yale.edu/homes/piskac/papers/2016SantolucitoETALConfigC.pdf) (CAV, 2016) - Learning a language model of configuration

* [ConfSeer: Leveraging Customer Support Knowledge Bases for Automated Misconfiguration Detection](http://www.vldb.org/pvldb/vol8/p1828-potharaju.pdf) (VLDB, 2015) - Using NLP to find configuration KB articles; Integrated in Microsoft Operations Management Suite

* [Hey, You Have Given Me Too Many Knobs! Understanding and Dealing with Over-Designed Configuration in System Software](https://tianyin.github.io/pub/knobs.pdf) (ESEC/FSE, 2015) - Statistics of configuration files in the field

* [Which Configuration Option Should I Change?](https://zhang-sai.github.io/pdf/zhang-icse14.pdf) (ICSE, 2014) - Re-configuration due to software evolution


## Tuning for Performance

* [Understanding and Auto-Adjusting Performance-Sensitive Configurations](https://people.cs.uchicago.edu/~shanlu/paper/asplos18_smartconf.pdf) (ASPLOS, 2018)

* [Datasize-Aware High Dimensional Configurations Auto-Tuning of In-Memory Cluster Computing](https://dl.acm.org/doi/10.1145/3173162.3173187) (ASPLOS, 2018)

* [CherryPick: Adaptively Unearthing the Best Cloud Configurations for Big Data Analytics](https://www.usenix.org/conference/nsdi17/technical-sessions/presentation/alipourfard) (NSDI, 2017)

* [BestConfig: Tapping the Performance Potential of Systems via Automatic Configuration Tuning](https://arxiv.org/pdf/1710.03439.pdf) (SoCC, 2017)

* [Automatic Database Management System Tuning Through Large-scale Machine Learning](https://www.cs.cmu.edu/~ggordon/van-aken-etal-parameters.pdf) (SIGMOD, 2017)

* [Transfer Learning for Performance Modeling of Configurable Systems: An Exploratory Analysis](https://arxiv.org/pdf/1709.02280.pdf) (ASE, 2017)

* [The Starfish Project at Duke University](http://www2.cs.duke.edu/starfish/)


## Access Control

* [Forensic Analysis in Access Control: Foundations and a Case-Study from Practice](https://dl.acm.org/doi/abs/10.1145/3372297.3417860) (CCS, 2020)

* [Towards Continuous Access Control Validation and Forensics](https://tianyin.github.io/pub/pdiff.pdf) (CCS, 2019)

* [How Do System Administrators Resolve Access-Denied Issues in the Real World?](https://tianyin.github.io/pub/chi17.pdf) (CHI, 2017)

* [Detecting and Resolving Policy Misconfigurations in Access-Control Systems](https://dl.acm.org/doi/abs/10.1145/1952982.1952984) (TISSEC, 2011)

* [Baaz: A System for Detecting Access Control Misconfigurations](https://www.usenix.org/conference/usenixsecurity10/baaz-system-detecting-access-control-misconfigurations) (USENIX Security, 2010)


## Datasets

* [Configuration Dataset](https://github.com/tianyin/configuration_datasets) - Both configuration files and user-reported configuration issues collected from ServerFault, StackOverflow, and mailing lists

* [Ctest Dataset](https://github.com/xlab-uiuc/openctest/tree/main/data) - Historical configuration-related JIRA issues

* [Mining Container Image Repositories for Software Configurations and Beyond](https://tianyin.github.io/pub/icse-nier18.pdf) - You can collect configuration files from Docker images 


## Notes

Feel free to open an issue or send me a PR, if you have any suggestions or feedback. 

