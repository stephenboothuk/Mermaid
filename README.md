# Mermaid

## Example Graph DB Model (graph.md)
```mermaid

  graph LR
   subgraph Crime
   Area --- Transport
   Transport --- Bus Route
   end
  
   subgraph Suspect 1
   Home --- Relative
   Relative --- Friend
   end
  
   Area --- Home
   Area --- Friend

```

