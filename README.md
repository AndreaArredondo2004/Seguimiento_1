SOLUCIÓN SEGUIMIENTO 1
1. Descripción del archivo.
   El formato GFF3 es muy utilizado en la bioinformática con el fin de representar anotaciones genómicas sobre secuencias de ADN o ARN. Fue desarrollado para escribir
   de manera estructurada y jerárquica los features (características) biológicos de una secuencia, como genes, exones, CDS, mRNA, etc.
   Estos archivos contiene anotaciones genómicas organizadas en líneas tabuladas con 9 campos fijos, los cuales son:
   
   1. SEQID: Es el identificador de la secuencia sobre la que se hace la anotación, puede ser un cromosoma, . Es el nombre de la secuencia.
      Ejemplo: NC_045512.2, JH920573.1 o chr1.
      
   2. SOURCE: Es el origen del feature o anotación, es decir, de donde se generó (programa, base de datos, etc.).
      Ejemplo: RefSeq, Ensembl, NCBI, etc.
      
   3. TYPE: El tipo de Feature o característica anotado. Se usa Sequence Ontology.
      Ejemplo: gene, exon, mRNA, CDS, etc.
      
   4. START: Posición inicial del feature en la secuencia.
      Ejemplo: 11843.
      
   5. END: Posición final del feature.
      Ejemplo: 12091.
      
   6. SCORE: Valor que indica el nivel de confianza de la anotación, puede tener un valor numérico o punto (.).
      Ejemplo: 960 ó .

   7. STRAND: Indica la hebra del ADN en donde está la anotación.
      Ejemplo: + (Hebra positiva en sentido 5'-> 3').

   8. PHASE: Indica el marco de lectura correcto (0, 1 ó 2) para traducir codones, por lo que solo se usa en CDS.
      Ejemplo: 0, 1, 2 ó . si no aplica.

   9. ATTRIBUTES: Información adicional y se escribe clave=valor separados por punto y coma.
       Ejemplo: ID=gene1.

2. Descripción del organismo: BOS MUTUS.
   
   El Yak salvaje del Tíbet, conocido científicamente como Bos Mutus, es un mamífero grande de la familia Bovidae, que habita en las regiones montañosas del Himalaya,
   principalmente se encuentra en Tíbet, Nepal y partes del oeste chino. Tiene un gran tamaño, pelaje largo y denso y cuernos prominentes, lo que les permitío adaptarse
   a ambientes extremos de gran altitud, bajas temperaturas y escacez de oxígeno. Es el mamífero asiático capaz de habitar a maños altitud, viviendo entre los 3.000 y
   5.5000 metros sobre el nivel del mar (Parada, 2020).
   Es el ancestro salvaje del yak doméstico (Bos grunniens), con el cual comparte similitudes genéticas; y desde el punto de vista genómico su estudio es relevante para
   comprender la adaptación a condiciones hóstiles y la evolución del ganado en zonas de gran altura (Parada, 2020).

   Referencia: Parada, R. (2020). Lifeder. https://www.lifeder.com/yak-bos-mutus/

4.  Resolución de preguntas.
   
    1. ¿Cuantos features contiene el archivo?:
       El archivo contiene 1'158.366 de features.
       
    3. ¿Cuantas regiones de la secuencia (cromosomas) contiene el archivo?:
       El archivo en la columna 1 no contiene secuencias que correspondan a cromosomas nombrados CM[0-9]+ ó chr, lo cuál difiere de la literatura que indica que el Bos mutus
       tiene 60 cromosomas (2n=60). Esto no se debe a un error, si no a la forma en la que está representado el genoma del Bos mutus en el archivo .gff3 descargado de
       Ensembl; puesto que, las secuencias de la columna 1 tienen identificadores como JH912421.1, JH912422.1 ó JH912423.1, los cuales indican que las anotaciones están
       referidas a contigs o scaffolds, que son fragmentos del genoma ensambaldo y no cromosomas completos.
       
       Los contigs son conjuntos de segmentos que se superponen parcialmente, de forma que todos juntos dan una representación continua del genoma (NIH, 2025).
       Los scaffolds por su parte son estructuras de ADN un poco más largas que están ensambladas a partir de los contigs y ayudan a representar regiones más amplias del            genoma (Salerno et al, 2025).

       En total en el archivo hay 41.191 contigs o scaffolds (JH[0-9]+\.)

       
       
       
    5. ¿Cuántos genes están listados en el organismo?:
       El archivo contiene 20.847 genes listados del Yak salvaje.
       
    6. ¿Cuál es el top 10 de tipo de features (columna 3 más anotados en el genoma?:
       El top 10 de tipo de features en la columna 3 más anotados en el genoma son:
        3'89.870 exon
        374.084 CDS
        256.746 biological_region
        41.192 region
        34.663 mRNA
        20.847 gene
        18.270 five_prime_UTR
        12.328 three_prime_UTR
        4.339 ncRNA_gene
        1.437 lnc_RNA






   
     




      
   
