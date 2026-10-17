#Versiones 
clustalo --version:
1.2.4

mafft --version
v7.526 (2024/Apr/26)

 muscle --version
Invalid command line option "-version"

MUSCLE v3.8.1551 by Robert C. Edgar

trimal --version

trimAl 1.2rev59

Se copiaron lo datos de :
# $origen guarda la ruta de los datos compartidos
origen=/mnt/data/bioinfo1/jmiranda/sesion09

# copiar datos/ y scripts/ a la carpeta actual
cp -r $origen/{datos,scripts} .



*****************************************************
seq1       seq2          Sim   [ALL]           Tot  
rspo_mafft_fftns2 17         41.8    77.4 [100.0]   [63650]
(prokka-1.14.6) [aaviles@ken sesion09]$ 



tentativo rspo:
columna  pos_RSPO2_human  n_residuos  n_pares  pares_concordantes  acuerdo
5        1                14          91       37                  0.407
6        2                14          91       37                  0.407
7        3                15          105      37                  0.352
8        4                15          105      37                  0.352
# columnas en aln1: 409; con acuerdo < 0.5: 158
# region 1: columnas 4-11 (8 col)
# region 2: columnas 17-20 (4 col)
# region 3: columnas 40-45 (6 col)
# region 4: columnas 55-59 (5 col)


tentativo lgr:
columna  pos_LGR5_human  n_residuos  n_pares  pares_concordantes  acuerdo
1156     1               9           36       5                   0.139
1157     2               10          45       5                   0.111
1158     3               11          55       5                   0.091
1159     4               8           28       4                   0.143
# columnas en aln1: 3205; con acuerdo < 0.5: 1129
# region 1: columnas 500-520 (21 col)
# region 2: columnas 524-539 (16 col)
# region 3: columnas 543-557 (15 col)
# region 4: columnas 601-601 (1 col)

