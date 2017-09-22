# rancher-logging - Get stdout+stderr in console and kibana at the same time
based on Idea by @cloudnautique from rancher.com, https://hub.docker.com/r/picoded/docker-filebeat/  and ELK of-course

- This is for use with containers.
- Filebeat runs on every docker host, tails the dockerd logs and ships them directly to ElasticSearch.
- So stdout & stderr which are normally available ONLY in the console, also get shipped to Kibana
