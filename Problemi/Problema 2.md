# Problema 2

Status: In progress

**Evento: L’Allocazione degli Equipaggi**

Con la *Nova Pioneira* finalmente stabilizzata e i motori pronti a spingere la nave verso la colonia di Alpha Centauri, una nuova sfida si presentò all’equipaggio. Il computer centrale, ancora influenzato dalle complessità del linguaggio alieno, assegnò le postazioni operative in maniera casuale, creando il caos nella disposizione dei membri dell’equipaggio.

**“Capitano,”** disse il responsabile delle operazioni, cercando di contenere il panico, **“l’allocazione delle postazioni è completamente sbagliata! Abbiamo tecnici e piloti assegnati alle postazioni sbagliate, e dobbiamo rimediare prima che i motori possano essere attivati.”**

Il capitano si strofinò le tempie. **“Qual è il problema esatto?”**

**“Le postazioni sono già configurate, ma ogni membro dell’equipaggio deve spostarsi verso il posto corretto. Ogni movimento da una posizione all’altra costa tempo e risorse, quindi dobbiamo minimizzare il numero totale di spostamenti.”**

**“E se non lo facciamo in tempo?”** chiese un ufficiale.

**“I motori non si attiveranno,”** rispose l’ingegnere capo. **“La nave rimarrà alla deriva nel sistema di Alpha Centauri, un bersaglio facile per qualsiasi pericolo spaziale.”**

**Il Problema**

L’equipaggio ricevette la seguente lista:

•	posti: La posizione di ciascuna postazione operativa già configurata.

•	membri: La posizione iniziale di ciascun membro dell’equipaggio.

Ogni membro doveva spostarsi verso una postazione, e ogni spostamento (di 1 unità in qualsiasi direzione) rappresentava un costo. Non erano ammessi conflitti: ogni postazione doveva avere un solo membro.

Il compito dell’equipaggio era calcolare il **numero minimo totale di spostamenti** necessari per allineare tutti ai loro posti.

**Esempio di Configurazione**

Immaginiamo che il sistema abbia assegnato:

```
posti = [3, 1, 5]
membri = [2, 7, 4]
```

**Soluzione:**

•	Il primo membro dell’equipaggio si sposta da 2 a 1 (1 mossa).

•	Il secondo membro si sposta da 7 a 5 (2 mosse).

•	Il terzo membro si sposta da 4 a 3 (1 mossa).

Totale mosse: **1 + 2 + 1 = 4**.

**Output:**

```
4
```

**La Sfida Finale**

Con il tempo che scorreva inesorabilmente, l’equipaggio doveva affrontare un’allocazione molto più complessa. Il sistema aveva assegnato **1000 postazioni** a **1000 membri**, tutti sparsi su posizioni casuali lungo la nave.

L’obiettivo era calcolare il numero minimo di spostamenti necessario per garantire che ogni membro fosse nella sua postazione senza errori. Ogni secondo era cruciale, e il destino della missione dipendeva da una soluzione rapida e ottimale.

**“Non possiamo sbagliare,”** disse il capitano. **“Ogni mossa deve essere calcolata con precisione. Se falliamo, la missione potrebbe finire qui.”**

Riuscirai a ottimizzare l’allocazione e salvare la missione? Il futuro dell’esplorazione spaziale è nelle tue mani. 🚀

**Input:**

[posti.txt](Problema%202/posti.txt)

[membri.txt](Problema%202/membri.txt)