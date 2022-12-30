---
title: "ISO OSI - Livello Datalink"
author: ["Federico Zotti"]
date: 2022-01-17
tags: ["Scuola", "OSI", "Networking"]
titlepage: true
toc-own-page: true
---

# Error control

Per essere sicuri che tutti i frame inviati sulla rete siano privi di errori e in ordine verranno usati alcuni bit per la _parità_.

## Parità dispari | pari

Viene aggiunto un bit finale per fare in modo che i bit ad 1 siano pari/dispari.

Questo permette solo di rilevare un solo errore (non due), ma non di correggerlo.

## Tasso di errore

Il tasso di errori è il rapptte solo di rilevare un solo errore (non due), ma non di correggerlo.

## Tasso di erroreorto tra i bit ricevuti e gli errori.

Esempi:

- fibra ottica: $\tau = 10^{-14}$
- ethernet: $\tau = 10^{-10}$

probabilità:
$$
p = 1 - \tau
$$

## Codici di Hamming

$$
n = m + r
$$

- Le codeword totali sono: $2^n$.
- Le codeword totali valide sono: $2^m$.
- Codeword con un bit diverso: $n+1$.
- Codeword valide e con un bit diverso da quelle valide: $(n+1) \times 2^m$.

Queste devono essere meno delle codeword valide: $(n+1) \times 2^m < 2^n \rightarrow m+r+1 < 2^r$.

//La distanza minima tra codeword deve essere $2d+1$.

### Esempio

- $m = 5$;
- $r = 4$;
- $n = 9$;

Hamming code (9, 5) autocorrezione ad un bit.

|  syn  r   r   m   r   m   m   m   r   m
|   0   1   2   3   4   5   6   7   8   9
| 
|      r0  r1  m0  r2  m1  m2  m3  r3  m4
| [  ][   |   |   |   |   |   |   |   |   ]

syn indica la posizione del bit sbagliato.

# Medium Access Control Sublayer

## Giocattolini che permettono di creare una rete

I bridge hanno più NIC con lo stesso MAC che permettono di collegare più protocolli diversi (ethernet / wifi).

## :/

Se più dispositivi parlano sullo stesso canale si crea una collisione.

### Punti chiave

- Comunicazioni indipendenti;
- Single channel;
- Observable collision by the trasmitter;
- Continuous or Slotted time;
- Carrier Sense or No Carrier Sense.
 
## ALOHA

pag. 263

Il primo protocollo di rete.
Si appoggiava ad un satellite geostazionario.

# 802.11: WiFi

Le reti wireless hanno un costo minore perché si elimina tutto il costo dietro l'installazione dei cavi e dell'infrastruttura collegata hai cavi ethernet fisici.

Nella _infrastructure mode_tutto il traffico avviene tra access point e NIC, due NIC non si possono parlare direttamente.

Nella rete _ad hoc_ invece le NIC possono inviare frame direttamente tra di loro e non è presente un access point.
