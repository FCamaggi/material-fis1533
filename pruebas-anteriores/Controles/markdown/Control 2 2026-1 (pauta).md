# Pauta Control 2 — Circuitos de corriente continua y leyes de Kirchhoff

> **Curso:** FIS1533-2 (Primer semestre 2026) · **Fecha:** 27 de mayo de 2026 · **Evaluación:** Control 2 (Forma 1)

---

## Problema 1

En el circuito de la figura, todas las resistencias tienen la misma magnitud $R_1 = R_2 = R_3 = R_4 = R_5 = 1\,\Omega$, mientras que los voltajes son de magnitud $\mathcal{E}_1 = 10\,\text{V}$ y $\mathcal{E}_2 = 6\,\text{V}$.

a) **(5 pts.)** Calcule la corriente eléctrica que circula por cada resistencia. Exprese sus resultados en Amperes.

b) **(1 pto.)** Determine la diferencia de potencial entre los nodos $d$ y $b$ del circuito.

> **[Figura]:** Circuito plano con cuatro vértices exteriores formando un cuadrilátero —$a$ (superior izquierdo), $b$ (superior derecho, marcado con un punto verde), $c$ (inferior derecho) y $d$ (inferior izquierdo, marcado con un punto verde)— más un nodo central $e$ conectado mediante ramas diagonales a $a$, $b$ y $d$ (sin conexión directa entre $e$ y $c$):
> - **Borde superior ($a$–$b$):** contiene la resistencia $R_2$, con una flecha roja de corriente $I_2$ apuntando hacia la **izquierda** (de $b$ hacia $a$).
> - **Borde izquierdo ($a$–$d$):** contiene la resistencia $R_1$, con una flecha roja de corriente $I_1$ apuntando hacia **abajo** (de $a$ hacia $d$).
> - **Borde inferior ($d$–$c$):** contiene la resistencia $R_5$, con una flecha roja de corriente $I_5$ apuntando hacia la **derecha** (de $d$ hacia $c$).
> - **Borde derecho ($b$–$c$):** contiene la fuente de fem $\mathcal{E}_1$, con su borne positivo (placa larga) hacia **arriba** (conectado a $b$) y su borne negativo (placa corta) hacia **abajo** (conectado a $c$).
> - **Diagonal de $a$ a $e$:** contiene la fuente de fem $\mathcal{E}_2$ (sin resistencia), con su borne positivo (placa larga) hacia **arriba-izquierda** (hacia $a$) y su borne negativo (placa corta) hacia **abajo-derecha** (hacia $e$).
> - **Diagonal de $b$ a $e$:** contiene la resistencia $R_3$, con una flecha roja de corriente $I_3$ apuntando hacia **abajo-izquierda** (de $b$ hacia $e$).
> - **Diagonal de $e$ a $d$:** contiene la resistencia $R_4$, con una flecha roja de corriente $I_4$ apuntando hacia **arriba-derecha** (de $d$ hacia $e$).

---

### Solución

**Idea:** Se tienen $5$ corrientes desconocidas ($I_1, I_2, I_3, I_4, I_5$), asociadas una a cada resistencia $R_j$. Aplicamos las leyes de Kirchhoff: tres ecuaciones independientes de mallas (segunda ley de Kirchhoff) y dos ecuaciones de nodos en los nodos $d$ y $b$ (primera ley de Kirchhoff), para luego resolver el sistema lineal simbólica y numéricamente.

#### Parte a) Corriente en cada resistencia (5.0 pts.)

Definimos las corrientes en cada resistencia $R_j$ como $I_j$ con los sentidos indicados en la figura. Como todas las resistencias son iguales, denotamos $R_j = R = 1\,\Omega$.

Planteamos $3$ ecuaciones de malla para las mallas definidas por los nodos $dcbe$, $eba$ y $badc$:

1. **Malla $d \to c \to b \to e \to d$:**  
   - En $R_5$ ($d \to c$, a favor de $I_5$): $-I_5 R$.  
   - En $\mathcal{E}_1$ ($c \to b$, de $-$ a $+$): $+\mathcal{E}_1$.  
   - En $R_3$ ($b \to e$, a favor de $I_3$): $-I_3 R$.  
   - En $R_4$ ($e \to d$, en contra de $I_4$): $+I_4 R$.  
   $$\mathcal{E}_1 = R(I_3 - I_4 + I_5) \qquad \text{(0.6 pts.)}$$

2. **Malla $e \to b \to a \to e$:**  
   - En $R_3$ ($e \to b$, en contra de $I_3$): $+I_3 R$.  
   - En $R_2$ ($b \to a$, a favor de $I_2$): $-I_2 R$.  
   - En $\mathcal{E}_2$ ($a \to e$, de $+$ a $-$): $-\mathcal{E}_2$.  
   $$\mathcal{E}_2 = R(I_3 - I_2) \qquad \text{(0.6 pts.)}$$

3. **Malla $b \to a \to d \to c \to b$:**  
   - En $R_2$ ($b \to a$, a favor de $I_2$): $-I_2 R$.  
   - En $R_1$ ($a \to d$, a favor de $I_1$): $-I_1 R$.  
   - En $R_5$ ($d \to c$, a favor de $I_5$): $-I_5 R$.  
   - En $\mathcal{E}_1$ ($c \to b$, de $-$ a $+$): $+\mathcal{E}_1$.  
   $$\mathcal{E}_1 = R(I_2 + I_1 + I_5) \qquad \text{(0.6 pts.)}$$

> **Nota:** La solución oficial menciona «lo cual define las siguientes cuatro ecuaciones» por error de redacción, pero en realidad plantea correctamente estas tres ecuaciones de malla junto con dos ecuaciones de nodos para completar el sistema de cinco ecuaciones.

Agregamos dos ecuaciones de nodos para los nodos $d$ y $b$ (en verde en la figura):

- **Nodo $d$:** entra $I_1$ y salen $I_5$ e $I_4$:
  $$I_1 = I_5 + I_4 \qquad \text{(0.6 pts.)}$$
- **Nodo $b$:** entra $I_5$ (desde $c$ a través de $\mathcal{E}_1$) y salen $I_2$ e $I_3$:
  $$I_5 = I_2 + I_3 \qquad \text{(0.6 pts.)}$$

Sustituimos $I_5 = I_2 + I_3$ e $I_1 = I_5 + I_4 = I_2 + I_3 + I_4$ en las tres ecuaciones de malla:
$$\begin{aligned}
\mathcal{E}_1 &= R(2I_3 - I_4 + I_2), \\
\mathcal{E}_2 &= R(I_3 - I_2), \\
\mathcal{E}_1 &= R(3I_2 + 2I_3 + I_4).
\end{aligned}$$

Sumando la primera ecuación con la segunda se elimina $I_2$, y sumando tres veces la segunda con la tercera también se elimina $I_2$:
$$\begin{aligned}
\mathcal{E}_1 + \mathcal{E}_2 &= R(3I_3 - I_4), \\
\mathcal{E}_1 + 3\mathcal{E}_2 &= R(5I_3 + I_4).
\end{aligned}$$

Sumando ambas ecuaciones se elimina $I_4$ y se obtiene $I_3$:
$$2\mathcal{E}_1 + 4\mathcal{E}_2 = 8 R I_3 \implies I_3 = \frac{\mathcal{E}_1 + 2\mathcal{E}_2}{4R} \qquad \text{(0.2 pts.)}$$

Reemplazando en la ecuación $\mathcal{E}_1 + \mathcal{E}_2 = R(3I_3 - I_4)$ para despejar $I_4$:
$$I_4 = 3I_3 - \frac{\mathcal{E}_1 + \mathcal{E}_2}{R} = \frac{3\mathcal{E}_1 + 6\mathcal{E}_2 - 4\mathcal{E}_1 - 4\mathcal{E}_2}{4R} \implies I_4 = \frac{2\mathcal{E}_2 - \mathcal{E}_1}{4R} \qquad \text{(0.2 pts.)}$$

Combinando $I_3$ con la ecuación $\mathcal{E}_2 = R(I_3 - I_2)$ para obtener $I_2$:
$$I_2 = I_3 - \frac{\mathcal{E}_2}{R} = \frac{\mathcal{E}_1 + 2\mathcal{E}_2 - 4\mathcal{E}_2}{4R} \implies I_2 = \frac{\mathcal{E}_1 - 2\mathcal{E}_2}{4R} \qquad \text{(0.2 pts.)}$$

Para $I_5$:
$$I_5 = I_2 + I_3 = \frac{(\mathcal{E}_1 - 2\mathcal{E}_2) + (\mathcal{E}_1 + 2\mathcal{E}_2)}{4R} \implies I_5 = \frac{\mathcal{E}_1}{2R} \qquad \text{(0.2 pts.)}$$

Finalmente, para $I_1$:
$$I_1 = I_5 + I_4 = \frac{2\mathcal{E}_1 + (2\mathcal{E}_2 - \mathcal{E}_1)}{4R} \implies I_1 = \frac{\mathcal{E}_1 + 2\mathcal{E}_2}{4R} \qquad \text{(0.2 pts.)}$$

Reemplazando los valores numéricos $\mathcal{E}_1 = 10\,\text{V}$, $\mathcal{E}_2 = 6\,\text{V}$ y $R = 1\,\Omega$:
$$\boxed{I_1 = 5.5\,[\text{A}]} \qquad \text{(0.2 pts.)}$$
$$\boxed{I_2 = -0.5\,[\text{A}]} \qquad \text{(0.2 pts.)}$$
$$\boxed{I_3 = 5.5\,[\text{A}]} \qquad \text{(0.2 pts.)}$$
$$\boxed{I_4 = 0.5\,[\text{A}]} \qquad \text{(0.2 pts.)}$$
$$\boxed{I_5 = 5\,[\text{A}]} \qquad \text{(0.2 pts.)}$$

*(El signo negativo de $I_2$ indica que la corriente real por $R_2$ circula en sentido contrario al dibujado en la figura, es decir, de $a$ hacia $b$, con magnitud $0.5\,\text{A}$.)*

---

#### Parte b) Diferencia de potencial entre los nodos $d$ y $b$ (1.0 pto.)

Escogemos el camino desde el nodo $d$ hasta el nodo $b$ pasando por el nodo $e$ ($d \to e \to b$). Partiendo de $V_d$, se resta $I_4 R$ al avanzar por $R_4$ en el sentido de $I_4$, y se suma $I_3 R$ al avanzar por $R_3$ en sentido contrario a $I_3$:
$$V_b - V_d = -I_4 R + I_3 R = R(I_3 - I_4)$$

En la notación de la pauta oficial ($\Delta\mathcal{E}_{bd} \equiv V_b - V_d$):
$$\Delta\mathcal{E}_{bd} = R(I_3 - I_4) \qquad \text{(0.8 pts.)}$$

Sustituyendo $R = 1\,\Omega$, $I_3 = 5.5\,\text{A}$ e $I_4 = 0.5\,\text{A}$:
$$\boxed{\Delta\mathcal{E}_{bd} = V_b - V_d = 5\,[\text{V}]} \qquad \text{(0.2 pts.)}$$
*(Equivalentemente, $V_d - V_b = -5\,[\text{V}]$.)*

**Verificación:**
- **Comprobación por camino alternativo ($d \to a \to b$):** Recorriendo $d \to a$ en contra de $I_1$ y $a \to b$ en contra de $I_2$, se obtiene $V_b - V_d = I_1 R + I_2 R = (5.5\,\text{A} - 0.5\,\text{A})(1\,\Omega) = 5\,\text{V}$, idéntico al resultado anterior.
- **Comprobación de nodos y mallas restantes:** En el nodo $a$, la corriente que sube desde $e$ hacia $a$ por la rama de $\mathcal{E}_2$ es $I_{ea} = I_3 + I_4 = 5.5 + 0.5 = 6\,\text{A}$, y entra al nodo $a$ junto con $I_2 = -0.5\,\text{A}$ para dar $I_1 = 6 - 0.5 = 5.5\,\text{A}$ saliendo hacia $d$. En todas las mallas se cumple $\sum \Delta V = 0$: $R(I_3 - I_4 + I_5) = 1(5.5 - 0.5 + 5) = 10\,\text{V} = \mathcal{E}_1$, $R(I_3 - I_2) = 1(5.5 - (-0.5)) = 6\,\text{V} = \mathcal{E}_2$, y $R(I_2 + I_1 + I_5) = 1(-0.5 + 5.5 + 5) = 10\,\text{V} = \mathcal{E}_1$.

---

## Resumen de resultados

| Problema | Parte | Magnitud buscada | Expresión simbólica | Valor numérico |
| :--- | :--- | :--- | :--- | :--- |
| **Problema 1** | a) | Corriente en $R_1$ | $I_1 = \dfrac{\mathcal{E}_1 + 2\mathcal{E}_2}{4R}$ | $I_1 = 5.5\,\text{A}$ |
| | a) | Corriente en $R_2$ | $I_2 = \dfrac{\mathcal{E}_1 - 2\mathcal{E}_2}{4R}$ | $I_2 = -0.5\,\text{A}$ |
| | a) | Corriente en $R_3$ | $I_3 = \dfrac{\mathcal{E}_1 + 2\mathcal{E}_2}{4R}$ | $I_3 = 5.5\,\text{A}$ |
| | a) | Corriente en $R_4$ | $I_4 = \dfrac{2\mathcal{E}_2 - \mathcal{E}_1}{4R}$ | $I_4 = 0.5\,\text{A}$ |
| | a) | Corriente en $R_5$ | $I_5 = \dfrac{\mathcal{E}_1}{2R}$ | $I_5 = 5\,\text{A}$ |
| | b) | Diferencia de potencial entre $d$ y $b$ | $\Delta\mathcal{E}_{bd} = V_b - V_d = R(I_3 - I_4)$ | $\Delta\mathcal{E}_{bd} = 5\,\text{V}$ ($V_d - V_b = -5\,\text{V}$) |
