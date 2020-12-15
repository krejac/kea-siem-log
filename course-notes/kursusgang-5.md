# 6 - Baseline Your Data

## Preparation

Books - approx 64 pages

* [ ] DDS 7. Learning from Security Breaches VERIS 28   
* [ ] DDS 12. Moving Toward Data-Driven Security 11   
* [ ] IDIR 1. Introduction 8   
* [ ] IDIR 2. Basics of Intelligence 17   

### Notes and question re: Preparation

DDS kap. 7 Learning from breaches VERIS

- We all see the same attacks, make it easier to communicate between applications and organizations   
- Learn from others   
- Another example [MITRE ATT&CK](https://attack.mitre.org/)   
- Find and Collect Relevant Data   
- Learn through Iteration   
- Find Statistics   
- First, explore the open source versions of tools before engaging vendors. *"If you don’t know how the sausage is being made, you really have no idea what’s being done, and this is vital when working with real data"*.   
- Second, follow the mantra of *"no single tool; no single database; and, no single approach to solving a problem."* Do not put blinders on because you are either comfortable with certain technologies or have an affinity for acertain tool.   
- Third, failure is expected, but you must learn from each journey down the wrong path. Continuous adaptationand adjustment is the name of the game.   


IDIR kap. 2. Basics of Intelligence

  > *There was a time when many people considered indicators of compromise, or IOCs, to be synonymous withthreat intelligence. IOCs, which we will reference a lot and cover in depth later in the book, are things to look for on a system or in network logs that may indicate that a compromise has taken place. This includes IP addresses and domains associated with command-and-control servers or malware downloads, hashes of malicious files, and other network- or host-based artifacts that may indicate an intrusion. As we will discuss throughout this book, however, there is far more to threat intelligence than IOCs, although IOCs still remain one of the most common types of technical intelligence around intrusions.*

- List sources of intelligence, HUMINT, OSINT, SIGINT etc.   
- Introduces the OODA loop, “Observe, Orient, Decide, Act.” and the Intelligence Cycle.   
- OODA loop also used in the SOC book.   

## Noter fra undervisningen

### How to get started searching for security events?

**Collect basic data from your devices and networks**
- Netflow data from routers•Session data from firewalls
- Logging from applications: email, web, proxy systemsCentralize!

**Process data**
- Look at *Top 10*: interesting due to high frequency, occurs often, e.g. brute-force attacks
- Ignore, ignore, ignore
- Look at *Bottom 10*: least-frequent messages are interesting, e.g. malware


  > *Security is a process, not a product.Products provide some protection, but the only way to effectively dobusiness in an insecure world is to put processes in place that recognize the inherent insecurity in the products.The trick is to reduce your risk of exposure regardless of the products or patches.*
  >
  > Source:  [Bruce Schneier](https://www.schneier.com/essays/archives/2000/04/the_process_of_secur.html)

- **People** – make sure management is on board   
- **Sources** – which data to gather  
- **Technology** – select SIEM, architecture, tools and products  
- **Dashboards** – we have done parts of this, refer to SOC book also  
- **Procedures** – left as a home exercise today  

**TODO** - for implementing identification and detection – logging

- [ ] Enable system logging from servers
- [ ] Enable system logging from network devices
- [ ] Enable logging from client devices
- [ ] Centralize logging
- [ ] Add search facilities and dashboards
- [ ] Perform system audits manually or automatically
- [ ] Setup alerting and notification with procedures

Extend with

- [ ] DNS query logging – will enable multiple cases to be resolved, example malware identification and tracing, when wasa malware domain queried, when was the first infection
- [ ] Web proxy logging – which web pages did which client access
- [ ] Session data from Firewalls, Netflow – traffic patterns can be investigated and both attacks and cases like exfiltration can likely be seen

### Elastic native alerting (links)

- https://www.elastic.co/blog/introducing-the-new-alerting-framework-for-observability-security-and-the-elastic-stack
- https://www.elastic.co/what-is/kibana-alerting
- https://www.elastic.co/blog/alerting-in-the-elastic-stack

![MindMap](https://github.com/krejac/kea-siem-log/blob/master/media/xxxx-xxxx.png)
