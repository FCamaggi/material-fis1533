# Ayudantía 18 — Ley de Biot-Savart

> Clases relacionadas: [Clase 10 - Campo Magnetico](../../Clases/markdown/Clase%2010%20-%20Campo%20Magnetico.md), [Clase 11 - Ley de Biot Savart](../../Clases/markdown/Clase%2011%20-%20Ley%20de%20Biot%20Savart.md)

---

## Problema 1

Considere un disco de radio $R$ que posee una densidad de carga superficial $\sigma$, uniformemente distribuida. Partiendo del reposo, el disco comienza a girar, hasta alcanzar una velocidad angular constante $\omega$ en torno a su eje de simetría. Encuentre una expresión para el campo magnético en $z = R$. (Propuesto: ¿Cuánto vale el campo magnético para cualquier punto en el eje?).

> **[Figura]:** Un disco circular delgado de radio $R$ ubicado en el plano horizontal $XY$, centrado en el origen de coordenadas cartesianas $(0,0,0)$. El disco posee una densidad de carga superficial constante $\sigma$. El disco rota con velocidad angular constante $\vec{\omega} = \omega\,\hat{z}$ en torno a su eje de simetría axial (eje $Z$), con sentido de giro antihorario visto desde el semieje positivo de las $Z$. Se busca el vector campo magnético $\vec{B}$ en el punto sobre el eje a una altura $z = R$, es decir, en $(0,0,R)$, así como la expresión general para cualquier punto $(0,0,z)$ del eje.

### Solución

**Idea:** La rotación del disco cargado pone en movimiento continuo las cargas superficiales, generando una distribución de densidad de corriente superficial $\vec{K} = \sigma \vec{v}$. Podemos concebir el disco como una superposición continua de anillos concéntricos diferenciales de radio $r$ y ancho $dr$, cada uno transportando una corriente elemental $dI$, y aplicar la ley de Biot-Savart integrando la contribución de campo magnético sobre todo el disco. Por simetría azimutal, las componentes perpendiculares al eje $Z$ se cancelan al integrar en $\theta \in [0, 2\pi]$, resultando un campo puramente axial dirigido a lo largo de $+\hat{z}$.

#### 1. Planteamiento de la Ley de Biot-Savart

La ley de Biot-Savart para un elemento de corriente diferencial es:

$$d\vec{B} = \frac{\mu_0}{4\pi} \frac{I\,d\vec{\ell} \times (\vec{r} - \vec{r}')}{|\vec{r} - \vec{r}'|^3}$$

Para una carga en movimiento sobre una superficie, el elemento de corriente se relaciona con la carga elemental y la velocidad tangencial mediante:

$$I\,d\vec{\ell} = \left(\frac{dq}{dt}\right) d\vec{\ell} = dq\left(\frac{d\vec{\ell}}{dt}\right) = dq\,\vec{v}$$

En coordenadas polares sobre el plano del disco ($z' = 0$):
- Elemento de área: $dS = r'\,dr'\,d\theta'$ (en adelante denotamos simplemente las variables de integración de la fuente como $r$ y $\theta$).
- Carga diferencial: $dq = \sigma\,dS = \sigma r\,dr\,d\theta$, con $r \in [0, R]$ y $\theta \in [0, 2\pi]$.
- Posición de la carga elemental de la fuente: $\vec{r}' = r\,\hat{r}$.
- Velocidad de rotación: $\vec{v} = \vec{\omega} \times \vec{r}' = (\omega\,\hat{z}) \times (r\,\hat{r}) = \omega r\,\hat{\theta}$.
- Posición del punto de observación sobre el eje: $\vec{r} = z\,\hat{z} = R\,\hat{z}$.

Por lo tanto, el vector desplazamiento relativo y su distancia euclidiana son:

$$\vec{r} - \vec{r}' = R\,\hat{z} - r\,\hat{r}$$

$$|\vec{r} - \vec{r}'| = \sqrt{R^2 + r^2}$$

El elemento de corriente es:

$$dq\,\vec{v} = (\sigma r\,dr\,d\theta)(\omega r\,\hat{\theta}) = \sigma \omega r^2 dr\,d\theta\,\hat{\theta}$$

---

#### 2. Producto vectorial y descomposición de componentes

Calculamos el producto vectorial de los vectores unitarios:

$$\hat{\theta} \times (\vec{r} - \vec{r}') = \hat{\theta} \times (R\,\hat{z} - r\,\hat{r}) = R\,(\hat{\theta} \times \hat{z}) - r\,(\hat{\theta} \times \hat{r})$$

Recordando las relaciones de la base cilíndrica ortonormal $(\hat{r}, \hat{\theta}, \hat{z})$:
$$\hat{\theta} \times \hat{z} = \hat{r}$$
$$\hat{\theta} \times \hat{r} = -\hat{z} \implies -r\,(\hat{\theta} \times \hat{r}) = +r\,\hat{z}$$

Así:
$$\hat{\theta} \times (R\,\hat{z} - r\,\hat{r}) = R\,\hat{r} + r\,\hat{z}$$

Al integrar sobre el ángulo azimutal $\theta \in [0, 2\pi]$, el vector unitario radial $\hat{r}(\theta) = \cos\theta\,\hat{i} + \sin\theta\,\hat{j}$ se anula por simetría:

$$\int_0^{2\pi} \hat{r}(\theta)\,d\theta = \left(\int_0^{2\pi} \cos\theta\,d\theta\right)\hat{i} + \left(\int_0^{2\pi} \sin\theta\,d\theta\right)\hat{j} = \vec{0}$$

En consecuencia, la componente radial neta del campo magnético es nula, y sobrevive únicamente la componente axial a lo largo de $\hat{z}$:

$$\vec{B}(R) = \frac{\mu_0}{4\pi} \int_0^{2\pi} d\theta \int_0^R \frac{\sigma \omega r^2 \cdot r}{(R^2 + r^2)^{3/2}} dr\,\hat{z}$$

La integral angular entrega simplemente $\int_0^{2\pi} d\theta = 2\pi$:

$$\vec{B}(R) = \frac{\mu_0 \sigma \omega}{2} \left[ \int_0^R \frac{r^3\,dr}{(R^2 + r^2)^{3/2}} \right] \hat{z}$$

---

#### 3. Resolución de la integral radial

Para resolver la integral:
$$J = \int_0^R \frac{r^3\,dr}{(R^2 + r^2)^{3/2}}$$

Efectuamos el cambio de variable:
$$u = R^2 + r^2 \implies du = 2r\,dr \implies r\,dr = \frac{du}{2}$$
$$r^2 = u - R^2$$

Los límites de integración se transforman como:
- Para $r = 0 \implies u = R^2$
- Para $r = R \implies u = R^2 + R^2 = 2R^2$

Sustituyendo en la integral:
$$J = \int_{R^2}^{2R^2} \frac{(u - R^2) \cdot \frac{1}{2}du}{u^{3/2}} = \frac{1}{2} \int_{R^2}^{2R^2} \left( \frac{u}{u^{3/2}} - \frac{R^2}{u^{3/2}} \right) du$$

$$J = \frac{1}{2} \left[ \int_{R^2}^{2R^2} u^{-1/2}\,du - R^2 \int_{R^2}^{2R^2} u^{-3/2}\,du \right]$$

Integrando cada término:
$$\int u^{-1/2}\,du = 2u^{1/2} = 2\sqrt{u}$$
$$\int u^{-3/2}\,du = \frac{u^{-1/2}}{-1/2} = -\frac{2}{\sqrt{u}}$$

Evaluando entre los límites $R^2$ y $2R^2$:
$$J = \frac{1}{2} \left[ 2\sqrt{u} + \frac{2R^2}{\sqrt{u}} \right]_{R^2}^{2R^2} = \left[ \sqrt{u} + \frac{R^2}{\sqrt{u}} \right]_{R^2}^{2R^2}$$

Evaluando en el límite superior ($u = 2R^2$):
$$\sqrt{2R^2} + \frac{R^2}{\sqrt{2R^2}} = \sqrt{2}R + \frac{R^2}{\sqrt{2}R} = \sqrt{2}R + \frac{R}{\sqrt{2}} = \sqrt{2}R + \frac{\sqrt{2}}{2}R = \frac{3\sqrt{2}}{2}R$$

Evaluando en el límite inferior ($u = R^2$):
$$\sqrt{R^2} + \frac{R^2}{\sqrt{R^2}} = R + \frac{R^2}{R} = R + R = 2R$$

Restando ambos resultados:
$$J = \frac{3\sqrt{2}}{2}R - 2R = \frac{3\sqrt{2} - 4}{2}R$$

---

#### 4. Campo magnético en $z = R$

Multiplicando por la constante exterior:

$$\vec{B}(R) = \frac{\mu_0 \sigma \omega}{2} \cdot \left( \frac{3\sqrt{2} - 4}{2}R \right) \hat{z}$$

$$\boxed{\vec{B}(0,0,R) = \frac{\mu_0 \sigma \omega R}{4} (3\sqrt{2} - 4)\,\hat{z}}$$

Numéricamente, $3\sqrt{2} - 4 \approx 3(1{,}4142) - 4 = 4{,}2426 - 4 = 0{,}2426 > 0$, lo que confirma que el campo apunta en la dirección $+\hat{z}$.

---

#### 5. Campo magnético para cualquier punto en el eje (pregunta propuesta)

Para un punto genérico $\vec{r} = z\,\hat{z}$ sobre el eje de simetría con $z > 0$:

$$\vec{B}(z) = \frac{\mu_0 \sigma \omega}{2} \left[ \int_0^R \frac{r^3\,dr}{(z^2 + r^2)^{3/2}} \right] \hat{z}$$

Aplicando idéntica sustitución $u = z^2 + r^2$, con $u \in [z^2, z^2 + R^2]$:

$$J(z) = \left[ \sqrt{u} + \frac{z^2}{\sqrt{u}} \right]_{z^2}^{z^2 + R^2} = \left( \sqrt{z^2 + R^2} + \frac{z^2}{\sqrt{z^2 + R^2}} \right) - \left( z + \frac{z^2}{z} \right)$$

$$J(z) = \frac{(z^2 + R^2) + z^2}{\sqrt{z^2 + R^2}} - 2z = \frac{2z^2 + R^2}{\sqrt{z^2 + R^2}} - 2z$$

Por lo tanto, para cualquier punto sobre el semieje positivo ($z > 0$):

$$\boxed{\vec{B}(0,0,z) = \frac{\mu_0 \sigma \omega}{2} \left( \frac{2z^2 + R^2}{\sqrt{z^2 + R^2}} - 2z \right)\hat{z}}$$

**Verificación:**
- **Límite en el centro ($z \to 0$):** $\vec{B}(0) = \frac{\mu_0 \sigma \omega}{2}\left(\frac{R^2}{R} - 0\right)\hat{z} = \frac{\mu_0 \sigma \omega R}{2}\,\hat{z}$. Esto coincide exactamente con integrar anillos concéntricos de campo en el centro $dB = \frac{\mu_0 dI}{2r} = \frac{\mu_0 (\sigma \omega r\,dr)}{2r} = \frac{\mu_0 \sigma \omega}{2}dr \implies B = \frac{\mu_0 \sigma \omega R}{2}$.
- **Evaluación en $z = R$:** $\frac{2R^2 + R^2}{\sqrt{2R^2}} - 2R = \frac{3R^2}{\sqrt{2}R} - 2R = \frac{3\sqrt{2}-4}{2}R$, recuperando de forma idéntica el resultado del problema.
- **Límite lejano ($z \gg R$):** Desarrollando en serie de potencias de $R/z$:
  $$\frac{2z^2 + R^2}{z\sqrt{1 + R^2/z^2}} - 2z = (2z + R^2/z)\left(1 - \frac{R^2}{2z^2} + \frac{3R^4}{8z^4} - \dots\right) - 2z = \frac{R^4}{4z^3} + \mathcal{O}(z^{-5})$$
  $$B(z) \approx \frac{\mu_0 \sigma \omega R^4}{8z^3} = \frac{\mu_0 m_{\text{dip}}}{2\pi z^3}$$
  donde el momento dipolar magnético total del disco rotante es $m_{\text{dip}} = \int_0^R I(r)\pi r^2 = \int_0^R (\sigma \omega r\,dr)(\pi r^2) = \frac{\pi \sigma \omega R^4}{4}$, con el decaimiento dipolar característico $\propto 1/z^3$.

---

## Problema 2

Calcule el campo magnético en el punto M de la figura. (Suponga que los dos segmentos rectos de alambres son muy largos con respecto hacia $a$. Calcular valor numérico de B si $I = 2\text{ [A]}$ y $a = 5\text{ [cm]}$).

> **[Figura]:** Un conductor continuo coplanar en el plano $XY$ formado por tres secciones consecutivas:
> 1. **Tramo rectilíneo superior semi-infinito:** Se ubica sobre la recta horizontal $y = +a$, extendiéndose desde $x = 0$ hasta $x \to +\infty$. La flecha indica que la corriente $I$ circula hacia la derecha ($+\hat{i}$).
> 2. **Tramo semicircular:** Arco de circunferencia de radio $a$ ubicado en el semiplano izquierdo ($x \le 0$), centrado en el punto $M = (0,0)$. Conecta el extremo del alambre inferior $(0,-a)$ con el extremo del alambre superior $(0,+a)$. La corriente circula en sentido horario (desde $(0,-a)$, pasando por $(-a,0)$, hasta $(0,+a)$).
> 3. **Tramo rectilíneo inferior semi-infinito:** Se ubica sobre la recta horizontal $y = -a$, extendiéndose desde $x \to +\infty$ hasta $x = 0$. La corriente $I$ circula hacia la izquierda ($-\hat{i}$).
> El punto $M$ se ubica en el origen de coordenadas $(0,0)$, coincidente con el centro de curvatura del arco semicircular.

### Solución

**Idea:** Aplicar el principio de superposición descomponiendo el circuito en tres tramos independientes: dos alambres semi-infinitos rectilíneos y un arco semicircular. El campo magnético total en $M(0,0)$ es la suma vectorial:
$$\vec{B}_T = \vec{B}_1 + \vec{B}_2 + \vec{B}_3$$
donde calculamos cada contribución mediante la ley de Biot-Savart.

El punto de observación es el origen: $\vec{r} = \vec{0}$.

---

#### 1. Tramo 1: Alambre rectilíneo semi-infinito superior ($y = +a$)

El alambre recorre desde $x = 0$ hasta $x \to +\infty$ a lo largo de la recta $y = +a$.
- Posición de un elemento de corriente: $\vec{r}' = x\,\hat{i} + a\,\hat{j}$, con $x \in [0, \infty)$.
- Vector diferencial de longitud en la dirección de la corriente: $d\vec{\ell} = dx\,\hat{i}$.
- Vector posición relativa: $\vec{r} - \vec{r}' = -x\,\hat{i} - a\,\hat{j}$.
- Distancia euclidiana: $|\vec{r} - \vec{r}'| = (x^2 + a^2)^{1/2}$.

El producto vectorial entrega:
$$d\vec{\ell} \times (\vec{r} - \vec{r}') = (dx\,\hat{i}) \times (-x\,\hat{i} - a\,\hat{j}) = -a\,dx\,(\hat{i} \times \hat{j}) = -a\,dx\,\hat{k}$$

Por la ley de Biot-Savart:
$$\vec{B}_1 = \frac{\mu_0 I}{4\pi} \int_0^\infty \frac{-a\,dx}{(x^2 + a^2)^{3/2}}\,\hat{k}$$

Efectuando la sustitución trigonométrica estándar $x = a\tan\alpha \implies dx = a\sec^2\alpha\,d\alpha$ con $\alpha \in [0, \pi/2)$:
$$\int_0^\infty \frac{a\,dx}{(x^2 + a^2)^{3/2}} = \int_0^{\pi/2} \frac{a^2\sec^2\alpha\,d\alpha}{a^3\sec^3\alpha} = \frac{1}{a} \int_0^{\pi/2} \cos\alpha\,d\alpha = \frac{1}{a} [\sin\alpha]_0^{\pi/2} = \frac{1}{a}$$

Por lo tanto:
$$\vec{B}_1 = -\frac{\mu_0 I}{4\pi a}\,\hat{k}$$

El campo apunta entrando a la hoja ($-\hat{k}$).

---

#### 2. Tramo 2: Alambre rectilíneo semi-infinito inferior ($y = -a$)

El alambre inferior se ubica en $y = -a$, y la corriente circula hacia la izquierda ($-\hat{i}$), viniendo desde $x \to +\infty$ hasta $x = 0$.
- Posición de un elemento de corriente: $\vec{r}' = x\,\hat{i} - a\,\hat{j}$, con $x \in [\infty, 0]$.
- Vector diferencial de longitud: $d\vec{\ell} = dx\,(-\hat{i}) = -dx\,\hat{i}$.
- Vector relativo: $\vec{r} - \vec{r}' = -x\,\hat{i} + a\,\hat{j}$.

El producto vectorial es:
$$d\vec{\ell} \times (\vec{r} - \vec{r}') = (-dx\,\hat{i}) \times (-x\,\hat{i} + a\,\hat{j}) = -a\,dx\,(\hat{i} \times \hat{j}) = -a\,dx\,\hat{k}$$

Integrando desde $x = \infty$ hasta $x = 0$ con el sentido correcto de circulación:
$$\vec{B}_2 = \frac{\mu_0 I}{4\pi} \int_0^\infty \frac{-a\,dx}{(x^2 + a^2)^{3/2}}\,\hat{k} = -\frac{\mu_0 I}{4\pi a}\,\hat{k}$$

Por la regla de la mano derecha, un alambre horizontal ubicado debajo del punto con corriente hacia la izquierda genera en los puntos sobre él un campo magnético que entra a la hoja ($-\hat{k}$), reforzando el campo del alambre superior.

---

#### 3. Tramo 3: Arco semicircular de radio $a$ ($x \le 0$)

El arco une $(0,-a)$ con $(0,+a)$ a través del semiplano izquierdo con radio fijo $r' = a$.
- Posición de la fuente: $\vec{r}' = a\,\hat{r}(\theta)$, con $\theta \in [-\pi/2, \pi/2]$ medido desde el eje $-X$, o bien parametrizado como $\vec{r}' = a(-\cos\theta\,\hat{i} + \sin\theta\,\hat{j})$ con $\theta \in [-\pi/2, \pi/2]$.
- Vector relativo: $\vec{r} - \vec{r}' = -a\,\hat{r}$.
- Elemento de longitud: la corriente recorre el arco en sentido horario, de $(0,-a)$ a $(0,+a)$, de modo que $d\vec{\ell} = a\,d\theta\,\hat{\theta}$.

El producto vectorial entre el vector tangencial y el vector radial opuesto es:
$$d\vec{\ell} \times (\vec{r} - \vec{r}') = (a\,d\theta\,\hat{\theta}) \times (-a\,\hat{r}) = -a^2 d\theta\,(\hat{\theta} \times \hat{r}) = a^2 d\theta\,\hat{k}'$$
Dado que el giro es horario en el plano $XY$, el producto vectorial apunta entrando a la hoja ($-\hat{k}$):
$$d\vec{\ell} \times (\vec{r} - \vec{r}') = -a^2 d\theta\,\hat{k}$$

Integrando sobre el ángulo del semicírculo ($\Delta\theta = \pi$ rad):
$$\vec{B}_3 = -\frac{\mu_0 I}{4\pi} \int_{-\pi/2}^{\pi/2} \frac{a^2 d\theta}{a^3}\,\hat{k} = -\frac{\mu_0 I}{4\pi a} \int_{-\pi/2}^{\pi/2} d\theta\,\hat{k} = -\frac{\mu_0 I \pi}{4\pi a}\,\hat{k} = -\frac{\mu_0 I}{4a}\,\hat{k}$$

---

#### 4. Campo magnético total y evaluación numérica

Sumando las tres contribuciones:

$$\vec{B}_T = \vec{B}_1 + \vec{B}_2 + \vec{B}_3 = -\left( \frac{\mu_0 I}{4\pi a} + \frac{\mu_0 I}{4\pi a} + \frac{\mu_0 I}{4a} \right) \hat{k}$$

$$\vec{B}_T = -\left( \frac{\mu_0 I}{2\pi a} + \frac{\mu_0 I}{4a} \right) \hat{k} = -\frac{\mu_0 I}{2a}\left(\frac{1}{\pi} + \frac{1}{2}\right)\hat{k}$$

$$\boxed{\vec{B}_M = -\frac{\mu_0 I}{2a}\left(\frac{1}{2} + \frac{1}{\pi}\right)\hat{k} = -\frac{\mu_0 I (\pi + 2)}{4\pi a}\,\hat{k}}$$

**Cálculo numérico:**  
Con los valores dados en el enunciado:
- $I = 2\text{ A}$
- $a = 5\text{ cm} = 0{,}05\text{ m}$
- $\mu_0 = 4\pi \times 10^{-7}\text{ T}\cdot\text{m/A}$

Reemplazando:
$$B = \frac{(4\pi \times 10^{-7}\text{ T}\cdot\text{m/A}) (2\text{ A})}{2(0{,}05\text{ m})} \left(\frac{1}{2} + \frac{1}{\pi}\right) = \frac{8\pi \times 10^{-7}}{0{,}10} \left(0{,}5 + \frac{1}{\pi}\right)$$
$$B = 8\pi \times 10^{-6} \left(\frac{\pi + 2}{2\pi}\right) = 4 \times 10^{-6} (\pi + 2)\text{ T}$$
$$B = 4 \times 10^{-6} (3{,}14159 + 2)\text{ T} = 4 \times 10^{-6} (5{,}14159)\text{ T} \approx 2{,}057 \times 10^{-5}\text{ T} = 20{,}57\,\mu\text{T}$$

$$\boxed{|\vec{B}_M| \approx 2{,}06 \times 10^{-5}\text{ T} = 20{,}6\,\mu\text{T} \quad (\text{entrando a la hoja, }-\hat{k})}$$

> **Nota:** La solución manuscrita oficial concluye con la deducción de la expresión algebraica $\vec{B} = -\frac{\mu_0 I}{2a}\left(\frac{1}{2} + \frac{1}{\pi}\right)\hat{k}$ y omite el reemplazo aritmético explícito pedido en el enunciado. Aquí se ha incluido el cálculo numérico completo correspondiente a $I = 2\text{ A}$ y $a = 5\text{ cm}$.

**Verificación:**
- **Unidades:** $[\mu_0 I / a] = \frac{(\text{T}\cdot\text{m/A})\cdot\text{A}}{\text{m}} = \text{T}$, dimensionalmente correcto.
- **Regla de la mano derecha global:** Al seguir el contorno del circuito con la mano derecha (entrando por la rama inferior hacia la izquierda, girando en sentido horario por el semicírculo y saliendo hacia la derecha por la rama superior), los cuatro dedos apuntan en todo momento de modo que el pulgar apunta hacia el interior de la página ($-\hat{k}$). Todas las componentes se suman constructivamente.

---

## Problema 3

Considere un alambre infinito por el que circula una corriente $I_1$ y una espira rectangular de lados $a$ y $b$, coplanar con el alambre y tal que el lado $a$ es paralelo a éste y a una distancia $h$ del alambre. Suponga que por la espira rectangular circula una corriente $I_2$. ¿Cuál es la fuerza entre el alambre y la espira rectangular?

> **[Figura]:** En el plano horizontal $XY$:
> - Un alambre recto de longitud infinita sobre el eje $X$ ($y = 0$) transporta una corriente $I_1$ dirigida hacia la derecha ($+\hat{i}$).
> - Una espira rectangular de lados $a$ (horizontal) y $b$ (vertical) se ubica en el semiplano $y > 0$, coplanar con el alambre infinito.
> - El lado inferior de la espira, de longitud $a$, está a una distancia $y = h$ del alambre, transportando corriente $I_2$ hacia la izquierda ($-\hat{i}$).
> - El lado superior de la espira, también de longitud $a$, está a una distancia $y = h + b$ del alambre, transportando corriente $I_2$ hacia la derecha ($+\hat{i}$).
> - Los dos lados verticales de longitud $b$ conectan ambos segmentos: el lado izquierdo (en $x = 0$, $y \in [h, h+b]$) con corriente hacia arriba ($+\hat{j}$), y el lado derecho (en $x = a$, $y \in [h, h+b]$) con corriente hacia abajo ($-\hat{j}$). La corriente $I_2$ circula en sentido horario.

### Solución

**Idea:** Un alambre rectilíneo infinito con corriente genera en su entorno un campo magnético cuya magnitud decae inversamente con la distancia radial $y$. Cada segmento de la espira conductora sumergido en este campo variable experimenta una fuerza magnética dada por la ley de Lorentz en conductores:
$$\vec{F} = \int_{\text{tramo}} I_2\,d\vec{\ell} \times \vec{B}$$
Calculamos la fuerza sobre cada uno de los cuatro tramos de la espira y sumamos vectorialmente para obtener la fuerza neta.

#### 1. Campo magnético producido por el alambre infinito

Por la ley de Biot-Savart (o ley de Ampère), el alambre infinito sobre el eje $X$ con corriente $I_1\,\hat{i}$ genera en cualquier punto del semiplano superior ($y > 0$) un campo magnético dirigido hacia afuera de la hoja ($+\hat{k}$):

$$\vec{B}(y) = \frac{\mu_0 I_1}{2\pi y}\,\hat{k}$$

---

#### 2. Fuerza sobre los tramos verticales (tramos 1 y 3)

1. **Tramo vertical izquierdo ($x = 0$, $y \in [h, h+b]$):**  
   La corriente fluye hacia arriba: $d\vec{\ell} = dy\,\hat{j}$.  
   La fuerza diferencial es:
   $$d\vec{F}_1 = I_2\,(dy\,\hat{j}) \times \left( \frac{\mu_0 I_1}{2\pi y}\,\hat{k} \right) = \frac{\mu_0 I_1 I_2}{2\pi y} dy\,(\hat{j} \times \hat{k}) = \frac{\mu_0 I_1 I_2}{2\pi y} dy\,\hat{i}$$
   Integrando desde $y = h$ hasta $y = h+b$:
   $$\vec{F}_1 = \frac{\mu_0 I_1 I_2}{2\pi} \left[ \int_h^{h+b} \frac{dy}{y} \right] \hat{i} = \frac{\mu_0 I_1 I_2}{2\pi} \ln\left(\frac{h+b}{h}\right)\hat{i}$$

2. **Tramo vertical derecho ($x = a$, $y \in [h, h+b]$):**  
   La corriente fluye hacia abajo con idéntico rango de distancias respecto al alambre: $d\vec{\ell} = dy\,(-\hat{j}) = -dy\,\hat{j}$.  
   Por simetría y sentido opuesto de la corriente:
   $$\vec{F}_3 = -\vec{F}_1 = -\frac{\mu_0 I_1 I_2}{2\pi} \ln\left(\frac{h+b}{h}\right)\hat{i}$$

La suma vectorial de las fuerzas sobre ambos laterales se cancela exactamente:
$$\vec{F}_1 + \vec{F}_3 = \vec{0}$$

---

#### 3. Fuerza sobre los tramos horizontales (tramos 2 y 4)

En los tramos horizontales, la distancia $y$ al alambre es constante a lo largo de todo el segmento de longitud $a$, por lo que el campo magnético $\vec{B}$ es uniforme a lo largo del tramo.

1. **Tramo horizontal superior ($y = h+b$, longitud $a$):**  
   La corriente fluye hacia la derecha: $d\vec{\ell} = dx\,\hat{i}$, para $x \in [0, a]$.  
   El campo en esta posición es $\vec{B}(h+b) = \frac{\mu_0 I_1}{2\pi(h+b)}\,\hat{k}$.  
   La fuerza sobre este tramo es:
   $$\vec{F}_2 = \int_0^a I_2\,dx\,\hat{i} \times \left(\frac{\mu_0 I_1}{2\pi(h+b)}\,\hat{k}\right) = \frac{\mu_0 I_1 I_2}{2\pi(h+b)} \left[ \int_0^a dx \right] (\hat{i} \times \hat{k})$$
   Dado que $\hat{i} \times \hat{k} = -\hat{j}$:
   $$\vec{F}_2 = -\frac{\mu_0 I_1 I_2 a}{2\pi(h+b)}\,\hat{j}$$
   Esta fuerza es atractiva hacia el alambre o dirigida hacia abajo ($-\hat{j}$).

2. **Tramo horizontal inferior ($y = h$, longitud $a$):**  
   La corriente fluye hacia la izquierda (sentido opuesto a $I_1$): $d\vec{\ell} = dx\,(-\hat{i}) = -dx\,\hat{i}$.  
   El campo magnético en $y = h$ es $\vec{B}(h) = \frac{\mu_0 I_1}{2\pi h}\,\hat{k}$.  
   La fuerza sobre este tramo es:
   $$\vec{F}_4 = \int_0^a I_2\,(-dx\,\hat{i}) \times \left(\frac{\mu_0 I_1}{2\pi h}\,\hat{k}\right) = -\frac{\mu_0 I_1 I_2 a}{2\pi h} (\hat{i} \times \hat{k}) = +\frac{\mu_0 I_1 I_2 a}{2\pi h}\,\hat{j}$$
   Esta fuerza es repulsiva (hacia arriba, $+\hat{j}$) porque las corrientes $I_1$ e $I_2$ son antiparalelas en este tramo.

---

#### 4. Fuerza magnética total

Sumando las cuatro contribuciones:

$$\vec{F}_T = \vec{F}_1 + \vec{F}_2 + \vec{F}_3 + \vec{F}_4 = \vec{F}_2 + \vec{F}_4$$

$$\vec{F}_T = \left( \frac{\mu_0 I_1 I_2 a}{2\pi h} - \frac{\mu_0 I_1 I_2 a}{2\pi (h+b)} \right) \hat{j}$$

Factorizando:

$$\boxed{\vec{F}_T = \frac{\mu_0 I_1 I_2 a}{2\pi} \left( \frac{1}{h} - \frac{1}{h+b} \right)\hat{j} = \frac{\mu_0 I_1 I_2 a b}{2\pi h(h+b)}\,\hat{j}}$$

Dado que $h < h+b$, se cumple estrictamente $\frac{1}{h} > \frac{1}{h+b}$, de modo que la fuerza total apunta en $+\hat{j}$.  
La fuerza neta entre el alambre y la espira es **repulsiva** (la espira es empujada alejándose del alambre).

**Verificación:**
- **Unidades:** $[\mu_0] = \frac{\text{N}}{\text{A}^2}$, $[I_1 I_2] = \text{A}^2$, $[a b] = \text{m}^2$, $[h(h+b)] = \text{m}^2$. Por ende:
  $$[\vec{F}_T] = \frac{\text{N}}{\text{A}^2} \cdot \text{A}^2 \cdot \frac{\text{m}^2}{\text{m}^2} = \text{N}$$
  La unidad es Newtons.
- **Límites físicos:**
  - Si la espira se aleja infinitamente del alambre ($h \to \infty$), el campo magnético decae a cero y $\vec{F}_T \to \vec{0}$.
  - Si la altura de la espira tiende a cero ($b \to 0$), los tramos 2 y 4 se superponen con corrientes opuestas y $\vec{F}_T \to \vec{0}$.
- **Física del fenómeno:** Dos corrientes paralelas que circulan en el mismo sentido se atraen, mientras que corrientes antiparalelas se repelen. El lado inferior (antiparalelo a $I_1$) está más cerca del alambre donde el campo $\vec{B}$ es más intenso, por lo que su repulsión domina sobre la atracción del lado superior más alejado. La fuerza neta es por tanto necesariamente repulsiva.

---

## Resumen de resultados

| Problema / Inciso | Expresión / Resultado | Comentarios |
| :--- | :--- | :--- |
| **P1** Campo magnético en $z = R$ | $\vec{B}(R) = \frac{\mu_0 \sigma \omega R}{4}(3\sqrt{2} - 4)\,\hat{z}$ | Integración por Biot-Savart sobre anillos concéntricos con velocidad tangencial $\omega r$. |
| **P1** Campo para cualquier punto axial $z > 0$ *(propuesto)* | $\vec{B}(z) = \frac{\mu_0 \sigma \omega}{2} \left( \frac{2z^2 + R^2}{\sqrt{z^2 + R^2}} - 2z \right)\hat{z}$ | Solución general en el eje; recupera $\vec{B}(0) = \frac{\mu_0 \sigma \omega R}{2}\hat{z}$ y dipolo magnético en campo lejano. |
| **P2** Campo magnético en $M(0,0)$ | $\vec{B}_M = -\frac{\mu_0 I}{2a}\left(\frac{1}{2} + \frac{1}{\pi}\right)\hat{k}$ | Superposición de dos alambres semi-infinitos ($-\frac{\mu_0 I}{4\pi a}\hat{k}$ c/u) y un semicírculo ($-\frac{\mu_0 I}{4a}\hat{k}$). |
| **P2** Valor numérico | $|\vec{B}_M| \approx 20{,}6\,\mu\text{T} \quad (2{,}057 \times 10^{-5}\text{ T})$ | Evaluado para $I = 2\text{ A}$ y $a = 0{,}05\text{ m}$; dirección entrando a la hoja ($-\hat{k}$). |
| **P3** Fuerza neta sobre la espira | $\vec{F}_T = \frac{\mu_0 I_1 I_2 a b}{2\pi h(h+b)}\,\hat{j}$ | Fuerza neta repulsiva ($+\hat{j}$); las fuerzas horizontales en los laterales se cancelan mutuamente. |
