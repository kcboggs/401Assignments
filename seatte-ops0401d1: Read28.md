# Threat Hunting with ELK Stack
### What is the ELK stack?
> "The ELK stack is an acronym used to describe a stack that comprises of three popular open-source projects: Elasticsearch, Logstash, and Kibana."  

**E = Elasticsearch**
Elasticsearch is an open-source, RESTful, distributed search and analytics engine built on Apache Lucene. Support for various languages, high performance, and schema-free JSON documents makes Elasticsearch an ideal choice for various log analytics and search use cases.  
**L = Logstash**  
Logstash is an open-source data ingestion tool that allows you to collect data from a variety of sources, transform it, and send it to your desired destination. With pre-built filters and support for over 200 plugins, Logstash allows users to easily ingest data regardless of the data source or type.    
**K = Kibana**
Kibana is an open-source data visualization and exploration tool for reviewing logs and events. Kibana offers easy-to-use, interactive charts, pre-built aggregations and filters, and geospatial support and making it the preferred choice for visualizing data stored in Elasticsearch.

 *** Why is the ELK stack so popular?
 _The ELK Stack is popular because it fulfills a need in the log analytics space._  
 
 ### The ELK stack – Choosing the right option  
You can choose to deploy and manage the ELK stack yourself. But, would you prefer that your developers or DevOps engineers spend time on building innovative applications or on managing operational tasks such as deployment, upgrades, software installation and patching, backups, and monitoring?  
https://aws.amazon.com/elasticsearch-service/the-elk-stack/

# A Framework for Cyber Threat Hunting  
1. What is hunting? 
_the process of proactively and iteratively
searching through networks to detect and isolate advanced threats that evade existing
security solutions._  
2.HMM    
_The Hunting Maturity Model, rst developed by Sqrrl’s own security technologist and chief hunter,
David J. Bianco, describes five levels of organizational hunting capability, ranging from HM0 (the
least capable) to HM4 (the most)._  
* HM0 - INITIAL  
* HM1 - MINIMAL  
* HM2 - PROCEDURAL  
* HM3 - INNOVATIVE  
* HM4 - LEADING  
3. Hunting Loop    
_The goal of a hunt team should
be to get through the loop as quickly and effectively as possible._  
* Hypothesis Generation  
* Tool and Technique Enabled Investigation   
* Pattern and TTP Discovery    
* Automated Analytics    
4. Hunt Matrix   
_» Maturing hypothesis creationis dependent on crafting increasingly more dynamic questions, and
moving from manual hypothesis creation to automatic generation via risk scoring analytics._  
_» Maturing the tools and techniques used to follow up on hypotheses is dependent on moving from
using simple searches and histograms to using tools with advanced visualizations and graph
search capabilities._  
_» Maturing your pattern and TTP detectionis dependent on expanding the kinds of Indicators of
» Finally, maturing analytics and automation is dependent on moving from simple analytics such as
stack counting, to advanced and automated analytics powered by machine learning, and moving
from repeated searches to feeding gathered information back into your automated detection
systems._


https://www.threathunting.net/files/framework-for-threat-hunting-whitepaper.pdf
