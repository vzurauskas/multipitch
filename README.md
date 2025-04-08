# Multipitch

## High level process
```mermaid
sequenceDiagram
    Leader ->> Leader: Užlipa pirmą pitchą.
    Leader ->> Leader: Įsisega savisaugą.
    Leader ->> Second: Savisauga!
    Second -->> Leader: Supratau!
    Second ->> Second: Išsega virvę iš reverso.
    
    
```
### Communication

| Verbal        | After         | Rope      |
| ------------- | ------------- | ---------- |
| Savisauga     | --            | 3 patraukimai, 5 sec, 3 patraukimai. (1) |
| Supratau      | --            | ?            |
| Gali lipt     | Savisauga     | 3 patraukimai   |
| Lipu          | Gali lipt     | 3 patraukimai    |

Questions:
1) Kaip padaryt, kad jaustųsi patraukimai, jei virvėje slackas?
