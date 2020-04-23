# Control Room
[azure](https://dev.azure.com/anyvent/Control Room)

## C# app
### Algemene info
Deze applicatie luistert naar alle heartbeats en verwerkt deze data. Deze doet ook de nodige aanpassingen in Elasticsearch.

## Kibana
### Algemene info
Kibana is de interface waar je kan zien welke systemen up of down zijn.
Hoe kan er bepaald worden of een systeem up of down is? => Heartbeat
 
Kibana gaat data van uit Elasticsearch indexeren en die visualiseren.
 
URL: [http://10.3.56.3:5601](http://10.3.56.3:5601) (VPN nodig)

### Links visualisatie

[Klik hier voor visualisatie 1](http://10.3.56.3:5601/app/kibana#/dashboard/b2bde400-8174-11ea-8f95-adbfd2c32966?_g=(refreshInterval:(pause:!f,value:5000),time:(from:now-15m,to:now)))

[Klik hier voor visualisatie 2](http://10.3.56.3:5601/app/canvas#/workpad/workpad-274ba810-be9e-46f8-8591-2c017014df87/page/1?__refreshInterval=5s)

### Officiële documentatie Kibana
[Docs Kibana](https://www.elastic.co/guide/en/kibana/7.6/index.html)

## Heartbeat

Vanuit jullie systeem elke seconde een heartbeat (XML) sturen naar de "heartbeat-exchange" met routing key "heartbeat".

[Link naar XML formaat](https://anyvent.github.io/docs/XML/#heartbeat)
 
IP rabbitmq: `10.3.56.9`
Port rabbitmq: `5672`


## Elasticsearch
### Algemene info
Elasticsearch is simpelweg een nosql database.
Hierin wordt data opgeslagen over de status van een specifiek systeem alsook logs van de systemen.

### Handige links

[Indexen in elasticsearch](http://10.3.56.3:9200/_cat/indices?v)

[Basis info over elasticsearch instantie](http://10.3.56.3:9200/)

### Officiële documentatie Elasticsearch
[Docs Elasticsearch](https://www.elastic.co/guide/en/elasticsearch/reference/7.6/index.html)