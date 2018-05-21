# Elasticsearch Curator

## Intro

This is a Docker image for the [Elasticsearch Curator](https://www.elastic.co/guide/en/elasticsearch/client/curator/current/index.html) based on the Python 3 Alpine image.

## Build

	docker build -t jenciso/elasticsearch-curator .

## Usage

Run using environment vars. Example:

	docker run  -e "ELASTICSEARCH_HOST=elasticsearch.domain.com" -e "INDEX_TO_DELETE=filebeat" -e "OLDER_THAN_IN_DAYS=7" jenciso/elasticsearch-curator
