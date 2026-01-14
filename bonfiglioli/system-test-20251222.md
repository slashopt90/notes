# System Test 2025 12 22

## Data collection custom
### Errori
- errore in creazione 
- add parameter non apre il popup in fase di creazione
- aggiungere un parametro dalla lista esistente
- current version sempre false 
- verificare il salvataggio dei custom data ( O,S etc... )
- non funziona la modifica di un parametro dalla gestione parametri


### Feature
- implementare max/min con il delta
- implementare backend parametri function
- implementare backend attended/unattended
- implementare backend controllo periodico basato su pezzi contati
- se esco da unattended e non ho raggiungto la soglia proporre cmq piano di controllo


## Machining POD
### Feature
- fare il reset all'avvio dell'ordine
- cambiare da Machine Status a "stato super fermo" e cambiare connected in "SI\NO"
- raggruppare buoni e scarto e non conformi in una tile
- raggruppare prodotti e disponibili in una tile
- aggiungere sign off ( verificare che i giri setup etcc funzionino da capo )
- non passare al moving se Q1 non fatto
- proporre Q1 solo se InitialChecking partito
- aggiunta campo note nell'apertura non conformità
- salvataggio body per ristampa manca report type
- invio alert non funziona / buggato. Ticket?
- naming-convention per colata
- errore nell'apertura di direct labor per sfc?
- stampa automatica alla dichiarazione di produzione, stampo tutti i pezzi della HU, svuoto la HU.
- plugin stampa fare solo reprint
- fare partire in automatico la quantità sulla fase successiva se sfc è già active
- all'apertura della nonconformità controllo sulla disponibilità
- all'apertura della nonconoformità decremento la disponibilità
- se non ho quantità disponibile per lo scarto, la incremento automaticamente
- Work instructions non VIOLA


## Quality POD
- Aggiungere plugin next step se selezionata SFC SETUP per far partira Compensation
- Creare indirect labor Returning se Nonconformità KO, WaitingForStart se OK
- Aggiungere descrizione, materiale, order,  note
- Opened At mancante
- Nella description della stampa della nonconformità, aggiungere il workcenter di destinazione ("EVO")
- Quando i pezzi nonconformi sono dichiarati come buoni non faccio niente, sarà l'operatore della produzione che li dichiara normalmente 
- se non ho quantità disponibile per lo scarto, la incremento automaticamente

## Error
- controllare popup setup obbligatorio spostandomi di ordine
- disabilitare interfaccia machining se SFC non in stato ACTIVE
- controllare invio alert

## Andon sala metrologica
### Errori
- Non funziona
