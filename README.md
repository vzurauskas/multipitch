# Multipitch

## High level process
```mermaid
sequenceDiagram
    Leader ->> Leader: Užlipa pitchą.
    Leader ->> Leader: Įsisega savisaugą.
    Leader ->> Leader: Pastato stotį.
    Leader ->> Leader: Sutraukia virvę (per atotampą) kol traukiasi.
    Leader ->> Second: Savisauga!
    Leader ->> Leader: Atpalaiduoja virvę.
    Second ->> Second: Išsega virvę iš reverso.
    Second ->> Leader: Saugos nėra!
    Leader ->> Leader: Pastato saugą (su autoblock).
    Leader ->> Leader: Sutraukia likusią virvę iki įtempimo.
    Leader ->> Second: Sauga yra!
    Second ->> Second: Išrenka stotį.
    Second ->> Leader: Lipu!
    Second ->> Second: Užlipa iki stoties.
    Leader ->> Leader: Knisasi stoty.
    Second ->> Second: Knisasi stoty.
    Leader ->> Leader: Lipa kitą pitchą.
    
```

### Communication

| Verbal        | After         | Rope      |
| ------------- | ------------- | ---------- |
| Savisauga     | --            | 3 patraukimai, 5 sec, 3 patraukimai. |
| Saugos nėra   | Savisauga     | 3 patraukimai   |
| Sauga yra     | Saugos nėra   | 3 patraukimai   |
| Lipu          | Sauga yra     | 3 patraukimai    |

