# Pauta Control 1 — Ley de Gauss y corazas esféricas conductoras

> **Curso:** FIS1533-2 (Primer semestre 2026) · **Fecha:** 08 de abril de 2026 · **Evaluación:** Control 1 (Forma 1)

---

## Problema 1

Una coraza esférica conductora pequeña con radio interior $a$ y radio exterior $b$ es concéntrica respecto a otra coraza conductora esférica más grande cuyo radio interior es $c$ y radio exterior $d$. La coraza interior tiene una carga total de $+2q$, y la exterior tiene carga de $+4q$.

a) **(3 pts.)** Calcule el campo eléctrico (magnitud y dirección) en términos de $q$ y la distancia $r$ a partir del centro común de las dos corazas para:
- I) $r < a$
- II) $a < r < b$
- III) $b < r < c$
- IV) $c < r < d$
- V) $r > d$

b) **(3 pts.)** ¿Cuál es la densidad de carga superficial total en:
- I) la superficie interior de la coraza pequeña
- II) la superficie exterior de la coraza pequeña
- III) la superficie interior de la coraza grande
- IV) la superficie exterior de la coraza grande?

> **[Figura]:** Corte transversal de dos corazas esféricas conductoras concéntricas con radios ordenados $a < b < c < d$. Desde el centro común parten cuatro flechas radiales que indican los radios: la cavidad central vacía tiene radio $a$; la coraza conductora interior (sombreada en gris pardo) se extiende entre $a$ y $b$ y posee carga total $+2q$; la región intermedia vacía se extiende entre $b$ y $c$; la coraza conductora exterior (sombreada en amarillo ocre) se extiende entre $c$ y $d$ y posee carga total $+4q$; fuera de $r = d$ hay espacio libre.

---

### Solución

**Idea:** Por la simetría esférica del sistema y las propiedades de los conductores en equilibrio electrostático, el campo eléctrico es puramente radial ($\vec{E}(\vec{r}) = E(r)\,\hat{r}$) y se anula en el interior de cada material conductor. Se aplica la ley de Gauss con superficies gaussianas esféricas concéntricas de radio $r$ en cada región, donde el flujo eléctrico es $\oint_S \vec{E}\cdot d\vec{A} = E(r)\,(4\pi r^2) = Q_{\text{enc}}/\varepsilon_0$.

#### Parte a) Campo eléctrico en todo el espacio (3.0 pts.)

Utilizando una superficie gaussiana esférica concéntrica de radio $r$ y la constante de Coulomb $k = \dfrac{1}{4\pi\varepsilon_0}$, se analiza cada región:

- **I) Para $r < a$:**  
  No existe carga encerrada dentro de la cavidad interior ($Q_{\text{enc}} = 0$), por lo que el campo eléctrico es nulo:
  $$\boxed{\vec{E}_{\text{I}} = 0 \qquad (r < a)} \qquad \text{(0.5 pts.)}$$

- **II) Para $a < r < b$:**  
  Nos encontramos dentro del material de la coraza conductora interior; en equilibrio electrostático, el campo eléctrico dentro de un conductor es nulo:
  $$\boxed{\vec{E}_{\text{II}} = 0 \qquad (a < r < b)} \qquad \text{(0.5 pts.)}$$

- **III) Para $b < r < c$:**  
  Nos encontramos en el espacio vacío entre ambos conductores. Una superficie gaussiana esférica de radio $r$ encierra únicamente la carga total de la coraza interior:
  $$Q_{\text{enc}} = +2q \qquad \text{(0.25 pts.)}$$
  Aplicando la ley de Gauss:
  $$E_{\text{III}}\,(4\pi r^2) = \frac{2q}{\varepsilon_0} \implies E_{\text{III}} = \frac{2q}{4\pi\varepsilon_0 r^2} = 2k\frac{q}{r^2}$$
  En forma vectorial:
  $$\boxed{\vec{E}_{\text{III}} = 2k\frac{q}{r^2}\,\hat{r} \qquad (b < r < c)} \qquad \text{(0.5 pts.)}$$

- **IV) Para $c < r < d$:**  
  Nos encontramos nuevamente dentro de un material conductor (la coraza exterior), por lo que el campo eléctrico es nulo:
  $$\boxed{\vec{E}_{\text{IV}} = 0 \qquad (c < r < d)} \qquad \text{(0.5 pts.)}$$

- **V) Para $r > d$ ($d < r$):**  
  Aplicando la ley de Gauss a una esfera de radio $r > d$, la carga encerrada es la suma de las cargas totales de ambas corazas:
  $$Q_{\text{enc}} = 4q + 2q = 6q \qquad \text{(0.25 pts.)}$$
  Por lo tanto,
  $$E_{\text{V}}\,(4\pi r^2) = \frac{6q}{\varepsilon_0} \implies E_{\text{V}} = \frac{6q}{4\pi\varepsilon_0 r^2} = 6k\frac{q}{r^2}$$
  En forma vectorial:
  $$\boxed{\vec{E}_{\text{V}} = 6k\frac{q}{r^2}\,\hat{r} \qquad (r > d)} \qquad \text{(0.5 pts.)}$$

---

#### Parte b) Densidad superficial de carga en cada superficie (3.0 pts.)

Utilizando la ley de Gauss y la condición de campo nulo en el interior de los conductores ($a < r < b$ y $c < r < d$), se determina la carga en cada superficie y su densidad $\sigma = q_{\text{sup}} / (4\pi R^2)$:

- **I) Superficie interior de la coraza pequeña ($r = a$):**  
  Dado que el campo eléctrico en la cavidad $r < a$ es nulo (y también en $a < r < b$), al elegir una superficie gaussiana justo dentro del conductor rodeando $r = a$ se obtiene que no hay carga encerrada ($q_{\text{int, peq}} = 0$). Entonces:
  $$\boxed{\sigma_{\text{int, pequeña}} = 0} \qquad \text{(0.5 pts.)}$$

- **II) Superficie exterior de la coraza pequeña ($r = b$):**  
  La carga total de la coraza pequeña es $+2q$ y su superficie interior no tiene carga, de modo que toda la carga $+2q$ debe residir en la superficie exterior (equivalente a considerar una superficie gaussiana en el borde exterior que encierra $+2q$):
  $$\sigma_{\text{ext, pequeña}} = \frac{2q}{4\pi b^2} = \frac{q}{2\pi b^2}$$
  $$\boxed{\sigma_{\text{ext, pequeña}} = \frac{q}{2\pi b^2}} \qquad \text{(0.5 pts.)}$$

- **III) Superficie interior de la coraza grande ($r = c$):**  
  Para una superficie gaussiana esférica dentro del conductor grande ($c < r < d$), el campo eléctrico es nulo, por lo que el flujo es cero y la carga total encerrada también debe ser nula:
  $$q_{\text{enc}} = q_{\text{int, grande}} + 2q = 0 \implies q_{\text{int, grande}} = -2q \qquad \text{(0.5 pts.)}$$
  Luego, la densidad superficial en $r = c$ es:
  $$\sigma_{\text{int, grande}} = -\frac{2q}{4\pi c^2} = -\frac{q}{2\pi c^2}$$
  $$\boxed{\sigma_{\text{int, grande}} = -\frac{q}{2\pi c^2}} \qquad \text{(0.5 pts.)}$$

- **IV) Superficie exterior de la coraza grande ($r = d$):**  
  Por conservación de la carga, la carga total de la coraza grande es $+4q$:
  $$Q = 4q = q_{\text{int, grande}} + q_{\text{ext, grande}} \implies q_{\text{ext, grande}} = 4q - (-2q) = 6q \qquad \text{(0.5 pts.)}$$
  Dividiendo por el área de la esfera de radio $d$:
  $$\sigma_{\text{ext, grande}} = \frac{6q}{4\pi d^2} = \frac{3q}{2\pi d^2}$$
  $$\boxed{\sigma_{\text{ext, grande}} = \frac{3q}{2\pi d^2}} \qquad \text{(0.5 pts.)}$$

**Verificación:**
- **Discontinuidad del campo en las fronteras:** En todo conductor en equilibrio, el salto del campo normal es $\Delta E_r = \sigma/\varepsilon_0$. Se cumple en $r = b$: $E_{\text{III}}(b^+) - E_{\text{II}}(b^-) = \frac{2q}{4\pi\varepsilon_0 b^2} = \frac{\sigma_{\text{ext, pequeña}}}{\varepsilon_0}$; en $r = c$: $E_{\text{IV}}(c^+) - E_{\text{III}}(c^-) = -\frac{2q}{4\pi\varepsilon_0 c^2} = \frac{\sigma_{\text{int, grande}}}{\varepsilon_0}$; y en $r = d$: $E_{\text{V}}(d^+) - E_{\text{IV}}(d^-) = \frac{6q}{4\pi\varepsilon_0 d^2} = \frac{\sigma_{\text{ext, grande}}}{\varepsilon_0}$.
- **Unidades:** $[k q / r^2] = (\text{N}\cdot\text{m}^2/\text{C}^2)(\text{C})/\text{m}^2 = \text{N/C}$; $[\sigma] = \text{C}/\text{m}^2$.
- **Nota sobre el signo de $q$:** Las expresiones vectoriales $\vec{E}$ son válidas para cualquier signo de $q$ (si $q > 0$, apuntan en $+\hat{r}$; si $q < 0$, apuntan hacia adentro, $-\hat{r}$).

---

## Resumen de resultados

| Problema | Parte | Región / Superficie | Resultado |
| :--- | :--- | :--- | :--- |
| **Problema 1** | a) I | $r < a$ | $\vec{E}_{\text{I}} = 0$ |
| | a) II | $a < r < b$ | $\vec{E}_{\text{II}} = 0$ |
| | a) III | $b < r < c$ | $\vec{E}_{\text{III}} = 2k\dfrac{q}{r^2}\,\hat{r}$ |
| | a) IV | $c < r < d$ | $\vec{E}_{\text{IV}} = 0$ |
| | a) V | $r > d$ | $\vec{E}_{\text{V}} = 6k\dfrac{q}{r^2}\,\hat{r}$ |
| | b) I | Superficie interior coraza pequeña ($r = a$) | $\sigma_{\text{int, pequeña}} = 0$ |
| | b) II | Superficie exterior coraza pequeña ($r = b$) | $\sigma_{\text{ext, pequeña}} = \dfrac{q}{2\pi b^2}$ |
| | b) III | Superficie interior coraza grande ($r = c$) | $\sigma_{\text{int, grande}} = -\dfrac{q}{2\pi c^2}$ |
| | b) IV | Superficie exterior coraza grande ($r = d$) | $\sigma_{\text{ext, grande}} = \dfrac{3q}{2\pi d^2}$ |
