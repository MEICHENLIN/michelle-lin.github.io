## Software Projects

---

### Audit Data Automation

As the volume and complexity of audit data at ARPANSA (Australian Radiation Protection and Nuclear Safety Agency) increased, traditional Excel-based workflows became inefficient and unsustainable. The audit files were often unstructured, with inconsistent formats, complicated columns, and data that was difficult to interpret or analyse effectively. These issues resulted in manual, error-prone processes and slow turnaround times for key tasks.

This system addresses those challenges by: (i) transforming the traditional Excel worksheets into a normalised MySQL database schema, (ii) generating IMRT and 3DRT graphs automatically to visualise distributions of data for further analysis.

A local program written in Python is implemented to act as a frontend support on sending RESTful requests for audit data operations and graph generation.

#### Data Normalisation
<img src="images/full.png?raw=true"/>

#### Data Visualisation
<img src="images/fig-1.png?raw=true" width="250x" style="margin-right: 30px;"/>
<img src="images/fig-2.png?raw=true" width="250x"/>
<div style="height: 30px;"></div>
<img src="images/fig-3.png?raw=true" width="250x" style="margin-right: 30px;"/>
<img src="images/fig-4.png?raw=true" width="250x"/>


[![](https://img.shields.io/badge/Python-white?logo=Python)](#) [![](https://img.shields.io/badge/Django-white?logo=django)](#) [![](https://img.shields.io/badge/MySQL-white?logo=mysql)](#) [![](https://img.shields.io/badge/Docker-white?logo=docker)](#) [![](https://img.shields.io/badge/Bash-white?logo=gnubash)](#) [![](https://img.shields.io/badge/Matplotlib-white?logo=matplotlib)](#)
[![](https://img.shields.io/badge/NumPy-white?logo=numpy)](#) [![](https://img.shields.io/badge/pandas-white?logo=pandas)](#)


[View code on GitHub](https://github.com/MEICHENLIN/arpansa-audit-automation)

---

### Twitter harvesting and Sentiment Analysis

During the COVID-19 pandemic, the Australian residents were ordered into lockdown and a large
proportion of the public concerns have been focused on the economic impact that this pandemic
would have. As a response, the government introduced some economic initiatives such as Jobseeker and Jobkeeper payments to provide economic support for the residents.

The project investigated in the following topics
* Observe whether tweets mentioning #jobseeker/#jobkeeper had an overall positive or negative inclination using a sentiment analysis tool [VADER-Sentiment](https://github.com/cjhutto/vaderSentiment) for social media
* Infer which industries are most benefited by these economic schemes by aggregating sentiment for each major city and comparing with a labor market dataset
* Infer how people's attitude towards the initiatives in a certain period by aggregating historical sentiment by time


#### Data Flows
1. Collect live and recent tweets by Twitter search/stream APIs using Python
2. Enrich the tweets using Python sentiment library
3. Store processed tweets into the distributed CouchDB nodes
4. Visualise tweets on a dashboard implemented in Node.js and Bootstrap

<img src="images/twitter-data-flow.png?raw=true"/>

#### Deployment Architecture
* Automated cloud deployement using Ansible orchestration on Docker containers

<img src="images/twitter-deployment.png?raw=true"/>

#### Sentiment Analysis
* Dashboard Visualisation of historical and location sentiment data

<img src="images/historical.png?raw=true" width="300x" style="margin-right: 30px;"/>
<img src="images/location.png?raw=true" width="300x"/>


[![](https://img.shields.io/badge/Python-white?logo=Python)](#) [![](https://img.shields.io/badge/Node.js-white?logo=nodedotjs)](#) [![](https://img.shields.io/badge/Express-white?logo=express)](#
) [![](https://img.shields.io/badge/Bootstrap-white?logo=bootstrap)](#) [![](https://img.shields.io/badge/CouchDB-white?logo=apachecouchdb)](#) [![](https://img.shields.io/badge/Ansible-white?logo=ansible)](#) [![](https://img.shields.io/badge/Docker-white?logo=docker)](#) [![](https://img.shields.io/badge/Bash-white?logo=gnubash)](#) [![](https://img.shields.io/badge/NumPy-white?logo=numpy)](#) [![](https://img.shields.io/badge/pandas-white?logo=pandas)](#)

[View code on GitHub](link)

---
