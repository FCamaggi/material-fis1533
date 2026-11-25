# Ayudantía 20 — Ley de Ampère

> Clases relacionadas: [Clase 11 - Ley de Biot Savart](../../Clases/markdown/Clase%2011%20-%20Ley%20de%20Biot%20Savart.md), [Clase 12 - Ley de Ampere](../../Clases/markdown/Clase%2012%20-%20Ley%20de%20Ampere.md)

---

## Problema 1

Un cable coaxial muy largo consiste en un cilindro sólido de radio $a$, rodeado por un cascarón cilíndrico conductor concéntrico de radio interno $b$ y exterior $c$. El conductor interior tiene una densidad de corriente no uniforme $\vec{J}_1 = \alpha r\,\hat{z}$ donde $\alpha$ es una constante. El cilindro exterior tiene una densidad de corriente $\vec{J}_2 = -\beta\,\hat{z}$ donde $\beta$ es una constante positiva. Los conductores llevan una igual y opuesta corriente de magnitud $I_0$. Entre ambos conductores existe vacío.

a) Encuentre los valores $\alpha$ y $\beta$ en términos de $a$, $b$, $c$ e $I_0$.  
b) Determine el campo magnético en todo el espacio. Exprese sus resultados en términos de $a$, $b$, $c$ e $I_0$.

> **[Figura]:** Sección transversal de un cable coaxial concéntrico en el plano perpendicular al eje $z$. En el centro, un cilindro macizo de radio interior $a$ con densidad de corriente $\vec{J}_1$ saliendo perpendicularmente del plano ($\odot$, $+\hat{z}$). Entre el radio $a$ y el radio $b$ se tiene una región hueca (vacío). Entre el radio interno $b$ y el radio externo $c$ se ubica un cascarón cilíndrico conductor concéntrico que transporta corriente con densidad $\vec{J}_2$ entrando perpendicularmente al plano ($\otimes$, $-\hat{z}$). Fuera del cascarón ($r > c$) la región corresponde a vacío.

### Solución

**Idea:** La corriente total transportada por cada conductor corresponde al flujo de su densidad de corriente a través de la sección transversal perpendicular al eje $z$, $I = \int \vec{J} \cdot d\vec{A}$. La simetría cilíndrica (invariancia bajo traslaciones axiales en $z$ y rotaciones azimutales en $\theta$) permite determinar el campo magnético mediante la ley de Ampère en forma integral, $\oint \vec{B} \cdot d\vec{\ell} = \mu_0 I_{\text{enc}}$, utilizando espiras amperianas circulares concéntricas centradas sobre el eje del cable.

---

#### Parte a) Constantes $\alpha$ y $\beta$

La corriente $I$ que atraviesa una sección transversal $S$ está dada por:
$$I = \int_S \vec{J} \cdot d\vec{A}$$

1. **Conductor interior ($0 \le r \le a$):**  
   Tomamos elementos de área en forma de anillos concéntricos de radio $r$ y espesor diferencial $dr$, con vector de área $d\vec{A} = 2\pi r\,dr\,\hat{z}$:
   $$I_0 = \int_0^a (\alpha r\,\hat{z}) \cdot (2\pi r\,dr\,\hat{z}) = 2\pi\alpha \int_0^a r^2\,dr = 2\pi\alpha \left[ \frac{r^3}{3} \right]_0^a = \frac{2\pi\alpha a^3}{3}$$

   Despejando $\alpha$:
   $$\boxed{\alpha = \frac{3I_0}{2\pi a^3}}$$

2. **Cascarón exterior ($b \le r \le c$):**  
   La densidad de corriente es uniforme en magnitud $\beta$ y apunta en $-\hat{z}$. El área de la sección transversal de la corona circular es $A_{\text{ext}} = \pi(c^2 - b^2)$. La magnitud de la corriente total es $I_0$:
   $$I_0 = \int_{S_{\text{ext}}} |\vec{J}_2|\,dA = \beta \pi (c^2 - b^2)$$

   Despejando $\beta$:
   $$\boxed{\beta = \frac{I_0}{\pi (c^2 - b^2)}}$$

---

#### Parte b) Campo magnético en todo el espacio

Por simetría, el campo magnético depende exclusivamente de la coordenada radial $r$. Como la corriente fluye en dirección axial ($\pm\hat{z}$), la regla de la mano derecha establece que las líneas de inducción magnética forman circunferencias azimutales centradas en el eje:
$$\vec{B}(r) = B(r)\,\hat{\theta}$$

Tomamos una circunferencia amperiana de radio $r$ centrada en el eje coaxial recorrida en sentido antihorario ($d\vec{\ell} = r\,d\theta\,\hat{\theta}$):
$$\oint \vec{B} \cdot d\vec{\ell} = B(r) \int_0^{2\pi} r\,d\theta = B(r) \cdot 2\pi r = \mu_0 I_{\text{enc}} \implies B(r) = \frac{\mu_0 I_{\text{enc}}}{2\pi r}$$

Calculamos la corriente neta encerrada $I_{\text{enc}}$ en cada una de las cuatro regiones del espacio:

1. **Región I: $0 \le r < a$ (interior del cilindro macizo)**  
   La espira de radio $r$ encierra únicamente una fracción del cilindro central:
   $$I_{\text{enc}}(r) = \int_0^r \alpha r' \cdot 2\pi r'\,dr' = \frac{2\pi\alpha r^3}{3} = \frac{2\pi r^3}{3} \left( \frac{3I_0}{2\pi a^3} \right) = I_0 \frac{r^3}{a^3}$$

   Por tanto:
   $$B(r) = \frac{\mu_0 I_0 r^3 / a^3}{2\pi r} = \frac{\mu_0 I_0 r^2}{2\pi a^3}$$
   $$\boxed{\vec{B}(r) = \frac{\mu_0 I_0 r^2}{2\pi a^3}\,\hat{\theta}}$$

2. **Región II: $a \le r < b$ (vacío entre conductores)**  
   La espira encierra la totalidad de la corriente transportada por el conductor interior:
   $$I_{\text{enc}} = I_0$$

   Por tanto:
   $$\boxed{\vec{B}(r) = \frac{\mu_0 I_0}{2\pi r}\,\hat{\theta}}$$

3. **Región III: $b \le r < c$ (interior del cascarón exterior)**  
   La espira encierra toda la corriente $I_0$ del conductor interior en $+\hat{z}$, más la fracción de corriente del cascarón contenida entre los radios $b$ y $r$ en dirección $-\hat{z}$:
   $$I_{\text{enc}}(r) = I_0 - \beta \pi (r^2 - b^2) = I_0 - \left( \frac{I_0}{\pi (c^2 - b^2)} \right) \pi (r^2 - b^2) = I_0 \left( 1 - \frac{r^2 - b^2}{c^2 - b^2} \right) = I_0 \left( \frac{c^2 - r^2}{c^2 - b^2} \right)$$

   Por tanto:
   $$\boxed{\vec{B}(r) = \frac{\mu_0 I_0 (c^2 - r^2)}{2\pi r (c^2 - b^2)}\,\hat{\theta}}$$

4. **Región IV: $r \ge c$ (exterior del cable coaxial)**  
   La espira amperiana encierra ambas corrientes en su totalidad, las cuales tienen igual magnitud y sentido opuesto:
   $$I_{\text{enc}} = I_0 - I_0 = 0$$

   Por tanto:
   $$\boxed{\vec{B}(r) = \vec{0}}$$

En resumen:
$$\vec{B}(r) = \begin{cases}
\dfrac{\mu_0 I_0 r^2}{2\pi a^3}\,\hat{\theta}, & 0 \le r < a \\[1.5ex]
\dfrac{\mu_0 I_0}{2\pi r}\,\hat{\theta}, & a \le r < b \\[1.5ex]
\dfrac{\mu_0 I_0 (c^2 - r^2)}{2\pi r (c^2 - b^2)}\,\hat{\theta}, & b \le r < c \\[1.5ex]
\vec{0}, & r \ge c
\end{cases}$$

**Verificación:**
- **Continuidad:**
  - En la interfaz $r \to a^-$: $B(a) = \frac{\mu_0 I_0 a^2}{2\pi a^3} = \frac{\mu_0 I_0}{2\pi a}$, que coincide con el valor evaluado desde la región II ($r \to a^+$).
  - En la interfaz $r \to b^-$: $B(b) = \frac{\mu_0 I_0}{2\pi b}$, que coincide con el valor evaluado desde la región III ($r \to b^+$), donde $\frac{c^2 - b^2}{c^2 - b^2} = 1$.
  - En la superficie exterior $r \to c^-$: el factor $(c^2 - c^2) = 0$, asegurando que $B(c) = 0$, continuo con el campo nulo de la región IV.
- **Unidades:** $[\alpha] = \text{A}/\text{m}^3$, $[\beta] = \text{A}/\text{m}^2$; en todas las regiones $[\vec{B}] = [\mu_0 I_0 / r] = \text{T}$, dimensionalmente correcto.

---

## Problema 2

Se tiene dos corrientes, ambas con igual sentido en dirección $z$ (en el dibujo, saliendo de la hoja). Una de ellas es una densidad corriente en una lámina plana e infinita de grosor $b$ y densidad de corriente uniforme $\vec{j}_s = j_s\,\vec{e}_z$, y la otra es una densidad de corriente no uniforme, $\vec{j}_c = j_0 (1 - r/R)\,\vec{e}_z$, en un cilindro infinitamente largo con radio $R$ donde $r$ es la distancia al eje del cilindro.  
Encuentre el valor de $j_0$ en función de $j_s$, que hace que el campo magnético resultante en el punto $P$, ubicado a distancia $R/2$ del centro del cilindro, sea nulo.

> **[Figura]:** Corte transversal en el plano perpendicular al eje $z$. En la parte inferior se ubica una lámina horizontal plana e infinita de grosor vertical $b$, transportando una densidad de corriente uniforme $\vec{j}_s$ saliendo de la hoja ($\odot$, $+\hat{z}$). Sobre la lámina, centrado a cierta distancia, se ubica un cilindro macizo infinito de radio $R$ que transporta una corriente $\vec{j}_c$ con densidad variable también saliendo de la hoja ($\odot$, $+\hat{z}$). Una línea vertical perpendicular a la lámina une el centro del cilindro con la superficie superior de la lámina; a lo largo de este segmento, a una distancia $R/2$ directamente debajo del centro del cilindro (dentro del cilindro), se ubica el punto de observación $P$.

### Solución

**Idea:** Aplicar el principio de superposición: el campo magnético total en el punto $P$ es la suma vectorial de las contribuciones del cilindro y de la lámina, $\vec{B}_{\text{total}}(P) = \vec{B}_c(P) + \vec{B}_s(P)$. Determinamos individualmente cada campo mediante la ley de Ampère aprovechando las simetrías geométrica cilíndrica y planar, e imponemos la condición $\vec{B}_{\text{total}}(P) = \vec{0}$.

#### 1. Sistema de coordenadas

Definimos un sistema cartesiano centrado en el eje del cilindro:
- Eje $X$: horizontal hacia la derecha ($\hat{x}$).
- Eje $Y$: vertical hacia arriba ($\hat{y}$), de modo que la lámina se ubica en el semiespacio $y < -R$.
- Eje $Z$: perpendicular a la página hacia afuera ($\hat{z} = \vec{e}_z$).

En este sistema, el punto $P$ está ubicado sobre el eje vertical por debajo del centro del cilindro a una distancia $R/2$, es decir:
$$\vec{r}_P = \left(0,\, -\frac{R}{2},\, 0\right)$$

---

#### 2. Campo magnético del cilindro en $P$

Por simetría cilíndrica, el campo magnético $\vec{B}_c$ circula en dirección azimutal $\hat{\theta}$. Usamos una curva amperiana circular de radio $r < R$:
$$\oint \vec{B}_c \cdot d\vec{\ell} = B_c(r) \cdot 2\pi r = \mu_0 I_{\text{enc}}(r)$$

La corriente encerrada en un círculo de radio $r$ se calcula integrando la densidad de corriente:
$$I_{\text{enc}}(r) = \int_0^{2\pi} d\theta \int_0^r j_0 \left(1 - \frac{r'}{R}\right) r'\,dr' = 2\pi j_0 \left[ \frac{{r'}^2}{2} - \frac{{r'}^3}{3R} \right]_0^r = 2\pi j_0 \left( \frac{r^2}{2} - \frac{r^3}{3R} \right)$$

Evaluando en la posición del punto $P$, con $r = R/2$:
$$\frac{r^2}{2} - \frac{r^3}{3R} = \frac{(R/2)^2}{2} - \frac{(R/2)^3}{3R} = \frac{R^2}{8} - \frac{R^2}{24} = \frac{3R^2 - R^2}{24} = \frac{R^2}{12}$$

Por lo tanto:
$$I_{\text{enc}}\left(\frac{R}{2}\right) = 2\pi j_0 \left(\frac{R^2}{12}\right) = \frac{\pi j_0 R^2}{6}$$

La magnitud del campo magnético del cilindro en $r = R/2$ es:
$$B_c\left(\frac{R}{2}\right) = \frac{\mu_0 I_{\text{enc}}}{2\pi (R/2)} = \frac{\mu_0}{\pi R} \left( \frac{\pi j_0 R^2}{6} \right) = \frac{\mu_0 j_0 R}{6}$$

Para la dirección: en coordenadas polares, el punto $P = (0, -R/2)$ corresponde a $\theta = -\frac{\pi}{2}$ (o $270^\circ$). Como $\hat{\theta} = -\sin\theta\,\hat{x} + \cos\theta\,\hat{y}$:
$$\hat{\theta}\Big|_{\theta = -\pi/2} = -\sin\left(-\frac{\pi}{2}\right)\hat{x} + \cos\left(-\frac{\pi}{2}\right)\hat{y} = -(-1)\hat{x} + 0\,\hat{y} = +\hat{x}$$

En consecuencia:
$$\vec{B}_c(P) = \frac{\mu_0 j_0 R}{6}\,\hat{x}$$

---

#### 3. Campo magnético de la lámina en $P$

La lámina plana es infinita en $x$ y $z$, de grosor $b$ en $y$, y transporta corriente uniforme en $+\hat{z}$.  
Por simetría planar y regla de la mano derecha, el campo magnético $\vec{B}_s$ es paralelo a la superficie de la lámina ($\pm\hat{x}$), con sentidos opuestos a cada lado del plano medio.

Consideramos una curva amperiana rectangular de longitud $L$ en la dirección $X$ simétrica respecto al plano central de la lámina, cuyos lados horizontales están situados a una distancia $h > b/2$ fuera de la lámina:
$$\oint \vec{B}_s \cdot d\vec{\ell} = 2 B_s L = \mu_0 I_{\text{enc}} = \mu_0 (j_s \cdot b L)$$
$$B_s = \frac{\mu_0 j_s b}{2}$$

Este valor es constante en todo el espacio exterior a la lámina (independiente de la distancia vertical a la misma).  
Como la corriente sale de la hoja ($+\hat{z}$), en cualquier punto situado por encima de la lámina (incluyendo el punto $P$), el campo magnético apunta hacia la izquierda:
$$\vec{B}_s(P) = -\frac{\mu_0 j_s b}{2}\,\hat{x}$$

---

#### 4. Condición de anulación en el punto $P$

Imponiendo la anulación del campo magnético total:
$$\vec{B}_{\text{total}}(P) = \vec{B}_c(P) + \vec{B}_s(P) = \left( \frac{\mu_0 j_0 R}{6} - \frac{\mu_0 j_s b}{2} \right)\hat{x} = \vec{0}$$

$$\frac{\mu_0 j_0 R}{6} = \frac{\mu_0 j_s b}{2}$$
$$\frac{j_0 R}{3} = j_s b$$
$$\boxed{j_0 = \frac{3b}{R} j_s}$$

**Verificación:**
- **Signo y consistencia:** Como las distancias geométricas satisfacen $b > 0$ y $R > 0$, si $j_s > 0$ se obtiene $j_0 > 0$, lo que corrobora que ambas densidades de corriente apuntan en la misma dirección ($+\hat{z}$), en perfecto acuerdo con el enunciado.
- **Unidades:** $[j_0] = \left[\frac{\text{m}}{\text{m}}\right] [j_s] = \text{A}/\text{m}^2$, dimensionalmente homogéneo.

---

## Problema 3

Un conductor cilíndrico infinito de radio $R$ con su eje de simetría coincidente con la dirección $\hat{z}$, conduce una densidad de corriente no uniforme $\vec{J} = k r^2\,\hat{z}$, donde $k$ es una constante desconocida y $r$ es la distancia radial al eje de simetría del cilindro. Además una espira rectangular de lados $b$ y $c$ con corriente constante $I_2$ es colocada paralela al cilindro a una distancia $a$, como lo muestra la figura.  
Considere que la dirección $\hat{x}$ es perpendicular a la hoja, de esta manera, la espira rectangular está sobre el plano $y$-$z$. Si el cilindro conduce una corriente total $I_1$:

a) Determine la constante $k$ en función de $I_1$, $R$ y $\mu_0$.  
b) Encuentre el campo magnético originado por el cilindro para cualquier valor de $r$. Puede dejar su resultado en función de $k$.  
c) Calcule la fuerza total y el torque magnético que el cilindro ejerce sobre la espira. Puede dejar su resultado en función de $k$.

> **[Figura]:** Cilindro vertical infinito alineado con el eje $Z$, de radio $R$, con densidad de corriente $\vec{J}$ hacia arriba ($+\hat{z}$). El eje $X$ apunta saliendo perpendicularmente de la hoja ($\odot\,\hat{x}$). En el plano $YZ$ (el plano del papel), a la derecha del cilindro, se ubica una espira rectangular coplanar con dimensiones $b$ (ancho horizontal en $y$) y $c$ (alto vertical en $z$). El lado vertical más cercano está a distancia horizontal $y = a$ del eje $Z$, extendiéndose el lado opuesto hasta $y = a + b$. La espira transporta una corriente constante $I_2$ que circula en sentido horario: sube por el tramo vertical izquierdo ($y = a$), avanza hacia la derecha por el tramo horizontal superior ($z = c$), desciende por el tramo vertical derecho ($y = a + b$), y regresa hacia la izquierda por el tramo inferior ($z = 0$).

### Solución

**Idea:** La corriente total en el cilindro fija el valor de $k$ mediante integración directa en la sección transversal. El campo magnético $\vec{B}$ del cilindro se determina con la ley de Ampère. Conociendo el campo en el plano $YZ$, se aplica la fuerza magnética de Lorentz sobre corrientes filiformes $\vec{F} = I_2 \int d\vec{\ell} \times \vec{B}$ sobre cada uno de los cuatro lados de la espira. El torque se deduce analizando las fuerzas o el momento magnético dipolar de la espira $\vec{\tau} = \vec{m} \times \vec{B}$.

---

#### Parte a) Determinación de la constante $k$

La corriente total $I_1$ es el flujo de la densidad de corriente a través de la sección circular del cilindro:
$$I_1 = \int_S \vec{J} \cdot d\vec{A} = \int_0^{2\pi} d\theta \int_0^R (k r^2\,\hat{z}) \cdot (r\,dr\,d\theta\,\hat{z}) = 2\pi k \int_0^R r^3\,dr = 2\pi k \left[ \frac{R^4}{4} \right] = \frac{\pi k R^4}{2}$$

Despejando $k$:
$$\boxed{k = \frac{2I_1}{\pi R^4}}$$

*(Nota: el enunciado menciona expresar $k$ en función de $I_1, R$ y $\mu_0$; la constante de permeabilidad $\mu_0$ no interviene en la relación dimensional de $k$, por lo que su dependencia es trivial: $\mu_0^0$).*

---

#### Parte b) Campo magnético para cualquier valor de $r$

Por simetría cilíndrica, el campo magnético es puramente azimutal: $\vec{B}(r) = B(r)\,\hat{\theta}$.  
Aplicando la ley de Ampère en una circunferencia de radio $r$:
$$\oint \vec{B} \cdot d\vec{\ell} = B(r) \cdot 2\pi r = \mu_0 I_{\text{enc}}(r)$$

1. **Región interior ($r < R$):**
   $$I_{\text{enc}}(r) = \int_0^{2\pi} d\theta \int_0^r k {r'}^2 \cdot r'\,dr' = 2\pi k \int_0^r {r'}^3\,dr' = \frac{\pi k r^4}{2}$$
   $$B(r) \cdot 2\pi r = \mu_0 \left( \frac{\pi k r^4}{2} \right) \implies B(r) = \frac{\mu_0 k r^3}{4}$$

   En términos de $I_1$ (sustituyendo $k = \frac{2I_1}{\pi R^4}$):
   $$B(r) = \frac{\mu_0 I_1 r^3}{2\pi R^4}$$

   Vectorialmente:
   $$\boxed{\vec{B}(r < R) = \frac{\mu_0 k r^3}{4}\,\hat{\theta} = \frac{\mu_0 I_1 r^3}{2\pi R^4}\,\hat{\theta}}$$

2. **Región exterior ($r > R$):**
   La espira amperiana encierra la corriente total $I_1$:
   $$I_{\text{enc}} = I_1 = \frac{\pi k R^4}{2}$$
   $$B(r) \cdot 2\pi r = \mu_0 \left( \frac{\pi k R^4}{2} \right) \implies B(r) = \frac{\mu_0 k R^4}{4r}$$

   En términos de $I_1$:
   $$B(r) = \frac{\mu_0 I_1}{2\pi r}$$

   Vectorialmente:
   $$\boxed{\vec{B}(r > R) = \frac{\mu_0 k R^4}{4r}\,\hat{\theta} = \frac{\mu_0 I_1}{2\pi r}\,\hat{\theta}}$$

---

#### Parte c) Fuerza total y torque sobre la espira

La espira está en el plano $YZ$ con coordenadas $y > 0$. En esta zona, el vector unitario azimutal apunta perpendicularmente hacia el interior del papel:
$$\hat{\theta}\Big|_{y > 0,\, x=0} = -\hat{x}$$

Por lo tanto, en todo el plano de la espira, el campo magnético del cilindro es entrante:
$$\vec{B}(y) = -\frac{\mu_0 k R^4}{4y}\,\hat{x} = -\frac{\mu_0 I_1}{2\pi y}\,\hat{x}$$

La fuerza magnética sobre cada tramo conductor con corriente $I_2$ se calcula mediante:
$$\vec{F} = I_2 \int d\vec{\ell} \times \vec{B}$$

Desglosamos los cuatro lados de la espira:

1. **Tramo 1 (lado vertical izquierdo, $y = a$, corriente en $+\hat{z}$ desde $z = 0$ hasta $z = c$):**
   $$d\vec{\ell}_1 = dz\,\hat{z}$$
   $$\vec{F}_1 = I_2 \int_0^c dz\,\hat{z} \times \left( -\frac{\mu_0 I_1}{2\pi a}\,\hat{x} \right) = - \frac{\mu_0 I_1 I_2}{2\pi a} (\hat{z} \times \hat{x}) \int_0^c dz = - \frac{\mu_0 I_1 I_2 c}{2\pi a}\,\hat{y}$$

2. **Tramo 2 (lado horizontal superior, $z = c$, corriente en $+\hat{y}$ desde $y = a$ hasta $y = a+b$):**
   $$d\vec{\ell}_2 = dy\,\hat{y}$$
   $$\vec{F}_2 = I_2 \int_a^{a+b} dy\,\hat{y} \times \left( -\frac{\mu_0 I_1}{2\pi y}\,\hat{x} \right) = \frac{\mu_0 I_1 I_2}{2\pi} (\hat{y} \times (-\hat{x})) \int_a^{a+b} \frac{dy}{y} = + \frac{\mu_0 I_1 I_2}{2\pi} \ln\left( \frac{a+b}{a} \right)\,\hat{z}$$

3. **Tramo 3 (lado vertical derecho, $y = a+b$, corriente en $-\hat{z}$ desde $z = c$ hasta $z = 0$):**
   $$d\vec{\ell}_3 = -dz\,\hat{z}$$
   $$\vec{F}_3 = I_2 \int_c^0 (-dz\,\hat{z}) \times \left( -\frac{\mu_0 I_1}{2\pi (a+b)}\,\hat{x} \right) = I_2 \int_0^c dz\,\hat{z} \times \left( \frac{\mu_0 I_1}{2\pi (a+b)}\,\hat{x} \right) = + \frac{\mu_0 I_1 I_2 c}{2\pi (a+b)}\,\hat{y}$$

4. **Tramo 4 (lado horizontal inferior, $z = 0$, corriente en $-\hat{y}$ desde $y = a+b$ hasta $y = a$):**
   $$d\vec{\ell}_4 = -dy\,\hat{y}$$
   $$\vec{F}_4 = I_2 \int_{a+b}^a (-dy\,\hat{y}) \times \left( -\frac{\mu_0 I_1}{2\pi y}\,\hat{x} \right) = - \frac{\mu_0 I_1 I_2}{2\pi} \ln\left( \frac{a+b}{a} \right)\,\hat{z} = -\vec{F}_2$$

Las fuerzas sobre los tramos horizontales se anulan mutuamente ($\vec{F}_2 + \vec{F}_4 = \vec{0}$).  
La fuerza magnética total neta sobre la espira es:
$$\vec{F}_{\text{total}} = \vec{F}_1 + \vec{F}_3 = - \frac{\mu_0 I_1 I_2 c}{2\pi} \left[ \frac{1}{a} - \frac{1}{a+b} \right]\,\hat{y} = - \frac{\mu_0 I_1 I_2 b c}{2\pi a(a+b)}\,\hat{y}$$

Expresada en función de la constante $k$ (empleando $I_1 = \frac{\pi k R^4}{2}$):
$$\boxed{\vec{F}_{\text{total}} = - \frac{\mu_0 k I_2 c R^4}{4} \left[ \frac{1}{a} - \frac{1}{a+b} \right]\,\hat{y} = - \frac{\mu_0 k I_2 b c R^4}{4 a (a+b)}\,\hat{y}}$$

> **Nota:** La solución oficial presenta una errata tipográfica en su ecuación (16) al escribir dentro del corchete $\left[ \frac{1}{a} - \frac{1}{a+c} \right]$; lo correcto es $\left[ \frac{1}{a} - \frac{1}{a+b} \right]$, ya que la dimensión horizontal de la espira es $b$, tal como se deriva correctamente en las ecuaciones (10) y (15) de la misma pauta oficial.

**Torque magnético:**  
Dado que la corriente circula en sentido horario en el plano $YZ$, el momento dipolar magnético de la espira apunta entrando a la hoja por la regla de la mano derecha:
$$\vec{m} = I_2 \vec{A} = - I_2 b c\,\hat{x}$$
Como el campo magnético $\vec{B}(y)$ producido por el cilindro sobre el plano de la espira también está alineado con la dirección perpendicular al plano ($\vec{B} \parallel -\hat{x}$), el momento dipolar y el campo son colineales:
$$\vec{\tau} = \vec{m} \times \vec{B} = (-I_2 b c\,\hat{x}) \times (B_x\,\hat{x}) = \vec{0}$$

$$\boxed{\vec{\tau} = \vec{0}}$$

*(Alternativamente, como todas las fuerzas $\vec{F}_1, \vec{F}_2, \vec{F}_3, \vec{F}_4$ están contenidas en el plano de la espira y sus líneas de acción pasan por dicho plano, el torque resultante es nulo).*

---

## Problema 4

Se tiene un conductor en la forma de una capa cilíndrica recta, infinita, de radio interior $a$ y radio exterior $b$. Este conductor tiene una densidad de corriente que, expresada en coordenadas cilíndricas, es:
$$\vec{J}(a \le r \le b) = \frac{\alpha}{r}\,\hat{\theta} + \beta\,\hat{z}$$
Con $\alpha$ y $\beta$ constantes conocidas. Obtenga el campo magnético en todo el espacio.

> **[Figura]:** Capa cilíndrica hueca infinita centrada sobre el eje $z$, con radio interior $a$ y radio exterior $b$. La corriente transportada posee dos componentes ortogonales simultáneas: una componente azimutal $\vec{J}_\theta = \frac{\alpha}{r}\hat{\theta}$ que enrolla circunferencialmente el cilindro, y una componente axial $\vec{J}_z = \beta \hat{z}$ uniforme a lo largo del eje del cilindro.

### Solución

**Idea:** Aplicamos el principio de superposición descomponiendo la densidad de corriente en dos distribuciones independientes:
$$\vec{J} = \vec{J}_1 + \vec{J}_2, \qquad \vec{J}_1 = \frac{\alpha}{r}\,\hat{\theta}, \qquad \vec{J}_2 = \beta\,\hat{z}$$
El campo magnético total será $\vec{B}(\vec{r}) = \vec{B}_1(\vec{r}) + \vec{B}_2(\vec{r})$. Determinamos $\vec{B}_1$ mediante analogía con un solenoide continuo (o ley de Biot-Savart/Ampère meridiana) y $\vec{B}_2$ mediante la ley de Ampère azimutal.

---

#### 1. Campo debido a la corriente azimutal $\vec{J}_1 = \frac{\alpha}{r}\,\hat{\theta}$

Una corriente puramente circular alrededor del eje $z$ es análoga a la de un solenoide infinito. Por simetría y regla de la mano derecha, genera un campo magnético estrictamente axial:
$$\vec{B}_1(r) = B_1(r)\,\hat{z}$$

Para calcular este campo mediante la ley de Ampère, se utiliza un lazo rectangular $\Gamma$ en un plano meridiano $rz$ de altura $L$ en la dirección axial $z$:
- El lado interior se coloca a lo largo del eje de simetría $r = 0$.
- El lado exterior se coloca a un radio arbitrario $r$.
- Los lados perpendiculares en $r$ tienen aporte nulo porque $\vec{B}_1 \cdot d\vec{r} = 0$.

La circulación a lo largo de $\Gamma$ orientada convenientemente es:
$$\oint_\Gamma \vec{B}_1 \cdot d\vec{\ell} = [B_1(0) - B_1(r)] L = \mu_0 I_{\text{enc}}$$

Para fijar la condición de contorno o el valor central $B_1(0)$, se evalúa la ley de Biot-Savart sobre el eje ($r = 0$):
$$\vec{B}_1(0) = \frac{\mu_0}{4\pi} \int_{-\infty}^\infty dz \int_0^{2\pi} d\theta \int_a^b dr \frac{\left( \frac{\alpha}{r}\,\hat{\theta} \right) \times (-r\,\hat{r} + z\,\hat{z})}{(r^2 + z^2)^{3/2}}$$

Como $\hat{\theta} \times (-\hat{r}) = \hat{z}$ y la componente en $\hat{\theta} \times \hat{z} = \hat{r}$ se cancela al integrar en $\theta \in [0, 2\pi]$:
$$\vec{B}_1(0) = \frac{\mu_0}{4\pi} \cdot 2\pi \hat{z} \int_a^b \frac{\alpha}{r} r\,dr \int_{-\infty}^\infty \frac{dz}{(r^2 + z^2)^{3/2}} = \frac{\mu_0 \alpha}{2} \hat{z} \int_a^b dr \left[ \frac{z}{r^2 \sqrt{r^2 + z^2}} \right]_{-\infty}^\infty$$
$$\vec{B}_1(0) = \frac{\mu_0 \alpha}{2} \hat{z} \int_a^b dr \left( \frac{2}{r} \right) = \mu_0 \alpha \ln\left(\frac{b}{a}\right)\,\hat{z}$$

Asimismo, por simetría de solenoide infinito, el campo magnético en el exterior debe anularse:
$$\vec{B}_1(r > b) = \vec{0}$$

Evaluando las distintas regiones con la ley de Ampère:
- **Para $r < a$ (región hueca interior):**  
  No hay corriente azimutal encerrada entre $0$ y $r$, por lo que:
  $$[B_1(0) - B_1(r)] L = 0 \implies B_1(r) = B_1(0) = \mu_0 \alpha \ln\left(\frac{b}{a}\right)$$
  $$\vec{B}_1(r < a) = \mu_0 \alpha \ln\left(\frac{b}{a}\right)\,\hat{z}$$

- **Para $a \le r \le b$ (dentro del conductor):**  
  La corriente azimutal que atraviesa el lazo amperiano entre $a$ y $r$ es:
  $$I_{\text{enc}} = \int_0^L dz \int_a^r dr'\, J_\theta(r') = L \int_a^r \frac{\alpha}{r'}\,dr' = L \alpha \ln\left(\frac{r}{a}\right)$$
  $$[B_1(0) - B_1(r)] L = \mu_0 L \alpha \ln\left(\frac{r}{a}\right)$$
  $$B_1(r) = B_1(0) - \mu_0 \alpha \ln\left(\frac{r}{a}\right) = \mu_0 \alpha \ln\left(\frac{b}{a}\right) - \mu_0 \alpha \ln\left(\frac{r}{a}\right) = \mu_0 \alpha \ln\left(\frac{b}{r}\right)$$
  $$\vec{B}_1(a \le r \le b) = \mu_0 \alpha \ln\left(\frac{b}{r}\right)\,\hat{z}$$

- **Para $r > b$ (región exterior):**  
  $$\vec{B}_1(r > b) = \vec{0}$$

---

#### 2. Campo debido a la corriente axial $\vec{J}_2 = \beta\,\hat{z}$

La corriente axial produce un campo puramente azimutal: $\vec{B}_2(r) = B_2(r)\,\hat{\theta}$.  
Aplicando la ley de Ampère en circunferencias concéntricas de radio $r$:
$$\oint \vec{B}_2 \cdot d\vec{\ell} = B_2(r) \cdot 2\pi r = \mu_0 I_{\text{enc}}$$

- **Para $r < a$:**  
  No hay corriente encerrada:
  $$I_{\text{enc}} = 0 \implies \vec{B}_2(r < a) = \vec{0}$$

- **Para $a \le r \le b$:**  
  $$I_{\text{enc}}(r) = \int_0^{2\pi} d\theta \int_a^r \beta r'\,dr' = \beta \pi (r^2 - a^2)$$
  $$B_2(r) \cdot 2\pi r = \mu_0 \beta \pi (r^2 - a^2) \implies B_2(r) = \frac{\mu_0 \beta (r^2 - a^2)}{2r}$$
  $$\vec{B}_2(a \le r \le b) = \frac{\mu_0 \beta (r^2 - a^2)}{2r}\,\hat{\theta}$$

- **Para $r > b$:**  
  Se encierra toda la corriente axial de la capa cilíndrica:
  $$I_{\text{enc}} = \beta \pi (b^2 - a^2)$$
  $$B_2(r) \cdot 2\pi r = \mu_0 \beta \pi (b^2 - a^2) \implies B_2(r) = \frac{\mu_0 \beta (b^2 - a^2)}{2r}$$
  $$\vec{B}_2(r > b) = \frac{\mu_0 \beta (b^2 - a^2)}{2r}\,\hat{\theta}$$

---

#### 3. Campo magnético total

Superponiendo vectorialmente $\vec{B}(r) = \vec{B}_1(r) + \vec{B}_2(r)$:

$$\boxed{\vec{B}(r) = \begin{cases}
\mu_0 \alpha \ln\left(\dfrac{b}{a}\right)\,\hat{z}, & r < a \\[2ex]
\dfrac{\mu_0 \beta (r^2 - a^2)}{2r}\,\hat{\theta} + \mu_0 \alpha \ln\left(\dfrac{b}{r}\right)\,\hat{z}, & a \le r \le b \\[2ex]
\dfrac{\mu_0 \beta (b^2 - a^2)}{2r}\,\hat{\theta}, & r > b
\end{cases}}$$

**Verificación:**
- **Continuidad de componentes:**
  - En $r \to a^-$: $\vec{B} = \mu_0 \alpha \ln(b/a)\,\hat{z}$. En $r \to a^+$: el término azimutal vale $\frac{\mu_0 \beta (a^2 - a^2)}{2a} = 0$, y el término axial vale $\mu_0 \alpha \ln(b/a)\,\hat{z}$. Coinciden perfectamente.
  - En $r \to b^-$: el término axial vale $\mu_0 \alpha \ln(b/b) = 0$, y el término azimutal vale $\frac{\mu_0 \beta (b^2 - a^2)}{2b}\,\hat{\theta}$, que coincide exactamente con el límite para $r \to b^+$.
- **Límites:** Si $\alpha = 0$, se recupera el cilindro hueco con corriente axial común; si $\beta = 0$, se recupera el solenoide grueso de espesor $b-a$.

---

## Resumen de resultados

| Problema | Parte | Parámetro / Variable | Resultado Final |
| :--- | :--- | :--- | :--- |
| **Problema 1** | a) | Constante $\alpha$ | $\displaystyle \alpha = \frac{3I_0}{2\pi a^3}$ |
| | a) | Constante $\beta$ | $\displaystyle \beta = \frac{I_0}{\pi (c^2 - b^2)}$ |
| | b) | Campo $\vec{B}$ ($0 \le r < a$) | $\displaystyle \vec{B} = \frac{\mu_0 I_0 r^2}{2\pi a^3}\,\hat{\theta}$ |
| | b) | Campo $\vec{B}$ ($a \le r < b$) | $\displaystyle \vec{B} = \frac{\mu_0 I_0}{2\pi r}\,\hat{\theta}$ |
| | b) | Campo $\vec{B}$ ($b \le r < c$) | $\displaystyle \vec{B} = \frac{\mu_0 I_0 (c^2 - r^2)}{2\pi r (c^2 - b^2)}\,\hat{\theta}$ |
| | b) | Campo $\vec{B}$ ($r \ge c$) | $\displaystyle \vec{B} = \vec{0}$ |
| **Problema 2** | — | Densidad $j_0(j_s)$ para campo nulo en $P$ | $\displaystyle j_0 = \frac{3b}{R} j_s$ |
| **Problema 3** | a) | Constante $k$ | $\displaystyle k = \frac{2I_1}{\pi R^4}$ |
| | b) | Campo $\vec{B}$ ($r < R$) | $\displaystyle \vec{B} = \frac{\mu_0 k r^3}{4}\,\hat{\theta} = \frac{\mu_0 I_1 r^3}{2\pi R^4}\,\hat{\theta}$ |
| | b) | Campo $\vec{B}$ ($r > R$) | $\displaystyle \vec{B} = \frac{\mu_0 k R^4}{4r}\,\hat{\theta} = \frac{\mu_0 I_1}{2\pi r}\,\hat{\theta}$ |
| | c) | Fuerza neta $\vec{F}_{\text{total}}$ sobre la espira | $\displaystyle \vec{F}_{\text{total}} = -\frac{\mu_0 k I_2 b c R^4}{4a(a+b)}\,\hat{y} = -\frac{\mu_0 I_1 I_2 b c}{2\pi a(a+b)}\,\hat{y}$ |
| | c) | Torque magnético $\vec{\tau}$ sobre la espira | $\displaystyle \vec{\tau} = \vec{0}$ |
| **Problema 4** | — | Campo $\vec{B}$ ($r < a$) | $\displaystyle \vec{B} = \mu_0 \alpha \ln\left(\frac{b}{a}\right)\,\hat{z}$ |
| | — | Campo $\vec{B}$ ($a \le r \le b$) | $\displaystyle \vec{B} = \frac{\mu_0 \beta (r^2 - a^2)}{2r}\,\hat{\theta} + \mu_0 \alpha \ln\left(\frac{b}{r}\right)\,\hat{z}$ |
| | — | Campo $\vec{B}$ ($r > b$) | $\displaystyle \vec{B} = \frac{\mu_0 \beta (b^2 - a^2)}{2r}\,\hat{\theta}$ |
