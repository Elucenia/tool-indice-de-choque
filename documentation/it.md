<!-- ELUCENIA technical documentation · indice-de-choque · it · no clinical/professional/rights approval -->

# Indice di shock (e modificato)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/indice-de-choque)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Frequenza cardiaca

`fc`

bpm · intervallo: 20–250

### Pressione sistolica

`pas`

mmHg · intervallo: 30–300

### Pressione diastolica (per l’indice modificato)

`pad`

mmHg · facoltativo · intervallo: 10–200

## Edizione del metodo

Shock Index/Allgöwer 1967 FC/PAS e indice modificato/Liu 2012 FC/PAM

## Formula documentata

Indice di shock = FC ÷ PAS (normale: 0,5–0,7).

Indice di shock modificato = FC ÷ PAM, con PAM = PAD + (PAS − PAD) ÷ 3 (normale: 0,7–1,3).

## Limiti e popolazione

L’indice di shock usa la frequenza cardiaca divisa per la pressione sistolica; quello modificato usa la pressione arteriosa media. Sono rapporti diversi e da soli non diagnosticano shock né necessità di trasfusione. Mutschler 2013 ha valutato l’indice all’arrivo in pronto soccorso in 21.853 adulti traumatizzati; Liu 2012 ha studiato retrospettivamente 22.161 pazienti di 10–100 anni che avevano ricevuto liquidi endovenosi, escludendo arresti cardiorespiratori rianimati senza triage. Queste coorti non dimostrano soglie universali per bambini di tutte le età, gestanti o altre situazioni. Registra momento e condizioni delle misure; le associazioni con mortalità ospedaliera di una coorte non sono previsioni individuali automatiche.

## Riferimenti

- [Allgöwer M, Burri C. „Schockindex". Dtsch Med Wochenschr, 1967.](https://doi.org/10.1055/s-0028-1106070)

- [Mutschler M et al. The Shock Index revisited – a fast guide to transfusion requirement? A retrospective analysis on 21,853 patients derived from the TraumaRegister DGU. Crit Care, 2013.](https://doi.org/10.1186/cc12851)

- [Liu YC et al. Modified shock index and mortality rate of emergency patients. World J Emerg Med, 2012.](https://doi.org/10.5847/wjem.j.issn.1920-8642.2012.02.006)

- [Liu2012](https://pmc.ncbi.nlm.nih.gov/articles/PMC4129788/)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Nessuno shock (IC < 0,6)


### 2

Shock lieve (IC 0,6 a < 1,0)

| Dettagli del risultato | |
| --- | --- |
| Indice di shock modificato (FC/PAM) | 1,18 (0,7 a 1,3) |


### 3

Shock moderato (IC 1,0 a < 1,4)


### 4

Shock grave (IC ≥ 1,4)

