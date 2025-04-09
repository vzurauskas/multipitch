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
    Leader ->> Leader: Pastato saugą (dar be virvės).
    Second ->> Second: Išsega virvę iš reverso.
    Second ->> Leader: Saugos nėra!
    Leader ->> Leader: Įsega virvę į saugą ir patestuoja autoblock.
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

Prieš kiekvieną virvės signalą, signalizuojantis įtempia virvę.
| Verbal        | After         | Rope      |
| ------------- | ------------- | ---------- |
| Savisauga     | --            | 3 patraukimai, 5 sec, 3 patraukimai. |
| Saugos nėra   | Savisauga     | 3 patraukimai   |
| Sauga yra     | Saugos nėra   | 3 patraukimai   |
| Lipu          | Sauga yra     | 3 patraukimai    |


## Stoties statymas
### Part I.
Užlipęs iki stoties boltų, leaderis:
1) Įsega paskutinę atotampą į stoties boltą toje pusėje, į kurią bus lipama toliau.
2) Įsega virvę į paskutinę atotampą.

### Jei nėra grandinių su žiedu
1) Įsega karabiną į kitą boltą, ir abi savisaugas į jį.
2) Įsega piemens mazgą į atotampą (for redundancy).
3) [Pastato stotį](https://www.wallrat.com/PDF_Files/Anchoring.pdf). Statant teks trumpam atidaryti karabiną, kuriame savisaugos, ir išsegti atotampą, kurioje piemens mazgas, bet viskas ok, nes abiem atvejais dar yra kitas taškas.
4) Išsega savisaugas iš bolto karabino ir įsega į stoties žiedą.

