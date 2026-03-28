# Funzione Capotavolo

Questa implementazione introduce una modalità "capotavolo" attivabile su tavoli specifici.

## Funzionalità principali

- Il primo giocatore che si siede al tavolo diventa capotavolo.
- Il tavolo non parte automaticamente quando è pieno.
- Solo il capotavolo vede il comando di avvio tavolo.
- Solo il capotavolo può avviare manualmente la partita.
- Solo il capotavolo può espellere un giocatore seduto.
- L'espulsione è consentita solo prima dell'inizio della partita.
- Il capotavolo non può espellere se stesso.
- Dopo l'espulsione, il giocatore viene bloccato temporaneamente dal rientro al tavolo.

## Regole aggiuntive sui ruoli

La funzione di espulsione è consentita solo se il capotavolo è: (richiesta mop)
- apprendista
- registrato
- certificato

Un utente non registrato può sedersi al tavolo e diventare capotavolo, ma non può usare l'espulsione.

## Configurazione attuale

```php
$G_enable_captain_mode = true;
$G_captain_tables = array(0,1,2,3,40,41,42,43);
