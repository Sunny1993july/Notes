# This the note for Graph Database
``` 
                  ┌─────────┐
      ╔═══════════╣  Server ╠════════════╗
      ║           └─────────┘            ║
      ║                 │                ║
  ┌───┴───┐       ┌─────┴─────┐      ┌───┴───┐
  │  DB-1 ├───┐   │  Load     │      │  User │
  └───────┘   │   │ Balancer  │      └───────┘
              │   └─────┬─────┘          │
              │         │                │
          ┌───┴───┐     │                │
          │  App  │◄────┼───────────────►│
          │ Node1 │     │                │
          └───────┘     │                │
             │          │                │
             v          v                v
          ┌───┴───┐   ┌──┴──┐   ┌─────────┐
          │ Cache │───┤  API├───┤Billing  │
          └──┬────┘   └─────┘   └─────────┘
             │
             │
             v
        ┌─────────┐
        │  Data   │
        │  Store  │
        └─────────┘




```
#### Neo4J is a database that use the graph to store the data.

Graph database is use when the data and its relationship, both are important.

*Labeled property graph* -> used in the Neo4j.

## The Data within Neo4j is stored and organized as:

- Nodes
  - In above example, the square in graph is *Node*.
  - They typically represent an *objects* or *entities*.
  - Eg. people, locations and customers.
  - 


