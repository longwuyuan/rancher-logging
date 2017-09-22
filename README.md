# rancher-logging
based on  ;
- Idea by @cloudnautique from rancher.com
- https://hub.docker.com/r/picoded/docker-filebeat/
- https://hub.docker.com/r/picoded/docker-logrotate/
- and Elastic.co ELK of-course

## Get stdout+stderr in Kibana without losing it in rancher "logs" button
## Rotate the logs so disk does not get filled up

- This is for use with containers in general and Rancher.com in particular
- Filebeat runs on every docker host, tails the dockerd logs and ships them directly to ElasticSearch.
- So stdout & stderr which are normally available ONLY in the console, also get shipped to Kibana
- In Kibana you get to see the log text, create alerts, create graphs and lots more

## Read docs on Rancher.com & Elastic.co to change config as per your needs 
