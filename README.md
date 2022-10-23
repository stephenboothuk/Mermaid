# Mermaid

## Example Graph DB Model (graph.md)
```mermaid

  graph LR
   subgraph Crime
   Victim --- Transport
   Transport --- Bus_Route
   end
  
   subgraph Suspect_1
   Home --- Relative
   Relative --- Friend
   end
  
   Victim --- Home
   Victim --- Friend

```

