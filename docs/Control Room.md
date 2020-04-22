# Control Room
[azure](https://dev.azure.com/anyvent/Control Room)

## Kibana
### Algemene info
Kibana is de interface waar je kan zien welke systemen up of down zijn.
Hoe kan er bepaald worden of een systeem up of down is? => Heartbeat
 
Kibana gaat data van uit Elasticsearch indexeren en die visualiseren.
 
URL: `http://10.3.56.3:5601` (VPN nodig)

### Links visualisatie

[Klik hier voor visualisatie 1](http://10.3.56.3:5601/app/kibana#/dashboard/b2bde400-8174-11ea-8f95-adbfd2c32966?_g=(refreshInterval:(pause:!f,value:5000),time:(from:now-15m,to:now))&_a=(description:'',filters:!(),fullScreenMode:!f,options:(hidePanelTitles:!f,useMargins:!t),panels:!((embeddableConfig:(),gridData:(h:15,i:'577055ee-975a-4e11-83ec-b07117c6fe8c',w:24,x:0,y:0),id:a79aca30-8169-11ea-8f95-adbfd2c32966,panelIndex:'577055ee-975a-4e11-83ec-b07117c6fe8c',type:visualization,version:'7.6.1'),(embeddableConfig:(),gridData:(h:15,i:'8e138d6a-71d5-407a-a259-af0d62542686',w:24,x:24,y:0),id:'610e7bb0-8174-11ea-8f95-adbfd2c32966',panelIndex:'8e138d6a-71d5-407a-a259-af0d62542686',type:lens,version:'7.6.1')),query:(language:kuery,query:''),timeRestore:!f,title:'Status%20of%20Queues',viewMode:view))

[Klik hier voor visualisatie 2](http://10.3.56.3:5601/app/canvas#/workpad/workpad-274ba810-be9e-46f8-8591-2c017014df87/page/1?__refreshInterval=5s)

## Heartbeat

Vanuit jullie systeem elke seconde een heartbeat (XML) sturen naar de "heartbeat-exchange" met routing key "heartbeat".
 
IP rabbitmq: `10.3.56.9`
Port rabbitmq: `5672`
