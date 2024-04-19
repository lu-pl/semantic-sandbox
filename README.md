# Semantic Sandbox

Semantic Sandbox is a simple compose stack for running popular Triplestores.

The setup can be useful for end-to-end testing or simply tinkering. 🔧🐱

## Usage
Run `docker-compose` to start the compose environment with all featured Tripelstores.  

```shell
git clone git@github.com:lu-pl/semantic-sandbox.git
cd semantic-sandbox
docker-compose up
```

For port mappings see [Triplestores](https://github.com/lu-pl/semantic-sandbox?tab=readme-ov-file#triplestores) below.  

To run only a single store or a selection of stores, pass the store handle to docker-compose, e.g. `docker-compose up <store1> <store2>`.

## Triplestores

The following Triplestores are currently supported:

***
### <ins>GraphDB</ins>

#### Info
- image: [khaller/graphdb-free](https://hub.docker.com/r/khaller/graphdb-free)
- port: 7270
- SPARQL endpoint: http://127.0.0.1:7270/sparql

#### Notes

Resources: 
- GraphDB Docs: [Configuring a repository](https://graphdb.ontotext.com/documentation/10.6/configuring-a-repository.html)  
- Dockerhub Overview: [khaller/graphdb-free](https://hub.docker.com/r/khaller/graphdb-free)  
- Pokemon Playground: [ontotext-graphdb-playground](https://github.com/pokemon-kg/ontotext-graphdb-playground/tree/main)  
  Very instructive compose setup for GraphDB by [khaller93](https://github.com/khaller93).

***
### <ins>Blazegraph</ins>

#### Info
- image: [lyrasis/blazegraph](https://hub.docker.com/r/lyrasis/blazegraph)
- port: 8889
- SPARQL endpoint: http://127.0.0.1:8889/bigdata/sparql

#### Notes
Resources:
- [Blazegraph Overview](https://blazegraph.com/)
- [Blazegraph Wiki](https://github.com/blazegraph/database/wiki)


***
### <ins>Fuseki</ins>
#### Info
- image: [secoresearch/fuseki](https://hub.docker.com/r/secoresearch/fuseki)
- port: 3030
- SPARQL endpoint: http://127.0.0.1:3030/ds/sparql

For other endpoints see the [Data access](https://hub.docker.com/r/secoresearch/fuseki) section or [SOH - SPARQL over HTTP](https://jena.apache.org/documentation/fuseki2/soh.html).

#### Notes

Resources:
- [Fuseki Docs](https://jena.apache.org/documentation/fuseki2/index.html)



<!-- ################################################## -->
<!-- *** -->
<!-- ### <store name> -->
<!-- #### Info  -->
<!-- - image  -->
<!-- - port -->
<!-- - SPARQL endpoint -->

<!-- #### Notes -->
<!-- ################################################## -->
