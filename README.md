# Log Aggregation 📝

EFK stack for centralized log aggregation.

## Architecture

```
Apps → Fluentd → Elasticsearch → Kibana
```

## Deploy

```bash
helm upgrade --install elasticsearch elastic/elasticsearch -f elasticsearch/values.yaml
helm upgrade --install kibana elastic/kibana -f kibana/values.yaml
kubectl apply -f fluentd/
```

## License

Apache 2.0