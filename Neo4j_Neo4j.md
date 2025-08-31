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
  - Each entity are stored as a separate node in the graph.

- Labels
  - The nodes are grouped by using *labels*.
  - Like person, customer
  - Same types of Nodes have same label.
  - mainly used to filter the Nodes.
  - A Node can has multiple labels

- Relationships
  - The lines in the above graph are *relationship*.
  - Describe how nodes are connected with each other.
  - *Start* and *End* nodes are connected.
  - All the relationship has:
    - *type*
    - *direction*
  - Nodes can have multiple relationships.

- Properties
  - Can store data against nodes and relationships as *properties*.
  - It is key-value pair.


>When relationship is created between the two odes, 
>a pointer to the relationship is created and stored in 
>the memory. When querying, the pointer is used.
>This is used query faster.






