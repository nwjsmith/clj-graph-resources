Clojure graph resources
=======================
This is a curated list of mostly mature and/or actively developed Clojure resources relevant for dealing with graph-like data. It's currently being expanded as I explore this area more thoroughly. Suggestions are welcome in the form of pull requests or Github issues. I try to steer around abandonware, though.

Data structures / algorithms
----------------------------
* [aysylu/loom](https://github.com/aysylu/loom): Graph library for Clojure.
* [Engelberg/ubergraph](https://github.com/Engelberg/ubergraph): An all-purpose Clojure graph data structure that implements Loom protocols and more.
* [ont-app/igraph](https://github.com/ont-app/igraph): IGraph defines a protocol which aims to provide a general interface to a variety of graph-based representations.

Visualisation
-------------
* [jebberjeb/specviz](https://github.com/jebberjeb/specviz): Generate Graphviz images from clojure.spec.

Databases
---------
### Labeled-property graph
Labeled-property graph databases use complex graph models where edges and vertices can have both labels and associated properties.

* [gorillalabs/neo4j-clj](https://github.com/gorillalabs/neo4j-clj): Clojuresque client to Neo4j database, based upon the bolt protocol.
* [full-spectrum/neo4clj](https://github.com/full-spectrum/neo4clj): Neo4clj is a idomatic clojure client, exclusivly using Bolt for performance.         

### RDF
RDF triplestores are a specialised type of graph database for representing knowledge graphs; part of the W3C Semantic Web standards.

* [arachne-framework/aristotle](https://github.com/arachne-framework/aristotle): An RDF/OWL library for Clojure, providing a data-oriented wrapper for Apache Jena.
  - [ont-app/igraph-jena](https://github.com/ont-app/igraph-jena): This is a port of the Jena APIs to the IGraph protocol.
* [Swirrl/grafter](https://github.com/Swirrl/grafter): Linked Data & RDF Manufacturing Tools in Clojure.
  - [ont-app/igraph-grafter](https://github.com/ont-app/igraph-grafter): A port of the IGraph protocols to the Grafter protocols.
* [fluree/db](https://github.com/fluree/db): Fluree is an immutable, temporal, ledger-backed semantic graph database that has a cloud-native architecture.
* [Swirrl/csv2rdf](https://github.com/Swirrl/csv2rdf): Clojure library and application for converting CSV to RDF.
* [ont-app/vocabulary](https://github.com/ont-app/vocabulary): Utilities to map between clojure namespaced keywords and RDF-style URIs.

### Datalog
Clojure's Datomic-like databases also model data as triplets... or technically as quintuplets AKA datoms.

* [Datomic.com](https://www.datomic.com/): _(PROPRIETARY)_ A transactional database with a flexible data model, elastic scaling, and rich queries.
  - [vvvvalvalval/datofu](https://github.com/vvvvalvalval/datofu): This library provides common utilities for working with Datomic, mostly in the form of database functions.
  - [vvvvalvalval/datalog-rules](https://github.com/vvvvalvalval/datalog-rules): Utilities for managing Datalog rulesets from Clojure.
  - [Provisdom/spectomic](https://github.com/Provisdom/spectomic): Generate Datomic or Datascript schema from your Clojure(script) specs.
  - [ont-app/datomic-client](https://github.com/ont-app/datomic-client): Ports the Datomic Client to the IGraph protocols.
* [tonsky/datascript](https://github.com/tonsky/datascript): An immutable in-memory database and Datalog query engine in Clojure and ClojureScript.
  - [mpdairy/posh](https://github.com/mpdairy/posh): Posh is a ClojureScript / React library that lets you use a single DataScript database to store your app state.
  - [denistakeda/re-posh](https://github.com/denistakeda/re-posh): Re-posh allows Posh and re-frame to work together by adding support for re-frame specific subscriptions, events, effects, and co-effects to Posh.
  - [metasoarous/datsync](https://github.com/metasoarous/datsync): This library offers tools for building DataScript databases as materialized views (very much in the re-frame/samsa sense) of some master/central Datomic database.
  - [ont-app/datascript-graph](https://github.com/ont-app/datascript-graph): An implementation of the IGraph protocol extended to datascript.
* [replikativ/datahike](https://github.com/replikativ/datahike): Datahike is a durable Datalog database powered by an efficient Datalog query engine.
  - [replikativ/datahike-frontend](https://github.com/replikativ/datahike-frontend): A front-end to Datahike written in Fulcro.
* [juji-io/datalevin](https://github.com/juji-io/datalevin): Datalevin is a simple durable Datalog database.
* [threatgrid/asami](https://github.com/threatgrid/asami): An in-memory graph database, for Clojure and ClojureScript.
  - [threatgrid/asami-loom](https://github.com/threatgrid/asami-loom): This library extends Asami in-memory graphs to Loom.
* [juxt/crux](https://github.com/juxt/crux): Crux is a general purpose database with graph-oriented bitemporal indexes.
* [Workiva/eva](https://github.com/Workiva/eva): Eva is a distributed database-system implementing an entity-attribute-value data-model that is time-aware, accumulative, and atomically consistent.
* [threatgrid/naga](https://github.com/threatgrid/naga): Datalog based rules engine.
* [den1k/nldl](https://github.com/den1k/nldl): Natural Language for Clojure's Datalog flavor as present in Datomic, Datascript, Datahike etc.

Community
---------
RDF has a small, but steady Clojure following. People are using Neo4j with Clojure, but not talking much about it. Datomic-like Datalog databases have the most momentum.

* [Clojurians Slack](https://clojurians.slack.com/messages): Where Clojure's most active users seem to hang out.
  - [#neo4j](https://clojurians.slack.com/archives/C01BMKFSL14)
  - [#rdf](https://clojurians.slack.com/archives/C09GHBXRC)
  - [#datalog](https://clojurians.slack.com/archives/CJ322KHNX)
  - [#datomic](https://clojurians.slack.com/archives/C03RZMDSH)
  - [#datascript](https://clojurians.slack.com/archives/C07V8N22C)
  - [#datahike](https://clojurians.slack.com/archives/CB7GJAN0L)
