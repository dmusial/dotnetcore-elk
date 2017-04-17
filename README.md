Before "docker-compose up" make sure to 

* allocate at least 2.5GB RAM to the docker host
* run "sudo sysctl -w vm.max_map_count=262144" on host (required by Elasticsearch)
* change logstash listen address used in gelf driver config in docker-compose.yml