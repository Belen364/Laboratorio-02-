# **Laboratorio 02 - Alineamiento de secuencias** 
## Parte 1: colectar genes homólogos
##### 1. **¿Qué función cumple el gen SRY?** 
- Codifica una proteína de unión a DNA del grupo HMG de la familia box, el cual determina el sexo del organismo. 
##### 2.	**¿Cuántos genes ortólogos están anotados en esa base de datos?**
- 29

## Parte 2: alineamiento múltiple
##### 3.	**¿Qué es el EMBL-EBI?**
- El EBI es un instituto Europeo de bioinformática sin fines de lucro que pertenece al EMBL, es decir, al laboratorio Europeo de biología. Fue el primer database de nucleótidos que se estableció en Europa.
##### 4.	**¿Cuál es el programa que ellos ofrecen que funciona mejor para secuencias de proteínas?**
- El mejor programa que ofrece es MUSCLE.
##### 5.	**¿Qué otros tipo de herramientas ofrece EMBL-EBI?**
- El EMBL-EBI ofrece herramientas para generar alineaciones, buscar secuencias o homologas de estas, entre otras cosas a partir de DNA, RNA, genes de expresión o proteínas, por otro lado utiliza estructuras o sistemas. Además entrega información sobre la biología química, ontología, literatura y dominios cruzados.
##### 6.	**¿Cuál es el costo de abrir un gap?** [1]
- 1.53
##### 7.	**¿Cuál es el costo de extender un gap?** 
- 0.123

![MAFFT][https://github.com/Belen364/Imagenes/blob/master/MAFFT.docx]
##### 8.	**¿Cuál es la longitud total del alineamiento?** [1]
- 1934 apróx.
##### 9.	**¿Cuál es la especie cuyo gen SRY está más relacionado con el gen SRY de humanos?** [2]
- El más cercano al ser humano fue Piliocolobus tephrosceles que corresponde a un tipo de primate.
##### 10.	**¿Cuál es el más lejano?** [2]
- El más lejano es Miniopterus natalensis o murciélago 
##### 11.	**¿Cuál es la especie cuyo gen SRY es más cercana a la del burro?** [2]
- La especie más cercana al burro o Equus asinus es la especie Equus przewalskii que corresponde a un caballo de przewalskii.

![Phylogenetic Tree][https://github.com/Belen364/Imagenes/blob/master/Phylogenetic%20Tree.docx]
##### 12.	**¿Cómo esperas que sea el alineamiento si el costo de abrir un gap aumenta? ¿Y si disminuye?** [3]
- Al aumentar los costos del gap las secuencias más cortas pierden nucleótidos provocando que los largos estén en el medio de la secuencia y por lo tanto aumentaría el largo de la secuencia consenso. por otro lado si se disminuye el costo de abrir un gap el número de estos gap aumentas provocando mayor espacio, sobre todo en la zona central y por lo tanto aumenta mucho más el largo de la secuencia.
##### 13.	**¿Cómo esperas que sea el alineamiento si el costo de extender un gap aumenta? ¿Y si disminuye?** [3]
- Si el costo de extender un gap aumenta los genes más pequeños pierden muchos nucleótidos por lo tanto se centran los alineamientos en el centro de la secuencia y así esta disminuye su tamaño original, por el contrario, al disminuir el costo de la extensión de los gaps, el largo de los genes cortos aumentan de gaps, aumentando el tamaño total de la secuencia.
##### 14.	**¿Cuál fue el efecto de aumentar el costo de abrir un gap en la longitud total del alineamiento?** [2]
- En este caso, al igual que en el caso de la pregunta 12 al aumentar los costos las secuencias más cortas pierden nucleótidos y los mas largos quedan en la zona central, provocando un aumento de la secuencia consenso.
##### 15.	**Prueba lo mismo, pero esta vez disminuyendo al mínimo el costo de extender un gap. Describe cómo cambia el alineamiento.** [2]
- Al igual que en la pregunta 13 esto provoca que los genes más cortos aumenten su largo y por lo tanto aumenten el largo total de la secuencia.

## Parte 3: Diseño de partidores
##### 16.	**Agrega a tu informe una lista de los "LEFT PRIMER" y "RIGHT PRIMER" que obtuviste usando Primer3.** [3]
1.  LEFT PRIMER        346   20   59.02   50.00    5.01   0.00    0.00 TTACAGGCCATGCACAGAGA
   RIGHT PRIMER       524   20   58.70   50.00    0.00   0.00    0.00 CTTGAGTGTGTGGCTTTCGT
   PRODUCT SIZE: 179, PAIR ANY_TH COMPL: 14.17, PAIR 3'_TH COMPL: 5.45

 2.  LEFT PRIMER        171   20   58.89   55.00    0.00   0.00    0.00 GGATAGAGTGAAGCGACCCA
   RIGHT PRIMER       369   20   59.31   50.00    3.32   0.00    0.00 TTTCTCTCTGTGCATGGCCT
   PRODUCT SIZE: 199, PAIR ANY_TH COMPL: 0.54, PAIR 3'_TH COMPL: 0.00

 3.  LEFT PRIMER        407   20   59.26   50.00    0.00   0.00    0.00 AGATGCTGCCGAAGAATTGC
   RIGHT PRIMER       610   20   58.84   55.00    3.51   0.58    0.00 GCTTTGTCCAGTGGCTGTAG
   PRODUCT SIZE: 204, PAIR ANY_TH COMPL: 0.00, PAIR 3'_TH COMPL: 0.00

 4.  LEFT PRIMER        404   20   58.71   50.00    0.00   0.00    0.00 CGAAGATGCTGCCGAAGAAT
   RIGHT PRIMER       615   20   58.84   55.00    3.51   0.00    0.00 CTACAGCTTTGTCCAGTGGC
   PRODUCT SIZE: 212, PAIR ANY_TH COMPL: 0.00, PAIR 3'_TH COMPL: 0.00
##### 17.	**Indica los partidores forward y reverse que escogiste y explica por qué son la mejor opción para amplificar el gen SRY de humano.** [5] 
- Los genes escogidos son el 8 y 9 ya que de todas las combinaciones posibles esta esla que tiene un mayor porcentaje de GC (57%).
##### 18.	**¿Cuál es el largo del amplicón? ¿Y la temperatura de annealing sugerida?** [3]
- El largo del amplicón es de 207 nucleótidos y la temperatura de annealing sugerida es de 55°C.

![Partidor 8 y 9][https://github.com/Belen364/Imagenes/blob/master/AmplifX.docx]
