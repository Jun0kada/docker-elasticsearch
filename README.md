# docker-elasticsearch

Elasticsearch docker images for development and testing.

<!-- TOC -->

- [docker-elasticsearch](#docker-elasticsearch)
  - [Feature](#feature)
  - [Docker Hub](#docker-hub)
  - [Usage](#usage)
  - [Maintenance](#maintenance)
  - [Release Engineering](#release-engineering)
  - [Copyright](#copyright)

<!-- /TOC -->
<!-- TOC generated by https://marketplace.visualstudio.com/items?itemName=AlanWalk.markdown-toc -->

## Feature

- Disable Bootstrap check
  - https://discuss.circleci.com/t/running-elasticsearch-5/8559/7
- Disable X-Packs Security
  - because it is not required for development

## Docker Hub

https://hub.docker.com/r/jun0kada/elasticsearch

## Usage

```sh
docker pull jun0kada/elasticsearch
```

## Maintenance

Use the latest version of Amazon Elasticsearch Service:

* https://aws.amazon.com/elasticsearch-service/faqs/

The available versions are listed here:

* https://github.com/elastic/elasticsearch/releases

And you can check to build images with:

```console
make # or `make check`
```

## Release Engineering

The docker images are automatically published via Circle CI when merging to `master` branch.

In order to manually publish a new image, run:

```sh
docker login
make publish
```

## Copyright

Copyright 2017, Bit Journey, Inc.
