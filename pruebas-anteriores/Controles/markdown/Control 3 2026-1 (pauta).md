# Pauta Control 3 — Ley de Ampère en una hoja infinita de corriente

> **Curso:** FIS1533-2 (Primer semestre 2026) · **Fecha:** 24 de junio de 2026 · **Evaluación:** Control 3 (Forma 1)

---

## Problema 1

Una hoja infinita de corriente que yace en el plano $y$–$z$ porta una corriente superficial con densidad lineal $J_s$. La corriente es en la dirección $y$, y $J_s$ representa la corriente por unidad de longitud medida a lo largo del eje $z$. La figura muestra una vista del borde de la hoja. Pruebe que el campo magnético cerca de la hoja es paralelo a la hoja y perpendicular a la dirección de la corriente, con una magnitud de $\mu_0 J_s / 2$. *Sugerencia:* Use la ley de Ampère y evalúe la integral de línea para una trayectoria rectangular alrededor de la hoja, representada por la línea discontinua en la figura.

> **[Figura]:** Vista de perfil (corte en el plano $x$–$z$) de la hoja infinita de corriente ubicada en $x = 0$ a lo largo del eje vertical $z$. El eje $z$ apunta hacia arriba y el eje $x$ apunta horizontalmente hacia la izquierda (por regla de la mano derecha $\hat{x}\times\hat{y}=\hat{z}$, el eje $+y$ apunta saliendo de la página hacia el lector). La hoja se representa como una franja vertical delgada con bordes quebrados en sus extremos superior e inferior (indicando extensión infinita) y puntos morados en su interior acompañados de la etiqueta «$J_s$ (alejándose del papel)», indicando corriente en dirección $+\hat{y}$ saliendo del plano. Alrededor de un tramo de la hoja se traza en línea celeste discontinua una trayectoria amperiana rectangular centrada en la hoja, con lados verticales paralelos al eje $z$ (uno a la izquierda y otro a la derecha) y lados horizontales paralelos al eje $x$ que cruzan la hoja simétricamente arriba y abajo.

---

### Solución

**Idea:** Descomponer la hoja infinita en filamentos rectos paralelos al eje $y$ y analizar la simetría de sus campos magnéticos (regla de la mano derecha y principio de superposición) para determinar la dirección y uniformidad de $\vec{B}$. Luego aplicar la ley de Ampère $\oint \vec{B}\cdot d\vec{\ell} = \mu_0 I_{\text{enc}}$ sobre el lazo rectangular simétrico de alto $\ell$.

> **[Figura de la solución]:** Dos esquemas explicativos lado a lado:
> 1. *Esquema izquierdo (superposición por simetría):* Se dibujan dos círculos de líneas de campo magnético $\vec{B}$ centrados en dos elementos de corriente vecinos sobre la hoja vertical (punto morado arriba y punto azul abajo, con corriente saliendo de la página). En ambos círculos $\vec{B}$ gira en sentido antihorario. A la izquierda de la hoja la componente vertical de $\vec{B}$ apunta hacia abajo y a la derecha apunta hacia arriba; entre elementos simétricos, las componentes horizontales (en $\pm\hat{x}$) se cancelan entre sí, mientras que las componentes verticales (en $\pm\hat{z}$) se suman.
> 2. *Esquema derecho (trayectoria amperiana):* La hoja se dibuja como una columna vertical de puntos negros (corriente saliendo del plano). El rectángulo amperiano negro se recorre en **sentido antihorario**, con sus cuatro tramos etiquetados en rojo: `1` (inferior, horizontal hacia la derecha), `2` (derecho, vertical hacia arriba, de longitud $\ell$), `3` (superior, horizontal hacia la izquierda) y `4` (izquierdo, vertical hacia abajo, de longitud $\ell$). Las flechas rojas indican el sentido de $d\vec{\ell}$ y las flechas azules punteadas muestran el campo magnético resultante $\vec{B}$: vertical hacia arriba en el lado derecho y vertical hacia abajo en el lado izquierdo.

#### 1. Dirección y simetría del campo magnético (2.0 pts.)

Como se ilustra en la figura de la solución, podemos considerar la contribución al campo magnético de pequeños elementos de corriente (hilos paralelos al eje $y$ distribuidos a lo largo de $z$). Por simetría, para cualquier punto fuera de la hoja, las componentes horizontales (en la dirección $x$, perpendicular a la hoja) generadas por pares de elementos ubicados simétricamente por encima y por debajo se anularán entre sí, mientras que las componentes verticales (paralelas a la hoja y perpendiculares a la corriente) se intensificarán constructivamente.

Como la hoja es infinita y uniforme, el sistema es invariante bajo traslaciones en $y$ y en $z$, por lo que las líneas de campo resultantes son rectas paralelas a la hoja y perpendiculares a la corriente, y la magnitud $B$ es uniforme a una misma distancia de la hoja (de hecho, independiente de la distancia cerca de la hoja, e igual en ambos lados por simetría especular).

Denotando por $\hat{k}$ al vector unitario vertical a lo largo del eje $z$ de la figura ($\hat{k} \equiv \hat{z}$):
- En la parte **izquierda** ($x > 0$ en los ejes de la figura), el campo magnético apunta hacia abajo, en dirección $-\hat{k}$.
- En la parte **derecha** ($x < 0$ en los ejes de la figura), el campo magnético apunta hacia arriba, en dirección $+\hat{k}$.

$$\text{(2 pts.)}$$

#### 2. Evaluación de la integral de línea con la ley de Ampère (4.0 pts.)

Calculamos la magnitud del campo magnético usando la ley de Ampère siguiendo la trayectoria rectangular sugerida de altura vertical $\ell$ alrededor de la hoja, descompuesta en sus cuatro tramos:
$$\oint \vec{B}\cdot d\vec{\ell} = \sum_{i=1}^{4} \int_{\text{tramo } i} \vec{B}\cdot d\vec{\ell}_i$$

- **Tramos horizontales superior e inferior (tramos `3` y `1`):**  
  El campo magnético $\vec{B}$ (paralelo al eje $z$) es perpendicular al elemento de desplazamiento $d\vec{\ell}$ (paralelo al eje $x$), de modo que $\vec{B}\cdot d\vec{\ell} = 0$ y no contribuyen a la integral.
- **Tramos verticales izquierdo y derecho (tramos `4` y `2`, ambos de largo $\ell$):**  
  Si recorremos la trayectoria en **sentido antihorario**, como muestra la figura de la solución:
  - En el tramo derecho (`2`), $\vec{B}$ apunta hacia arriba ($+\hat{k}$) y $d\vec{\ell}_2$ apunta hacia arriba ($+\hat{k}$), por lo que $\int_2 \vec{B}\cdot d\vec{\ell}_2 = B\ell$.
  - En el tramo izquierdo (`4`), $\vec{B}$ apunta hacia abajo ($-\hat{k}$) y $d\vec{\ell}_4$ apunta hacia abajo ($-\hat{k}$), por lo que $\int_4 \vec{B}\cdot d\vec{\ell}_4 = B\ell$.

En ambos tramos verticales el campo es paralelo al camino y constante sobre ellos, por lo tanto:
$$\sum_i \int \vec{B}\cdot d\vec{\ell}_i = 2B\ell \qquad \text{(2 pts.)}$$

Aplicando la ley de Ampère, la corriente total encerrada por el rectángulo de altura $\ell$ es $I_{\text{enc}} = I = J_s \ell$:
$$2B\ell = \mu_0 I_{\text{enc}} = \mu_0 I \qquad \text{(1 pto.)}$$

Despejando $B$ y recordando que la densidad lineal superficial es $J_s = I/\ell$:
$$B = \frac{1}{2}\mu_0 \frac{I}{\ell} = \frac{1}{2}\mu_0 J_s \qquad \text{(1 pto.)}$$

$$\boxed{B = \frac{\mu_0 J_s}{2}, \qquad \vec{B} = \begin{cases} -\dfrac{\mu_0 J_s}{2}\,\hat{k}, & \text{lado izquierdo de la hoja } (x > 0) \\[6pt] +\dfrac{\mu_0 J_s}{2}\,\hat{k}, & \text{lado derecho de la hoja } (x < 0) \end{cases}}$$

**Verificación:**
- **Nota sobre la notación vectorial:** En el texto de la pauta oficial se usa $\hat{k}$ para indicar el eje vertical ($z$) dibujado en la figura ($\hat{k} \equiv \hat{z}$). Con el eje $x$ apuntando hacia la izquierda, $z$ hacia arriba y $y$ saliendo de la página, se verifica la terna derecha $\hat{x} \times \hat{y} = \hat{z}$ y la regla de la mano derecha para la corriente en $+\hat{y}$.
- **Discontinuidad tangencial de $\vec{B}$:** La discontinuidad de la componente tangencial al cruzar la hoja es $\Delta B_{\parallel} = B_{\text{der}} - B_{\text{izq}} = \frac{\mu_0 J_s}{2} - \left(-\frac{\mu_0 J_s}{2}\right) = \mu_0 J_s$, condición de borde exacta de la magnetostática.
- **Unidades:** $[\mu_0] = \text{T}\cdot\text{m}/\text{A}$ y $[J_s] = \text{A}/\text{m}$, por lo que $[\mu_0 J_s] = \text{T}$, consistente.

---

## Resumen de resultados

| Problema | Magnitud / Dirección | Condición | Resultado |
| :--- | :--- | :--- | :--- |
| **Problema 1** | Magnitud del campo magnético | Cerca de la hoja infinita | $B = \dfrac{\mu_0 J_s}{2}$ |
| | Vector campo magnético ($\hat{k} \equiv \hat{z}$) | Lado izquierdo ($x > 0$) | $\vec{B} = -\dfrac{\mu_0 J_s}{2}\,\hat{k}$ |
| | Vector campo magnético ($\hat{k} \equiv \hat{z}$) | Lado derecho ($x < 0$) | $\vec{B} = +\dfrac{\mu_0 J_s}{2}\,\hat{k}$ |
