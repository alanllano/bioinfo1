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


#LC_MEDIO
acuerdo>=0.5	n=192	LC medio 8.93	LC<=6: 0.01
acuerdo<0.5 	n=51	LC medio 7.92	LC<=6: 0.14

#TRIM
seqkit stats ${F}_mafft.fasta ${F}_mafft_trimal.fasta
processed files:  2 / 2 [======================================] ETA: 0s. done
file                     format  type     num_seqs  sum_len  min_len  avg_len  max_len
rspo_mafft.fasta         FASTA   Protein        17    6,647      391      391      391
rspo_mafft_trimal.fasta  FASTA   Protein        17    3,927      231      231      231


head -3 ${F}_tabla.tsv
1	0.407	9	1
2	0.407	9	1
3	0.352	9	1

#COMPARACION
                   g, n[g], b[g]/n[g], s[g]/n[g]}' \
    ${F}_tabla.tsv | sort
conservada	n=206	acuerdo<0.5: 0.16	LC medio 8.94
recortada 	n=37	acuerdo<0.5: 0.49	LC medio 7.51
