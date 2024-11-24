# Problema 5

Status: In progress

**Evento Finale: Il Puzzle del Motore Finale**

Dopo aver superato il codice delle stelle e decifrato il messaggio alieno, la *Nova Pioneira* sembrava pronta a completare la sua missione verso Alpha Centauri. Ma il capitano sapeva che gli alieni non avevano ancora rivelato tutto. Proprio mentre i motori principali si riavviavano, un’ultima sequenza di dati criptati venne inviata dalla sonda aliena.

**“Capitano,”** disse l’ingegnere capo con voce tesa. **“Abbiamo un altro problema… e questa volta è più complesso di qualsiasi cosa vista finora.”**

Sul monitor olografico apparve una lista di compiti meccanici essenziali per stabilizzare il reattore a curvatura. Tuttavia, ogni compito aveva una difficoltà intrinseca e doveva essere completato in un ordine preciso. La situazione era critica: i lavori dovevano essere distribuiti nell’arco di **d giorni**, rispettando la complessità di ciascuno e garantendo che almeno un compito venisse completato ogni giorno. La stabilizzazione del motore dipendeva dalla minimizzazione dello stress giornaliero sull’equipaggio e sulle risorse disponibili.

**“Se non pianifichiamo questa operazione perfettamente,”** spiegò l’ingegnere, **“il reattore si sovraccaricherà, e perderemo la capacità di navigare nello spazio profondo. Dobbiamo trovare il modo di completare tutti i lavori nel tempo dato, riducendo al minimo la difficoltà complessiva delle operazioni quotidiane.”**

Il capitano fissò lo schermo, osservando i valori delle difficoltà come se fossero geroglifici alieni.

**“E se non ci riusciamo?”** chiese l’ufficiale scientifico.

**“Se non ci riusciamo,”** rispose il capitano con tono grave, **“la *Nova Pioneira* diventerà un relitto alla deriva nello spazio.”**

**Esempio della Situazione**

Per esempio, i compiti erano elencati come segue:

```
jobDifficulty = [6, 5, 4, 3, 2, 1]
d = 2
```

•	In un giorno, potevano essere completati i primi 5 lavori, con una difficoltà massima di 6. 

**nota:** La difficoltà di un giorno è la massima difficoltà di un lavoro svolto in quel giorno.

•	Nel giorno successivo, il lavoro rimanente avrebbe avuto una difficoltà di 1.

Il totale sarebbe stato **6 + 1 = 7**, una soluzione accettabile. Ma ogni decisione contava, e la nave non poteva permettersi errori.

![https://assets.leetcode.com/uploads/2020/01/16/untitled.png](https://assets.leetcode.com/uploads/2020/01/16/untitled.png)

**Altri esempi:**

**Input 1:**

```
jobDifficulty = [9, 9, 9]
d = 4
```

**Output 1:**

```
-1
```

**Spiegazione:** Se completi un lavoro al giorno, avrai ancora un giorno libero. Non è possibile trovare una pianificazione per i lavori assegnati.

**Input 2:**

```
jobDifficulty = [1, 1, 1]
d = 3
```

**Output 2:**

```
3
```

**Spiegazione:** La pianificazione prevede un lavoro al giorno. La difficoltà totale sarà 3.

**Input 3:**

```
jobDifficulty = [7, 1, 7, 1, 7, 1]
d = 3
```

**Output 3:**

```
15
```

**La Sfida Suprema**

La sequenza di difficoltà per il motore finale è lunga **1000 valori**, e i giorni disponibili sono solo **10**. 

Ogni compito deve essere completato in ordine, rispettando la sequenza e riducendo al minimo il carico giornaliero.

Se fallisci, la *Nova Pioneira* sarà condannata a vagare nello spazio profondo, un monumento silenzioso alla fallibilità umana. Ma se ci riesci… Alpha Centauri sarà finalmente alla portata. Il destino della nave e del sogno umano di colonizzare le stelle è nelle tue mani. 🚀

**Input:**

[sequenza_di_difficoltà.txt](Problema%205/sequenza_di_difficolta.txt)

- Suggerimento 1
    
    Usa la programmazione dinamica (DP). Prova a suddividere l'array in d sotto-array non vuoti. Prova tutte le possibili suddivisioni dell'array.
    

---

- Suggerimento 2
    
    Usa dp[i][j] dove gli stati DP sono i l'indice dell'ultimo taglio e j il numero di tagli rimanenti. La complessità è O(n * *n ** d).