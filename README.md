# Elasticsearch Dockerfile

NOTE: If you want to run the whole ELK stack checkout: https://github.com/denibertovic/elk-stack-docker


Pull from the Hub:

    docker pull denibertovic/elasticsearch

Run

    docker run --name elasticsearch -d -t denibertovic/elasticsearch

Use volumes to mount conf dir:

    docker run --name elasticsearch -v `pwd`/config-example:/opt/elasticsearch/config \
        -d -t denibertovic/elasticsearch

Ports

    9200
    9300

Volumes

    /opt/elasticsearch/config
    /opt/elasticsearch/data
    /opt/elasticsearch/logs

