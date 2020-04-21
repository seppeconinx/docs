# Control Room
[azure](https://dev.azure.com/anyvent/Control Room)

## Kibana
Kibana is de interface waar je kan zien welke systemen up of down zijn.
Hoe kan er bepaald worden of een systeem up of down is? => Heartbeat
 
Kibana gaat data van uit Elasticsearch indexeren en die visualiseren.
 
URL: `http://10.3.56.3:5601` (VPN nodig)

## Heartbeat

Vanuit jullie systeem elke seconde een heartbeat (XML) sturen naar de "heartbeat-exchange" met routing key "heartbeat".
 
IP rabbitmq: `10.3.56.9`
Port rabbitmq: `5672`
