# Problema 1

Status: In progress

**Evento: La Crisi dei Pezzi di Motore**

Durante un’ispezione di routine, il capo ingegnere della *Nova Pioneira* scoprì un problema critico nei propulsori della nave. Alcuni dei moduli motore erano gravemente usurati e necessitavano di pezzi di ricambio per continuare a funzionare. Tuttavia, i pezzi di ricambio disponibili non erano sufficienti per migliorare tutti i moduli allo stesso livello.

Il capitano convocò una riunione urgente per discutere la situazione.

**“Abbiamo *n* moduli motore,”** spiegò il capo ingegnere, indicando un diagramma. **“Ogni modulo ha una sua efficienza attuale. Se diamo a un modulo tutti i pezzi di ricambio extra, la sua efficienza aumenterà di un valore fisso. Dobbiamo capire per quali moduli questo miglioramento li renderà i migliori rispetto agli altri.”**

**“E se nessuno dei moduli migliorati riesce a superare gli altri?”** chiese l’ufficiale di navigazione.

**“Allora quei pezzi saranno stati sprecati,”** rispose il capo ingegnere, preoccupato. **“Dobbiamo calcolare attentamente quale modulo, con i pezzi extra, potrebbe davvero diventare il più efficiente.”**

Il compito era chiaro: analizzare ogni modulo motore, calcolando se, con i pezzi extra, la sua efficienza avrebbe superato o eguagliato quella di tutti gli altri.

**Esempio di Input e Spiegazione**

Supponiamo di avere 5 moduli motore con le seguenti efficienze iniziali e **3 pezzi di ricambio** disponibili:

```
efficienza = [4, 2, 7, 1, 6]
pezziExtra = 3
```

Dopo aver aggiunto i pezzi di ricambio a ogni modulo, si ottiene:

- Modulo 1:  → Può raggiungere l’efficienza del migliore **(4 + 3 = 7)** → **`true`**.
- Modulo 2:  → Non può superare il migliore **(2 + 3 < 7)** → **`false`**.
- Modulo 3:  → Può raggiungere l’efficienza del migliore **(7 + 3 > 7)** → **`true`**.
- Modulo 4:  → Non può superare il migliore **(1 + 3 < 7)** → **`false`**.
- Modulo 5:  → Può raggiungere l’efficienza del migliore **(6 + 3 > 7)** → **`true`**.

**Output finale**:

```
[true, false, true, false, true]
```

**Compito Finale**

Ora tocca a te: il computer centrale ha rilevato un problema su scala molto più grande. Ci sono **100 moduli motore** e il valore di pezziExtra è **18**. Ogni modulo ha una sua efficienza casuale (compresa tra 1 e 100). Calcola per ciascun modulo se, con i pezzi extra, diventerà o meno il migliore.

**Compito:**

Scrivi un algoritmo per determinare, per ogni modulo, se potrebbe diventare il migliore tra tutti aggiungendo i pezzi extra. Buona fortuna, l’equipaggio della *Nova Pioneira* conta su di te! 🚀

**Input:**

[efficienza.txt](Problema%201/efficienza.txt)