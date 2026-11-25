# Ayudantía 03 — Distribuciones continuas de carga

> Clases relacionadas: [Clase 02 - Carga eléctrica, ley de Coulomb, Campo eléctrico](../../Clases/markdown/Clase%2002%20-%20Carga%20el%C3%A9ctrica%2C%20ley%20de%20Coulomb%2C%20Campo%20el%C3%A9ctrico.md), [Clase 03 - Distribuciones continuas y Gauss](../../Clases/markdown/Clase%2003%20-%20Distribuciones%20continuas%20y%20Gauss.md)

---

## Problema 1

Un alambre infinito con densidad lineal de carga $\lambda$ se dobla en forma de horquilla como se muestra en la figura. Determine el campo eléctrico en el centro del sistema de referencia generado por:

a) Las porciones rectas vertical y horizontal.  
b) La porción de curva de radio $R$ (un cuarto de circunferencia).  
c) El alambre completo. Además, calcule la magnitud del campo eléctrico total.

> **[Figura]:** Plano cartesiano $xy$ con el origen $(0, 0)$ en el centro. El alambre cargado con densidad uniforme $\lambda$ se divide en tres secciones continuas:
> 1. Una porción recta vertical semi-infinita ubicada sobre la recta $x = -R$, que se extiende desde $y = 0$ hasta $y \to +\infty$.
> 2. Un cuarto de circunferencia de radio $R$ ubicado en el tercer cuadrante, que conecta el punto $(-R, 0)$ con el punto $(0, -R)$, con centro de curvatura en el origen $(0, 0)$.
> 3. Una porción recta horizontal semi-infinita ubicada sobre la recta $y = -R$, que se extiende desde $x = 0$ hasta $x \to +\infty$.
> El punto donde se calcula el campo electrostático es el origen de coordenadas $(0, 0)$.

### Solución

**Idea:** Para una distribución continua de carga lineal, el campo eléctrico en una posición $\vec{r}$ viene dado por la integral de Coulomb:

$$\vec{E} = \frac{1}{4\pi\varepsilon_0} \int \frac{\vec{r} - \vec{r}'}{\|\vec{r} - \vec{r}'\|^3} \, dq = k \int \frac{\vec{r} - \vec{r}'}{\|\vec{r} - \vec{r}'\|^3} \, \lambda \, dl$$

Donde $\vec{r} = \vec{0}$ es el origen de coordenadas, $\vec{r}'$ es la posición de cada elemento diferencial de carga $dq = \lambda\,dl$, y $k = \frac{1}{4\pi\varepsilon_0}$. Se resuelve por superposición calculando por separado las dos ramas rectas y el arco circular.

---

#### Parte a) Porciones rectas vertical y horizontal

##### 1. Porción recta vertical

- **Densidad de carga y elemento de longitud:**
  $$dq = \lambda\,dl = \lambda\,dy, \qquad y \in [0, \infty)$$
- **Vector de posición de la fuente $\vec{r}'$ y vector relativo:**
  $$\vec{r}' = -R\,\hat{x} + y\,\hat{y}$$
  $$\vec{r} - \vec{r}' = \vec{0} - (-R\,\hat{x} + y\,\hat{y}) = R\,\hat{x} - y\,\hat{y}$$
- **Distancia al cubo:**
  $$\|\vec{r} - \vec{r}'\| = \sqrt{R^2 + y^2} \implies \|\vec{r} - \vec{r}'\|^3 = (R^2 + y^2)^{3/2}$$

El campo electrostático $\vec{E}_1$ generado por el alambre vertical es:
$$\vec{E}_1 = k\lambda \int_0^\infty \frac{R\,\hat{x} - y\,\hat{y}}{(R^2 + y^2)^{3/2}}\,dy = k\lambda \left( \hat{x} \int_0^\infty \frac{R}{(R^2 + y^2)^{3/2}}\,dy - \hat{y} \int_0^\infty \frac{y}{(R^2 + y^2)^{3/2}}\,dy \right)$$

Evaluamos ambas integrales:
1. **Componente en $\hat{x}$:**  
   Mediante la sustitución trigonométrica $y = R\tan\theta \implies dy = R\sec^2\theta\,d\theta$, con límites $\theta \in [0, \pi/2]$:
   $$\int_0^\infty \frac{R}{(R^2 + y^2)^{3/2}}\,dy = \int_0^{\pi/2} \frac{R \cdot R\sec^2\theta}{(R^2\sec^2\theta)^{3/2}}\,d\theta = \frac{1}{R} \int_0^{\pi/2} \cos\theta\,d\theta = \frac{1}{R} [\sin\theta]_0^{\pi/2} = \frac{1}{R}$$

2. **Componente en $\hat{y}$:**  
   Mediante la sustitución simple $u = R^2 + y^2 \implies du = 2y\,dy$, con límites $u \in [R^2, \infty)$:
   $$\int_0^\infty \frac{y}{(R^2 + y^2)^{3/2}}\,dy = \frac{1}{2} \int_{R^2}^\infty u^{-3/2}\,du = \frac{1}{2} \left[ -2 u^{-1/2} \right]_{R^2}^\infty = 0 - \left( -\frac{1}{R} \right) = \frac{1}{R}$$

Reuniendo las componentes:
$$\vec{E}_1 = \frac{k\lambda}{R} (\hat{x} - \hat{y}) = \frac{\lambda}{4\pi\varepsilon_0 R} (\hat{x} - \hat{y})$$

---

##### 2. Porción recta horizontal

- **Densidad de carga y elemento de longitud:**
  $$dq = \lambda\,dl = \lambda\,dx, \qquad x \in [0, \infty)$$
- **Vector de posición de la fuente $\vec{r}'$ y vector relativo:**
  $$\vec{r}' = x\,\hat{x} - R\,\hat{y}$$
  $$\vec{r} - \vec{r}' = \vec{0} - (x\,\hat{x} - R\,\hat{y}) = -x\,\hat{x} + R\,\hat{y}$$
- **Distancia al cubo:**
  $$\|\vec{r} - \vec{r}'\|^3 = (x^2 + R^2)^{3/2}$$

El campo electrostático $\vec{E}_2$ generado por el alambre horizontal es:
$$\vec{E}_2 = k\lambda \int_0^\infty \frac{-x\,\hat{x} + R\,\hat{y}}{(x^2 + R^2)^{3/2}}\,dx = k\lambda \left( -\hat{x} \int_0^\infty \frac{x}{(x^2 + R^2)^{3/2}}\,dx + \hat{y} \int_0^\infty \frac{R}{(x^2 + R^2)^{3/2}}\,dx \right)$$

Las integrales son idénticas a las resueltas para el alambre vertical:
$$\vec{E}_2 = k\lambda \left( -\frac{1}{R}\,\hat{x} + \frac{1}{R}\,\hat{y} \right) = -\frac{k\lambda}{R}(\hat{x} - \hat{y}) = \frac{\lambda}{4\pi\varepsilon_0 R}(-\hat{x} + \hat{y})$$

Nótese que la contribución neta combinada de ambas ramas rectas es:
$$\vec{E}_{\text{rectas}} = \vec{E}_1 + \vec{E}_2 = \frac{k\lambda}{R}(\hat{x} - \hat{y}) - \frac{k\lambda}{R}(\hat{x} - \hat{y}) = \vec{0}$$

$$\boxed{\vec{E}_{\text{vertical}} = \frac{\lambda}{4\pi\varepsilon_0 R}(\hat{x} - \hat{y}), \qquad \vec{E}_{\text{horizontal}} = \frac{\lambda}{4\pi\varepsilon_0 R}(-\hat{x} + \hat{y})}$$

---

#### Parte b) Porción de curva de radio $R$

La curva es un cuarto de circunferencia de radio $R$ centrado en el origen, contenido en el tercer cuadrante:
- **Parametrización polar:** $\theta \in [\pi, 3\pi/2]$ en sentido antihorario.
- **Elemento de longitud y carga:**
  $$dl = R\,d\theta \implies dq = \lambda R\,d\theta$$
- **Posición del diferencial:**
  $$\vec{r}' = R\cos\theta\,\hat{x} + R\sin\theta\,\hat{y}$$
  $$\vec{r} - \vec{r}' = -R(\cos\theta\,\hat{x} + \sin\theta\,\hat{y})$$
- **Distancia:**
  $$\|\vec{r} - \vec{r}'\| = R \implies \|\vec{r} - \vec{r}'\|^3 = R^3$$

El campo $\vec{E}_3$ generado por el arco circular es:
$$\vec{E}_3 = k \int_\pi^{3\pi/2} \frac{-R(\cos\theta\,\hat{x} + \sin\theta\,\hat{y})}{R^3} \, (\lambda R\,d\theta) = -\frac{k\lambda}{R} \int_\pi^{3\pi/2} (\cos\theta\,\hat{x} + \sin\theta\,\hat{y})\,d\theta$$

Evaluando cada integral trigonométrica:
$$\int_\pi^{3\pi/2} \cos\theta\,d\theta = [\sin\theta]_\pi^{3\pi/2} = \sin\left(\frac{3\pi}{2}\right) - \sin(\pi) = -1 - 0 = -1$$
$$\int_\pi^{3\pi/2} \sin\theta\,d\theta = [-\cos\theta]_\pi^{3\pi/2} = -\cos\left(\frac{3\pi}{2}\right) - (-\cos(\pi)) = 0 - (1) = -1$$

Sustituyendo los resultados:
$$\vec{E}_3 = -\frac{k\lambda}{R} \left( (-1)\,\hat{x} + (-1)\,\hat{y} \right) = \frac{k\lambda}{R} (\hat{x} + \hat{y})$$

$$\boxed{\vec{E}_{\text{curva}} = \frac{\lambda}{4\pi\varepsilon_0 R}(\hat{x} + \hat{y})}$$

---

#### Parte c) Alambre completo y magnitud

Sumando las tres contribuciones por el principio de superposición:
$$\vec{E}_T = \vec{E}_1 + \vec{E}_2 + \vec{E}_3 = \vec{0} + \vec{E}_3 = \frac{\lambda}{4\pi\varepsilon_0 R}(\hat{x} + \hat{y})$$

La magnitud del campo eléctrico total es:
$$\|\vec{E}_T\| = \frac{\lambda}{4\pi\varepsilon_0 R} \sqrt{1^2 + 1^2} = \frac{\sqrt{2}\lambda}{4\pi\varepsilon_0 R} = \frac{\sqrt{2}k\lambda}{R}$$

$$\boxed{\vec{E}_T = \frac{\lambda}{4\pi\varepsilon_0 R}(\hat{x} + \hat{y}), \qquad \|\vec{E}_T\| = \frac{\sqrt{2}\lambda}{4\pi\varepsilon_0 R}}$$

**Verificación:**
- **Dirección física:** El arco de carga positiva se encuentra en el tercer cuadrante ($x < 0, y < 0$). Al repeler una carga positiva de prueba colocada en el origen, el campo debe apuntar necesariamente en la dirección radial saliente hacia el primer cuadrante ($+\hat{x} + \hat{y}$), formando un ángulo de $45^\circ$, lo cual concuerda con la bisectriz del arco circular.
- **Unidades:** $[\lambda] / ([\varepsilon_0][R]) = (\text{C/m}) / ((\text{C}^2/(\text{N}\cdot\text{m}^2))\cdot\text{m}) = \text{N/C}$, consistente.

---

## Problema 2

Considere un plano infinito el cual tiene un agujero circular de radio $a$. Sobre el plano existe una densidad superficial de carga dada por $\sigma(r) = \sigma_0 a/r$ donde $r$ es la distancia desde el centro del agujero. A distancia $b$ bajo el plano existe una barra de largo $a$, masa $M$ y carga desconocida, la cual reposa inmóvil en esa posición a pesar de la gravedad. Suponiendo que la densidad de carga es uniforme en la barra, determine la carga que posee. Para esto:

a) Determine el campo eléctrico del plano en el eje del agujero.  
b) Escriba una expresión (integral) para determinar la fuerza que el plano ejerce sobre la barra.  
c) Haga el balance de fuerzas y concluya determinando la carga total de la barra.

> **Hint:**
> $$\int \frac{du}{(u^2+1)^{3/2}} = \frac{u}{\sqrt{u^2+1}} + C$$
> $$\int \frac{du}{u\sqrt{u^2+1}} = \ln\left( \frac{u}{\sqrt{u^2+1} + 1} \right) + C$$

> **[Figura]:** Plano infinito horizontal con un orificio circular de radio $a$ en su centro. El plano tiene densidad superficial no uniforme $\sigma(r) = \sigma_0 \frac{a}{r}$ para $r \ge a$. El eje $Z$ coincide con el eje de simetría perpendicular al plano que pasa por el centro del agujero, orientado hacia abajo ($+\hat{z}$). A una distancia $z = b$ bajo el plano comienza una barra delgada de longitud $a$ (ocupando el intervalo $z \in [b, b+a]$ sobre el eje $Z$), con masa $M$ y carga total $Q$ distribuida uniformemente. La gravedad $\vec{g} = g\,\hat{z}$ actúa hacia abajo. Para que la barra esté en equilibrio estático, la fuerza electrostática debe actuar hacia arriba (hacia el plano), compensando exactamente el peso.

### Solución

**Idea:** Calcular el campo eléctrico en el eje de simetría integrando anillos concéntricos de radio $r \ge a$. Luego, integrar la fuerza sobre los elementos diferenciales de carga $dq$ de la barra a lo largo de su longitud $z \in [b, b+a]$, y finalmente aplicar la primera ley de Newton ($\sum \vec{F} = \vec{0}$) para despejar la carga $Q$.

---

#### Parte a) Campo eléctrico del plano en el eje del agujero

Elegimos el origen en el centro del agujero:
- El plano cargado ocupa el plano perpendicular al eje $Z$, extendiéndose en coordenadas polares desde $r = a$ hasta $r \to \infty$ y $\phi \in [0, 2\pi]$.
- Definimos el eje $Z$ orientado hacia abajo (hacia la barra), de modo que un punto sobre el eje bajo el plano tiene coordenadas $\vec{r} = z\,\hat{z}$ (con $z > 0$).
- Un punto sobre el plano tiene vector de posición $\vec{r}' = r\cos\phi\,\hat{i} + r\sin\phi\,\hat{j} = r\,\hat{\rho}$.
- El vector relativo es:
  $$\vec{r} - \vec{r}' = z\,\hat{z} - r\,\hat{\rho}$$
  $$\|\vec{r} - \vec{r}'\|^3 = (z^2 + r^2)^{3/2}$$

El diferencial de carga en el plano es:
$$dq = \sigma(r)\,dA = \left( \sigma_0 \frac{a}{r} \right) (r\,d\phi\,dr) = \sigma_0 a\,d\phi\,dr$$

Por simetría azimutal en $\phi \in [0, 2\pi]$, la componente radial perpendicular al eje se anula:
$$\int_0^{2\pi} \hat{\rho}\,d\phi = \vec{0}$$

Por tanto, solo sobrevive la componente a lo largo del eje $Z$:
$$\vec{E}(z) = \frac{1}{4\pi\varepsilon_0} \int_{r=a}^\infty \int_{\phi=0}^{2\pi} \frac{z\,\hat{z}}{(z^2 + r^2)^{3/2}} (\sigma_0 a\,d\phi\,dr) = \frac{\sigma_0 a z}{4\pi\varepsilon_0} (2\pi) \hat{z} \int_a^\infty \frac{dr}{(z^2 + r^2)^{3/2}}$$

$$\vec{E}(z) = \frac{\sigma_0 a z}{2\varepsilon_0} \hat{z} \int_a^\infty \frac{dr}{(z^2 + r^2)^{3/2}}$$

Utilizando la sustitución $r = z u \implies dr = z du$, con límites $u \in [a/z, \infty)$:
$$\int_a^\infty \frac{dr}{(z^2 + r^2)^{3/2}} = \frac{1}{z^2} \int_{a/z}^\infty \frac{du}{(u^2 + 1)^{3/2}} = \frac{1}{z^2} \left[ \frac{u}{\sqrt{u^2 + 1}} \right]_{a/z}^\infty = \frac{1}{z^2} \left( 1 - \frac{a/z}{\sqrt{(a/z)^2 + 1}} \right) = \frac{1}{z^2} \left( 1 - \frac{a}{\sqrt{z^2 + a^2}} \right)$$

Sustituyendo en la expresión del campo:
$$\vec{E}(z) = \frac{\sigma_0 a z}{2\varepsilon_0} \left[ \frac{1}{z^2} \left( 1 - \frac{a}{\sqrt{z^2 + a^2}} \right) \right] \hat{z} = \frac{\sigma_0 a}{2\varepsilon_0 z} \left( 1 - \frac{a}{\sqrt{z^2 + a^2}} \right) \hat{z}$$

*(Si se toma el eje vertical habitual donde el eje apunta hacia el plano, el campo apunta alejándose del plano, con signo negativo en la coordenada de alejamiento).*

$$\boxed{\vec{E}(z) = \frac{\sigma_0 a}{2\varepsilon_0 z} \left( 1 - \frac{a}{\sqrt{z^2 + a^2}} \right) \hat{z}}$$

---

#### Parte b) Expresión integral de la fuerza sobre la barra

La barra tiene longitud $a$ y se extiende desde $z = b$ hasta $z = b + a$. Su carga total $Q$ está distribuida uniformemente:
$$\lambda = \frac{Q}{a} \implies dq = \lambda\,dz = \frac{Q}{a}\,dz$$

La fuerza electrostática total sobre la barra es:
$$\vec{F}_e = \int_{\text{barra}} \vec{E}(z)\,dq = \int_b^{b+a} \left[ \frac{\sigma_0 a}{2\varepsilon_0 z} \left( 1 - \frac{a}{\sqrt{z^2 + a^2}} \right) \hat{z} \right] \left( \frac{Q}{a}\,dz \right)$$

Simplificando el factor constante $a$:
$$\boxed{\vec{F}_e = \frac{\sigma_0 Q}{2\varepsilon_0} \hat{z} \int_b^{b+a} \left( \frac{1}{z} - \frac{a}{z\sqrt{z^2 + a^2}} \right) dz}$$

---

#### Parte c) Balance de fuerzas y determinación de $Q$

1. **Evaluación de la integral:**
   $$\int \left( \frac{1}{z} - \frac{a}{z\sqrt{z^2 + a^2}} \right) dz = \ln z - \int \frac{a}{z\sqrt{z^2 + a^2}}\,dz$$

   Para la segunda integral, usamos la sustitución $z = a u \implies dz = a\,du$:
   $$\int \frac{a\,dz}{z\sqrt{z^2 + a^2}} = \int \frac{du}{u\sqrt{u^2 + 1}}$$
   Aplicando el segundo hint:
   $$\int \frac{du}{u\sqrt{u^2 + 1}} = \ln\left( \frac{u}{\sqrt{u^2 + 1} + 1} \right) = \ln\left( \frac{z/a}{\sqrt{(z/a)^2 + 1} + 1} \right) = \ln\left( \frac{z}{\sqrt{z^2 + a^2} + a} \right) = \ln z - \ln\left( a + \sqrt{z^2 + a^2} \right)$$

   Restando ambas partes:
   $$\ln z - \left[ \ln z - \ln\left( a + \sqrt{z^2 + a^2} \right) \right] = \ln\left( a + \sqrt{z^2 + a^2} \right)$$

   Evaluando entre los límites $z = b$ y $z = b + a$:
   $$I = \left[ \ln\left( a + \sqrt{z^2 + a^2} \right) \right]_b^{b+a} = \ln\left( \frac{a + \sqrt{(a+b)^2 + a^2}}{a + \sqrt{b^2 + a^2}} \right)$$

2. **Condición de equilibrio:**
   La barra está en equilibrio estático bajo la acción de la gravedad hacia abajo ($\vec{F}_g = Mg\,\hat{z}$) y la fuerza electrostática $\vec{F}_e$:
   $$\sum \vec{F} = \vec{F}_e + \vec{F}_g = \vec{0} \implies \vec{F}_e = -Mg\,\hat{z}$$

   Como el plano tiene carga $\sigma_0 > 0$, el campo $\vec{E}$ apunta hacia abajo ($+\hat{z}$). Para que la fuerza eléctrica sea atractiva (hacia el plano, $-\hat{z}$) y contrarreste el peso, la barra debe poseer carga negativa ($Q < 0$):
   $$\frac{\sigma_0 Q}{2\varepsilon_0} \ln\left( \frac{a + \sqrt{(a+b)^2 + a^2}}{a + \sqrt{b^2 + a^2}} \right) = -Mg$$

   Despejando $Q$:
   $$Q = -\frac{2\varepsilon_0 Mg}{\sigma_0 \ln\left( \frac{a + \sqrt{(a+b)^2 + a^2}}{a + \sqrt{b^2 + a^2}} \right)}$$

   Invirtiendo el argumento del logaritmo mediante la propiedad $-\ln(A/B) = \ln(B/A)$, se obtiene exactamente la expresión oficial:
   $$Q = \frac{2\varepsilon_0 Mg}{\sigma_0 \ln\left( \frac{a + \sqrt{a^2 + b^2}}{a + \sqrt{a^2 + (a+b)^2}} \right)}$$

> **Nota:** La solución oficial escribe el denominador con el cociente invertido $\ln\left( \frac{a + \sqrt{a^2 + b^2}}{a + \sqrt{a^2 + (a+b)^2}} \right)$. Dado que $b < a+b$, el numerador es menor que el denominador, por lo que este logaritmo es intrínsecamente negativo. Esto incorpora automáticamente el signo negativo de la carga $Q < 0$, necesario para que la fuerza con un plano cargado positivamente sea de atracción y sostenga la barra frente a la gravedad.

$$\boxed{Q = -\frac{2\varepsilon_0 Mg}{\sigma_0 \ln\left( \frac{a + \sqrt{a^2 + (a+b)^2}}{a + \sqrt{a^2 + b^2}} \right)} = \frac{2\varepsilon_0 Mg}{\sigma_0 \ln\left( \frac{a + \sqrt{a^2 + b^2}}{a + \sqrt{a^2 + (a+b)^2}} \right)}}$$

**Verificación:**
- **Unidades:**
  $$\left[ \frac{\left(\frac{\text{C}^2}{\text{N}\cdot\text{m}^2}\right)(\text{kg})\left(\frac{\text{m}}{\text{s}^2}\right)}{\frac{\text{C}}{\text{m}^2}} \right] = \left[ \frac{\frac{\text{C}^2}{\text{m}^2}}{\frac{\text{C}}{\text{m}^2}} \right] = [\text{C}]$$
  Dimensionalmente consistente.

---

## Problema 3

Un casquete semiesférico no conductor de radio interior $a$ tiene una carga total $Q$ distribuida uniformemente en su superficie interior. Encuentre el campo eléctrico en el centro de curvatura.

> **[Figura]:** Casquete semiesférico de radio $a$ ubicado en el espacio tridimensional. El centro de curvatura se encuentra en el origen $(0, 0, 0)$. El casquete se sitúa en el hemisferio inferior $z \le 0$, abriéndose hacia arriba con su borde en el plano $xy$ ($z = 0$). Sobre la superficie interior actúa una densidad superficial uniforme $\sigma$. El vector de campo eléctrico resultante $\vec{E}$ en el origen apunta verticalmente hacia arriba a lo largo del semieje positivo $+Z$ ($+\hat{k}$ o $+\hat{z}$).

### Solución

**Idea:** La carga total $Q$ se reparte sobre el área de la semiesfera $A = 2\pi a^2$, determinando una densidad superficial $\sigma = \frac{Q}{2\pi a^2}$. En coordenadas esféricas $(r, \theta, \phi)$, el centro de curvatura está en el origen $\vec{r} = \vec{0}$. Por simetría axial respecto al eje $Z$, las componentes perpendiculares ($E_x$ y $E_y$) se anulan por pares diametralmente opuestos, sobreviviendo únicamente la componente a lo largo del eje $Z$.

#### 1. Densidad de carga y elemento diferencial

- **Área del casquete semiesférico de radio $a$:**
  $$A = \int_0^{2\pi} d\phi \int_{\pi/2}^\pi a^2\sin\theta\,d\theta = 2\pi a^2 [-\cos\theta]_{\pi/2}^\pi = 2\pi a^2 (-(-1) - 0) = 2\pi a^2$$
- **Densidad superficial de carga:**
  $$\sigma = \frac{Q}{A} = \frac{Q}{2\pi a^2}$$
- **Diferencial de carga:**
  $$dq = \sigma\,dA = \left( \frac{Q}{2\pi a^2} \right) (a^2\sin\theta\,d\theta\,d\phi) = \frac{Q}{2\pi}\sin\theta\,d\theta\,d\phi$$

#### 2. Vectores de posición

Ubicando el casquete en el hemisferio inferior ($z \le 0$):
- Ángulo polar $\theta \in [\pi/2, \pi]$, ángulo azimutal $\phi \in [0, 2\pi]$.
- Posición de un punto sobre el casquete:
  $$\vec{r}' = a(\sin\theta\cos\phi\,\hat{x} + \sin\theta\sin\phi\,\hat{y} + \cos\theta\,\hat{z})$$
- Posición del centro de curvatura: $\vec{r} = \vec{0}$.
- Vector relativo:
  $$\vec{r} - \vec{r}' = -a(\sin\theta\cos\phi\,\hat{x} + \sin\theta\sin\phi\,\hat{y} + \cos\theta\,\hat{z})$$
  $$\|\vec{r} - \vec{r}'\| = a \implies \|\vec{r} - \vec{r}'\|^3 = a^3$$

#### 3. Integración del campo eléctrico

Por la ley de Coulomb:
$$\vec{E} = \frac{1}{4\pi\varepsilon_0} \int_{\theta=\pi/2}^\pi \int_{\phi=0}^{2\pi} \frac{-a(\sin\theta\cos\phi\,\hat{x} + \sin\theta\sin\phi\,\hat{y} + \cos\theta\,\hat{z})}{a^3} \left( \frac{Q}{2\pi}\sin\theta\,d\theta\,d\phi \right)$$

Por simetría azimutal en el intervalo $\phi \in [0, 2\pi]$:
$$\int_0^{2\pi} \cos\phi\,d\phi = 0, \qquad \int_0^{2\pi} \sin\phi\,d\phi = 0$$
Por ende, las componentes horizontales se cancelan: $E_x = E_y = 0$.

Para la componente en $\hat{z}$, la integración sobre $\phi$ entrega directamente un factor $2\pi$:
$$\vec{E} = -\frac{1}{4\pi\varepsilon_0 a^2} \left( \frac{Q}{2\pi} \right) (2\pi)\,\hat{z} \int_{\pi/2}^\pi \cos\theta\sin\theta\,d\theta = -\frac{Q}{4\pi\varepsilon_0 a^2}\,\hat{z} \int_{\pi/2}^\pi \cos\theta\sin\theta\,d\theta$$

Utilizando la identidad trigonométrica $\sin\theta\cos\theta = \frac{1}{2}\sin(2\theta)$:
$$\int_{\pi/2}^\pi \cos\theta\sin\theta\,d\theta = \frac{1}{2} \int_{\pi/2}^\pi \sin(2\theta)\,d\theta = \frac{1}{2} \left[ -\frac{1}{2}\cos(2\theta) \right]_{\pi/2}^\pi = -\frac{1}{4} \left( \cos(2\pi) - \cos(\pi) \right) = -\frac{1}{4} (1 - (-1)) = -\frac{1}{2}$$

*(Alternativamente, haciendo la sustitución $u = \cos\theta \implies du = -\sin\theta\,d\theta$: $\int_{\pi/2}^\pi \cos\theta\sin\theta\,d\theta = -\int_0^{-1} u\,du = -\left[\frac{u^2}{2}\right]_0^{-1} = -\frac{1}{2}$).*

Sustituyendo el valor de la integral:
$$\vec{E} = -\frac{Q}{4\pi\varepsilon_0 a^2} \left( -\frac{1}{2} \right)\,\hat{z} = \frac{Q}{8\pi\varepsilon_0 a^2}\,\hat{z}$$

$$\boxed{\vec{E} = \frac{Q}{8\pi\varepsilon_0 a^2}\,\hat{z}}$$

**Verificación:**
- **Dirección física:** El casquete con carga positiva $Q > 0$ se ubica completamente en el semiespacio $z < 0$. Cada elemento de carga positiva empuja hacia $+Z$ al pasar por el origen. Por ende, el campo en el origen debe apuntar necesariamente hacia arriba ($+\hat{z}$), alejándose del casquete.
- **Unidades:** $[Q] / ([\varepsilon_0][a^2]) = [\text{C}] / ((\text{C}^2/(\text{N}\cdot\text{m}^2))\cdot\text{m}^2) = [\text{N/C}]$, dimensionalmente correcto.
- **Comparación geométrica:** El campo de una esfera completa cerrada en su centro es $\vec{0}$. Cada hemisferio aporta exactamente la mitad para cancelar al opuesto; el valor obtenido $\frac{Q}{8\pi\varepsilon_0 a^2} = \frac{\sigma}{4\varepsilon_0}$ coincide con la mitad del salto de campo superficial de una cáscara esférica.

---

## Resumen de resultados

| Problema / Parte | Descripción | Expresión / Resultado Final |
| :--- | :--- | :--- |
| **Problema 1 a)** | Campo de porción recta vertical | $\vec{E}_1 = \frac{\lambda}{4\pi\varepsilon_0 R}(\hat{x} - \hat{y})$ |
| **Problema 1 a)** | Campo de porción recta horizontal | $\vec{E}_2 = \frac{\lambda}{4\pi\varepsilon_0 R}(-\hat{x} + \hat{y})$ |
| **Problema 1 a)** | Campo total de ambas rectas | $\vec{E}_{\text{rectas}} = \vec{E}_1 + \vec{E}_2 = \vec{0}$ |
| **Problema 1 b)** | Campo de porción curva (cuarto de círculo) | $\vec{E}_3 = \frac{\lambda}{4\pi\varepsilon_0 R}(\hat{x} + \hat{y})$ |
| **Problema 1 c)** | Campo total del alambre y su magnitud | $\vec{E}_T = \frac{\lambda}{4\pi\varepsilon_0 R}(\hat{x} + \hat{y}), \quad \|\vec{E}_T\| = \frac{\sqrt{2}\lambda}{4\pi\varepsilon_0 R}$ |
| **Problema 2 a)** | Campo eléctrico en el eje del plano con agujero | $\vec{E}(z) = \frac{\sigma_0 a}{2\varepsilon_0 z}\left(1 - \frac{a}{\sqrt{z^2+a^2}}\right)\hat{z}$ |
| **Problema 2 b)** | Fuerza integral sobre la barra cargada | $\vec{F}_e = \frac{\sigma_0 Q}{2\varepsilon_0}\hat{z}\int_b^{b+a}\left(\frac{1}{z} - \frac{a}{z\sqrt{z^2+a^2}}\right)dz$ |
| **Problema 2 c)** | Carga total $Q$ de la barra para equilibrio | $Q = -\frac{2\varepsilon_0 Mg}{\sigma_0 \ln\left(\frac{a+\sqrt{a^2+(a+b)^2}}{a+\sqrt{a^2+b^2}}\right)} = \frac{2\varepsilon_0 Mg}{\sigma_0 \ln\left(\frac{a+\sqrt{a^2+b^2}}{a+\sqrt{a^2+(a+b)^2}}\right)}$ |
| **Problema 3** | Campo en el centro de curvatura del casquete semiesférico | $\vec{E} = \frac{Q}{8\pi\varepsilon_0 a^2}\,\hat{z}$ |
