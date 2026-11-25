# Ayudantía 04 — Ley de Gauss

> Clases relacionadas: [Clase 03 - Distribuciones continuas y Gauss](../../Clases/markdown/Clase%2003%20-%20Distribuciones%20continuas%20y%20Gauss.md), [Clase 04 - Calculo y Gauss diferencial](../../Clases/markdown/Clase%2004%20-%20Calculo%20y%20Gauss%20diferencial.md)

---

## Problema 1

Una distribución de carga esférica $\rho$ se extiende desde $r = 0$ a $r = R$, con

$$\rho = \rho_0 \left( 1 - \frac{r^2}{R^2} \right)$$

Calcular:

a) La carga total $Q$.  
b) El campo eléctrico en todo el espacio.

> **[Figura]:** Esfera de radio $R$ con simetría esférica centrada en el origen de coordenadas. La densidad volumétrica de carga disminuye radialmente desde su valor máximo $\rho_0$ en el centro ($r = 0$) hasta anularse exactamente en la superficie exterior ($r = R$). Para $r > R$, la densidad de carga es nula.

### Solución

**Idea:** La distribución posee simetría esférica, por lo que el campo eléctrico es estrictamente radial $\vec{E}(\vec{r}) = E(r)\,\hat{r}$ y su magnitud depende únicamente de la distancia radial $r$. La carga total se obtiene integrando la densidad en coordenadas esféricas mediante cáscaras esféricas de volumen $dV = 4\pi r^2 dr$, y el campo eléctrico en todo el espacio se determina mediante la ley de Gauss con superficies gaussianas esféricas concéntricas de radio $r$.

---

#### Parte a) Carga total $Q$

La carga total contenida en la esfera de radio $R$ es la integral de volumen:

$$Q = \iiint_V \rho(r)\,dV = \int_0^{2\pi} d\phi \int_0^\pi \sin\theta\,d\theta \int_0^R \rho_0 \left( 1 - \frac{r^2}{R^2} \right) r^2\,dr$$

Las integrales angulares entregan el factor de ángulo sólido completo $4\pi$:

$$Q = 4\pi\rho_0 \int_0^R \left( r^2 - \frac{r^4}{R^2} \right) dr$$

Integrando término a término respecto a $r$:

$$Q = 4\pi\rho_0 \left[ \frac{r^3}{3} - \frac{r^5}{5R^2} \right]_0^R = 4\pi\rho_0 \left( \frac{R^3}{3} - \frac{R^5}{5R^2} \right) = 4\pi\rho_0 R^3 \left( \frac{1}{3} - \frac{1}{5} \right)$$

$$Q = 4\pi\rho_0 R^3 \left( \frac{5 - 3}{15} \right) = 4\pi\rho_0 R^3 \left( \frac{2}{15} \right) = \frac{8\pi}{15}\rho_0 R^3$$

$$\boxed{Q = \frac{8\pi}{15}\rho_0 R^3}$$

**Verificación:**
- **Unidades:** $[\rho_0][R^3] = (\text{C/m}^3)(\text{m}^3) = [\text{C}]$, dimensionalmente homogéneo.
- **Signo:** Como $r \le R$, el factor $(1 - r^2/R^2) \ge 0$, por lo que si $\rho_0 > 0$, la carga neta es estrictamente positiva.

---

#### Parte b) Campo eléctrico en todo el espacio

Por la ley de Gauss:

$$\oint_{\partial V} \vec{E} \cdot d\vec{A} = \frac{Q_{\text{enc}}}{\varepsilon_0}$$

Tomamos como superficie gaussiana una esfera concéntrica de radio $r$. Por la simetría esférica, $\vec{E} = E(r)\,\hat{r}$ y $d\vec{A} = dA\,\hat{r}$, de modo que el flujo es:

$$\oint_{\partial V} \vec{E} \cdot d\vec{A} = E(r) \oint_{\partial V} dA = E(r) \cdot 4\pi r^2$$

Distinguimos dos regiones del espacio:

##### 1. Región exterior ($r \ge R$)

La superficie gaussiana encierra a la totalidad de la carga de la esfera ($Q_{\text{enc}} = Q$):

$$E(r) \cdot 4\pi r^2 = \frac{Q}{\varepsilon_0} = \frac{\frac{8\pi}{15}\rho_0 R^3}{\varepsilon_0}$$

Despejando $E(r)$:

$$E(r) = \frac{8\pi\rho_0 R^3}{15(4\pi\varepsilon_0 r^2)} = \frac{2\rho_0 R^3}{15\varepsilon_0 r^2}$$

Vectorialmente:
$$\vec{E}(r) = \frac{2\rho_0 R^3}{15\varepsilon_0 r^2}\,\hat{r}$$

##### 2. Región interior ($r < R$)

La superficie gaussiana de radio $r$ encierra únicamente la carga dentro del radio $r$:

$$Q_{\text{enc}}(r) = 4\pi\rho_0 \int_0^r \left( r'^2 - \frac{r'^4}{R^2} \right) dr' = 4\pi\rho_0 \left( \frac{r^3}{3} - \frac{r^5}{5R^2} \right) = 4\pi\rho_0 r^3 \left( \frac{1}{3} - \frac{r^2}{5R^2} \right)$$

Aplicando Gauss:

$$E(r) \cdot 4\pi r^2 = \frac{4\pi\rho_0 r^3}{\varepsilon_0} \left( \frac{1}{3} - \frac{r^2}{5R^2} \right)$$

Dividiendo por $4\pi r^2$:

$$E(r) = \frac{\rho_0}{\varepsilon_0} r \left( \frac{1}{3} - \frac{r^2}{5R^2} \right) = \frac{\rho_0}{\varepsilon_0} \left( \frac{r}{3} - \frac{r^3}{5R^2} \right)$$

Vectorialmente:
$$\vec{E}(r) = \frac{\rho_0}{\varepsilon_0} \left( \frac{r}{3} - \frac{r^3}{5R^2} \right)\hat{r}$$

$$\boxed{\vec{E}(r) = \begin{cases} \dfrac{\rho_0}{\varepsilon_0} \left( \dfrac{r}{3} - \dfrac{r^3}{5R^2} \right)\hat{r} & \text{si } r < R \\ \dfrac{2\rho_0 R^3}{15\varepsilon_0 r^2}\,\hat{r} & \text{si } r \ge R \end{cases}}$$

**Verificación:**
- **Continuidad en la frontera $r = R$:**
  $$E(R^-) = \frac{\rho_0}{\varepsilon_0} \left( \frac{R}{3} - \frac{R^3}{5R^2} \right) = \frac{\rho_0 R}{\varepsilon_0} \left( \frac{1}{3} - \frac{1}{5} \right) = \frac{2\rho_0 R}{15\varepsilon_0}$$
  $$E(R^+) = \frac{2\rho_0 R^3}{15\varepsilon_0 R^2} = \frac{2\rho_0 R}{15\varepsilon_0}$$
  El campo es continuo en $r = R$, como corresponde a una distribución volumétrica finita sin densidades superficiales.
- **Comportamiento en el origen ($r \to 0$):** $E(0) = 0$, consistente con la simetría esférica donde los aportes en el centro se cancelan mutuamente.

---

## Problema 2

Considere la siguiente distribución volumétrica de carga en coordenadas esféricas

$$\rho(r) = \begin{cases} -n\rho & 0 < r < a \\ \rho & a \le r \le b \end{cases}$$

Donde $\rho$ es una constante y $n$ es un entero no negativo. Encuentre el campo eléctrico en todo el espacio.

> **[Figura]:** Sección transversal de una esfera concéntrica de dos capas con simetría esférica. El núcleo interior de radio $a$ ($0 < r < a$) posee una densidad de carga constante negativa $-n\rho$. La cáscara esférica intermedia entre los radios $a$ y $b$ ($a \le r \le b$) posee una densidad de carga constante positiva $+\rho$. Para $r > b$, el medio carece de carga ($\rho = 0$).

### Solución

**Idea:** Debido a la simetría esférica completa, el campo eléctrico es puramente radial $\vec{E} = E(r)\,\hat{r}$. Aplicamos la ley de Gauss utilizando cáscaras esféricas gaussianas concéntricas para cada una de las tres regiones del espacio: $0 < r < a$, $a \le r \le b$ y $r > b$.

El flujo a través de una esfera gaussiana de radio $r$ es:

$$\oint_{\partial V} \vec{E} \cdot d\vec{A} = E(r) \cdot 4\pi r^2 = \frac{Q_{\text{enc}}(r)}{\varepsilon_0}$$

---

#### 1. Región $0 < r < a$ (núcleo interior)

La carga encerrada por la superficie de radio $r$ es:

$$Q_{\text{enc}}(r) = \int_0^r (-n\rho) (4\pi r'^2)\,dr' = -4\pi n\rho \left[ \frac{r'^3}{3} \right]_0^r = -\frac{4\pi n\rho r^3}{3}$$

Por la ley de Gauss:

$$E(r) \cdot 4\pi r^2 = \frac{Q_{\text{enc}}(r)}{\varepsilon_0} = -\frac{4\pi n\rho r^3}{3\varepsilon_0}$$

Despejando el campo radial:

$$E(r) = -\frac{n\rho r}{3\varepsilon_0}$$

Vectorialmente:
$$\vec{E}(r) = -\frac{n\rho r}{3\varepsilon_0}\,\hat{r}$$

> **Nota:** En el apunte manuscrito oficial, en el renglón final del cálculo para esta región se omitió la constante dieléctrica $\varepsilon_0$ en el denominador (escribiendo $-\frac{n\rho}{3}r$). Lo correcto es incluir $\varepsilon_0$ en el denominador, tal como figura en los pasos previos del propio apunte al plantear la ley de Gauss $E \cdot 4\pi r^2 = \frac{Q_{\text{enc}}}{\varepsilon_0}$.

---

#### 2. Región $a \le r \le b$ (cáscara intermedia)

La carga encerrada se compone de la totalidad de la carga del núcleo interior ($r \le a$) más la fracción de la cáscara positiva contenida entre $a$ y $r$:

$$Q_{\text{enc}}(r) = \int_0^a (-n\rho)(4\pi r'^2)\,dr' + \int_a^r \rho(4\pi r'^2)\,dr'$$

$$Q_{\text{enc}}(r) = -\frac{4\pi n\rho a^3}{3} + \frac{4\pi\rho}{3}(r^3 - a^3) = \frac{4\pi\rho}{3} \left[ -n a^3 + r^3 - a^3 \right] = \frac{4\pi\rho}{3} \left[ r^3 - (n+1)a^3 \right]$$

Aplicando la ley de Gauss:

$$E(r) \cdot 4\pi r^2 = \frac{4\pi\rho}{3\varepsilon_0} \left[ r^3 - (n+1)a^3 \right]$$

Dividiendo por $4\pi r^2$:

$$E(r) = \frac{\rho}{3\varepsilon_0 r^2} \left[ r^3 - (n+1)a^3 \right] = \frac{\rho}{3\varepsilon_0} \left( r - \frac{(n+1)a^3}{r^2} \right)$$

Vectorialmente:
$$\vec{E}(r) = \frac{\rho}{3\varepsilon_0 r^2} \left[ r^3 - (n+1)a^3 \right] \hat{r} = \frac{\rho}{3\varepsilon_0} \left( r - \frac{(n+1)a^3}{r^2} \right) \hat{r}$$

---

#### 3. Región $r > b$ (exterior)

Para cualquier radio $r > b$, la superficie gaussiana encierra la carga total de la distribución esférica ($Q_{\text{enc}} = Q_{\text{total}}$):

$$Q_{\text{total}} = Q_{\text{enc}}(b) = \frac{4\pi\rho}{3} \left[ b^3 - (n+1)a^3 \right]$$

Aplicando la ley de Gauss:

$$E(r) \cdot 4\pi r^2 = \frac{Q_{\text{total}}}{\varepsilon_0} = \frac{4\pi\rho}{3\varepsilon_0} \left[ b^3 - (n+1)a^3 \right]$$

Despejando $E(r)$:

$$E(r) = \frac{\rho}{3\varepsilon_0 r^2} \left[ b^3 - (n+1)a^3 \right]$$

Vectorialmente:
$$\vec{E}(r) = \frac{\rho}{3\varepsilon_0 r^2} \left[ b^3 - (n+1)a^3 \right] \hat{r}$$

> **Nota:** En el apunte manuscrito oficial, en el recuadro final para $r > b$ se omitió nuevamente $\varepsilon_0$ en el denominador. La expresión dimensionalmente y físicamente correcta debe contener $\varepsilon_0$, es decir, $\frac{\rho}{3\varepsilon_0 r^2}\left[ b^3 - (n+1)a^3 \right]\hat{r}$.

$$\boxed{\vec{E}(r) = \begin{cases} -\dfrac{n\rho r}{3\varepsilon_0}\,\hat{r} & \text{si } 0 < r < a \\ \dfrac{\rho}{3\varepsilon_0} \left( r - \dfrac{(n+1)a^3}{r^2} \right)\hat{r} & \text{si } a \le r \le b \\ \dfrac{\rho}{3\varepsilon_0 r^2} \left[ b^3 - (n+1)a^3 \right]\hat{r} & \text{si } r > b \end{cases}}$$

**Verificación:**
- **Continuidad en $r = a$:**
  $$E(a^-) = -\frac{n\rho a}{3\varepsilon_0}$$
  $$E(a^+) = \frac{\rho}{3\varepsilon_0}\left( a - \frac{(n+1)a^3}{a^2} \right) = \frac{\rho}{3\varepsilon_0}(a - (n+1)a) = -\frac{n\rho a}{3\varepsilon_0}$$
  Continuo.
- **Continuidad en $r = b$:**
  $$E(b^-) = \frac{\rho}{3\varepsilon_0}\left( b - \frac{(n+1)a^3}{b^2} \right) = \frac{\rho}{3\varepsilon_0 b^2}[b^3 - (n+1)a^3]$$
  $$E(b^+) = \frac{\rho}{3\varepsilon_0 b^2}[b^3 - (n+1)a^3]$$
  Continuo.
- **Caso $n = 0$ (sin núcleo negativo):** Para $r < a$ el campo es cero ($\rho = 0$), y para $r > a$ se recupera la cáscara hueca estándar de densidad uniforme $\rho$.

---

## Problema 3

Considere una carga $q$ en el origen de un sistema de coordenadas cartesianas. En el mismo sistema de referencia existe un rectángulo paralelo al plano $xz$ de ancho $2a$ y altura $2z_0$ ubicado en $y = a$ (ver Figura).

a) Usando la ley de Gauss en forma adecuada, determine el flujo sobre el rectángulo si $z_0 = a$.  
b) ¿Cuántas veces aumenta el flujo de la parte anterior en el caso $z_0 \to \infty$?

> **[Figura]:** Sistema de coordenadas tridimensional cartesiano $xyz$ con una carga puntual $q$ fija en el origen $(0, 0, 0)$. A una distancia perpendicular $y = a$ se encuentra un rectángulo contenido en el plano plano paralelo a $xz$. El rectángulo tiene ancho horizontal $2a$ a lo largo de $x$ (con $x \in [-a, a]$) y altura vertical $2z_0$ a lo largo de $z$ (con $z \in [-z_0, z_0]$), centrado en el punto $(0, a, 0)$.

### Solución

**Idea:** Para la parte a), cuando $z_0 = a$, el rectángulo es un cuadrado perfecto de lado $2a$. Construyendo un cubo gaussiano de arista $2a$ centrado en el origen, la carga queda en su centro exacto y la simetría permite calcular el flujo sin evaluar integrales. Para la parte b), cuando $z_0 \to \infty$, la superficie se transforma en una franja plana infinita; el flujo puede calcularse mediante integración directa de Coulomb de $\vec{E}\cdot d\vec{A}$ o por el ángulo plano subtendido alrededor del eje $Z$.

---

#### Parte a) Flujo sobre el rectángulo cuando $z_0 = a$

Cuando $z_0 = a$, el rectángulo tiene dimensiones:
$$-a \le x \le a, \qquad -a \le z \le a, \qquad \text{en } y = a$$
Se trata de un cuadrado de lado $2a$ situado a una distancia perpendicular $a$ del origen.

Construimos una superficie gaussiana cerrada en forma de **cubo de arista $2a$**, centrado en el origen:
- Las 6 caras planas del cubo se ubican en:
  $$x = \pm a, \qquad y = \pm a, \qquad z = \pm a$$
- La carga $q$ se sitúa en el centro geométrico del cubo $(0, 0, 0)$.
- Por la ley de Gauss, el flujo eléctrico total que atraviesa las seis caras del cubo es:
  $$\Phi_{\text{total}} = \oint_{\text{cubo}} \vec{E} \cdot d\vec{A} = \frac{q}{\varepsilon_0}$$

Dado que el cubo posee simetría cúbica respecto al origen, las seis caras son indistinguibles y equidistantes a la carga puntual $q$. Por lo tanto, el flujo total se reparte en partes exactamente iguales entre cada una de las 6 caras:

$$\Phi_\square = \frac{\Phi_{\text{total}}}{6} = \frac{q}{6\varepsilon_0}$$

$$\boxed{\Phi_\square = \frac{q}{6\varepsilon_0}}$$

**Verificación:** La suma del flujo a través de las 6 caras es $6 \times \frac{q}{6\varepsilon_0} = \frac{q}{\varepsilon_0}$, satisfaciendo rigurosamente la ley de Gauss.

---

#### Parte b) Flujo en el límite $z_0 \to \infty$ y razón de aumento

En el límite $z_0 \to \infty$, la superficie rectangular se convierte en una franja plana infinita en la dirección vertical:
$$-a \le x \le a, \qquad -\infty < z < \infty, \qquad \text{en } y = a$$

Evaluamos el flujo eléctrico por los dos métodos:

##### Método 1: Integración directa del flujo de Coulomb (método oficial)

El vector de posición de un elemento en el plano es $\vec{r}' = x\,\hat{i} + a\,\hat{j} + z\,\hat{k}$.
La distancia a la carga en el origen es $r = \sqrt{x^2 + a^2 + z^2}$.
El elemento de área orientado hacia afuera ($+Y$) es:
$$d\vec{A} = dx\,dz\,\hat{j}$$

El campo eléctrico generado por la carga $q$ en el origen es:
$$\vec{E} = \frac{1}{4\pi\varepsilon_0}\frac{q}{r^3}(x\,\hat{i} + a\,\hat{j} + z\,\hat{k}) = \frac{k q}{(x^2 + a^2 + z^2)^{3/2}}(x\,\hat{i} + a\,\hat{j} + z\,\hat{k})$$

El producto escalar con el elemento de área es:
$$\vec{E} \cdot d\vec{A} = \frac{k q a}{(x^2 + a^2 + z^2)^{3/2}}\,dx\,dz$$

El flujo total es la integral doble:
$$\Phi_\infty = k q a \int_{-a}^a dx \int_{-\infty}^\infty \frac{dz}{(x^2 + a^2 + z^2)^{3/2}}$$

Definiendo $w^2 \equiv x^2 + a^2$, la integral en $z$ es:
$$\int_{-\infty}^\infty \frac{dz}{(w^2 + z^2)^{3/2}} = \left[ \frac{z}{w^2 \sqrt{w^2 + z^2}} \right]_{-\infty}^\infty = \frac{1}{w^2}(1 - (-1)) = \frac{2}{w^2} = \frac{2}{x^2 + a^2}$$

Sustituyendo en la integral respecto a $x$:
$$\Phi_\infty = k q a \int_{-a}^a \frac{2}{x^2 + a^2}\,dx = 2 k q a \left[ \frac{1}{a}\arctan\left(\frac{x}{a}\right) \right]_{-a}^a$$

$$\Phi_\infty = 2 k q \left[ \arctan(1) - \arctan(-1) \right] = 2 k q \left( \frac{\pi}{4} - \left(-\frac{\pi}{4}\right) \right) = 2 k q \left( \frac{\pi}{2} \right) = \pi k q$$

Reemplazando la constante $k = \frac{1}{4\pi\varepsilon_0}$:
$$\Phi_\infty = \pi \left( \frac{1}{4\pi\varepsilon_0} \right) q = \frac{q}{4\varepsilon_0}$$

##### Método 2: Gauss en prisma infinito y simetría angular

Considerando un prisma infinito de sección transversal cuadrada de ancho $2a$ a lo largo del eje $Z$:
En el plano transversal $xy$, la franja subtiende un ángulo desde el origen entre los rayos que van a $(-a, a)$ y $(+a, a)$:
$$\theta_1 = 135^\circ = \frac{3\pi}{4}, \qquad \theta_2 = 45^\circ = \frac{\pi}{4} \implies \Delta\theta = 90^\circ = \frac{\pi}{2}$$
Como la circunferencia completa subtiende $2\pi$ radianes en el plano horizontal, la fracción del flujo que incide en esta franja es:
$$\frac{\Delta\theta}{2\pi} = \frac{\pi/2}{2\pi} = \frac{1}{4} \implies \Phi_\infty = \frac{1}{4}\Phi_{\text{total}} = \frac{q}{4\varepsilon_0}$$

---

##### Aumento del flujo respecto a la parte a)

El enunciado consulta: *¿Cuántas veces aumenta el flujo de la parte anterior en el caso $z_0 \to \infty$?*

Calculamos el cociente entre ambos flujos:

$$\frac{\Phi_\infty}{\Phi_\square} = \frac{\frac{q}{4\varepsilon_0}}{\frac{q}{6\varepsilon_0}} = \frac{6}{4} = \frac{3}{2} = 1{,}5$$

> **Nota:** En el apunte oficial manuscrito se calcula rigurosamente el valor de la integral obteniendo $\Phi_\infty = \frac{q}{4\varepsilon_0}$, pero no se explicita la respuesta directa a la pregunta textual sobre cuántas veces aumenta. Al extender la altura $z_0$ de $a$ a $\infty$, el flujo aumenta un factor de $\frac{3}{2}$ ($1{,}5$ veces, equivalente a un aumento del $50\%$).

$$\boxed{\Phi_\infty = \frac{q}{4\varepsilon_0}, \qquad \frac{\Phi_\infty}{\Phi_\square} = \frac{3}{2} = 1{,}5 \text{ veces}}$$

**Verificación:**
- Cuando $z_0 = a$, la cara cubre un ángulo sólido finito de la esfera. Al alargar la placa verticalmente hasta el infinito ($z_0 \to \infty$), se capturan más líneas de campo eléctrico que escapan hacia arriba y abajo, aumentando el flujo de $\frac{1}{6}\frac{q}{\varepsilon_0} \approx 0{,}167\frac{q}{\varepsilon_0}$ a $\frac{1}{4}\frac{q}{\varepsilon_0} = 0{,}25\frac{q}{\varepsilon_0}$. El factor $1{,}5$ es coherente y físicamente exacto.

---

## Resumen de resultados

| Problema / Parte | Descripción | Expresión / Resultado Final |
| :--- | :--- | :--- |
| **Problema 1 a)** | Carga total de la esfera con $\rho(r) = \rho_0(1 - r^2/R^2)$ | $Q = \frac{8\pi}{15}\rho_0 R^3$ |
| **Problema 1 b)** | Campo eléctrico interior ($r < R$) | $\vec{E}(r) = \frac{\rho_0}{\varepsilon_0} \left( \frac{r}{3} - \frac{r^3}{5R^2} \right)\hat{r}$ |
| **Problema 1 b)** | Campo eléctrico exterior ($r \ge R$) | $\vec{E}(r) = \frac{2\rho_0 R^3}{15\varepsilon_0 r^2}\,\hat{r}$ |
| **Problema 2** | Campo para $0 < r < a$ ($\rho_1 = -n\rho$) | $\vec{E}(r) = -\frac{n\rho r}{3\varepsilon_0}\,\hat{r}$ |
| **Problema 2** | Campo para $a \le r \le b$ ($\rho_2 = \rho$) | $\vec{E}(r) = \frac{\rho}{3\varepsilon_0} \left( r - \frac{(n+1)a^3}{r^2} \right)\hat{r}$ |
| **Problema 2** | Campo para $r > b$ ($\rho = 0$) | $\vec{E}(r) = \frac{\rho}{3\varepsilon_0 r^2} \left[ b^3 - (n+1)a^3 \right]\hat{r}$ |
| **Problema 3 a)** | Flujo sobre el cuadrado ($z_0 = a$) centrado en $y = a$ | $\Phi_\square = \frac{q}{6\varepsilon_0}$ |
| **Problema 3 b)** | Flujo sobre la franja infinita ($z_0 \to \infty$) | $\Phi_\infty = \frac{q}{4\varepsilon_0}$ |
| **Problema 3 b)** | Razón de aumento del flujo ($\Phi_\infty / \Phi_\square$) | $\frac{\Phi_\infty}{\Phi_\square} = \frac{3}{2} = 1{,}5\text{ veces (aumento del 50\%)}$ |
