# Forme Selvatiche per Android

App Android del calcolatore delle **Forme Selvatiche** per Druido e Morfico (Collana v2.4): Animali, Vegetali, Parassitiche, Elementali, Draconiche e Giganti, con aspetti, forme minori, evoluzioni, archetipi e armi impugnate.

## Scaricare e installare l'app
1. Apri la pagina **Releases** di questo repository dal telefono.
2. Tocca il file `FormeSelvatiche-N.apk` dell'ultima versione per scaricarlo.
3. Aprilo dalle notifiche o dalla cartella Download. Android chiederà di consentire l'installazione da questa fonte: consentila solo per il browser che hai usato.
4. Le versioni successive si installano sopra la precedente e i personaggi salvati restano.

## Come nasce l'APK
Ogni volta che si aggiorna il ramo `main`, GitHub Actions compila l'app (file `.github/workflows/apk.yml`) e pubblica una nuova release con l'APK. Si può avviare anche a mano da **Actions → Crea APK Android → Run workflow**.

## Struttura
- `www/index.html` — l'app completa (una sola pagina, funziona senza connessione).
- `www/vendor/` — font locali (Alegreya, Alegreya Sans).
- `android/` — progetto Android generato da Capacitor 6.
- `android/app/formeselvatiche.keystore` — chiave di firma: serve per installare gli aggiornamenti sopra la versione precedente. Non cancellarla.
