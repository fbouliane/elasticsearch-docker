## Do it

Do

    ELASTIC_VERSION=5.6 make build
    docker run -P -it docker.elastic.co/elasticsearch/elasticsearch:5.6
    curl -u elastic:changeme localhost:9200/_cluster/health | jq .

now you can change your docker files to inherit from

    elasticsearch:5 => docker.elastic.co/elasticsearch/elasticsearch:5.6
