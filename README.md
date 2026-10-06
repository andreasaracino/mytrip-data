# MyTrip — dati per il percorso offline

Questo repository contiene solo i **dati** che l'app [MyTrip](https://github.com/andreasaracino/mytrip)
scarica per calcolare il percorso dei camion sul telefono, senza internet.

Ogni [Release](../../releases) contiene:

- `italia.mytripgraph.gz`: il grafo stradale dell'Italia per mezzi pesanti, compresso;
- `manifest.json`: formato, data dei dati, dimensione e impronta SHA-256 del grafo.

L'app legge sempre l'ultima Release (`releases/latest/download/manifest.json`).
I file sono preparati e pubblicati dal workflow "Grafo offline" del repository
`mytrip`: non vanno modificati a mano.

## Licenza dei dati

Il grafo è un database derivato da [OpenStreetMap](https://www.openstreetmap.org/copyright):

**© OpenStreetMap contributors**, disponibile con licenza
[Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/).
Chi lo usa o lo ridistribuisce deve citare OpenStreetMap e mantenere la stessa licenza.
