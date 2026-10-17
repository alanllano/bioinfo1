## Análisis de Desacuerdo entre Métodos (Clustal Omega vs. MAFFT L-INS-i), MUSCLE5 y trimAl

### Familia 1: RSPO2 (RSPO2_human)

#### 1. Péptido señal (Posiciones 1–21)
* **Desacuerdo (Clustal vs. MAFFT):** El acuerdo medio es bajo (0.49) y el 52% de sus posiciones tienen un acuerdo menor a 0.5 (concentrándose en el arranque, posiciones 1–7).
* **Por qué:** Es una región hidrofóbica y sin homología real ni conservación estricta entre especies; cualquier péptido señal se alinea de manera distinta sin una presión de selección posicional rigurosa.
* **Coincidencia con MUSCLE5 y trimAl:** Coincide con las letras de baja confianza en el ensemble de MUSCLE5 (valores de LC entre 2 y 6) y trimAl elimina 10 de estas posiciones (junto con el enlace N) porque presentan alta divergencia y gaps. *(Nota: Los dominios centrales de cisteínas FU1+FU2 y TSP1 tienen un acuerdo perfecto de 0.99, LC de 9, y trimAl los conserva intactos).*

#### 2. Cola C-terminal (Posiciones 204–243)
* **Desacuerdo (Clustal vs. MAFFT):** Presenta un acuerdo medio de 0.35 y un 82% de sus posiciones con desacuerdo (< 0.5).
* **Por qué:** Es una cola de baja complejidad, con composición sesgada y longitud variable entre taxones, lo que impide un anclaje unívoco entre algoritmos.
* **Coincidencia con MUSCLE5 y trimAl:** Muestra valores bajos de confianza en MUSCLE5 (LC medio de 7.9 y letras con LC de 2 a 6) y trimAl recorta 17 de estas posiciones, eliminando el ruido terminal.

---

### Familia 2: LGR5 (LGR5_human)

#### 1. Dominio LRR - Ectodominio (Posiciones 1–454)
* **Desacuerdo (Clustal vs. MAFFT):** Tiene un acuerdo medio moderado de 0.61, con un 45% de posiciones bajo 0.5.
* **Por qué:** Se trata de 14 repeticiones en tándem con un consenso idéntico (LxxLxLxxNxL). Desplazar una secuencia una repetición completa genera un alineamiento alternativo con un puntaje casi idéntico: es un problema de registro, no de falta de conservación individual, haciendo que diferentes programas elijan registros distintos.
* **Coincidencia con MUSCLE5 y trimAl:** Coincide con las caídas de confianza de MUSCLE5 (LC medio de 7.24) y trimAl elimina masivamente 357 de estas 454 posiciones, recortando las columnas ambiguas debidas al corrimiento de registros.

#### 2. Bisagra (Posiciones 455–573) y Cola C-terminal (Posiciones 821–907)
* **Desacuerdo (Clustal vs. MAFFT):** La bisagra tiene un acuerdo medio de 0.78 (25% de posiciones < 0.5), y la cola C-terminal colapsa a un acuerdo medio de 0.40 (74% de posiciones < 0.5).
* **Por qué:** En la bisagra, los bucles flexibles toleran inserciones y deleciones; en la cola, la longitud variable y la baja complejidad impiden una correspondencia confiable.
* **Coincidencia con MUSCLE5 y trimAl:** Coinciden con los valores más bajos de confianza de letra en MUSCLE5 (la cola cae a un LC medio de 4.76) y trimAl recorta 87 posiciones de la bisagra y casi la cola entera (82 de 87 posiciones), dejando prácticamente intacto únicamente el bloque transmembrana 7TM (donde el acuerdo sube a 0.96 y el LC a 9.01).
