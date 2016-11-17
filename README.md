# docker-elasticsearch5.0
Run Elasticsearch locally in Docker

Build docker image:
``` bash
sudo docker build -t agaton/elasticsearch .
```

Run Docker container:
``` bash
sudo docker run -p 9200:9200 agaton/elasticsearch
```

If elasticsearch:5.0.0 max virtual memory areas vm.max_map_count [65530] likely too low, increase to at least [262144]:
``` bash
sudo sysctl -w vm.max_map_count=262144
```