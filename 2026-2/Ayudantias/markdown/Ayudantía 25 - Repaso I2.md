# Ayudantía 25 — Repaso I2

> Clases relacionadas: [Clase 09 - Potencia, circuitos de resistencias y circuito RC](../../Clases/markdown/Clase%2009%20-%20Potencia%2C%20circuitos%20de%20resistencias%20y%20circuito%20RC.md), [Clase 10 - Campo Magnetico](../../Clases/markdown/Clase%2010%20-%20Campo%20Magnetico.md), [Clase 11 - Ley de Biot Savart](../../Clases/markdown/Clase%2011%20-%20Ley%20de%20Biot%20Savart.md), [Clase 12 - Ley de Ampere](../../Clases/markdown/Clase%2012%20-%20Ley%20de%20Ampere.md)

---

## Problema 1

En el circuito de la figura, los condensadores se encuentran completamente descargados.

Si el interruptor se cambia a la posición $1$ en $t = 0\text{ s}$, determinar:

a) La corriente $I_0$ que suministra la fuente en el instante justo después de cerrar el interruptor.  
b) La carga máxima almacenada en el condensador $C_1$.  
c) La carga almacenada en el capacitor $C_1$ en función del tiempo.

Si luego de mucho tiempo, el interruptor se cambia otra vez a la posición $2$, determine:

d) La carga almacenada en $C_1$ como función del tiempo.

> **[Figura]:** Circuito de dos mallas acopladas mediante un interruptor conmutable de dos posiciones ($1$ y $2$). En la rama vertical izquierda se encuentra una fuente ideal de fem $\mathcal{E}$ (polo positivo arriba, polo negativo abajo). Desde el polo negativo parte el riel inferior hacia la derecha pasando en serie por una resistencia $R_3$, luego continúa hasta un nodo inferior donde se conectan las placas inferiores de los condensadores $C_1$ (en la rama vertical central) y $C_2$ (en la rama vertical derecha). En la parte superior, desde el polo positivo de $\mathcal{E}$ el cable llega al terminal $1$ del interruptor. El terminal común (pivote) del interruptor se conecta hacia abajo a la rama vertical central, compuesta por la resistencia $R_1$ en serie con el condensador $C_1$. El terminal $2$ del interruptor se conecta hacia abajo a la rama vertical derecha, compuesta por la resistencia $R_2$ en serie con el condensador $C_2$.

### Solución

**Idea:** El análisis se divide en dos regímenes transitorios de circuitos RC de una sola malla cerrada. Cuando el interruptor está en la posición $1$, la fuente $\mathcal{E}$ carga al condensador $C_1$ a través de las resistencias en serie $R_1$ y $R_3$ (mientras la rama derecha permanece abierta). Cuando, tras alcanzar el equilibrio estacionario, el interruptor pasa a la posición $2$, la rama de la fuente queda abierta y el condensador cargado $C_1$ redistribuye parte de su carga hacia $C_2$ a través de las resistencias en serie $R_1$ y $R_2$, conservando la carga total en las placas conectadas entre sí.

#### Parte a) Corriente inicial $I_0$ en $t = 0^+$

Al cambiar el interruptor a la posición $1$ en $t = 0\text{ s}$, queda cerrada únicamente la malla izquierda ($\mathcal{E} - R_1 - C_1 - R_3$), por donde circula la corriente en sentido horario; la rama derecha ($R_2 - C_2$) queda abierta.

Como el condensador $C_1$ está inicialmente descargado ($q_1(0) = 0$), su diferencia de potencial en el instante inmediatamente posterior al cierre es nula ($\Delta V_{C_1}(0^+) = q_1(0)/C_1 = 0$), por lo que actúa momentáneamente como un cable ideal (cortocircuito).

Aplicando la ley de voltajes de Kirchhoff (LVK) en la malla izquierda, donde $R_1$ y $R_3$ están en serie y conducen la misma corriente $I_0$:
$$\mathcal{E} - I_0 R_1 - I_0 R_3 = 0$$

> **Nota:** en la ecuación intermedia de la solución oficial manuscrita aparece escrito $I_0 \cdot R_2$ por un lapsus de notación; el circuito y el despeje inmediatamente siguiente usan correctamente $R_3$.

Despejando $I_0$:
$$\mathcal{E} = I_0 (R_1 + R_3)$$

$$\boxed{I_0 = \frac{\mathcal{E}}{R_1 + R_3}}$$

---

#### Parte b) Carga máxima almacenada en $C_1$

Cuando el condensador $C_1$ se encuentra completamente cargado (régimen estacionario para $t \to \infty$), deja de circular corriente por la malla ($I = 0$). En consecuencia, no hay caída de potencial en las resistencias $R_1$ ni $R_3$, y la LVK sobre la malla izquierda se reduce a:
$$\mathcal{E} - \frac{Q_{\text{máx}}}{C_1} = 0$$

Despejando la carga máxima:
$$\boxed{Q_{\text{máx}} = \mathcal{E} C_1}$$

---

#### Parte c) Carga $q_1(t)$ en $C_1$ durante la carga

Para todo $t \ge 0$ con el interruptor en la posición $1$, la ley de mallas de Kirchhoff sobre la malla izquierda entrega:
$$\mathcal{E} - I R_1 - \frac{q_1}{C_1} - I R_3 = 0$$

Como la corriente positiva aumenta la carga en $C_1$, se tiene $I = \frac{dq_1}{dt}$. Sustituyendo:
$$\mathcal{E} - (R_1 + R_3)\frac{dq_1}{dt} - \frac{q_1}{C_1} = 0$$

Esta ecuación diferencial se resuelve por separación de variables:
$$(R_1 + R_3)\frac{dq_1}{dt} = \mathcal{E} - \frac{q_1}{C_1} = \frac{\mathcal{E} C_1 - q_1}{C_1}$$
$$\frac{dq_1}{\mathcal{E} C_1 - q_1} = \frac{dt}{(R_1 + R_3)C_1}$$

Integrando desde la condición inicial $q_1(0) = 0$ hasta $q_1(t)$:
$$\int_0^{q_1(t)} \frac{dq_1'}{\mathcal{E} C_1 - q_1'} = \int_0^t \frac{dt'}{(R_1 + R_3)C_1}$$
$$-\ln\left(\frac{\mathcal{E} C_1 - q_1(t)}{\mathcal{E} C_1}\right) = \frac{t}{(R_1 + R_3)C_1}$$

Exponenciando y despejando $q_1(t)$:
$$1 - \frac{q_1(t)}{\mathcal{E} C_1} = e^{-t/\tau_1} \implies q_1(t) = \mathcal{E} C_1 \left(1 - e^{-t/\tau_1}\right)$$
donde la constante de tiempo de carga es $\tau_1 = C_1 R_{\text{eq},1}$, con $R_{\text{eq},1} = R_1 + R_3$.

> **Nota:** la solución oficial manuscrita omite el signo menos en el exponente (escribe $1 - e^{t/\tau}$); lo correcto es $1 - e^{-t/\tau_1}$ porque la carga debe crecer exponencialmente hacia $\mathcal{E} C_1$ cuando $t \to \infty$ en lugar de diverger.

$$\boxed{q_1(t) = \mathcal{E} C_1 \left(1 - e^{-t/\tau_1}\right), \qquad \tau_1 = C_1(R_1 + R_3)}$$

---

#### Parte d) Carga en $C_1$ tras cambiar el interruptor a la posición $2$

Luego de mucho tiempo en la posición $1$, $C_1$ alcanza su carga máxima y $C_2$ sigue descargado. Reubicando el origen temporal en el instante en que se cambia el interruptor a la posición $2$ (y denotando la carga de $C_1$ en esta etapa como $Q_1'(t)$), las condiciones iniciales son:
$$Q_1'(0) = \mathcal{E} C_1, \qquad Q_2(0) = 0$$

Al pasar el interruptor a la posición $2$, la fuente $\mathcal{E}$ y $R_3$ quedan desconectadas, formándose una única malla cerrada con $R_1$, $C_1$, $R_2$ y $C_2$. El condensador $C_1$ actúa como batería y comienza a descargarse mientras $C_2$ se carga.

Tomando una corriente $I$ en sentido horario por la malla derecha (sube por $C_1$ y $R_1$, baja por $R_2$ y $C_2$), la LVK da:
$$\frac{Q_1'}{C_1} - R_2 I - R_1 I - \frac{Q_2}{C_2} = 0$$

Por conservación de la carga en las placas superiores conectadas entre sí (y análogamente en las inferiores):
$$Q_1'(t) + Q_2(t) = \mathcal{E} C_1$$

Derivando respecto del tiempo:
$$\frac{dQ_1'}{dt} + \frac{dQ_2}{dt} = 0 \implies I = -\frac{dQ_1'}{dt} = +\frac{dQ_2}{dt}$$

Reemplazando $Q_2 = \mathcal{E} C_1 - Q_1'$ y $I = -\frac{dQ_1'}{dt}$ en la ecuación de malla (donde las resistencias quedan en serie, $R_{\text{eq}} = R_1 + R_2$, y los condensadores también forman una capacitancia equivalente en serie):
$$\frac{Q_1'}{C_1} - \frac{\mathcal{E} C_1 - Q_1'}{C_2} + (R_1 + R_2)\frac{dQ_1'}{dt} = 0$$
$$Q_1'\left(\frac{1}{C_1} + \frac{1}{C_2}\right) - \frac{\mathcal{E} C_1}{C_2} + (R_1 + R_2)\frac{dQ_1'}{dt} = 0$$

Introduciendo la capacitancia equivalente serie $C_{\text{eq}}$ y la resistencia equivalente $R_{\text{eq}}$:
$$\frac{1}{C_{\text{eq}}} = \frac{1}{C_1} + \frac{1}{C_2} \implies C_{\text{eq}} = \frac{C_1 C_2}{C_1 + C_2}, \qquad R_{\text{eq}} = R_1 + R_2$$

La ecuación diferencial queda:
$$R_{\text{eq}} \frac{dQ_1'}{dt} + \frac{Q_1'}{C_{\text{eq}}} - \frac{\mathcal{E} C_1}{C_2} = 0$$

Multiplicando por $C_{\text{eq}}$:
$$R_{\text{eq}} C_{\text{eq}} \frac{dQ_1'}{dt} + Q_1' - \frac{\mathcal{E} C_1 C_{\text{eq}}}{C_2} = 0$$

La solución general de esta ecuación lineal de primer orden con coeficientes constantes es de la forma:
$$Q_1'(t) = A\, e^{-t/\tau} + B, \qquad \tau = R_{\text{eq}} C_{\text{eq}} = (R_1 + R_2)\frac{C_1 C_2}{C_1 + C_2}$$

1. **Cálculo de $B$ (límite estacionario $t \to \infty$):**  
   Cuando $t \to \infty$, el circuito alcanza el equilibrio ($\frac{dQ_1'}{dt} = 0$ y $Q_1'(\infty) = B$). Sustituyendo en la ecuación diferencial:
   $$0 + B - \frac{\mathcal{E} C_1 C_{\text{eq}}}{C_2} = 0 \implies B = \frac{\mathcal{E} C_1 C_{\text{eq}}}{C_2} = \frac{\mathcal{E} C_1^2}{C_1 + C_2}$$

2. **Cálculo de $A$ (condición inicial en $t = 0$):**  
   Evaluando $Q_1'(0) = \mathcal{E} C_1$:
   $$Q_1'(0) = \mathcal{E} C_1 = A + \frac{\mathcal{E} C_1 C_{\text{eq}}}{C_2}$$
   $$A = \mathcal{E} C_1 - \frac{\mathcal{E} C_1 C_{\text{eq}}}{C_2} = \mathcal{E} C_1\left(1 - \frac{C_1}{C_1 + C_2}\right) = \mathcal{E} \frac{C_1 C_2}{C_1 + C_2} = \mathcal{E} C_{\text{eq}}$$

Por lo tanto, el resultado final es:
$$\boxed{Q_1'(t) = \mathcal{E} C_{\text{eq}}\, e^{-t/\tau} + \frac{\mathcal{E} C_1 C_{\text{eq}}}{C_2} = \frac{\mathcal{E} C_1}{C_1 + C_2}\left(C_2\, e^{-t/\tau} + C_1\right)}$$
con $\tau = (R_1 + R_2)\frac{C_1 C_2}{C_1 + C_2}$ y $C_{\text{eq}} = \frac{C_1 C_2}{C_1 + C_2}$.

Cuando $t \to \infty$, $C_1$ no se descarga por completo, sino que la carga inicial se reparte con $C_2$ hasta que ambos condensadores alcanzan el mismo voltaje.

**Verificación:**
- **Unidades:** $[I_0] = \text{V}/\Omega = \text{A}$; $[Q] = \text{V}\cdot\text{F} = \text{C}$; $[\tau] = \Omega\cdot\text{F} = \text{s}$. Correcto.
- **Límites en parte c):** En $t = 0$, $q_1(0) = 0$ y $\frac{dq_1}{dt}(0) = \frac{\mathcal{E}C_1}{(R_1+R_3)C_1} = \frac{\mathcal{E}}{R_1+R_3} = I_0$. Para $t \to \infty$, $q_1 \to \mathcal{E} C_1 = Q_{\text{máx}}$.
- **Límites en parte d):** En $t = 0$, $Q_1'(0) = \mathcal{E}\frac{C_1 C_2 + C_1^2}{C_1 + C_2} = \mathcal{E} C_1$. Para $t \to \infty$, $Q_1'(\infty) = \frac{\mathcal{E} C_1^2}{C_1 + C_2}$ y $Q_2(\infty) = \mathcal{E} C_1 - Q_1'(\infty) = \frac{\mathcal{E} C_1 C_2}{C_1 + C_2}$, de modo que $\frac{Q_1'(\infty)}{C_1} = \frac{Q_2(\infty)}{C_2} = \frac{\mathcal{E} C_1}{C_1 + C_2}$ (igualdad de voltajes en equilibrio).

---

## Problema 2

En el plano $x$-$y$ considere un punto $P$, con coordenadas $(L, L)$, y dos configuraciones de corrientes estacionarias [figuras (a) y (b)]. Se pide calcular el campo magnético total en el punto $P$, en cada una de dichas configuraciones.

a) Un alambre con corriente $i_0$ que desciende por el eje $y$ desde infinito, hasta el origen, para luego continuar por el eje $x$ hasta el infinito, como se ve en la figura (a).  
b) Un alambre con corriente $2i_0$ que viene de infinito por la diagonal, $y = x$, se bifurca en dos alambres: uno en el sentido positivo del eje $x$ y el otro en el sentido positivo del eje $y$, como se muestra en la figura (b). Cada uno de ellos conduce una corriente $i_0$.

*Ayuda:*
$$\int \frac{dx}{\left(A + (B - x)^2\right)^{3/2}} = \frac{1}{A} \frac{x - B}{\left(A + (B - x)^2\right)^{1/2}} + C$$

> **[Figura]:** Dos gráficos en el plano cartesiano $x$-$y$ ($\hat{x}$ hacia la derecha, $\hat{y}$ hacia arriba), con el punto de observación $P$ ubicado en el primer cuadrante en las coordenadas $(L, L)$ (proyectado mediante líneas punteadas a $x = L$ e $y = L$):
> - **Figura (a):** Alambre continuo en ángulo recto: una rama semi-infinita desciende por el semieje $+y$ desde $y = +\infty$ hasta el origen $(0,0)$ con corriente $i_0$ en dirección $-\hat{y}$, y luego continúa por el semieje $+x$ desde $(0,0)$ hasta $x = +\infty$ con corriente $i_0$ en dirección $+\hat{x}$.
> - **Figura (b):** Alambre con bifurcación en el origen: una rama semi-infinita viene desde el infinito a lo largo de la diagonal $y = x$ en el tercer cuadrante ($x < 0, y < 0$) conduciendo una corriente $2i_0$ hacia el origen $(0,0)$, donde se divide en dos ramas semi-infinitas de corriente $i_0$ cada una: una asciende por el semieje $+y$ hacia $y = +\infty$ (dirección $+\hat{y}$) y la otra avanza por el semieje $+x$ hacia $x = +\infty$ (dirección $+\hat{x}$).

### Solución

**Idea:** Aplicamos la ley de Biot-Savart,
$$\vec{B}(\vec{r}) = \frac{\mu_0}{4\pi} \int \frac{I\, d\vec{l}' \times (\vec{r} - \vec{r}')}{|\vec{r} - \vec{r}'|^3}$$
por superposición sobre cada tramo recto de corriente. El punto de evaluación está fijo en $\vec{r} = L\hat{x} + L\hat{y}$ (con $L > 0$).

#### Parte a) Alambre en ángulo recto

Dividimos la configuración en dos tramos semi-infinitos:

1. **Tramo vertical superior (semieje $+y$, corriente descendiendo hacia el origen):**  
   Parametrizamos un punto de la fuente sobre el semieje $+y$ con $y' \in [0, \infty)$:
   $$\vec{r}' = y'\,\hat{y}$$
   Dado que la corriente desciende desde $y' = +\infty$ hasta $y' = 0$ (sentido $-\hat{y}$), al integrar con $y'$ creciente de $0$ a $\infty$ el elemento de corriente apunta hacia abajo:
   $$d\vec{l}' = -dy'\,\hat{y}$$
   El vector desplazamiento hacia $P$ es:
   $$\vec{r} - \vec{r}' = L\hat{x} + L\hat{y} - y'\hat{y} = L\hat{x} + (L - y')\hat{y}$$
   con módulo $|\vec{r} - \vec{r}'| = \sqrt{L^2 + (L - y')^2}$.

   Calculamos el producto vectorial usando $\hat{y} \times \hat{x} = -\hat{z}$ y $\hat{y} \times \hat{y} = \vec{0}$:
   $$d\vec{l}' \times (\vec{r} - \vec{r}') = (-dy'\,\hat{y}) \times \left[L\hat{x} + (L - y')\hat{y}\right] = -L\, dy'\,(\hat{y} \times \hat{x}) = L\, dy'\,\hat{z}$$

   Sustituyendo en la ley de Biot-Savart:
   $$\vec{B}_y = \frac{\mu_0 i_0}{4\pi} \int_0^\infty \frac{L\, dy'\,\hat{z}}{\left(L^2 + (L - y')^2\right)^{3/2}}$$

   Usando la integral de la *Ayuda* con $A = L^2$ y $B = L$:
   $$\vec{B}_y = \frac{\mu_0 i_0 L}{4\pi}\,\hat{z} \left[ \frac{1}{L^2} \frac{y' - L}{\left(L^2 + (L - y')^2\right)^{1/2}} \right]_0^\infty$$

   Evaluamos los límites de integración:
   - Límite superior ($y' \to \infty$):
     $$\lim_{y' \to \infty} \frac{y' - L}{\left(L^2 + (L - y')^2\right)^{1/2}} = \lim_{y' \to \infty} \frac{1 - L/y'}{\left(L^2/y'^2 + (1 - L/y')^2\right)^{1/2}} = 1$$
   - Límite inferior ($y' = 0$, con $L > 0$):
     $$\frac{0 - L}{\left(L^2 + (L - 0)^2\right)^{1/2}} = \frac{-L}{\sqrt{2} L} = -\frac{1}{\sqrt{2}}$$

   Por lo tanto:
   $$\vec{B}_y = \frac{\mu_0 i_0 L}{4\pi}\,\hat{z} \left[ \frac{1}{L^2}(1) - \frac{1}{L^2}\left(-\frac{1}{\sqrt{2}}\right) \right] = \frac{\mu_0 i_0}{4\pi L} \left(1 + \frac{1}{\sqrt{2}}\right)\hat{z}$$

2. **Tramo horizontal (semieje $+x$, corriente hacia $+\infty$):**  
   Parametrizamos con $x' \in [0, \infty)$:
   $$\vec{r}' = x'\,\hat{x}, \qquad d\vec{l}' = dx'\,\hat{x}$$
   El producto vectorial es (usando $\hat{x} \times \hat{y} = +\hat{z}$):
   $$d\vec{l}' \times (\vec{r} - \vec{r}') = dx'\,\hat{x} \times (L\hat{x} + L\hat{y} - x'\hat{x}) = L\, dx'\,\hat{z}$$
   Resulta exactamente la misma integral con los mismos límites de integración:
   $$\vec{B}_x = \frac{\mu_0 i_0}{4\pi} \int_0^\infty \frac{L\, dx'\,\hat{z}}{\left(L^2 + (L - x')^2\right)^{3/2}} = \vec{B}_y$$

3. **Campo magnético total en $P$:**  
   $$\vec{B}_T = \vec{B}_x + \vec{B}_y = 2\vec{B}_y$$

$$\boxed{\vec{B}_T = \frac{\mu_0 i_0}{2\pi L} \left(1 + \frac{1}{\sqrt{2}}\right)\hat{z}}$$

---

#### Parte b) Alambre diagonal que se bifurca en el origen

Separamos la configuración en sus tres tramos:

1. **Tramo superior (semieje $+y$) y tramo horizontal (semieje $+x$):**  
   - El tramo superior es geométricamente idéntico al de la parte a), pero ahora la corriente $i_0$ circula en sentido contrario (hacia $+\hat{y}$). Por ello, su contribución es exactamente opuesta: $-\vec{B}_y$.
   - El tramo horizontal es idéntico al de la parte a) tanto en geometría como en sentido de corriente ($+\hat{x}$), por lo que su contribución es $+\vec{B}_x = +\vec{B}_y$.

   Sumando ambas ramas:
   $$\vec{B}_{x\text{ y }y} = -\vec{B}_y + \vec{B}_y = \vec{0}$$

2. **Tramo diagonal (recta $y = x$ en el tercer cuadrante, corriente $2i_0$):**  
   Todo punto sobre la recta $y' = x'$ se parametriza como:
   $$\vec{r}' = x'(\hat{x} + \hat{y}), \qquad d\vec{l}' = dx'(\hat{x} + \hat{y}) \qquad (x' \in (-\infty, 0])$$
   El vector desde el elemento de corriente hasta $P = (L, L)$ es:
   $$\vec{r} - \vec{r}' = L(\hat{x} + \hat{y}) - x'(\hat{x} + \hat{y}) = (L - x')(\hat{x} + \hat{y})$$
   Como $d\vec{l}'$ y $(\vec{r} - \vec{r}')$ tienen la misma dirección (son vectores colineales a lo largo de $\hat{x} + \hat{y}$), su producto vectorial se anula idénticamente:
   $$d\vec{l}' \times (\vec{r} - \vec{r}') = \vec{0} \implies \vec{B}_{\text{diag}} = \vec{0}$$

3. **Campo magnético total en $P$:**  
   $$\vec{B}_T = \vec{B}_{x\text{ y }y} + \vec{B}_{\text{diag}} = \vec{0}$$

$$\boxed{\vec{B}_T = \vec{0}}$$

**Verificación:**
- **Unidades:** $[\mu_0 i_0 / L] = (\text{T}\cdot\text{m}/\text{A})\cdot \text{A} / \text{m} = \text{T}$ (Tesla). Correcto.
- **Regla de la mano derecha en a):** Al bajar por el eje $+y$, el pulgar apunta en $-\hat{y}$ y en el primer cuadrante los dedos salen de la hoja ($+\hat{z}$); al avanzar por el eje $+x$, el pulgar apunta en $+\hat{x}$ y por encima del eje ($y = L > 0$) los dedos también salen de la hoja ($+\hat{z}$), confirmando que ambos tramos se suman constructivamente en $+\hat{z}$.
- **Simetría en b):** El punto $P = (L, L)$ pertenece a la recta $y = x$, que es eje de simetría de la bifurcación (al reflejar respecto a $y = x$, el tramo $+x$ pasa al $+y$ manteniendo la misma corriente $i_0$, lo cual invierte la orientación respecto a la normal del plano $x$-$y$ y cancela el campo en $z$); además, sobre la diagonal misma el alambre entrante es colineal con $\vec{r} - \vec{r}'$ y aporta cero.

---

## Problema 3

Un conductor cilíndrico infinito de radio $R$ con su eje de simetría coincidente con la dirección $z$, conduce una densidad de corriente no uniforme $\vec{J} = k r^2\,\hat{z}$, donde $k$ es una constante desconocida y $r$ es la distancia radial al eje de simetría del cilindro. Además una espira rectangular de lados $b$ y $c$ con corriente constante $I_2$ es colocada paralela al cilindro a una distancia $a$, como lo muestra la figura. Considere que la dirección $\hat{x}$ es perpendicular a la hoja, de esta manera, la espira rectangular está sobre el plano $y$-$z$.

Si el cilindro conduce una corriente total $I_1$:

a) Determine la constante $k$ en función de $I_1$ y $R$.  
b) Encuentre el campo magnético originado por el cilindro para cualquier valor de $r$. Puede dejar su resultado en función de $k$.  
c) Calcule la fuerza total y el torque magnético que el cilindro ejerce sobre la espira. Puede dejar su resultado en función de $k$.

> **[Figura]:** Vista frontal en el plano $y$-$z$ (con el eje $+\hat{x}$ indicado mediante $\odot \hat{x}$, saliendo perpendicularmente de la hoja, $+\hat{z}$ vertical hacia arriba y $+\hat{y}$ horizontal hacia la derecha). A la izquierda, un cilindro macizo infinito de radio $R$ centrado en el eje $z$ transporta una densidad de corriente $\vec{J}$ dirigida hacia arriba ($+\hat{z}$). A la derecha del cilindro, en el plano $y$-$z$, hay una espira rectangular de ancho horizontal $b$ (a lo largo de $y$) y alto vertical $c$ (a lo largo de $z$). El lado vertical izquierdo de la espira se sitúa a una distancia horizontal $a$ medida desde el eje de simetría $z$ del cilindro ($a > R$), por lo que la espira abarca $y \in [a, a + b]$. La corriente $I_2$ circula por la espira en sentido horario: hacia arriba ($+\hat{z}$) por el lado izquierdo ($y = a$), hacia la derecha ($+\hat{y}$) por el lado superior, hacia abajo ($-\hat{z}$) por el lado derecho ($y = a + b$) y hacia la izquierda ($-\hat{y}$) por el lado inferior.

### Solución

**Idea:** Por simetría cilíndrica alrededor del eje $z$, el campo magnético del conductor depende únicamente de la distancia radial $r$ y apunta en dirección azimutal $\hat{\theta}$, por lo que se calcula directamente mediante la ley de Ampère. La fuerza sobre la espira rectangular se determina integrando la fuerza de Lorentz $\vec{F} = I_2 \oint d\vec{l} \times \vec{B}$ sobre sus cuatro lados rectos, mientras que el torque respecto al centro de la espira se analiza mediante la alineación entre el momento dipolar magnético $\vec{\mu}$ y el campo $\vec{B}$ (y se confirma por simetría mediante integración directa).

#### Parte a) Determinación de la constante $k$

La corriente total $I_1$ que atraviesa la sección transversal circular de radio $R$ del cilindro está dada por el flujo de $\vec{J}$ a través de dicha área ($d\vec{A} = r\, dr\, d\theta\,\hat{z}$):
$$I_1 = \iint_S \vec{J} \cdot d\vec{A} = \int_0^{2\pi} \int_0^R (k r^2\,\hat{z}) \cdot (r\, dr\, d\theta\,\hat{z}) = \int_0^{2\pi} \int_0^R k r^3\, dr\, d\theta$$

Resolviendo las integrales:
$$I_1 = 2\pi k \left[\frac{r^4}{4}\right]_0^R = 2\pi k \frac{R^4}{4} = \frac{\pi k R^4}{2}$$

Despejando $k$:
$$k = \frac{4 I_1}{2\pi R^4} = \frac{2 I_1}{\pi R^4}$$

$$\boxed{k = \frac{2 I_1}{\pi R^4}}$$

*(Nota de lectura del manuscrito: en un paso intermedio de la pauta manuscrita aparece momentáneamente $R^3/3$, que el mismo ayudante corrige en las líneas siguientes a $r^4/4$ para obtener el resultado correcto $k = \frac{2I_1}{\pi R^4}$.)*

---

#### Parte b) Campo magnético para todo $r$

Por simetría cilíndrica (traslacional en $z$ y rotacional en $\theta$) con $\vec{J}$ en $+\hat{z}$, el campo magnético tiene la forma $\vec{B}(r) = B(r)\,\hat{\theta}$. Tomamos curvas amperianas circulares concéntricas de radio $r$ perpendiculares al eje $z$, de modo que:
$$\oint \vec{B} \cdot d\vec{l} = B(r)\,(2\pi r) = \mu_0 I_{\text{enc}}$$

1. **Región interior ($r \le R$):**  
   La corriente encerrada dentro del radio $r$ es:
   $$I_{\text{enc}}(r) = \int_0^{2\pi} \int_0^r k r'^3\, dr'\, d\theta = 2\pi k \frac{r^4}{4} = \frac{\pi k r^4}{2}$$

   Aplicando la ley de Ampère:
   $$B(2\pi r) = \mu_0 \cdot 2\pi k \frac{r^4}{4} \implies B(r) = \frac{\mu_0 k r^3}{4}$$

   En forma vectorial (y expresado también en términos de $I_1 = \frac{\pi k R^4}{2}$):
   $$\vec{B}(r) = \frac{\mu_0 k r^3}{4}\,\hat{\theta} = \frac{\mu_0 I_1 r^3}{2\pi R^4}\,\hat{\theta} \qquad (r \le R)$$

2. **Región exterior ($r > R$):**  
   Toda la corriente del cilindro queda encerrada:
   $$I_{\text{enc}} = 2\pi k \frac{R^4}{4} = I_1$$

   Aplicando la ley de Ampère:
   $$B(2\pi r) = \mu_0 \cdot 2\pi k \frac{R^4}{4} \implies B(r) = \frac{\mu_0 k R^4}{4 r}$$

   En forma vectorial:
   $$\vec{B}(r) = \frac{\mu_0 k R^4}{4 r}\,\hat{\theta} = \frac{\mu_0 I_1}{2\pi r}\,\hat{\theta} \qquad (r > R)$$

$$\boxed{\vec{B}(r) = \begin{cases} \dfrac{\mu_0 k r^3}{4}\,\hat{\theta} = \dfrac{\mu_0 I_1 r^3}{2\pi R^4}\,\hat{\theta}, & r \le R \\[2ex] \dfrac{\mu_0 k R^4}{4 r}\,\hat{\theta} = \dfrac{\mu_0 I_1}{2\pi r}\,\hat{\theta}, & r > R \end{cases}}$$

---

#### Parte c) Fuerza total y torque magnético sobre la espira

Como la espira se ubica en el semiplano $y > 0$ ($x = 0$, con $r = y \in [a, a+b]$ y $a > R$), sobre todos sus lados el versor radial coincide con $\hat{r} = +\hat{y}$ y el versor azimutal apunta entrando perpendicularmente a la hoja: $\hat{\theta} = -\hat{x}$ (verificando el sistema derecho $\hat{x} \times \hat{y} = \hat{z}$ y $\hat{r} \times \hat{\theta} = \hat{y} \times (-\hat{x}) = \hat{z}$).

1. **Fuerza magnética total $\vec{F}_T$:**  
   Numeramos los cuatro lados de la espira siguiendo el sentido horario de $I_2$: lado $1$ (izquierdo, en $r = a$, hacia $+\hat{z}$), lado $2$ (superior, de $a$ a $a+b$, hacia $+\hat{r}$), lado $3$ (derecho, en $r = a+b$, hacia $-\hat{z}$) y lado $4$ (inferior, de $a+b$ a $a$, hacia $-\hat{r}$).

   Usamos $\vec{F} = I_2 \oint d\vec{l} \times \vec{B}$, de modo que $\vec{F}_T = \vec{F}_1 + \vec{F}_2 + \vec{F}_3 + \vec{F}_4$:

   - **Lado $1$ (vertical izquierdo, en $r = a$, $z \in [0, c]$, $d\vec{l}_1 = dz\,\hat{z}$):**  
     Usando $\hat{z} \times \hat{\theta} = -\hat{r}$:
     $$\vec{F}_1 = I_2 \int_0^c dz\,(\hat{z} \times \hat{\theta})\, B(a) = -I_2 B(a) c\,\hat{r} = -\frac{\mu_0 I_1 I_2 c}{2\pi a}\,\hat{r}$$
   - **Lado $2$ (horizontal superior, $r \in [a, a+b]$, $d\vec{l}_2 = dr\,\hat{r}$):**  
     $$\vec{F}_2 = I_2 \int_a^{a+b} B(r)\, dr\,(\hat{r} \times \hat{\theta}) = +I_2 \hat{z} \int_a^{a+b} B(r)\, dr$$
   - **Lado $4$ (horizontal inferior, de $a+b$ hacia $a$, $d\vec{l}_4 = -dr\,\hat{r}$ al recorrer de $a$ a $a+b$):**  
     $$\vec{F}_4 = I_2 \int_a^{a+b} B(r)\, dr\,(-\hat{r} \times \hat{\theta}) = -I_2 \hat{z} \int_a^{a+b} B(r)\, dr = -\vec{F}_2$$
     Por lo tanto, $\vec{F}_2$ y $\vec{F}_4$ tienen la misma magnitud y signo opuesto, cancelándose entre sí ($\vec{F}_2 + \vec{F}_4 = \vec{0}$).
   - **Lado $3$ (vertical derecho, en $r = a+b$, corriente en $-\hat{z}$):**  
     Usando $(-\hat{z}) \times \hat{\theta} = +\hat{r}$:
     $$\vec{F}_3 = I_2 \int_0^c dz\,(-\hat{z} \times \hat{\theta})\, B(a+b) = +I_2 B(a+b) c\,\hat{r} = +\frac{\mu_0 I_1 I_2 c}{2\pi (a+b)}\,\hat{r}$$

   Sumando las contribuciones netas (con $\hat{r} = \hat{y}$ en la ubicación de la espira):
   $$\vec{F}_T = \vec{F}_1 + \vec{F}_3 = \left(-\frac{\mu_0 I_1 I_2 c}{2\pi a} + \frac{\mu_0 I_1 I_2 c}{2\pi (a+b)}\right)\hat{y} = -\frac{\mu_0 I_1 I_2 b c}{2\pi a(a+b)}\,\hat{y}$$

   Expresado equivalentemente en función de $k$ (mediante $I_1 = \frac{\pi k R^4}{2}$):
   $$\vec{F}_T = \frac{\mu_0 k R^4 I_2 c}{4}\left(\frac{1}{a+b} - \frac{1}{a}\right)\hat{y} = -\frac{\mu_0 k R^4 I_2 b c}{4 a(a+b)}\,\hat{y}$$

   $$\boxed{\vec{F}_T = \left(-\frac{\mu_0 I_1 I_2 c}{2\pi a} + \frac{\mu_0 I_1 I_2 c}{2\pi (a+b)}\right)\hat{y} = -\frac{\mu_0 k R^4 I_2 b c}{4 a(a+b)}\,\hat{y}}$$

2. **Torque magnético $\vec{\tau}$:**  
   En la posición de la espira, el campo magnético $\vec{B}$ tiene dirección $\hat{\theta}$, es decir, **entrando perpendicularmente a la hoja**.  
   Por la regla de la mano derecha aplicada a la corriente horaria $I_2$ en la espira, el momento dipolar magnético $\vec{\mu} = I_2 \vec{A}$ también apunta **entrando a la hoja** (dirección $\hat{\theta}$).  

   Como $\vec{\mu}$ y $\vec{B}$ son paralelos (misma dirección y sentido), la expresión dipolar entrega:
   $$\vec{\tau} = \vec{\mu} \times \vec{B} = \vec{0}$$

   > **Nota:** en la solución oficial manuscrita se comete un lapsus de signo al identificar la dirección entrante a la hoja como $+\hat{x}$ en lugar de $-\hat{x}$ (dado que en la Figura 3 el eje $\odot \hat{x}$ sale de la hoja, la dirección entrante correcta es $\hat{\theta} = -\hat{x}$ para $\vec{B}$ y $\vec{\mu}$); como ambos vectores apuntan en $-\hat{x}$, siguen siendo paralelos. Además, aunque $\vec{\tau} = \vec{\mu}\times\vec{B}$ es estrictamente válida solo para un campo uniforme y aquí $\vec{B}(y) \propto 1/y$ varía con $y$, el cálculo directo del torque respecto al centro geométrico de la espira $\vec{r}_c = (a + b/2)\,\hat{y} + (c/2)\,\hat{z}$ confirma el mismo resultado: las fuerzas horizontales sobre los lados $1$ y $3$ son uniformes en $z$ y simétricas respecto a $z_c$ (torque nulo), y las fuerzas verticales sobre los lados $2$ y $4$ satisfacen $\vec{\tau}_2 + \vec{\tau}_4 = \vec{0}$ por simetría especular respecto a $z = c/2$, resultando $\vec{\tau}_{\text{centro}} = \vec{0}$.

   $$\boxed{\vec{\tau} = \vec{0}}$$

**Verificación:**
- **Continuidad de $\vec{B}$:** En $r = R$, ambas ramas coinciden en $\vec{B}(R) = \frac{\mu_0 k R^3}{4}\,\hat{\theta} = \frac{\mu_0 I_1}{2\pi R}\,\hat{\theta}$. Correcto.
- **Unidades:** $[k] = \text{A}/\text{m}^4$; $[B] = (\text{T}\cdot\text{m}/\text{A})(\text{A}/\text{m}^4)\text{m}^3 = \text{T}$; $[F_T] = (\text{T}\cdot\text{m}/\text{A})\text{A}^2 \cdot \text{m}/\text{m} = \text{N}$. Correcto.
- **Signo de $\vec{F}_T$:** Como $a < a + b$, resulta $F_{T,y} < 0$ (fuerza neta hacia $-\hat{y}$, atractiva hacia el cilindro). Esto es físicamente consistente porque la corriente en el lado más cercano ($y = a$) es paralela a $I_1$ (atracción) y experimenta un campo más intenso que la corriente antiparalela en el lado más lejano ($y = a + b$, repulsión).

---

## Resumen de resultados

| Problema | Magnitud requerida | Resultado analítico |
| :--- | :--- | :--- |
| **P1 (a)** | Corriente inicial $I_0$ ($t = 0^+$) | $I_0 = \dfrac{\mathcal{E}}{R_1 + R_3}$ |
| **P1 (b)** | Carga máxima $Q_{\text{máx}}$ en $C_1$ | $Q_{\text{máx}} = \mathcal{E} C_1$ |
| **P1 (c)** | Carga $q_1(t)$ durante la carga | $q_1(t) = \mathcal{E} C_1\left(1 - e^{-t/\tau_1}\right), \quad \tau_1 = C_1(R_1 + R_3)$ |
| **P1 (d)** | Carga $Q_1'(t)$ en posición $2$ | $Q_1'(t) = \mathcal{E} C_{\text{eq}}\, e^{-t/\tau} + \dfrac{\mathcal{E} C_1 C_{\text{eq}}}{C_2}, \quad C_{\text{eq}} = \dfrac{C_1 C_2}{C_1 + C_2}, \quad \tau = (R_1 + R_2)C_{\text{eq}}$ |
| **P2 (a)** | Campo magnético $\vec{B}_T$ en $P(L,L)$ | $\vec{B}_T = \dfrac{\mu_0 i_0}{2\pi L}\left(1 + \dfrac{1}{\sqrt{2}}\right)\hat{z}$ |
| **P2 (b)** | Campo magnético $\vec{B}_T$ en $P(L,L)$ | $\vec{B}_T = \vec{0}$ |
| **P3 (a)** | Constante $k$ | $k = \dfrac{2 I_1}{\pi R^4}$ |
| **P3 (b)** | Campo magnético $\vec{B}(r)$ ($r \le R$) | $\vec{B}(r) = \dfrac{\mu_0 k r^3}{4}\,\hat{\theta} = \dfrac{\mu_0 I_1 r^3}{2\pi R^4}\,\hat{\theta}$ |
| **P3 (b)** | Campo magnético $\vec{B}(r)$ ($r > R$) | $\vec{B}(r) = \dfrac{\mu_0 k R^4}{4 r}\,\hat{\theta} = \dfrac{\mu_0 I_1}{2\pi r}\,\hat{\theta}$ |
| **P3 (c)** | Fuerza magnética total $\vec{F}_T$ | $\vec{F}_T = -\dfrac{\mu_0 I_1 I_2 b c}{2\pi a(a+b)}\,\hat{y} = -\dfrac{\mu_0 k R^4 I_2 b c}{4 a(a+b)}\,\hat{y}$ |
| **P3 (c)** | Torque magnético $\vec{\tau}$ (respecto al centro) | $\vec{\tau} = \vec{0}$ |
