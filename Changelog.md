# Changelog

## Unreleased [2020-02-29]

- PathCollections to find similar paths with a simple API (`paths`, `step`, `steps`, and `follow` procs)
- Paths to easily walk the graph
- Neo4j client, use `dump` proc to load graph database as grim LPG

## v.0.2.0 [2020-02-07]

- Complete "Northwind" tutorial to show how SQL database is transferred to LPG.
- DSL module must now be explicitly imported ("import grim/dsl").
- Documentation for all procs, iterators, templates, and macros.
- Introduced directionality in the graph structure, i.e., discriminate between incoming and outgoing edges (or both) in all iterators and procs.
- Improved API: getNode, getEdge -> node, edge and getEdges -> edgesBetween.
- Closure iterators for nodes and edges.
- New procs delNode/delEdge to remove nodes and edges from the graph.
- New API where node/edge properties are available directly on the node/edge (myNode["name"] rather than myNode.properties["name"])
- Use HashTables for all node and edge indices.
- Updated and expanded all unit tests.
- Indexing by node and edge labels.
- Make sure entites are ref objects to avoid excessive copying.
- Updated all documentation.
- Equality operators for nodes and edges.
- Documentation website at https://ebran.github.io/grim/.

### v.0.1.1 [2020-01-12]

- Added grim icon
- Fixed README bugs
- Fixed .nimble bugs

## v0.1.0 [2020-01-12]

- Initial release!
- Basic usage: add, get, etc.
- DSL for graph building.
- Load/save YAML graphs
- Iterators for nodes and edges