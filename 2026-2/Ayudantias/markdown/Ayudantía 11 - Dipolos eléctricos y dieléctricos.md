# Ayudantía 11 — Dipolos eléctricos y dieléctricos

> Clases relacionadas: [Clase 05 - Potencial electroestático](../../Clases/markdown/Clase%2005%20-%20Potencial%20electroest%C3%A1tico.md), [Clase 06 - Condensadores](../../Clases/markdown/Clase%2006%20-%20Condensadores.md), [Clase 07 - Dieléctricos](../../Clases/markdown/Clase%2007%20-%20Diel%C3%A9ctricos.md)

---

## Problema 1

Considere una barra de largo $2L$, la cual se encuentra sobre el eje $x$ desde $x = -L$ hasta $x = L$. La barra posee una densidad de carga $\lambda(x) = \frac{5}{6}\alpha x^3$ donde $\alpha$ es una constante y una masa $M$ distribuida uniformemente en su largo. En el espacio donde se encuentre la barra existe un campo eléctrico constante $\vec{E} = E_0\,\hat{x}$.

a) Determine el momento dipolar de la barra.  
b) Si la barra puede rotar con respecto a su centro, determine la frecuencia con que oscilará la barra si es perturbada débilmente de su posición de equilibrio.

> **[Figura]:** Una barra delgada de longitud total $2L$ y masa $M$ descansa sobre el eje horizontal $x$, centrada en el origen, extendiéndose desde $x = -L$ hasta $x = L$. El eje vertical $y$ pasa por su punto medio ($x = 0$). Sobre ella se indica su densidad lineal de carga $\lambda(x) = \frac{5}{6}\alpha x^3$. En toda la región existe un campo eléctrico uniforme $\vec{E} = E_0\,\hat{x}$ representado por una flecha horizontal dirigida hacia el semieje $+X$.

### Solución

**Idea:** La carga total de la barra es nula debido a la antisimetría de $\lambda(x)$ respecto al origen, por lo que su momento dipolar eléctrico $\vec{p}$ es independiente de la elección del origen y se calcula integrando $\int \vec{r}'\,dq$. Al rotar la barra un ángulo pequeño respecto a la dirección del campo eléctrico, este ejerce un torque restaurador $\vec{\tau} = \vec{p} \times \vec{E}$. Combinando con la segunda ley de Newton para la rotación y el momento de inercia de una barra delgada respecto a su centro, se obtiene la ecuación de un oscilador armónico simple.

#### a) Determinación del momento dipolar de la barra

La carga total de la barra es:
$$Q = \int_{-L}^{L} \lambda(x)\,dx = \int_{-L}^{L} \frac{5}{6}\alpha x^3\,dx = 0$$
dado que el integrando es una función impar evaluada en un intervalo simétrico. Al ser la carga nula, el momento dipolar eléctrico $\vec{p}$ es unívoco e independiente del sistema de coordenadas elegido.

Definiendo el origen en el centro de la barra ($x = 0$), el vector de posición de cada elemento diferencial es $\vec{r}' = x\,\hat{x}$, y el diferencial de carga es $dq = \lambda(x)\,dx = \frac{5}{6}\alpha x^3\,dx$. El momento dipolar eléctrico para una distribución continua se define como:
$$\vec{p} = \int \vec{r}'\,dq = \int_{-L}^{L} (x\,\hat{x})\left(\frac{5}{6}\alpha x^3\right)dx$$

Sacando las constantes de la integral:
$$\vec{p} = \frac{5}{6}\alpha\,\hat{x} \int_{-L}^{L} x^4\,dx = \frac{5}{6}\alpha\,\hat{x} \left[ \frac{x^5}{5} \right]_{-L}^{L} = \frac{1}{6}\alpha\,\hat{x} \Big( L^5 - (-L)^5 \Big) = \frac{1}{6}\alpha\,\hat{x} (2L^5) = \frac{1}{3}\alpha L^5\,\hat{x}$$

$$\boxed{\vec{p} = \frac{1}{3}\alpha L^5\,\hat{x}}$$

---

#### b) Frecuencia de oscilación ante una perturbación débil

La posición de equilibrio estable ocurre cuando el momento dipolar está alineado con el campo eléctrico ($\theta = 0$, a lo largo de $\hat{x}$).

Si se perturba la barra haciéndola rotar un ángulo $\theta$ en el plano $xy$ en torno al eje $z$ que pasa por su centro de masa, el vector momento dipolar rota solidariamente con la barra:
$$\vec{p} = p\cos\theta\,\hat{x} + p\sin\theta\,\hat{y}$$
con $p = \|\vec{p}\| = \frac{1}{3}\alpha L^5$.

El torque ejercido por el campo eléctrico uniforme $\vec{E} = E_0\,\hat{x}$ sobre el dipolo es:
$$\vec{\tau} = \vec{p} \times \vec{E} = (p\cos\theta\,\hat{x} + p\sin\theta\,\hat{y}) \times (E_0\,\hat{x})$$

Usando las reglas del producto cruz ($\hat{x}\times\hat{x} = \vec{0}$, $\hat{y}\times\hat{x} = -\hat{z}$):
$$\vec{\tau} = -p E_0 \sin\theta\,\hat{z}$$

El momento de inercia $I$ de una barra uniforme de masa $M$ y longitud total $\ell = 2L$ que gira respecto a un eje perpendicular que pasa por su centro es:
$$I = \int_{-L}^{L} x^2\,dm = \int_{-L}^{L} x^2 \left(\frac{M}{2L}\right)dx = \frac{M}{2L} \left[ \frac{x^3}{3} \right]_{-L}^{L} = \frac{M}{2L}\left(\frac{2L^3}{3}\right) = \frac{1}{3} M L^2$$

Aplicando la segunda ley de Newton para rotaciones ($\sum \tau_z = I \ddot{\theta}$):
$$-p E_0 \sin\theta = I \ddot{\theta}$$

Para pequeñas oscilaciones ($\theta \ll 1$), empleamos la aproximación de primer orden de Taylor $\sin\theta \approx \theta$:
$$I \ddot{\theta} + p E_0 \theta = 0 \implies \ddot{\theta} + \left(\frac{p E_0}{I}\right)\theta = 0$$

Esta es la ecuación diferencial de un oscilador armónico simple:
$$\ddot{\theta} + \omega^2 \theta = 0$$

cuya frecuencia angular de oscilación es:
$$\omega = \sqrt{\frac{p E_0}{I}}$$

Sustituyendo $p = \frac{1}{3}\alpha L^5$ e $I = \frac{1}{3} M L^2$:
$$\omega = \sqrt{\frac{\frac{1}{3}\alpha L^5 E_0}{\frac{1}{3} M L^2}} = \sqrt{\frac{\alpha L^3 E_0}{M}}$$

$$\boxed{\omega = \sqrt{\frac{\alpha L^3 E_0}{M}} \qquad \left(\text{o bien } f = \frac{\omega}{2\pi} = \frac{1}{2\pi}\sqrt{\frac{\alpha L^3 E_0}{M}}\right)}$$

**Verificación:**
- **Unidades:**
  - Densidad $\lambda = \frac{5}{6}\alpha x^3 \implies [\alpha] = \frac{[\lambda]}{[x^3]} = \frac{\text{C/m}}{\text{m}^3} = \text{C}\cdot\text{m}^{-4}$.
  - Dipolo: $[p] = [\alpha][L^5] = (\text{C}\cdot\text{m}^{-4})(\text{m}^5) = \text{C}\cdot\text{m}$, unidad estándar de momento dipolar eléctrico.
  - Frecuencia angular:
    $$[\omega^2] = \frac{[\alpha][L^3][E]}{[M]} = \frac{(\text{C}\cdot\text{m}^{-4})(\text{m}^3)(\text{N/C})}{\text{kg}} = \frac{\text{N}\cdot\text{m}^{-1}}{\text{kg}} = \frac{\text{kg}\cdot\text{m}\cdot\text{s}^{-2}\cdot\text{m}^{-1}}{\text{kg}} = \text{s}^{-2} \implies [\omega] = \text{s}^{-1} = \text{rad/s}$$
    Dimensionalmente exacto.
- **Límites físicos:** Si $\alpha \to 0$ o $E_0 \to 0$, no hay fuerza restauradora eléctrica y $\omega \to 0$. Si la masa $M \to \infty$, la inercia impide la aceleración angular y $\omega \to 0$.

---

## Problema 2

Un dispositivo de uso frecuente en muchos artefactos eléctricos de uso diario son los condensadores variables. Este tipo de condensador posee una geometría que es fácil de modificar mecánicamente, con lo cual se puede ajustar su capacidad a gusto. Existen muchos diseños de este tipo de dispositivos, un ejemplo simple e idealizado es el que se muestra en la Figura. El cual consiste en dos placas paralelas y cuadradas de largo $a$ y separadas una distancia $b$. Entremedio de las cuales se introduce parcialmente un dieléctrico de permitividad $\varepsilon$, el cual penetra una distancia $x$ de uno de los bordes del condensador. Suponga que dispone de una batería que da un voltaje $V_0$, y desea almacenar una carga $Q$ en el condensador. Para ajustarlo, calcule:

a) La capacidad del condensador para un $x$ dado, despreciando los efectos de borde.  
b) La penetración $x$ del dieléctrico para el condensador tenga una carga $Q$.  
c) ¿Cuál es la fuerza que siente el condensador en esa posición?  
d) ¿Cuál es el rango de carga $Q$ que puede ser almacenado en el condensador?

> **[Figura]:** Dos placas cuadradas conductoras paralelas de lado $a$ dispuestas verticalmente y separadas una distancia horizontal $b$. Las placas están conectadas a una fuente de corriente continua de voltaje $V_0$. Por el extremo inferior, una lámina dieléctrica de permitividad $\varepsilon$, espesor $b$ y ancho $a$ se introduce verticalmente hacia arriba una distancia $x$ dentro del espacio entre placas. La porción restante de longitud $a - x$ entre las placas se encuentra vacía (permitividad del vacío $\varepsilon_0$).

### Solución

**Idea:** La región ocupada parcialmente por el dieléctrico puede modelarse como dos condensadores ideales en paralelo conectados a la misma diferencia de potencial $V_0$: uno con dieléctrico de longitud $x$ y otro de vacío de longitud $a - x$. La capacidad total equivalente es la suma de ambas capacidades. La fuerza sobre el dieléctrico a potencial constante se obtiene mediante la derivada de la energía electrostática respecto a la coordenada de desplazamiento.

#### a) Capacidad del condensador en función de $x$

Para un condensador plano de placas paralelas con área $A$ y separación $d$, lleno de un medio de permitividad $\varepsilon$, su capacitancia viene dada por:
$$C = \frac{\varepsilon A}{d}$$

Al introducir parcialmente el dieléctrico hasta una profundidad $x \in [0, a]$:
1. Una porción de área $A_1 = a \cdot x$ contiene el dieléctrico de permitividad $\varepsilon$:
   $$C_1 = \frac{\varepsilon a x}{b}$$
2. La porción restante de área $A_2 = a \cdot (a - x)$ contiene vacío con permitividad $\varepsilon_0$:
   $$C_2 = \frac{\varepsilon_0 a (a - x)}{b}$$

Ambas regiones comparten las mismas placas equipotenciales superior e inferior, por lo que están asociadas en paralelo. La capacidad equivalente total $C_T(x)$ es:
$$C_T(x) = C_1 + C_2 = \frac{\varepsilon a x}{b} + \frac{\varepsilon_0 a (a - x)}{b} = \frac{a}{b} \Big[ \varepsilon_0 a + (\varepsilon - \varepsilon_0)x \Big]$$

$$\boxed{C_T(x) = \frac{a}{b}\Big(\varepsilon_0 a + (\varepsilon - \varepsilon_0)x\Big)}$$

---

#### b) Penetración $x$ para almacenar una carga $Q$

La relación entre la carga total almacenada $Q$, la capacidad $C_T$ y la diferencia de potencial aplicada $V_0$ es:
$$Q = C_T(x) V_0 \implies C_T(x) = \frac{Q}{V_0}$$

Igualando con la expresión de la capacidad:
$$\frac{a}{b}\Big(\varepsilon_0 a + (\varepsilon - \varepsilon_0)x\Big) = \frac{Q}{V_0}$$

Multiplicando por $\frac{b}{a}$:
$$\varepsilon_0 a + (\varepsilon - \varepsilon_0)x = \frac{Q b}{V_0 a}$$

Despejando la penetración $x$:
$$(\varepsilon - \varepsilon_0)x = \frac{Q b}{V_0 a} - \varepsilon_0 a \implies x = \frac{1}{\varepsilon - \varepsilon_0}\left(\frac{Q b}{V_0 a} - \varepsilon_0 a\right)$$

$$\boxed{x = \frac{1}{\varepsilon - \varepsilon_0}\left(\frac{Q b}{V_0 a} - \varepsilon_0 a\right)}$$

---

#### c) Fuerza sobre el dieléctrico en esa posición

La energía potencial electrostática almacenada en el condensador a voltaje constante $V_0$ es:
$$U = \frac{1}{2} C_T(x) V_0^2 = \frac{V_0^2 a}{2b}\Big(\varepsilon_0 a + (\varepsilon - \varepsilon_0)x\Big)$$

Cuando el sistema está conectado a una batería que mantiene el potencial constante $V_0$, un desplazamiento infinitesimal $dx$ del dieléctrico altera la carga en $dQ = V_0\,dC$. La batería suministra un trabajo eléctrico $dW_{\text{bat}} = V_0\,dQ = V_0^2\,dC = 2\,dU$. Por el principio de conservación de la energía:
$$dW_{\text{mec}} + dW_{\text{bat}} = dU \implies F_x\,dx + 2\,dU = dU \implies F_x = +\left(\frac{\partial U}{\partial x}\right)_{V_0} = \frac{1}{2} V_0^2 \frac{dC_T}{dx}$$

Derivando respecto a $x$:
$$\frac{dC_T}{dx} = \frac{a(\varepsilon - \varepsilon_0)}{b}$$

Por lo tanto, la fuerza electrostática neta que actúa sobre la placa dieléctrica introduciéndola al condensador es:
$$\vec{F} = \frac{\partial U}{\partial x}\,\hat{x} = \frac{V_0^2 a(\varepsilon - \varepsilon_0)}{2b}\,\hat{x}$$

$$\boxed{\vec{F} = \frac{V_0^2 a(\varepsilon - \varepsilon_0)}{2b}\,\hat{x}}$$

> **Nota:** Dado que $\varepsilon > \varepsilon_0$, la fuerza sobre el dieléctrico es positiva ($+\hat{x}$), lo que significa que el campo marginal en los bordes del condensador atrae al dieléctrico hacia el interior. Por la tercera ley de Newton, la fuerza reactiva que el dieléctrico ejerce sobre la estructura del condensador tiene igual magnitud y sentido opuesto ($-\hat{x}$).

---

#### d) Rango de carga $Q$ almacenable

Como la placa dieléctrica solo puede desplazarse dentro de las dimensiones físicas del condensador, el parámetro de penetración está restringido al intervalo cerrado:
$$x \in [0,\, a]$$

La función de carga $Q(x)$ es linealmente creciente con $x$ (ya que $\varepsilon \ge \varepsilon_0$):
$$Q(x) = C_T(x)V_0 = \frac{V_0 a}{b}\Big(\varepsilon_0 a + (\varepsilon - \varepsilon_0)x\Big)$$

- **Valor mínimo** (condensador completamente vacío de dieléctrico, $x = 0$):
  $$Q_{\min} = Q(0) = \frac{\varepsilon_0 a^2 V_0}{b}$$

- **Valor máximo** (condensador completamente lleno de dieléctrico, $x = a$):
  $$Q_{\max} = Q(a) = \frac{V_0 a}{b}\Big(\varepsilon_0 a + (\varepsilon - \varepsilon_0)a\Big) = \frac{\varepsilon a^2 V_0}{b}$$

Por lo tanto, el rango de carga admisible es:
$$\boxed{\frac{\varepsilon_0 a^2 V_0}{b} \le Q \le \frac{\varepsilon a^2 V_0}{b}}$$

**Verificación:**
- **Unidades:**
  - Capacidad: $[\varepsilon a^2 / b] = (\text{F/m})\cdot \text{m}^2 / \text{m} = \text{F}$, correcto.
  - Fuerza: $[V_0^2 a \varepsilon / b] = \text{V}^2 \cdot \text{m} \cdot (\text{F/m}) / \text{m} = \text{V}^2 \cdot \text{C}/(\text{V}\cdot\text{m}) = \text{V}\cdot\text{C}/\text{m} = \text{J/m} = \text{N}$, correcto.
- **Caso límite:** Si $\varepsilon = \varepsilon_0$ (el material es el mismo vacío), $C_T = \varepsilon_0 a^2/b$, la fuerza resultante se anula ($\vec{F} = \vec{0}$) y la carga no depende de $x$, tal como se espera físicamente.

---

## Problema 3

Se ha encontrado un asteroide esférico de masa $M$ y radio $R$ cargado con una distribución superficial de carga dada por $\sigma(\theta) = \sigma_0 \cos\theta$. Con el objeto de estudiar el asteroide, se ha enviado una sonda espacial cuya trayectoria de acercamiento se encuentra en el plano $\theta = \frac{\pi}{2}$ (*en el original: "plano $\theta = \pi$"*), según muestra la figura.

a) Determine el momento dipolar del asteroide.  
b) Estime el campo eléctrico que afectará a la sonda, si esta se encuentra muy alejada del asteroide.

> **[Figura]:** Un asteroide esférico de radio $R$ centrado en el origen de coordenadas $(0,0,0)$. El eje vertical $z$ coincide con el eje polar $\theta = 0$. La distribución superficial de carga es $\sigma(\theta) = \sigma_0 \cos\theta$, mostrada con gradiente de color (positiva en el hemisferio superior $z > 0$, nula en el ecuador $z = 0$, y negativa en el hemisferio inferior $z < 0$). Los ejes $x$ e $y$ yacen en el plano ecuatorial horizontal ($\theta = \pi/2$). A una distancia lejana en este plano ecuatorial se observa una sonda espacial aproximándose radialmente hacia el asteroide.
>
> **Nota de redacción:** En el enunciado escrito se indica por errata tipográfica *"en el plano $\theta = \pi$"*; no obstante, $\theta = \pi$ describe únicamente el semieje polar negativo $-Z$ (un rayo, no un plano). Tanto el diagrama ilustrativo adjunto como la resolución oficial sitúan explícitamente la trayectoria en el plano ecuatorial caracterizado por $\theta = \frac{\pi}{2}$ (plano $xy$).

### Solución

**Idea:** La distribución $\sigma(\theta) = \sigma_0\cos\theta$ posee carga total nula debido a la antisimetría respecto al plano ecuatorial, lo que hace que su momento monopolar sea nulo y que el término dominante a grandes distancias sea el dipolar. El momento dipolar $\vec{p}$ se obtiene integrando sobre la superficie esférica. Para un punto en el plano ecuatorial ($\theta = \pi/2$), la posición de la sonda es perpendicular a $\vec{p}$, simplificando la fórmula general del campo dipolar lejano.

#### a) Determinación del momento dipolar del asteroide

La carga total del asteroide es:
$$Q_{\text{total}} = \iint \sigma(\theta)\,dA = \int_{0}^{2\pi} d\phi \int_{0}^{\pi} (\sigma_0 \cos\theta) R^2 \sin\theta\,d\theta = 2\pi \sigma_0 R^2 \left[ \frac{\sin^2\theta}{2} \right]_{0}^{\pi} = 0$$

Al ser la carga nula, el momento dipolar eléctrico no depende del origen elegido. Calculamos:
$$\vec{p} = \iint_{S} \sigma(\theta)\,\vec{r}'\,dA$$

En coordenadas esféricas para la superficie de radio $R$:
$$\vec{r}' = R\,\hat{r} = R \Big( \sin\theta\cos\phi\,\hat{x} + \sin\theta\sin\phi\,\hat{y} + \cos\theta\,\hat{z} \Big)$$
$$dA = R^2 \sin\theta\,d\theta\,d\phi$$

Sustituyendo:
$$\vec{p} = \sigma_0 R^3 \int_{0}^{2\pi} d\phi \int_{0}^{\pi} \cos\theta \sin\theta \Big( \sin\theta\cos\phi\,\hat{x} + \sin\theta\sin\phi\,\hat{y} + \cos\theta\,\hat{z} \Big) d\theta$$

Al integrar sobre $\phi \in [0, 2\pi]$:
$$\int_{0}^{2\pi} \cos\phi\,d\phi = 0, \qquad \int_{0}^{2\pi} \sin\phi\,d\phi = 0, \qquad \int_{0}^{2\pi} d\phi = 2\pi$$

Por tanto, las componentes transversales se anulan ($p_x = p_y = 0$), quedando únicamente la componente en $\hat{z}$:
$$p_z = \sigma_0 R^3 (2\pi) \int_{0}^{\pi} \cos^2\theta \sin\theta\,d\theta$$

Efectuando el cambio de variable $u = \cos\theta$, con $du = -\sin\theta\,d\theta$:
$$\int_{0}^{\pi} \cos^2\theta \sin\theta\,d\theta = \int_{-1}^{1} u^2\,du = \left[ \frac{u^3}{3} \right]_{-1}^{1} = \frac{1}{3} - \left(-\frac{1}{3}\right) = \frac{2}{3}$$

Reemplazando:
$$p_z = 2\pi \sigma_0 R^3 \left(\frac{2}{3}\right) = \frac{4\pi}{3}\sigma_0 R^3$$

$$\boxed{\vec{p} = \frac{4\pi}{3}\sigma_0 R^3\,\hat{z}}$$

---

#### b) Campo eléctrico sobre la sonda lejana

A una distancia $\rho \gg R$, el campo eléctrico se puede aproximar con excelente precisión mediante el término dipolar del desarrollo multipolar:
$$\vec{E}(\vec{r}) = \frac{1}{4\pi\varepsilon_0 r^3} \left( \frac{3(\vec{p}\cdot\vec{r})\vec{r}}{r^2} - \vec{p} \right)$$

Dado que la sonda se desplaza en el plano ecuatorial ($\theta = \frac{\pi}{2}$, equivalente al plano $xy$), su vector de posición es radial en el plano horizontal:
$$\vec{r} = \rho\,\hat{\rho}$$
donde $\rho$ es la distancia desde el centro del asteroide y $\hat{\rho} = \cos\phi\,\hat{x} + \sin\phi\,\hat{y}$.

Como $\hat{z} \cdot \hat{\rho} = 0$, el producto escalar entre el momento dipolar y la posición se anula:
$$\vec{p} \cdot \vec{r} = \left(\frac{4\pi}{3}\sigma_0 R^3\,\hat{z}\right) \cdot (\rho\,\hat{\rho}) = 0$$

Por consiguiente, el primer término en el paréntesis del campo dipolar desaparece por completo:
$$\vec{E}(\rho) = \frac{1}{4\pi\varepsilon_0 \rho^3} \Big( \vec{0} - \vec{p} \Big) = -\frac{\vec{p}}{4\pi\varepsilon_0 \rho^3}$$

Sustituyendo el vector $\vec{p} = \frac{4\pi}{3}\sigma_0 R^3\,\hat{z}$:
$$\vec{E}(\rho) = -\frac{\frac{4\pi}{3}\sigma_0 R^3\,\hat{z}}{4\pi\varepsilon_0 \rho^3} = -\frac{\sigma_0 R^3}{3\varepsilon_0 \rho^3}\,\hat{z}$$

$$\boxed{\vec{E}(\rho) = -\frac{\sigma_0 R^3}{3\varepsilon_0 \rho^3}\,\hat{z}}$$

**Verificación:**
- **Dirección física:** El dipolo $\vec{p}$ apunta en $+\hat{z}$ (cargas positivas arriba, negativas abajo). En el plano ecuatorial exterior, las líneas de campo eléctrico emergen del polo positivo norte y entran al polo negativo sur, viajando de arriba hacia abajo ($-\hat{z}$). El signo negativo coincide rigurosamente con la orientación física esperada.
- **Unidades:**
  $$[E] = \frac{[\sigma_0][R^3]}{[\varepsilon_0][\rho^3]} = \frac{(\text{C/m}^2)\cdot \text{m}^3}{(\text{C}^2/(\text{N}\cdot\text{m}^2))\cdot \text{m}^3} = \frac{\text{C}\cdot\text{m}}{\frac{\text{C}^2\cdot\text{m}}{\text{N}}} = \frac{\text{N}}{\text{C}}$$
  Dimensionalmente correcto.

---

## Resumen de resultados

| Problema | Inciso / Pregunta | Resultado final |
| :--- | :--- | :--- |
| **Problema 1** | **a)** Momento dipolar de la barra $\vec{p}$ | $\vec{p} = \dfrac{1}{3}\alpha L^5\,\hat{x}$ |
| | **b)** Frecuencia angular de oscilación $\omega$ | $\omega = \sqrt{\dfrac{\alpha L^3 E_0}{M}} \quad \left(f = \dfrac{1}{2\pi}\sqrt{\dfrac{\alpha L^3 E_0}{M}}\right)$ |
| **Problema 2** | **a)** Capacidad $C_T(x)$ | $C_T(x) = \dfrac{a}{b}\Big(\varepsilon_0 a + (\varepsilon - \varepsilon_0)x\Big)$ |
| | **b)** Penetración $x$ para carga $Q$ | $x = \dfrac{1}{\varepsilon - \varepsilon_0}\left(\dfrac{Q b}{V_0 a} - \varepsilon_0 a\right)$ |
| | **c)** Fuerza sobre el dieléctrico $\vec{F}$ | $\vec{F} = \dfrac{V_0^2 a(\varepsilon - \varepsilon_0)}{2b}\,\hat{x}$ |
| | **d)** Rango de carga almacenable $Q$ | $\dfrac{\varepsilon_0 a^2 V_0}{b} \le Q \le \dfrac{\varepsilon a^2 V_0}{b}$ |
| **Problema 3** | **a)** Momento dipolar del asteroide $\vec{p}$ | $\vec{p} = \dfrac{4\pi}{3}\sigma_0 R^3\,\hat{z}$ |
| | **b)** Campo eléctrico sobre la sonda lejana $\vec{E}$ | $\vec{E}(\rho) = -\dfrac{\sigma_0 R^3}{3\varepsilon_0 \rho^3}\,\hat{z}$ |
