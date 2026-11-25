# Control 1 — Ley de Gauss, conductores y potencial electrostático

> **Curso:** FIS1533 — Electricidad y Magnetismo (Segundo semestre 2025) · **Fecha:** 9 de septiembre de 2025 · **Forma:** 1  
> **Instrucciones y escala (enunciado oficial):** Control grupal (hasta 3 estudiantes), duración máxima de 25 minutos, 1 desarrollo por grupo. Calificación entre $4{,}0$ y $7{,}0$: $0 \le \text{ptje} < 2 \to \text{No rinde}$ (entrega en blanco también queda como no realizado); $2 \le \text{ptje} < 4 \to \text{Nota } 4{,}0$.

---

## Problema 1

Una esfera no conductora de radio $a$ posee una densidad volumétrica de carga dada por
$$\rho(r) = \beta r^{3/2}$$
donde $r \ge 0$ es la distancia radial desde el centro de la esfera y $\beta$ es una constante conocida.

Si la esfera es rodeada por un cascarón esférico neutro de radio interno $a$ y radio externo $b$ hecho de un material conductor:

- **i) (3 pts.)** Determine el campo electrostático en todo el espacio. Bosqueje un gráfico de la magnitud del campo eléctrico en función de $r$ (indique claramente los valores en el gráfico).
- **ii) (1 pto.)** Calcule la densidad de carga superficial inducida en las superficies interna y externa del cascarón conductor.
- **iii) (2 pts.)** Suponiendo que el potencial electrostático $V = 0$ en infinito, determine el potencial electrostático en el centro de la esfera no conductora $r = 0$.

> **[Figura]:** Corte transversal de dos regiones esféricas concéntricas centradas en el origen. En el interior se muestra la esfera sólida no conductora de radio $a$ (sombreado gris claro), con la etiqueta $\rho(r)$ en su interior y una flecha radial desde el centro hasta la frontera en $r = a$. Rodeándola inmediatamente, entre el radio interno $a$ y el radio externo $b$, se encuentra el cascarón esférico conductor neutro (sombreado gris más oscuro), con una flecha radial desde el centro hasta el borde exterior en $r = b$.

### Solución

**Idea:** Como la distribución de carga $\rho(r)$ posee simetría esférica (depende únicamente de la distancia radial $r$) y el cascarón conductor es concéntrico y neutro, el campo eléctrico en todo el espacio es radial y su magnitud depende solo de $r$: $\vec{E}(\vec{r}) = E(r)\,\hat{r}$. Esto permite hallar $\vec{E}$ en cada región mediante la ley de Gauss con superficies gaussianas esféricas concéntricas, usar el equilibrio electrostático del conductor ($\vec{E} = \vec{0}$ en $a < r < b$) junto con la conservación de carga para hallar las densidades inducidas, e integrar $\vec{E}$ desde infinito hasta $r = 0$ para obtener el potencial en el centro.

---

#### Parte i) Campo electrostático en todo el espacio y gráfico de $|\vec{E}(r)|$

Como la densidad de carga es función únicamente de $r$, aplicamos la ley de Gauss utilizando superficies gaussianas esféricas concéntricas de radio $r$, según las tres regiones del problema:

> **[Figura — Superficies gaussianas]:** Esquema concéntrico sobre las fronteras sólidas de radios $a$ y $b$ que ilustra tres superficies gaussianas esféricas en línea discontinua: una en el interior ($r < a$), una dentro del espesor del cascarón conductor ($a < r < b$) y una en el exterior ($r > b$). Desde el centro de la esfera se dibuja un vector unitario radial $\hat{r}$ apuntando hacia afuera.

En cada región, por simetría esférica, la magnitud del campo es constante sobre la superficie gaussiana y su dirección es radial ($\vec{E} \parallel d\vec{A}$), de modo que:
$$\oint \vec{E}\cdot d\vec{A} = \frac{q_{\text{enc}}}{\varepsilon_0} \implies 4\pi r^2 E = \frac{q_{\text{enc}}}{\varepsilon_0}$$

1. **Región $r < a$ (interior de la esfera no conductora):**  
   La carga encerrada dentro de una esfera de radio $r < a$ es:
   $$q_{\text{enc}} = \int dq = \int \rho(r')\,dV' = 4\pi \int_0^r \beta (r')^{3/2} (r')^2\,dr' = 4\pi\beta \int_0^r (r')^{7/2}\,dr' = 4\pi\beta \left[\frac{(r')^{9/2}}{9/2}\right]_0^r = \frac{8\pi\beta r^{9/2}}{9} \qquad \text{(0.4 pts)}$$

   > **Nota:** La solución oficial omite tipográficamente el exponente en el diferencial de volumen al escribir $4\pi\int_0^r \beta r^{3/2} r\,dr$, pero en el paso siguiente escribe correctamente el integrando $r^{7/2}\,dr$ y obtiene el resultado exacto $q_{\text{enc}} = \frac{8\pi\beta r^{9/2}}{9}$.

   Reemplazando $q_{\text{enc}}$ en la ley de Gauss ($E_1 = \frac{q_{\text{enc}}}{4\pi\varepsilon_0 r^2}$):
   $$\vec{E}_1 = \frac{8\pi\beta r^{9/2}}{9 \cdot 4\pi\varepsilon_0 r^2}\,\hat{r} = \frac{2}{9\varepsilon_0}\beta r^{5/2}\,\hat{r}, \qquad r < a \qquad \text{(0.4 pts)}$$

2. **Región $a < r < b$ (interior del cascarón conductor):**  
   Al encontrarse el material conductor en equilibrio electrostático, el campo eléctrico en su interior es nulo:
   $$\vec{E}_2 = \vec{0}, \qquad a < r < b \qquad \text{(0.8 pts)}$$

3. **Región $r > b$ (exterior del sistema):**  
   Como el cascarón conductor es neutro ($q_{\text{cascarón}} = 0$), la carga total encerrada por una superficie gaussiana de radio $r > b$ coincide con la carga total $Q$ de la esfera no conductora:
   $$Q = \int_0^a \rho(r')\,dV' = \left.\frac{8\pi}{9}\beta r^{9/2}\right|_{r=a} = \frac{8\pi}{9}\beta a^{9/2} \qquad \text{(0.4 pts)}$$

   Por lo tanto, el campo eléctrico exterior es:
   $$\vec{E}_3 = \frac{Q}{4\pi\varepsilon_0 r^2}\,\hat{r} = \frac{2\beta a^{9/2}}{9\varepsilon_0 r^2}\,\hat{r}, \qquad r > b \qquad \text{(0.4 pts)}$$

$$\boxed{\vec{E}(r) = \begin{cases} \dfrac{2\beta r^{5/2}}{9\varepsilon_0}\,\hat{r}, & r < a \\[8pt] \vec{0}, & a < r < b \\[8pt] \dfrac{2\beta a^{9/2}}{9\varepsilon_0 r^2}\,\hat{r}, & r > b \end{cases}}$$

4. **Bosquejo del gráfico de $|\vec{E}|$ en función de $r$ (0.6 pts: 0.2 pts por cada tramo):**

> **[Figura — Gráfico de $|\vec{E}(r)|$]:** Gráfico cartesiano con eje horizontal $r$ (con marcas en $0$, $a$ y $b$) y eje vertical $E = |\vec{E}|$ (con valores indicados $\frac{2}{9\varepsilon_0}\beta a^{5/2}$ y $\frac{2\beta a^{9/2}}{9\varepsilon_0 b^2}$).  
> - Para $0 \le r < a$ *(0.2 pts)*: la curva parte desde el origen $(0, 0)$ y crece de manera cóncava hacia arriba ($E \propto r^{5/2}$) hasta alcanzar el valor máximo $E(a^-) = \frac{2}{9\varepsilon_0}\beta a^{5/2}$ en $r = a$.  
> - Para $a < r < b$ *(0.2 pts)*: la magnitud cae bruscamente a cero en $r = a$ y permanece constante en $E = 0$ sobre el eje horizontal hasta $r = b$.  
> - Para $r > b$ *(0.2 pts)*: en $r = b$ presenta un salto vertical discontinuo hasta $E(b^+) = \frac{2\beta a^{9/2}}{9\varepsilon_0 b^2}$ (menor que $E(a^-)$ pues $b > a$) y luego decrece suavemente de forma asintótica hacia cero como $1/r^2$ cuando $r \to \infty$.

---

#### Parte ii) Densidades de carga superficial inducidas

Para determinar la carga total $q_{\text{int}}$ inducida en la superficie interna del cascarón conductor ($r = a$), aplicamos la ley de Gauss sobre una superficie esférica dentro del conductor ($a < r < b$). Como $\vec{E}_2 = \vec{0}$, la carga neta encerrada debe ser cero:
$$Q + q_{\text{int}} = 0 \implies q_{\text{int}} = -Q$$

Por simetría esférica, la densidad superficial $\sigma_{\text{int}}$ es uniforme sobre la esfera de radio $a$ ($A_{\text{int}} = 4\pi a^2$):
$$q_{\text{int}} = -Q = \int \sigma_{\text{int}}\,dA = \sigma_{\text{int}} A_{\text{int}}$$
$$\sigma_{\text{int}} = -\frac{Q}{4\pi a^2} = -\frac{\frac{8\pi}{9}\beta a^{9/2}}{4\pi a^2} = -\frac{2\beta a^{5/2}}{9} \qquad \text{(0.5 pts)}$$

Como el cascarón conductor es neutro en conjunto, la suma de las cargas inducidas en sus superficies interna y externa debe anularse:
$$q_{\text{int}} + q_{\text{ext}} = 0 \implies q_{\text{ext}} = -q_{\text{int}} = Q$$

Distribuyendo $q_{\text{ext}}$ uniformemente sobre la superficie exterior de radio $b$ ($A_{\text{ext}} = 4\pi b^2$):
$$\sigma_{\text{ext}} = \frac{q_{\text{ext}}}{4\pi b^2} = \frac{Q}{4\pi b^2} = \frac{\frac{8\pi}{9}\beta a^{9/2}}{4\pi b^2} = \frac{2\beta a^{9/2}}{9b^2} \qquad \text{(0.5 pts)}$$

$$\boxed{\sigma_{\text{int}} = -\frac{2\beta a^{5/2}}{9}, \qquad \sigma_{\text{ext}} = \frac{2\beta a^{9/2}}{9b^2}}$$

---

#### Parte iii) Potencial electrostático en el centro $r = 0$

La diferencia de potencial entre el centro $r = 0$ y el infinito se obtiene mediante la integral de línea del campo eléctrico:
$$\Delta V = V_0 - V_\infty = -\int_\infty^0 \vec{E}\cdot d\vec{\ell} \qquad \text{(0.5 pts)}$$

Considerando la referencia $V_\infty = 0$ y una trayectoria radial ($d\vec{\ell} = dr\,\hat{r}$), separamos la integral en las tres regiones del espacio:
$$V_0 = -\int_\infty^b E_3\,dr - \int_b^a E_2\,dr - \int_a^0 E_1\,dr \qquad \text{(0.5 pts)}$$

Sustituyendo $E_3 = \frac{2\beta a^{9/2}}{9\varepsilon_0 r^2}$, $E_2 = 0$ y $E_1 = \frac{2\beta r^{5/2}}{9\varepsilon_0}$:
$$V_0 = -\int_\infty^b \frac{2\beta a^{9/2}}{9\varepsilon_0 r^2}\,dr - \int_a^0 \frac{2\beta r^{5/2}}{9\varepsilon_0}\,dr$$
$$V_0 = -\frac{2\beta}{9\varepsilon_0}\left[a^{9/2}\int_\infty^b \frac{dr}{r^2} + \int_a^0 r^{5/2}\,dr\right]$$
$$V_0 = -\frac{2\beta}{9\varepsilon_0}\left[a^{9/2}\left.\left(-\frac{1}{r}\right)\right|_\infty^b + \left.\left(\frac{2r^{7/2}}{7}\right)\right|_a^0\right]$$
$$V_0 = -\frac{2\beta}{9\varepsilon_0}\left[a^{9/2}\left(-\frac{1}{b} - 0\right) + \left(0 - \frac{2a^{7/2}}{7}\right)\right]$$
$$V_0 = \frac{2\beta}{9\varepsilon_0}\left[\frac{a^{9/2}}{b} + \frac{2a^{7/2}}{7}\right] \qquad \text{(1 pto)}$$

$$\boxed{V_0 = \frac{2\beta}{9\varepsilon_0}\left(\frac{a^{9/2}}{b} + \frac{2a^{7/2}}{7}\right)}$$

**Verificación:**
- **Condiciones de frontera sobre el conductor:** El salto del campo radial al cruzar $r = a$ es $E(a^+) - E(a^-) = 0 - \frac{2\beta a^{5/2}}{9\varepsilon_0} = \frac{\sigma_{\text{int}}}{\varepsilon_0}$, y al cruzar $r = b$ es $E(b^+) - E(b^-) = \frac{2\beta a^{9/2}}{9\varepsilon_0 b^2} - 0 = \frac{\sigma_{\text{ext}}}{\varepsilon_0}$, cumpliendo exactamente la condición de discontinuidad $\Delta E_n = \sigma/\varepsilon_0$.
- **Unidades:** $[\rho] = \text{C}/\text{m}^3 \implies [\beta] = \text{C}/\text{m}^{9/2}$. Entonces $[\sigma_{\text{int}}] = [\beta a^{5/2}] = \text{C}/\text{m}^2$, $[E] = [\beta a^{5/2}/\varepsilon_0] = (\text{C}/\text{m}^2)/(\text{C}^2/(\text{N}\cdot\text{m}^2)) = \text{N}/\text{C}$, y $[V_0] = [E \cdot a] = \text{N}\cdot\text{m}/\text{C} = \text{V}$. Todo es dimensionalmente consistente.
- **Límite $b \to a^+$ (cascarón de espesor despreciable):** $V_0 \to \frac{2\beta a^{7/2}}{9\varepsilon_0}\left(1 + \frac{2}{7}\right) = \frac{2\beta a^{7/2}}{7\varepsilon_0}$, que corresponde exactamente al potencial en el centro de una esfera aislante aislada con $\rho(r) = \beta r^{3/2}$.

---

## Resumen de resultados

| Problema | Parte | Región / Cantidad | Resultado |
| :--- | :--- | :--- | :--- |
| **Problema 1** | i) Campo eléctrico | $r < a$ | $\vec{E}_1 = \dfrac{2\beta r^{5/2}}{9\varepsilon_0}\,\hat{r}$ |
| | i) Campo eléctrico | $a < r < b$ | $\vec{E}_2 = \vec{0}$ |
| | i) Campo eléctrico | $r > b$ | $\vec{E}_3 = \dfrac{2\beta a^{9/2}}{9\varepsilon_0 r^2}\,\hat{r}$ |
| | ii) Densidad superficial interna | $r = a$ | $\sigma_{\text{int}} = -\dfrac{2\beta a^{5/2}}{9}$ |
| | ii) Densidad superficial externa | $r = b$ | $\sigma_{\text{ext}} = \dfrac{2\beta a^{9/2}}{9b^2}$ |
| | iii) Potencial en el centro | $r = 0$ (con $V_\infty = 0$) | $V_0 = \dfrac{2\beta}{9\varepsilon_0}\left(\dfrac{a^{9/2}}{b} + \dfrac{2a^{7/2}}{7}\right)$ |
