# 2 - Initial Overview of SIEM Terms

## Preparation

Books: approx 61 pages without the skim part, lots of pictures

* [x] DDS 1. The Journey to Data-Driven Security 18   
* [x] DDS 2. Building Your Analytics Toolbox: R and Python 17   
* [x] CIP 1 Incident Response Fundamentals 13   
* [x] CIP 2 What Are You Trying to Protect? 13   
* [ ] Skim CIP 3 What Are the Threats? 14   

### Notes and question re: Preparation

**Key take-aways**

DDS pp. 2:   
> *We are not advocating replacing people with algorithms; we are advocating arming people with algorithms so that they can learn more and do a better job.*

DDS pp. 6:   
> Domains that a data scientist will benefit from knowing within information security   
> - **Domain expertise** -- Setting and maintaining a purpose to the analysis   
> - **Datamanagement** -- Being able to prepare, store, and maintain data   
> - **Programming** -- The glue that connects data to analysis   
> - **Statistics** -- To learn from the data   
> - **Visualization** -- Communicating the results effectively   

DDS 2: Building Your analytics Toolbox: A primer on ...
- Python er lim mellem systemer, R er Excel på steroider.

CIP 2: What are you trying to protect
- Define and understand your critical assets and what's most important in your information

CIP 3:
- Dem der ikke har hændelser kigger ikke godt nok.

## Noter fra undervisningen

Start i det små for at vise værdien i et SIEM.   
- Eks. DNS logs.   
- Iterativt projekt   


**Anatomy of an Auditing system**   
- Logger functions - collect
- Analyzer - analyze it, creating dashboard can provide some insights
- Notifier - report results by email or other means
  Example systems Windows Event Logs service can inform of successful and failed logins, both should be collected
  Logs should be protected and considered confidential information, by sending it to a centralized system with a high security level protects it

**Strategy for Implementing Identificatio and Detection**
- [ ] Enable system logging from servers
- [ ] Enable system logging from network devices
- [ ] Centralize logging
- [ ] Add search facilities and dashboards
- [ ] Perform system audits manually or automatically
- [ ] Setup notification and notification procedures


*Læs op på Grok + maltrail*


![MindMap](https://github.com/krejac/kea-siem-log/blob/master/media/SIEM.png)
