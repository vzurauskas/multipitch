# Multipitch

## High level process
```mermaid
sequenceDiagram
    Leader ->> Leader: Užlipa pitchą.
    Leader ->> Leader: Įsisega savisaugą.
    Leader ->> Leader: Pastato stotį.
    Leader ->> Leader: Sutraukia virvę (per atotampą) kol traukiasi.
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
    Second ->> Second: Išrenka stotį.
    Second ->> Leader: Lipu!
    Leader -->> Second: Supratau!
    Second ->> Second: Užlipa iki stoties.
    Leader ->> Leader: Knisasi stoty.
    Second ->> Second: Knisasi stoty.
    Leader ->> Leader: Lipa kitą pitchą.
    
```
Process questions:
1) Angliškai: "That's me!" Kaip lietuviškai?
2) Ar "Savisauga!" ?

### Communication

| Verbal                    | After         | Rope      |
| -------------             | ------------- | ---------- |
| That's me                 | --            | ?            |
| Savisauga / Gali išsisegt | --            | 3 patraukimai, 5 sec, 3 patraukimai. (1) |
| Supratau                  | --            | ?            |
| Saugos nėra               | Savisauga     | ?            |
| Sauga yra                 | Saugos nėra   | 3 patraukimai   |
| Lipu                      | Sauga yra     | 3 patraukimai    |

Communication questions:
1) Kaip padaryt, kad jaustųsi patraukimai, jei virvėje slackas?

### General questions
1) Verbal + rope communication, or rope only?
