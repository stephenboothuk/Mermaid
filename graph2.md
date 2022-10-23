```mermaid

  graph LR
   subgraph Crime
   Victim --- Bus
   Bus --- BusRoute
   end
  
   subgraph Suspect_1
   Home --- Relative
   Relative --- Friend
   end
   
   subgraph MobilePhone
   SamsungJ10 --- PawnBroker
   SamsungJ10 --- IMIE12345
   end
  
   Victim --- Home
   Victim --- Friend
   Victim --- SamsungJ10
   PawnBroker --- Home
   Relative --- PawnBroker

```
