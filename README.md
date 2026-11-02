# high-cde

Repository associato all’ecosistema ZDOS. Contiene documentazione e file sorgente `.zl` relativi al modulo `high-cde`, a una configurazione di mesh e a un manifest.

## Contenuti

- [`mesh_route.zl`](mesh_route.zl) dichiara un nodo `high-cde`, un protocollo di routing e un valore di cifratura.
- [`sovereign_manifest.zl`](sovereign_manifest.zl) definisce il modulo `high-cde` e richiama `verify_zero_legacy()` e `connect_dsn_mesh()`.
- [`zlang_core/high-cde_engine.zl`](zlang_core/high-cde_engine.zl) definisce `execute_native_workflow()`, che richiama funzioni indicate come appartenenti a `zdos.kernel` e `zdos.dsn_ledger`.
- [`docs/wiki/`](docs/wiki/) raccoglie pagine su architettura, operazioni e roadmap.

Queste descrizioni riportano ciò che è dichiarato nei file; da sole non attestano che le funzioni, le dipendenze o i protocolli siano implementati o verificati in un ambiente eseguibile.

## Installazione, esecuzione e test

Il repository non documenta una toolchain, dipendenze, comandi di installazione o avvio, né procedure o test automatizzati. Non è quindi possibile indicare comandi verificati per compilare, eseguire o testare i file `.zl`.

## Licenza

Il repository contiene un file [`LICENSE`](LICENSE) con i termini applicabili. Consultalo prima di usare, modificare o ridistribuire i contenuti.
