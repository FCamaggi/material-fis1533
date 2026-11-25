# Pauta Control 2 — Circuitos de corriente continua y leyes de Kirchhoff

> **Curso:** FIS1533 — Electricidad y Magnetismo (Segundo semestre 2025) · **Fecha:** 28 de octubre de 2025 · **Forma:** 1

---

## Problema 1

En la Figura adjunta, $R_1 = R_2 = 2\,\Omega$, $R_3 = 4\,\Omega$, $R_4 = 3\,\Omega$, $R_5 = 1\,\Omega$ y $R_6 = R_7 = R_8 = 8\,\Omega$. Las baterías son ideales, cuyas fem son $\varepsilon_1 = 16\text{ V}$ y $\varepsilon_2 = 8\text{ V}$.

- **a) (2 pts.)** Determine la resistencia equivalente de las 6 resistencias que se ubican a la izquierda de la batería $\varepsilon_1$, es decir, de las resistencias $R_1$, $R_2$, $R_3$, $R_6$, $R_7$ y $R_8$.
- **b) (2 pts.)** Determine el valor y la dirección de la corriente $i_1$.
- **c) (1 pto.)** ¿Cuál es la potencia que entregan las baterías 1 y 2? ¿La energía está siendo entregada o absorbida por las baterías 1 y 2?
- **d) (1 pto.)** Determine el valor y la dirección de la corriente $i_2$.

> **[Figura]:** Circuito plano de tres mallas rectangulares adyacentes dispuestas horizontalmente:  
> - **Rama vertical extrema izquierda:** contiene a $R_1$ en su mitad superior y a $R_8$ en su mitad inferior, conectados a un nodo intermedio entre ambos. Junto a $R_8$ (a su izquierda) aparece la etiqueta $i_2$. Desde ese nodo intermedio parte un cable hacia la derecha que baja por la resistencia vertical $R_7$ hasta el riel inferior común.  
> - **Riel superior:** desde la esquina superior izquierda avanza hacia la derecha pasando por $R_2$ hasta el nodo superior sobre la rama de $R_6$; luego continúa hacia la derecha pasando por $R_3$ hasta el nodo superior central (sobre $\varepsilon_1$); y desde allí prosigue a la derecha pasando por $R_4$ hasta la esquina superior derecha.  
> - **Rama vertical intermedia izquierda:** contiene a $R_6$ conectada entre el nodo entre $R_2$ y $R_3$ y el riel inferior.  
> - **Rama vertical central:** conecta el riel inferior con el nodo superior central e incluye la batería ideal $\varepsilon_1$ con borne positivo ($+$) arriba y borne negativo ($-$) abajo (acompañada de una flecha roja apuntando hacia arriba), y el tramo superior etiquetado con $i_1$.  
> - **Rama vertical extrema derecha:** contiene a $R_5$, bajando desde la esquina superior derecha hasta la esquina inferior derecha.  
> - **Riel inferior:** conecta sin resistencias los extremos inferiores de $R_8$, $R_7$, $R_6$ y el borne negativo ($-$) de $\varepsilon_1$; en el tramo inferior de la malla derecha, entre el nodo bajo $\varepsilon_1$ y la esquina inferior derecha, se ubica la batería ideal $\varepsilon_2$ con su borne negativo ($-$) a la izquierda y su borne positivo ($+$) a la derecha (acompañada arriba por una flecha roja cuyo extremo circular está a la derecha y apunta hacia la izquierda).

### Solución

**Idea:** Como la batería ideal $\varepsilon_1$ fija directamente la diferencia de potencial entre el nodo superior central y el nodo inferior central, la subred resistiva de la izquierda queda sometida a la tensión conocida $\varepsilon_1$ y puede reducirse mediante asociaciones en serie y paralelo. Asimismo, la malla derecha queda desacoplada respecto a los voltajes nodales porque $\varepsilon_1$ impone su diferencia de potencial entre sus extremos izquierdos, permitiendo hallar directamente la corriente en la rama derecha y luego $i_1$ por la primera ley de Kirchhoff.

---

#### Parte a) Resistencia equivalente de la red izquierda

1. **Paralelo entre $R_7$ y $R_8$:**  
   Las resistencias $R_7$ y $R_8$ comparten ambos nodos (arriba y abajo en el riel inferior), por lo que están en paralelo:
   $$R_{78} = \frac{R_7 R_8}{R_7 + R_8} = \frac{(8\,\Omega)(8\,\Omega)}{8\,\Omega + 8\,\Omega} = 4\,\Omega \qquad \text{(0.5 pts)}$$

2. **Serie de $R_{78}$ con $R_1$ y $R_2$:**  
   Luego, $R_{78}$, $R_1$ y $R_2$ quedan conectadas en serie, de modo que la resistencia equivalente de esa rama es:
   $$R = R_{78} + R_1 + R_2 = 4\,\Omega + 2\,\Omega + 2\,\Omega = 8\,\Omega \qquad \text{(0.5 pts)}$$

3. **Paralelo con $R_6$ y serie con $R_3$:**  
   Finalmente, la rama de resistencia $R$ está en paralelo con $R_6$, y esta combinación queda en serie con $R_3$:
   $$R_{\text{eq}} = \frac{R R_6}{R + R_6} + R_3 = \frac{(8\,\Omega)(8\,\Omega)}{8\,\Omega + 8\,\Omega} + 4\,\Omega = 4\,\Omega + 4\,\Omega = 8\,\Omega \qquad \text{(1.0 pto)}$$

$$\boxed{R_{\text{eq}} = 8\,\Omega}$$

---

#### Parte b) Valor y dirección de la corriente $i_1$

La subred izquierda de resistencia equivalente $R_{\text{eq}} = 8\,\Omega$ está conectada directamente en paralelo con la batería ideal $\varepsilon_1 = 16\text{ V}$, por lo que la corriente $i$ que sale del nodo superior central hacia la izquierda (a través de $R_3$) es:
$$i = \frac{\varepsilon_1}{R_{\text{eq}}} = \frac{16\text{ V}}{8\,\Omega} = 2\text{ A} \qquad \text{(0.25 pts)}$$

> **Nota:** La solución oficial escribe $i = \varepsilon_1 / R = 2\text{ A}$ usando el símbolo $R$ en lugar de $R_{\text{eq}}$; numéricamente ambos coinciden en $8\,\Omega$.

Aplicando la primera ley de Kirchhoff (LCK) en el nodo superior central —suponiendo que $i_1$ entra hacia arriba y que tanto $i$ (hacia la izquierda) como una corriente $i_{\text{der}}$ (hacia la derecha, a través de $R_4$ y $R_5$) salen del nodo— se tiene:
$$i_1 = i + i_{\text{der}} \implies i_{\text{der}} = i_1 - i \qquad \text{(0.25 pts)}$$

> **Nota:** En los incisos b) y c), la solución oficial denota temporalmente como $i_2$ a esta corriente $i_{\text{der}}$ que circula por $R_4$ y $R_5$, mientras que en el enunciado y en el inciso d) el símbolo $i_2$ designa la corriente que pasa por $R_8$. Aquí distinguimos $i_{\text{der}}$ en b) y c) para evitar ambigüedad, manteniendo el método y los valores exactos de la pauta.

Recorriendo la malla derecha en sentido horario mediante la segunda ley de Kirchhoff (LVK):
$$\varepsilon_1 - i_{\text{der}} R_4 - i_{\text{der}} R_5 - \varepsilon_2 = 0 \qquad \text{(0.5 pts)}$$
$$\varepsilon_1 - \varepsilon_2 - (i_1 - i)(R_4 + R_5) = 0$$

Despejando $i_1$:
$$i_1 = \frac{\varepsilon_1 - \varepsilon_2}{R_4 + R_5} + i = \frac{16\text{ V} - 8\text{ V}}{3\,\Omega + 1\,\Omega} + 2\text{ A} = \frac{8\text{ V}}{4\,\Omega} + 2\text{ A} = 4\text{ A} \qquad \text{(0.5 pts)}$$

> **Nota:** La pauta oficial presenta una errata tipográfica en el texto al escribir «Despejando $i$ de la expresión anterior», cuando en realidad despeja $i_1$.

Al obtener un valor positivo, el sentido supuesto para $i_1$ es correcto: $i_1$ circula **hacia arriba** (en dirección al nodo superior central) *(0.5 pts)*.

$$\boxed{i_1 = 4\text{ A}, \text{ hacia arriba (hacia el nodo superior)}}$$

---

#### Parte c) Potencia y flujo de energía en las baterías 1 y 2

Con $i_1 = 4\text{ A}$ saliendo por el borne positivo de $\varepsilon_1$ y $i_{\text{der}} = i_1 - i = 4\text{ A} - 2\text{ A} = 2\text{ A}$ entrando por el borne positivo de $\varepsilon_2$, las potencias asociadas a cada batería son *(0.5 pts: 0.25 pts cada una)*:
$$P_1 = i_1 \varepsilon_1 = (4\text{ A})(16\text{ V}) = 64\text{ W}$$
$$P_2 = i_{\text{der}} \varepsilon_2 = (i_1 - i)\varepsilon_2 = (2\text{ A})(8\text{ V}) = 16\text{ W}$$

Por el sentido de las corrientes respecto a las polaridades de las fuentes *(0.5 pts: 0.25 pts cada dirección)*:
- La **batería 1 entrega** $64\text{ W}$ de potencia al circuito (la corriente $i_1$ sale por su terminal positivo).
- La **batería 2 absorbe** $16\text{ W}$ de potencia (la corriente $i_{\text{der}} = 2\text{ A}$ entra por su terminal positivo).

$$\boxed{P_1 = 64\text{ W}\ (\text{entrega energía}), \qquad P_2 = 16\text{ W}\ (\text{absorbe energía})}$$

---

#### Parte d) Valor y dirección de la corriente $i_2$

Para hallar la corriente $i_2$ que pasa por $R_8$, aplicamos la primera ley de Kirchhoff en los dos nodos de la red izquierda:
$$i = i_A + i_6 \qquad \text{(0.2 pts)}$$
$$i_A = i_2 + i_7$$
donde $i_A$ es la corriente que circula hacia la izquierda por $R_2$ y luego baja por $R_1$, $i_6$ desciende por $R_6$, $i_7$ desciende por $R_7$, e $i_2$ desciende por $R_8$ (saliendo hacia abajo del nodo entre $R_1$ y $R_8$).

Aplicando la segunda ley de Kirchhoff en la malla formada por $\varepsilon_1$, $R_3$ y $R_6$:
$$\varepsilon_1 - i R_3 - i_6 R_6 = 0 \qquad \text{(0.2 pts)}$$
$$i_6 = \frac{\varepsilon_1 - i R_3}{R_6} = \frac{16\text{ V} - (2\text{ A})(4\,\Omega)}{8\,\Omega} = \frac{8\text{ V}}{8\,\Omega} = 1\text{ A}$$

Entonces, la corriente $i_A$ que sigue hacia la izquierda vale *(0.2 pts)*:
$$i_A = i - i_6 = 2\text{ A} - 1\text{ A} = 1\text{ A}$$

Como $R_8$ y $R_7$ están conectadas en paralelo, comparten la misma diferencia de potencial:
$$i_2 R_8 = i_7 R_7 = (i_A - i_2)R_7 \qquad \text{(0.2 pts)}$$

Despejando $i_2$:
$$i_2 = (i_A - i_2)\frac{R_7}{R_8} \qquad \text{(0.1 pts)}$$
$$i_2 \left(1 + \frac{R_7}{R_8}\right) = i_A \frac{R_7}{R_8} \implies i_2 = i_A \frac{R_7}{R_7 + R_8} = (1\text{ A})\frac{8\,\Omega}{8\,\Omega + 8\,\Omega} = \frac{i_A}{2} = 0{,}5\text{ A}$$

Como el resultado es positivo, el sentido supuesto en que $i_2$ «salía» hacia abajo del nodo superior de $R_8$ es correcto; por tanto, $i_2$ se dirige **hacia abajo** por $R_8$ *(0.1 pts)*.

$$\boxed{i_2 = 0{,}5\text{ A}, \text{ hacia abajo (por } R_8\text{)}}$$

**Verificación (balance global de potencias):**
- Potencia total entregada por las fuentes: $P_{\text{fuentes}} = P_1 - P_2 = 64\text{ W} - 16\text{ W} = 48\text{ W}$.
- Potencia disipada en las resistencias:
  - Rama izquierda: $P_{\text{izq}} = i^2 R_{\text{eq}} = (2\text{ A})^2 (8\,\Omega) = 32\text{ W}$. Verificando componente a componente: $i^2 R_3 + i_6^2 R_6 + i_A^2 (R_2 + R_1) + i_7^2 R_7 + i_2^2 R_8 = (4)(4) + (1)(8) + (1)(4) + (0{,}25)(8) + (0{,}25)(8) = 16 + 8 + 4 + 2 + 2 = 32\text{ W}$.
  - Rama derecha: $P_{\text{der}} = i_{\text{der}}^2 (R_4 + R_5) = (2\text{ A})^2 (3\,\Omega + 1\,\Omega) = 16\text{ W}$.
- Suma disipada: $32\text{ W} + 16\text{ W} = 48\text{ W}$, en perfecto acuerdo con la potencia neta entregada por las baterías.

---

## Resumen de resultados

| Problema | Parte | Cantidad | Resultado |
| :--- | :--- | :--- | :--- |
| **Problema 1** | a) | Resistencia equivalente red izquierda | $R_{\text{eq}} = 8\,\Omega$ |
| | b) | Corriente $i_1$ | $i_1 = 4\text{ A}$, hacia arriba |
| | c) | Potencia batería 1 | $P_1 = 64\text{ W}$ (entrega energía) |
| | c) | Potencia batería 2 | $P_2 = 16\text{ W}$ (absorbe energía) |
| | d) | Corriente $i_2$ (por $R_8$) | $i_2 = 0{,}5\text{ A}$, hacia abajo |
