# Example of monitoring using ELK stack

A simple example of monitoring using ELK stack consuming from other Elasticsearch;
###Reference:https://www.elastic.co/guide/en/logstash/current/plugins-inputs-elasticsearch.html

Change the hosts address to Elasticsearch data origin.
/monitorings/indexer/config/logstash.conf

```
input {
  elasticsearch {
    host =>  "URL_ELASTICSEARCH"
    index => "requestlog-*"
  }
}
```

- Indexer (Logstash)
- Elasticsearch
- Kibana
