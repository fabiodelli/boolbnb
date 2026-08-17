# BoolBnB

Piattaforma di annunci per affitti brevi: ricerca degli appartamenti per zona e servizi,
scheda del singolo alloggio, messaggi dal potenziale ospite al proprietario, area privata
con dashboard, sponsorizzazioni a pagamento degli annunci e statistiche di visualizzazione.

Progetto di gruppo realizzato in **cinque persone** durante il bootcamp, giugnoâ€“luglio 2023.
Diviso in due repository:

| | |
|---|---|
| **Frontend** (questo repo) | Vue 3 + Vite, consuma le API del backend |
| **Backend** | Laravel â€” [boolbnb-backend](https://github.com/fabiodelli/boolbnb-backend) |

Sono entrambi fork dei repository originali del team, di
[@luca-macedone](https://github.com/luca-macedone)
([frontend](https://github.com/luca-macedone/team_3_boolbnb_front) Â·
[backend](https://github.com/luca-macedone/team_3_boolbnb_back)).

## Stack

**Frontend** â€” Vue 3, Vue Router, Vite, Axios, Bootstrap 5 + Sass, Vuelidate per la
validazione dei form, Luxon per le date.

**Backend** â€” Laravel con autenticazione Breeze, MySQL. Modelli: `Apartment`, `Service`,
`Message`, `Sponsorship`, `View`, `User`. Controller separati per l'area utente e per le
API consumate dal front.

## Il mio contributo

79 commit sui due repository: 45 sul frontend, 34 sul backend.

**Backend** â€” La feature delle **visualizzazioni**, costruita end-to-end: il modello
`View` con la relazione verso `Apartment`, la migration, la policy di accesso, il CRUD del
controller e l'autorizzazione sui metodi di lettura. Sopra questa base, le statistiche
della dashboard: visite totali per utente e appartamento piÃ¹ visto. Infine la rotta API
che espone i dati al frontend.

**Frontend** â€” I metodi di chiamata alle API nello state condiviso, la barra di ricerca
in home e la ricerca avanzata con filtri, le card dei risultati con la valutazione a
stelle, e una parte consistente del layout (navigazione fissa, footer, jumbotron,
regole responsive).

---

*Questo README Ã¨ stato scritto per il fork: il repository originale non ne aveva uno.
Il codice Ã¨ il lavoro collettivo del team, i crediti sopra.*
