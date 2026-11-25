# Ayudantía 05 — Ley de Gauss

> Clases relacionadas: [Clase 03 - Distribuciones continuas y Gauss](../../Clases/markdown/Clase%2003%20-%20Distribuciones%20continuas%20y%20Gauss.md), [Clase 04 - Calculo y Gauss diferencial](../../Clases/markdown/Clase%2004%20-%20Calculo%20y%20Gauss%20diferencial.md)

---

## Problema 1

Un cilindro infinito de radio $R$ tiene su eje coincidente con el eje $z$. El cilindro posee una densidad volumétrica $\rho(r) = r/a$ donde $a$ es una constante positiva y $r$ es la distancia desde el eje del cilindro.

a) Calcule la carga contenida en un cilindro centrado en el eje $z$, de radio $r$ y altura $h$ para los casos $r < R$ y $r > R$.  
b) Determine el campo eléctrico $\vec{E}(\vec{r})$ en todo el espacio.

> **[Figura]:** Cilindro vertical infinito de radio $R$ centrado en el eje vertical $z$. La línea discontinua a lo largo del eje central representa el eje de simetría $z$. En el interior del cilindro se indica la ley para la densidad volumétrica de carga $\rho(r) = r/a$, la cual crece linealmente con la distancia radial $r$ al eje $z$. Una cota horizontal en la base señala el radio exterior $R$.

### Solución

**Idea:** Para la parte a), integrar la densidad volumétrica de carga diferencial $dq = \rho(r)\,dV$ en coordenadas cilíndricas sobre un volumen cilíndrico coaxial de radio $r$ y altura $h$. Para la parte b), aprovechar la simetría cilíndrica e invariancia longitudinal y azimutal del sistema para aplicar la ley de Gauss mediante una superficie cerrada cilíndrica coaxial de radio $r$ y altura $h$.

#### Parte a) Carga contenida en un cilindro de radio $r$ y altura $h$

La carga total encerrada en un volumen $V$ se define como:
$$Q_{\text{enc}} = \iiint_V \rho(\vec{r}')\,dV'$$

Trabajando en coordenadas cilíndricas $(r', \theta, z)$, el elemento diferencial de volumen es:
$$dV' = r'\,dr'\,d\theta\,dz$$

Los límites de integración para la altura y el ángulo azimutal son $z \in [0, h]$ y $\theta \in [0, 2\pi]$.

1. **Caso $r \le R$ (interior del cilindro):**  
   Toda la región de integración está dentro del cilindro cargado, donde $\rho(r') = r'/a$:
   $$Q_{\text{enc}}(r \le R) = \int_0^h dz \int_0^{2\pi} d\theta \int_0^r \left(\frac{r'}{a}\right) r'\,dr'$$
   $$Q_{\text{enc}}(r \le R) = h \cdot (2\pi) \cdot \frac{1}{a} \int_0^r {r'}^2\,dr' = \frac{2\pi h}{a} \left[\frac{{r'}^3}{3}\right]_0^r$$
   $$\boxed{Q_{\text{enc}}(r \le R) = \frac{2\pi h r^3}{3a}}$$

2. **Caso $r > R$ (exterior del cilindro):**  
   Dado que para $r' > R$ no existe carga eléctrica ($\rho(r') = 0$), la carga encerrada por el cilindro gaussiano corresponde a la carga total contenida hasta el radio físico $R$:
   $$Q_{\text{enc}}(r > R) = \int_0^h dz \int_0^{2\pi} d\theta \int_0^R \left(\frac{r'}{a}\right) r'\,dr'$$
   $$Q_{\text{enc}}(r > R) = \frac{2\pi h}{a} \left[\frac{{r'}^3}{3}\right]_0^R$$
   $$\boxed{Q_{\text{enc}}(r > R) = \frac{2\pi h R^3}{3a}}$$

---

#### Parte b) Campo eléctrico $\vec{E}(\vec{r})$ en todo el espacio

Por simetría cilíndrica:
- Invariancia bajo traslaciones a lo largo del eje $z$: $\vec{E}$ no depende de $z$.
- Invariancia bajo rotaciones respecto al eje $z$: $\vec{E}$ no depende de $\theta$.
- Por reflexión en planos perpendiculares al eje $z$ y planos que contienen al eje $z$, el campo no puede tener componentes en $\hat{z}$ ni en $\hat{\theta}$.

Por lo tanto, el campo eléctrico es puramente radial y solo depende de la distancia radial $r$:
$$\vec{E}(\vec{r}) = E(r)\,\hat{r}$$

Consideramos una superficie gaussiana cilíndrica de radio $r$, altura $h$ y coaxial con el eje $z$. El flujo del campo eléctrico a través de esta superficie cerrada se compone del flujo por el manto lateral y por las dos tapas planas:
$$\oint_S \vec{E}\cdot d\vec{A} = \int_{\text{manto}} \vec{E}\cdot d\vec{A} + \int_{\text{tapa sup}} \vec{E}\cdot d\vec{A} + \int_{\text{tapa inf}} \vec{E}\cdot d\vec{A}$$

- En las tapas superior e inferior, el vector normal de área apunta en $\pm\hat{z}$, de modo que $\vec{E}\cdot d\vec{A} \propto \hat{r}\cdot\hat{z} = 0$. Las tapas no aportan al flujo.
- En el manto lateral, el vector de área apunta en $\hat{r}$ ($d\vec{A} = dA\,\hat{r}$), con lo cual $\vec{E}\cdot d\vec{A} = E(r)\,dA$. Como $E(r)$ es constante sobre el manto:
$$\oint_S \vec{E}\cdot d\vec{A} = E(r) \int_{\text{manto}} dA = E(r) \cdot (2\pi r h)$$

Por la ley de Gauss:
$$\oint_S \vec{E}\cdot d\vec{A} = \frac{Q_{\text{enc}}}{\varepsilon_0} \implies E(r) \cdot 2\pi r h = \frac{Q_{\text{enc}}}{\varepsilon_0}$$

1. **Región interior ($r \le R$):**
   $$E(r) \cdot 2\pi r h = \frac{1}{\varepsilon_0}\left(\frac{2\pi h r^3}{3a}\right)$$
   Cancelando el factor común $2\pi h$:
   $$E(r) \cdot r = \frac{r^3}{3a\varepsilon_0} \implies E(r) = \frac{r^2}{3a\varepsilon_0}$$
   $$\boxed{\vec{E}(\vec{r}) = \frac{r^2}{3a\varepsilon_0}\,\hat{r} \qquad (r \le R)}$$

2. **Región exterior ($r > R$):**
   $$E(r) \cdot 2\pi r h = \frac{1}{\varepsilon_0}\left(\frac{2\pi h R^3}{3a}\right)$$
   Cancelando $2\pi h$:
   $$E(r) \cdot r = \frac{R^3}{3a\varepsilon_0} \implies E(r) = \frac{R^3}{3a\varepsilon_0 r}$$
   $$\boxed{\vec{E}(\vec{r}) = \frac{R^3}{3a\varepsilon_0 r}\,\hat{r} \qquad (r > R)}$$

**Verificación:**
- **Continuidad en la interfaz:** Evaluando en la frontera $r = R$:
  $$E(R^-) = \frac{R^2}{3a\varepsilon_0}, \qquad E(R^+) = \frac{R^3}{3a\varepsilon_0 R} = \frac{R^2}{3a\varepsilon_0}$$
  El campo es continuo en $r = R$, lo cual es físicamente correcto ya que no existe densidad superficial de carga en la superficie del cilindro.
- **Comportamiento asintótico:** Para $r \to 0$, $E \propto r^2 \to 0$, nulo en el eje como exige la simetría. Para $r \gg R$, $E \propto 1/r$, equivalente al campo de una línea infinita con densidad lineal efectiva $\lambda = Q_{\text{enc}}/h = \frac{2\pi R^3}{3a}$, para la cual $E = \frac{\lambda}{2\pi\varepsilon_0 r} = \frac{R^3}{3a\varepsilon_0 r}$.
- **Unidades:** $[\rho] = \text{C}/\text{m}^3 \implies [a] = [r/\rho] = \text{m}^4/\text{C}$.  
  Luego $[r^2/(a\varepsilon_0)] = \text{m}^2 / [(\text{m}^4/\text{C}) \cdot (\text{C}^2/(\text{N}\cdot\text{m}^2))] = \text{N}/\text{C} = \text{V}/\text{m}$, consistente.

---

## Problema 2

El plano $xy$ (descrito por $z = 0$) está cubierto de una densidad de carga superficial $\sigma$ uniforme (es decir, una placa de espesor infinitesimal). Inmediatamente al lado positivo del eje $z$ hay una placa también infinita de espesor $a$ con carga eléctrica de densidad volumétrica $\rho$ uniforme en $0 < z < a$ (ver figura). Obtenga el campo eléctrico en todo el espacio.

> **[Figura]:** Plano infinito en dos dimensiones sobre el plano cartesiano $xy$ ($z=0$) que posee una densidad superficial de carga uniforme $\sigma$. Justo sobre su cara positiva ($z > 0$), se encuentra una losa o placa tridimensional de espesor constante $a$, paralela al plano $xy$, ocupando el rango $0 < z < a$, con densidad volumétrica de carga constante $\rho$. A la derecha se representa un corte transversal en el plano $xz$: el plano infinitesimal en $z=0$ y la placa de ancho $a$ rellena uniformemente de cargas positivas ($+$).

### Solución

**Idea:** Aplicar el principio de superposición para campos electrostáticos: $\vec{E}(\vec{r}) = \vec{E}_1(\vec{r}) + \vec{E}_2(\vec{r})$, donde $\vec{E}_1$ es el campo generado por el plano infinito cargado en $z=0$ y $\vec{E}_2$ es el campo generado por la losa de espesor $a$ con carga volumétrica uniforme $\rho$. Ambos campos se obtienen mediante la ley de Gauss aprovechando la simetría planar.

#### 1. Campo del plano infinito en $z = 0$ ($\vec{E}_1$)

Para un plano infinito con densidad superficial uniforme $\sigma$, el campo eléctrico debe ser perpendicular al plano por simetría, apuntando alejándose del plano si $\sigma > 0$:
$$\vec{E}_1(z) = E_1(z)\,\hat{z}$$

Tomamos un cilindro gaussiano con eje perpendicular al plano (paralelo a $z$), cuyas tapas de área $A$ se encuentran simétricamente a distancias $+z$ y $-z$ respecto al plano:
- Flujo por las dos tapas: $\Phi_E = E_1 A + E_1 A = 2 E_1 A$.
- Flujo por la pared lateral: $\vec{E}_1 \cdot d\vec{A} = 0$, nulo.
- Carga encerrada: $Q_{\text{enc}} = \sigma A$.

Por ley de Gauss:
$$2 E_1 A = \frac{\sigma A}{\varepsilon_0} \implies E_1 = \frac{\sigma}{2\varepsilon_0}$$

Expresado vectorialmente en todo el espacio:
$$\vec{E}_1(z) = \begin{cases} +\dfrac{\sigma}{2\varepsilon_0}\,\hat{z}, & z > 0 \\ -\dfrac{\sigma}{2\varepsilon_0}\,\hat{z}, & z < 0 \end{cases}$$

---

#### 2. Campo de la placa de espesor $a$ con densidad $\rho$ ($\vec{E}_2$)

La losa ocupa la región $0 < z < a$. Su plano central de simetría se encuentra en $z_c = a/2$.  
Por simetría planar respecto al plano $z = a/2$, el campo apunta hacia $+z$ para $z > a/2$ y hacia $-z$ para $z < a/2$.

Definimos una superficie cilíndrica gaussiana de tapas de área $A$, centrada en $z = a/2$ y de longitud total $L$ en la dirección $z$, de modo que sus tapas están ubicadas a igual distancia del plano medio: en $z = a/2 + L/2$ y en $z = a/2 - L/2$.

El flujo neto a través de las dos tapas es:
$$\oint_S \vec{E}_2\cdot d\vec{A} = 2 E_2 A$$

Distinguimos dos casos según si el punto de observación está fuera o dentro de la placa:

1. **Fuera de la placa ($L > a$, es decir, $z > a$ o $z < 0$):**  
   La superficie gaussiana encierra todo el espesor de la placa en el área $A$:
   $$Q_{\text{enc}} = \rho \cdot (A \cdot a)$$
   Aplicando la ley de Gauss:
   $$2 E_2 A = \frac{\rho a A}{\varepsilon_0} \implies E_2 = \frac{\rho a}{2\varepsilon_0}$$
   Tomando en cuenta la orientación simétrica respecto al plano medio $z = a/2$:
   $$\vec{E}_2(z) = \begin{cases} +\dfrac{\rho a}{2\varepsilon_0}\,\hat{z}, & z > a \\ -\dfrac{\rho a}{2\varepsilon_0}\,\hat{z}, & z < 0 \end{cases}$$

2. **Interior de la placa ($L < a$, es decir, $0 < z < a$):**  
   Las tapas del cilindro gaussiano se encuentran dentro del material conductor/dieléctrico, a una distancia $|z - a/2|$ a ambos lados del plano medio. Por tanto, la longitud del cilindro es $L = 2|z - a/2|$, y el volumen cargado encerrado es $A \cdot L = 2 A |z - a/2|$:
   $$Q_{\text{enc}} = \rho A L = 2 \rho A \left|z - \frac{a}{2}\right|$$
   Aplicando la ley de Gauss:
   $$2 E_2 A = \frac{2\rho A |z - a/2|}{\varepsilon_0} \implies E_2 = \frac{\rho |z - a/2|}{\varepsilon_0}$$
   Considerando el signo y sentido del campo:
   - Para $\frac{a}{2} < z < a$: el campo apunta en $+\hat{z}$, con magnitud $\frac{\rho(z - a/2)}{\varepsilon_0} = \frac{\rho(2z - a)}{2\varepsilon_0}$.
   - Para $0 < z < \frac{a}{2}$: el campo apunta en $-\hat{z}$, con magnitud $\frac{\rho(a/2 - z)}{\varepsilon_0}$, es decir, $\vec{E}_2 = -\frac{\rho(a - 2z)}{2\varepsilon_0}\,\hat{z} = \frac{\rho(2z - a)}{2\varepsilon_0}\,\hat{z}$.

   De forma compacta y unificada para todo el interior $0 < z < a$:
   $$\vec{E}_2(z) = \frac{\rho(2z - a)}{2\varepsilon_0}\,\hat{z} = \frac{\rho\left(z - \frac{a}{2}\right)}{\varepsilon_0}\,\hat{z}$$

---

#### 3. Campo eléctrico total por superposición

Sumando vectorialmente ambas contribuciones, $\vec{E}_{\text{total}}(z) = \vec{E}_1(z) + \vec{E}_2(z)$, en las tres regiones del espacio:

1. **Para $z < 0$:**
   $$\vec{E}(z) = \left(-\frac{\sigma}{2\varepsilon_0} - \frac{\rho a}{2\varepsilon_0}\right)\hat{z}$$
   $$\boxed{\vec{E}(z) = -\frac{\sigma + \rho a}{2\varepsilon_0}\,\hat{z} \qquad (z < 0)}$$

2. **Para $0 < z < a$:**
   $$\vec{E}(z) = \left(\frac{\sigma}{2\varepsilon_0} + \frac{\rho(2z - a)}{2\varepsilon_0}\right)\hat{z}$$
   $$\boxed{\vec{E}(z) = \frac{\sigma + \rho(2z - a)}{2\varepsilon_0}\,\hat{z} \qquad (0 < z < a)}$$

3. **Para $z > a$:**
   $$\vec{E}(z) = \left(\frac{\sigma}{2\varepsilon_0} + \frac{\rho a}{2\varepsilon_0}\right)\hat{z}$$
   $$\boxed{\vec{E}(z) = \frac{\sigma + \rho a}{2\varepsilon_0}\,\hat{z} \qquad (z > a)}$$

**Verificación:**
- **Condición de salto en $z = 0$:**
  $$\vec{E}(0^+) - \vec{E}(0^-) = \frac{\sigma - \rho a}{2\varepsilon_0}\,\hat{z} - \left(-\frac{\sigma + \rho a}{2\varepsilon_0}\right)\hat{z} = \frac{\sigma}{\varepsilon_0}\,\hat{z}$$
  La discontinuidad del campo eléctrico en $z = 0$ es exactamente $\sigma / \varepsilon_0$, en total concordancia con la condición de borde electrostática para densidades superficiales.
- **Continuidad en $z = a$:**
  $$\vec{E}(a^-) = \frac{\sigma + \rho a}{2\varepsilon_0}\,\hat{z}, \qquad \vec{E}(a^+) = \frac{\sigma + \rho a}{2\varepsilon_0}\,\hat{z}$$
  El campo es continuo en $z = a$, tal como corresponde debido a la ausencia de carga superficial en esa interfaz.

---

## Problema 3

Considere dos cilindros infinitos de radios $R_0$ los cuales poseen sus ejes paralelos al eje $z$ (entran y salen de la hoja de papel). Las densidades de carga volumétricas de los cilindros son $\rho$ y $-\rho$ y sus ejes centrales pasan por los puntos $(x_0, 0)$ y $(-x_0, 0)$, respectivamente. Considerando que $x_0 < R_0$.

a) Determine el campo eléctrico en la zona de intersección.

> **[Figura]:** Sección transversal en el plano $xy$. Se observan dos circunferencias secantes de idéntico radio $R_0$. El cilindro de la izquierda está centrado en $(-x_0, 0)$ y porta una densidad volumétrica de carga uniforme $-\rho$. El cilindro de la derecha está centrado en $(x_0, 0)$ y porta una densidad volumétrica de carga uniforme $+\rho$. La separación entre centros es $2x_0 < 2R_0$. La zona de intersección es una región en forma de lente biconvexa simétrica respecto al eje $y$. En un punto interior arbitrario se indican los vectores de posición $\vec{r}_1$ (desde el centro del cilindro 1) y $\vec{r}_2$ (desde el centro del cilindro 2).

### Solución

**Idea:** Determinar primero la expresión vectorial del campo electrostático en el interior de un cilindro infinito uniforme mediante la ley de Gauss. Luego, calcular el campo en la región de intersección sumando por superposición los campos creados por ambos cilindros cargados, expresando adecuadamente los vectores de posición respecto a sus respectivos ejes de simetría.

#### 1. Campo en el interior de un cilindro infinito cargado

Consideremos un cilindro infinito aislado con densidad volumétrica constante $\rho$.  
Por simetría cilíndrica, a una distancia radial $r$ de su eje central, el campo eléctrico es puramente radial: $\vec{E} = E(r)\,\hat{r}$.

Aplicamos la ley de Gauss sobre un cilindro coaxial de radio $r < R_0$ y altura $h$:
$$\oint_S \vec{E}\cdot d\vec{A} = E(r) \cdot 2\pi r h$$

La carga encerrada en dicho volumen cilíndrico de radio $r$ es:
$$Q_{\text{enc}} = \rho \cdot (\pi r^2 h)$$

Igualando por la ley de Gauss:
$$E(r) \cdot 2\pi r h = \frac{\rho \pi r^2 h}{\varepsilon_0} \implies E(r) = \frac{\rho r}{2\varepsilon_0}$$

Expresado en forma vectorial, donde $\vec{r} = r\,\hat{r}$ es el vector posición relativo al eje del cilindro medido en el plano perpendicular al eje:
$$\vec{E}_{\text{int}}(\vec{r}) = \frac{\rho}{2\varepsilon_0}\,\vec{r}$$

---

#### 2. Superposición de los dos cilindros en la zona de intersección

Sean:
- **Cilindro 1:** densidad de carga volumétrica $-\rho$, con su eje pasando por el punto $(-x_0, 0, 0)$.
- **Cilindro 2:** densidad de carga volumétrica $+\rho$, con su eje pasando por el punto $(x_0, 0, 0)$.

Sea $P = (x, y)$ un punto cualquiera situado en la zona de intersección de ambos cilindros (donde $r_1 < R_0$ y $r_2 < R_0$).  
Los vectores que van desde el centro de cada cilindro hasta el punto $P$ son:
$$\vec{r}_1 = (x - (-x_0))\,\hat{x} + y\,\hat{y} = (x + x_0)\,\hat{x} + y\,\hat{y}$$
$$\vec{r}_2 = (x - x_0)\,\hat{x} + y\,\hat{y}$$

Notamos inmediatamente la relación vectorial entre ambos centros y el punto:
$$\vec{r}_1 - \vec{r}_2 = [(x + x_0)\,\hat{x} + y\,\hat{y}] - [(x - x_0)\,\hat{x} + y\,\hat{y}] = 2x_0\,\hat{x}$$

El campo electrostático generado por el cilindro 1 en $P$ es:
$$\vec{E}_1 = \frac{-\rho}{2\varepsilon_0}\,\vec{r}_1$$

El campo electrostático generado por el cilindro 2 en $P$ es:
$$\vec{E}_2 = \frac{\rho}{2\varepsilon_0}\,\vec{r}_2$$

Por el principio de superposición, el campo total en dicho punto de la intersección es:
$$\vec{E} = \vec{E}_1 + \vec{E}_2 = \frac{-\rho}{2\varepsilon_0}\,\vec{r}_1 + \frac{\rho}{2\varepsilon_0}\,\vec{r}_2 = \frac{\rho}{2\varepsilon_0}\left(-\vec{r}_1 + \vec{r}_2\right)$$

Sustituyendo $-\vec{r}_1 + \vec{r}_2 = -(\vec{r}_1 - \vec{r}_2) = -2x_0\,\hat{x}$:
$$\vec{E} = \frac{\rho}{2\varepsilon_0}\left(-2x_0\,\hat{x}\right)$$

$$\boxed{\vec{E} = -\frac{\rho x_0}{\varepsilon_0}\,\hat{x}}$$

**Verificación:**
- **Uniformidad:** El campo resultante no depende de $x$ ni de $y$; es estrictamente constante y homogéneo en toda la región de intersección.
- **Sentido físico:** El cilindro de la derecha posee carga positiva $+\rho$, por lo que en los puntos a su izquierda (la región de traslape) su campo apunta hacia la izquierda ($-\hat{x}$). El cilindro de la izquierda posee carga negativa $-\rho$, por lo que atrae hacia su eje (hacia la izquierda, $-\hat{x}$). Ambas contribuciones se suman constructivamente apuntando hacia $-\hat{x}$, confirmando el signo obtenido.
- **Límite $x_0 \to 0$:** Si los centros coinciden ($x_0 = 0$), las densidades $+\rho$ y $-\rho$ se anulan exactamente en todo el volumen común, resultando en un campo nulo $\vec{E} = 0$, consistente con la fórmula.

---

## Resumen de resultados

| Problema | Parte | Parámetro / Condición | Resultado |
| :--- | :--- | :--- | :--- |
| **Problema 1** | a) Carga encerrada | $r \le R$ | $Q_{\text{enc}} = \dfrac{2\pi h r^3}{3a}$ |
| | a) Carga encerrada | $r > R$ | $Q_{\text{enc}} = \dfrac{2\pi h R^3}{3a}$ |
| | b) Campo eléctrico | $r \le R$ | $\vec{E}(\vec{r}) = \dfrac{r^2}{3a\varepsilon_0}\,\hat{r}$ |
| | b) Campo eléctrico | $r > R$ | $\vec{E}(\vec{r}) = \dfrac{R^3}{3a\varepsilon_0 r}\,\hat{r}$ |
| **Problema 2** | Campo eléctrico total | $z < 0$ | $\vec{E}(z) = -\dfrac{\sigma + \rho a}{2\varepsilon_0}\,\hat{z}$ |
| | Campo eléctrico total | $0 < z < a$ | $\vec{E}(z) = \dfrac{\sigma + \rho(2z - a)}{2\varepsilon_0}\,\hat{z}$ |
| | Campo eléctrico total | $z > a$ | $\vec{E}(z) = \dfrac{\sigma + \rho a}{2\varepsilon_0}\,\hat{z}$ |
| **Problema 3** | a) Campo en intersección | Región de traslape ($x_0 < R_0$) | $\vec{E} = -\dfrac{\rho x_0}{\varepsilon_0}\,\hat{x}$ (campo uniforme) |
