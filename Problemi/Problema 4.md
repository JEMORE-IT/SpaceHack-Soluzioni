# Problema 4

Status: In progress

**Evento: La Terra Promessa**

Con il motore principale finalmente stabilizzato e la *Nova Pioneira* in rotta verso Alpha Centauri, il capitano ricevette una nuova trasmissione. Questa volta, i dati non erano un enigma alieno, ma una mappa critica del pianeta designato per la colonizzazione: **Nova Terra**. La mappa rappresentava il terreno del pianeta, con informazioni essenziali per pianificare l’atterraggio e la fondazione della colonia.

**“Capitano,”** disse il capo delle comunicazioni, **“questa è una rappresentazione binaria del terreno del pianeta. Gli 1 rappresentano ettari di terreni coltivabili, mentre gli 0 sono foreste o aree non adatte. Sembra che ci abbiano fornito una guida, ma c’è un problema.”**

Il capo ingegnere prese la parola, analizzando i dati con attenzione. **“I terreni coltivabili sono organizzati in gruppi rettangolari, ma non abbiamo informazioni dirette sui confini di ciascun gruppo. Se non identifichiamo i confini precisi, rischiamo di pianificare insediamenti in modo disorganizzato o di danneggiare risorse critiche.”**

Il capitano si strofinò il mento, fissando la griglia sul monitor. **“Dobbiamo sapere esattamente dove si trovano i terreni coltivabili. Questi rettangoli saranno la base per stabilire coltivazioni, alloggi e infrastrutture.”**

**Esempio del Terreno**

![image.png](Problema%204/image.png)

Sul monitor comparve una parte della mappa:

```
terra = [[1,0,0],[0,1,1],[0,1,1]] , mxn = 3x3
```

Ogni rettangolo di 1 rappresentava ettari contigui di terreno coltivabile. Per garantire un piano di insediamento efficace, era necessario identificare le coordinate dei confini superiori sinistri e inferiori destri di ciascun gruppo.

Un **gruppo** di terreno coltivabile con l'angolo in alto a sinistra in `(r1, c1)` e l'angolo in basso a destra in`(r2, c2)`è rappresentato dall'array di 4 elementi `[r1, c1, r2, c2]`.

**Output atteso:**

```
[[0,0,0,0],[1,1,2,2]]
```

- Il primo gruppo ha l'angolo in alto a sinistra in `terra[0][0]` e l'angolo in basso a destra in `terra[0][0]`.
- Il secondo gruppo ha l'angolo in alto a sinistra in `terra[1][1]` e l'angolo in basso a destra in `terra[2][2]`.

<aside>
🚨

**nota:** ritorna la somma di ogni riga della matrice ottenuta → **1 + 1 + 2 + 2 = 6**

</aside>

**Esempio 2:**

![image.png](Problema%204/image%201.png)

```
terra = [[1,1],[1,1]] , mxn = 2x2
```

**Output atteso:**

```
[[0,0,1,1]]
```

- Il primo gruppo ha l'angolo in alto a sinistra in `terra[0][0]` e l'angolo in basso a destra in `terra[1][1]`.

<aside>
🚨

**nota:** ritorna la somma di ogni riga della matrice ottenuta → **1 + 1 = 2**

</aside>

**La Sfida Finale**

L’intera mappa di Nova Terra era enorme, una griglia di **300x300** ettari. Ogni gruppo di terreni coltivabili doveva essere identificato con precisione. Senza queste informazioni, l’equipaggio non avrebbe potuto pianificare un atterraggio sicuro né iniziare la costruzione della colonia.

**“Questa non è solo una mappa,”** disse il capitano. **“È la chiave per il nostro futuro. L’equipaggio della *Nova Pioneira* non può fallire. Troviamo quei confini e prepariamoci a stabilire una nuova casa per l’umanità.”**

Ora, l’equipaggio contava su di te per completare la mappatura e garantire il successo della missione. **Se sbagli, la sopravvivenza della colonia sarà compromessa.** L’umanità guarda alle stelle, ma il tuo lavoro oggi determinerà se potrà toccarle.

**Input:**

[terra.txt](Problema%204/terra.txt)