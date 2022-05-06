## Do it

Do

    ELASTIC_VERSION=5 make build
    docker run -p 9200:9200 -it elasticsearch:5
    curl -u elastic:changeme localhost:9200/_cluster/health | jq .

now you can change your docker files to inherit from

    elasticsearch:5
