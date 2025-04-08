# Multipitch

## High level process
```mermaid
sequenceDiagram
    Leader ->> Leader: Užlipa pirmą pitchą.
    Leader ->> Leader: Įsisega savisaugą.
    Leader ->> Leader: Pastato stotį.
    Leader ->> Leader: Sutraukia virvę (kol traukiasi).
    Second ->> Leader: ? (1)
    Leader ->> Second: Gali išsisegt! (2)
    Second -->> Leader: Supratau!
    Second ->> Second: Išsega virvę iš reverso.
    Second ->> Leader: Saugos nėra!
    Leader -->> Second: Supratau!
    Leader ->> Leader: Pastato saugą (su autoblock).
    Leader ->> Leader: Sutraukia likusią virvę iki įtempimo.
    Leader ->> Second: Sauga yra!
    Second -->> Leader: Supratau!
    Second ->> Leader: Lipu!
    Leader -->> Second: Supratau!
    
```
Process questions:
1) Angliškai: "That's me!" Kaip lietuviškai?
2) Ar "Savisauga!" ?

### Communication

| Verbal        | After         | Rope      |
| ------------- | ------------- | ---------- |
| Savisauga     | --            | 3 patraukimai, 5 sec, 3 patraukimai. (1) |
| Supratau      | --            | ?            |
| Saugos nėra   | Savisauga     | ?            |
| Sauga yra     | Saugos nėra   | 3 patraukimai   |
| Lipu          | Sauga yra     | 3 patraukimai    |

Communication questions:
1) Kaip padaryt, kad jaustųsi patraukimai, jei virvėje slackas?

### General questions
1) Verbal + rope communication, or rope only?
