# Domande di competenza per l’ontologia ArCo4Archives (Archival resource)

## A. Gerarchia archivistica: ArchivalResourceSet, ArchivalUnit, ArchivalItem (e sottoclassi)

1. Quali sono i complessi archivistici disponibili? 
2. Quali fondi archivistici sono stati prodotti da una data persona, organizzazione o famiglia? 
3. Quali unità archivistiche appartengono a un dato complesso archivistico?  
4. Quali unità archivistiche appartengono a una data unità archivistica?  
5. Qual è il complesso archivistico padre di una data unità archivistica?  
6. Quali sono le unità archivistiche figlie di un dato complesso archivistico?  
7. Quali unità documentarie sono manoscritti?
8. Quali unità documentarie sono pergamene?
9. Quali unità documentarie sono fotografie?
10. Quali unità documentarie sono item audiovisivi?
11. Quali unità documentarie sono item cartografici?
12. Quali unità documentarie sono item grafici?
13. Quanti unità documentarie di ciascun tipo (manoscritto, pergamena, fotografia, audiovisivo, cartografico, grafico) contiene una data unità archivistica?
14. Quali risorse archivistiche non hanno un padre (cioè sono fondi di livello superiore)?  
15. Qual è il percorso gerarchico completo (complesso → unità → item) di una data unità documentaria?  
16. Quanti livelli di descrizione separano una data unità documentaria dal complesso di livello superiore a cui appartiene?  
17. Quali insiemi di risorse archivistiche contengono più di un dato numero di unità archivistiche?
18. Una data risorsa archivistica è un `ArchivalResourceSet`, un `ArchivalUnit` o un `ArchivalItem`?
19. Quali unità archivistiche di un dato fondo non hanno ulteriori unità figlie descritte (cioè sono foglie della gerarchia)?  

## B. Agenti: ArchivalCreator, ArchivalHolder, Responsibility, Family

20. Per quali risorse archivistiche il Presidente della Repubblica Italiana Einaudi è il produttore?
21. Chi è il soggetto conservatore di una data risorsa archivistica?
22. Quali risorse archivistiche sono detenute da una data istituzione?
23. Quali risorse archivistiche hanno una data persona o organizzazione come soggetto produttore?
24. Quali risorse archivistiche sono state prodotte da una famiglia (anziché da una singola persona o da un’organizzazione formale)?
25. Qual è la natura della responsabilità (produttore vs. conservatore) che un dato agente ha su una data risorsa archivistica?
26. Quali risorse archivistiche sono state sia prodotte sia sono attualmente conservate dalla stessa organizzazione?
27. Quali agenti (produttori o conservatori) sono associati a un dato complesso archivistico?
28. Quali risorse archivistiche hanno più di un soggetto produttore?
29. Quali persone fisiche hanno agito come soggetti produttori per almeno un fondo archivistico?
30. Quali organizzazioni formali hanno agito come conservatori archivistici per almeno un fondo archivistico?
31. Qual è il tipo (`FormalOrganizationType`) di una data organizzazione formale che agisce come soggetto produttore o conservatore?

## C. Titoli nobiliari, qualifiche e professioni delle persone (Attribute / AttributeInTime)

32. Quale titolo nobiliare, se presente, deteneva una data persona fisica, e in quale periodo?  

33. Quale professione esercitava un dato soggetto produttore, e in quale arco temporale?
34. Quale qualifica deteneva una data persona al momento in cui ha prodotto un dato fondo archivistico?
35. Quali soggetti produttori detenevano il titolo nobiliare di “Barone” (o un altro titolo dato)?
36. Quali persone esercitavano una data professione (ad es. “notaio”, “magistrato”) secondo le descrizioni dell’archivio?
37. La qualifica o professione di una data persona è cambiata nel tempo e, se sì, quando?
38. Quali risorse archivistiche sono state prodotte da una persona mentre deteneva uno specifico titolo nobiliare, qualifica o ruolo professionale?

## D. Soggetti

39. Quali risorse archivistiche hanno sia la figura politica XX sia YY come soggetti? 

40. Quali sono i soggetti associati a una data risorsa archivistica?
41. Quali risorse archivistiche condividono un soggetto comune con una data risorsa archivistica?
42. Quali soggetti ricorrono con maggiore frequenza nell’intera collezione archivistica?
43. Quali risorse archivistiche hanno un dato luogo come soggetto?
44. Quali risorse archivistiche trattano un soggetto appartenente a una data categoria/concetto (ad es. politica, economia, guerra)?

## E. Luogo

45. Quali luoghi sono menzionati in una data unità documentaria?  
46. Dove si trova fisicamente il conservatore/istituzione archivistica (sede)?
47. Quali risorse archivistiche sono correlate a luoghi all’interno di una data area amministrativa o regione?
48. Quali unità documentaria fanno riferimento a un dato nome di luogo?
49. Quali istituzioni hanno la propria sede in una data città?
50. Quali risorse archivistiche riguardano una giurisdizione che include un dato territorio?  

## F. Tempo / Eventi

51. Quali risorse archivistiche sono state prodotte nell’anno XX?  
52. Quali eventi sono associati a una data risorsa archivistica?
53. Qual è il tipo di un dato evento (ad es. acquisizione, intervento, digitalizzazione) collegato a una risorsa archivistica?
54. Quali risorse archivistiche hanno eventi avvenuti entro un dato arco temporale (secolo, intervallo di date)?
55. Qual è il secolo a cui appartiene una data unità documentaria?
56. Quali risorse archivistiche sono state oggetto di un intervento (ad es. restauro) e quando è avvenuto?
57. Quali eventi sono eventi ricorrenti del knowledge graph e con quale frequenza si verificano?
58. Qual è l’ordine temporale tra due eventi relativi alla stessa risorsa archivistica (quale precede/segue l’altro)?

## G. Descrizione, ordinamento, consistenza, livello di descrizione

59. Qual è il livello di descrizione (fondo, serie, unità, item, ecc.) di una data risorsa archivistica?  

60. Quali criteri di ordinamento sono stati applicati a un dato complesso archivistico?
61. Qual è la consistenza (ad es. numero di pagine/unità/ecc.) di una data risorsa archivistica?
62. Quali risorse archivistiche hanno una consistenza superiore a un dato valore?
63. Quali complessi archivistici condividono lo stesso livello di descrizione?
64. Qual è il sistema di numerazione applicato a un dato complesso archivistico?
65. Quali risorse archivistiche di livello “serie” appartengono a un dato fondo?
66. Quali livelli di descrizione sono usati nell’intero grafo della conoscenza e quante risorse sono descritte a ciascun livello?
67. Da quanti metri lineari è costituito il complesso archivistico X?

## H. Identificazione: ArchivalReferenceCode

68. Qual è il codice di riferimento archivistico (segnatura) di una data risorsa archivistica?
69. Quale risorsa archivistica corrisponde a un dato codice di riferimento archivistico?  
70. Quali sono tutti gli identificatori usati per riferirsi al complesso archivistico X?

## I. Accesso, uso e relazioni tra risorse

71. Quali sono le condizioni di accesso di una data risorsa archivistica?  
72. Quali sono le condizioni d’uso di una data risorsa archivistica?
73. Quali risorse archivistiche hanno una relazione copia/originale con una data risorsa archivistica (cioè quale è l’originale e quale la copia)?
74. Quali risorse archivistiche sono documentate/descritte da una data relazione di documentazione (interna o esterna al sistema SIA)?
75. Quali risorse archivistiche sono soggette a restrizioni di accesso pubblico e perché (tipo di condizione di accesso)?

## J. FindingAid

76. Quali risorse archivistiche sono documentate/descritte da un dato strumento di ricerca?  
77. Quali strumenti di ricerca (inventari, elenchi, elenchi di deposito, ecc.) esistono per un dato complesso archivistico?
78. Quali risorse archivistiche non hanno uno strumento di ricerca associato?
79. Quale strumento di ricerca descrive il maggior numero di risorse archivistiche?

## K. InstitutionalProfile e HistoricalOrInstitutionalContext

80. Qual è il profilo istituzionale di un dato soggetto conservatore/produttore (il suo profilo descrittivo generale come istituzione)?  
81. Quando è stata istituita una data istituzione (con un profilo istituzionale) e, se applicabile, quando è stata soppressa?
82. Qual è la classificazione/tipo di un dato profilo istituzionale?
83. Quali funzioni e mandato sono descritti nel profilo istituzionale di un dato ente?  
84. In quale contesto storico o istituzionale ha operato un dato soggetto produttore (ad es. uno Stato o un ramo amministrativo)?
85. Qual è la copertura spaziale di un dato contesto storico o istituzionale?
86. Qual è l’estensione temporale (inizio/fine) di un dato contesto storico o istituzionale?
87. Quali soggetti produttori hanno operato nello stesso contesto storico o istituzionale?
88. Qual è la giurisdizione associata a un dato profilo istituzionale nel tempo?
89. Quali istituzioni hanno cambiato profilo istituzionale nel tempo e quali sono stati i profili successivi?
90. Quali risorse archivistiche sono state prodotte da un’entità che operava in un dato contesto storico-istituzionale (ad es. il Regno d’Italia, uno specifico ministero)?

## L. Specifiche di ArchivalItem

91. Quale tecnica è stata usata per produrre una data unità documentaria di tipo grafica?  
92. Qual è il materiale di una data unità documentaria cartografica?
93. Quale tipo di fotografia è l’unità archivistica X?
94. Quali unità cartografiche descrivono un dato territorio a una data scala?
95. Quali sono l’incipit e l’explicit del manoscritto X?
96. Qual è la durata dell’unità audiovisiva X?

## M. Domande trasversali / aggregate

97. Quali risorse archivistiche soddisfano simultaneamente più criteri (ad es. prodotte da un dato produttore E detenute da una data istituzione E datate a un dato secolo)?  
98. Qual è il profilo completo di una data risorsa archivistica (produttore, conservatore, soggetti, luogo, livello di descrizione, consistenza, codice di riferimento, strumento di ricerca) in un’unica vista?
99. Quali insiemi di risorse archivistiche hanno la descrizione più ricca (più eventi, soggetti e risorse correlate)?
100. Quali coppie di risorse archivistiche sono collegate tramite una relazione di documentazione, copia/originale o gerarchica?
