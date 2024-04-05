# Semantic Sandbox

Compose stack for running popular Triplestores.

## Usage
Run `docker-compose` to start the compose environment with all featured Tripelstores.  

```shell
git clone git@github.com:lu-pl/semantic-sandbox.git
cd semantic-sandbox
docker-compose up
```

For port mappings see [Triplestores](https://github.com/lu-pl/semantic-sandbox?tab=readme-ov-file#triplestores).

[Todo: Add compose profiles for selecting which Triplestores to start.]

## Triplestores

The following Triplestores are currently supported:

### GraphDB

#### Info
- image: [khaller/graphdb-free](https://hub.docker.com/r/khaller/graphdb-free)
- port: 7270
- SPARQL endpoint: http://127.0.0.1:7270/sparql

#### Notes
[...]

Resources: 
- GraphDB Docs: [Configuring a repository](https://graphdb.ontotext.com/documentation/10.6/configuring-a-repository.html)  
- Dockerhub Overview: [khaller/graphdb-free](https://hub.docker.com/r/khaller/graphdb-free)  
- Pokemon Playground: [ontotext-graphdb-playground](https://github.com/pokemon-kg/ontotext-graphdb-playground/tree/main)  
  Very instructive compose setup for GraphDB by [khaller93](https://github.com/khaller93).
