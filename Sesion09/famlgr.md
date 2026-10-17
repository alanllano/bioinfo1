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

#LC_MEDIO
acuerdo<0.5 	n=311	LC medio 6.25	LC<=6: 0.47
acuerdo>=0.5	n=595	LC medio 8.07	LC<=6: 0.20


#Trim

processed files:  2 / 2 [======================================] ETA: 0s. done
file                    format  type     num_seqs  sum_len  min_len  avg_len  max_len
lgr_mafft.fasta         FASTA   Protein        50  145,100    2,902    2,902    2,902
lgr_mafft_trimal.fasta  FASTA   Protein        50   19,050      381      381      381


head -3 ${F}_tabla.tsv
1	0.139	9	0
2	0.111	9	0
3	0.091	9	0


#Comparaciom

    ${F}_tabla.tsv | sort
conservada	n=349	acuerdo<0.5: 0.01	LC medio 8.67
recortada 	n=558	acuerdo<0.5: 0.55	LC medio 6.68
