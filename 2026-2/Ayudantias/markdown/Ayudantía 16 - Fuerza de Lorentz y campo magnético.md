# Ayudantía 16 — Fuerza de Lorentz y campo magnético

> Clases relacionadas: [Clase 09 - Potencia, circuitos de resistencias y circuito RC](../../Clases/markdown/Clase%2009%20-%20Potencia%2C%20circuitos%20de%20resistencias%20y%20circuito%20RC.md), [Clase 10 - Campo Magnetico](../../Clases/markdown/Clase%2010%20-%20Campo%20Magnetico.md)

---

## Problema 1

En $t = 0$ el interruptor del circuito mostrado abajo se cierra. Obtenga las cargas en los capacitores, y las corrientes que fluyen por las resistencias (*en el original: "que fluyen por las resistencias que fluyen por las resistencias"*), si los condensadores inicialmente estaban descargados.

> **[Figura]:** Circuito de dos mallas conectado a una fuente de fem ideal continua $\varepsilon$ con un interruptor $S$ en serie sobre el riel inferior. El circuito consta de dos ramas conectadas en paralelo directamente entre los terminales de la fuente:
> - **Rama superior (malla 1):** Contiene una resistencia $R_1$ en serie con un condensador de capacitancia $C_1$.
> - **Rama intermedia/inferior (malla 2):** Contiene un condensador de capacitancia $C_2$ en serie con una resistencia $R_2$.
> Ambas ramas en paralelo comparten los mismos nodos de alimentación que se conectan a la fuente de voltaje $\varepsilon$ una vez cerrado el interruptor $S$.

### Solución

**Idea:** Al cerrar el interruptor $S$, ambas ramas quedan conectadas directamente en paralelo a la misma diferencia de potencial fija impuesta por la fuente ideal de fem $\varepsilon$. Al no existir resistencia interna ni elementos compartidos que acoplen las dos ramas, el circuito se desacopla en dos sistemas independientes de carga de un condensador en un circuito RC serie. Resolvemos cada malla planteando la Ley de Voltajes de Kirchhoff y resolviendo la ecuación diferencial ordinaria resultante mediante separación de variables sujeta a la condición de condensadores inicialmente descargados ($Q(0) = 0$).

#### 1. Malla 1 (Rama superior con $R_1$ y $C_1$)

1. **Ecuación de la malla (LVK):**  
   Recorriendo la malla que contiene la fuente $\varepsilon$, la resistencia $R_1$ y el condensador $C_1$:
   $$\sum V = 0 \implies \varepsilon - R_1 I_1(t) - V_{C_1}(t) = 0$$

   Sabiendo que $V_{C_1}(t) = \frac{Q_1(t)}{C_1}$ y que la corriente es la razón de cambio de la carga en las armaduras del condensador, $I_1(t) = \frac{dQ_1}{dt}$:
   $$\varepsilon - R_1 \frac{dQ_1}{dt} - \frac{Q_1}{C_1} = 0$$
   $$R_1 \frac{dQ_1}{dt} = \varepsilon - \frac{Q_1}{C_1} = \frac{\varepsilon C_1 - Q_1}{C_1}$$

2. **Resolución por separación de variables:**  
   $$\frac{dQ_1}{\varepsilon C_1 - Q_1} = \frac{dt}{R_1 C_1}$$

   Integrando desde el reposo inicial ($t = 0$, $Q_1(0) = 0$) hasta un tiempo genérico $t$:
   $$\int_0^{Q_1(t)} \frac{dq'}{\varepsilon C_1 - q'} = \int_0^t \frac{dt'}{R_1 C_1}$$
   $$\left[ -\ln(\varepsilon C_1 - q') \right]_0^{Q_1(t)} = \frac{t}{R_1 C_1}$$
   $$\ln\left(\frac{\varepsilon C_1 - Q_1(t)}{\varepsilon C_1}\right) = -\frac{t}{R_1 C_1}$$

3. **Carga y corriente en la rama 1:**  
   Despejando la carga $Q_1(t)$:
   $$\frac{\varepsilon C_1 - Q_1(t)}{\varepsilon C_1} = e^{-\frac{t}{R_1 C_1}} \implies Q_1(t) = \varepsilon C_1 \left(1 - e^{-\frac{t}{R_1 C_1}}\right)$$

   La corriente eléctrica $I_1(t)$ que fluye por la resistencia $R_1$ es la derivada temporal de $Q_1(t)$:
   $$I_1(t) = \frac{dQ_1}{dt} = \varepsilon C_1 \left( \frac{1}{R_1 C_1} e^{-\frac{t}{R_1 C_1}} \right) = \frac{\varepsilon}{R_1} e^{-\frac{t}{R_1 C_1}}$$
   con constante de tiempo $\tau_1 = R_1 C_1$.

$$\boxed{Q_1(t) = \varepsilon C_1 \left(1 - e^{-\frac{t}{R_1 C_1}}\right)}$$
$$\boxed{I_1(t) = \frac{\varepsilon}{R_1} e^{-\frac{t}{R_1 C_1}}}$$

---

#### 2. Malla 2 (Rama inferior con $R_2$ y $C_2$)

La rama formada por el condensador $C_2$ y la resistencia $R_2$ se encuentra sometida a la misma fem $\varepsilon$ en paralelo con la fuente. La ecuación de voltajes es idéntica en estructura:
$$\varepsilon - R_2 \frac{dQ_2}{dt} - \frac{Q_2}{C_2} = 0$$

Integrando bajo las mismas condiciones iniciales ($Q_2(0) = 0$):
$$\boxed{Q_2(t) = \varepsilon C_2 \left(1 - e^{-\frac{t}{R_2 C_2}}\right)}$$
$$\boxed{I_2(t) = \frac{\varepsilon}{R_2} e^{-\frac{t}{R_2 C_2}}}$$
con constante de tiempo $\tau_2 = R_2 C_2$.

**Verificación:**
- En $t = 0$: $Q_1(0) = Q_2(0) = 0$; $I_1(0) = \frac{\varepsilon}{R_1}$, $I_2(0) = \frac{\varepsilon}{R_2}$. Un condensador descargado actúa como un cortocircuito perfecto al instante inicial.
- En $t \to \infty$: $Q_1(\infty) = \varepsilon C_1$, $Q_2(\infty) = \varepsilon C_2$; $I_1(\infty) = I_2(\infty) = 0$. Un condensador completamente cargado actúa como un circuito abierto.

---

## Problema 2

Se lanza un electrón con velocidad inicial $\vec{v}_0$ en el medio de dos placas entre las cuales existe un campo magnético $\vec{B}$ constante (entrando a la hoja). Ignore todo efecto gravitacional.

a) ¿Hacia dónde se deflecta la trayectoria del electrón?  
b) ¿Cuál es la magnitud de la velocidad si la partícula choca exactamente con el fin de las placas?

> **[Figura]:** Dos placas metálicas horizontales y paralelas de longitud $l$, separadas verticalmente una distancia $d$. En la región comprendida entre ambas placas existe un campo magnético uniforme $\vec{B}$ perpendicular al plano, con sentido entrando a la hoja ($\vec{B} = -B\,\hat{k}$). Un electrón (masa $m$, carga $q = -e$) ingresa por el extremo izquierdo en el punto medio de la separación vertical ($y_0 = 0$, a una distancia $d/2$ de cada placa) con velocidad inicial puramente horizontal $\vec{v}_0 = v_0\,\hat{i}$.

### Solución

**Idea:** La fuerza que experimenta una partícula cargada en presencia de un campo magnético está dada por la ley de Lorentz: $\vec{F} = q(\vec{v} \times \vec{B})$. Como la fuerza magnética es siempre perpendicular a la velocidad instantánea ($\vec{F} \perp \vec{v}$), la potencia desarrollada y el trabajo mecánico son estrictamente nulos ($P = \vec{F} \cdot \vec{v} = 0 \implies W = 0$), lo que implica por el teorema del trabajo y la energía que la rapidez $v = \|\vec{v}\|$ permanece constante. Al ser la velocidad inicial perpendicular al campo magnético uniforme, la trayectoria es un arco de circunferencia en el plano de movimiento, donde la fuerza magnética suministra la aceleración centrípeta: $F_L = F_c \implies e v B = m \frac{v^2}{R}$.

#### Parte a) Sentido de deflexión del electrón

1. **Definición de sistema coordenado:**  
   - Eje $X$ ($\hat{i}$): horizontal hacia la derecha, en la dirección de la velocidad de ingreso.
   - Eje $Y$ ($\hat{j}$): vertical hacia arriba.
   - Eje $Z$ ($\hat{k}$): perpendicular al plano, saliendo de la hoja.  
   Por lo tanto, un vector entrando a la hoja tiene dirección $-\hat{k}$.

2. **Cálculo de la fuerza magnética de Lorentz:**  
   $$\vec{v}_0 = v_0\,\hat{i}$$
   $$\vec{B} = -B\,\hat{k}$$
   $$\vec{F} = q (\vec{v}_0 \times \vec{B}) = (-e) \left[ v_0\,\hat{i} \times (-B\,\hat{k}) \right]$$

   Evaluando el producto cruz fundamental:
   $$\hat{i} \times (-\hat{k}) = -(\hat{i} \times \hat{k}) = -(-\hat{j}) = +\hat{j}$$

   Multiplicando por la carga negativa del electrón ($q = -e$):
   $$\vec{F} = (-e) v_0 B\,\hat{j} = -e v_0 B\,\hat{j}$$

   La fuerza magnética inicial apunta en el sentido negativo del eje $Y$ ($-\hat{j}$). Por lo tanto, el electrón experimenta una aceleración hacia abajo.

$$\boxed{\text{El electrón se deflecta hacia abajo (hacia la placa inferior)}}$$

---

#### Parte b) Magnitud de la velocidad si choca con el extremo de las placas

1. **Dinámica circular y radio de curvatura:**  
   Igualando la fuerza magnética con la fuerza centrípeta:
   $$F_L = m a_c \implies e v B = m \frac{v^2}{R}$$
   $$v = \frac{e B R}{m} \qquad \text{o bien} \qquad R = \frac{m v}{e B}$$

2. **Geometría de la trayectoria circular:**  
   Ubicamos el origen $(0,0)$ en el punto de ingreso del electrón, equidistante de ambas placas.
   - La placa superior se encuentra en $y = +d/2$.
   - La placa inferior se encuentra en $y = -d/2$.
   - El extremo final de las placas se encuentra en la coordenada horizontal $x = l$.

   Dado que la trayectoria se desvía hacia abajo y en el origen la velocidad es puramente horizontal, la tangente a la curva en $(0,0)$ es horizontal ($\frac{dy}{dx} = 0$). En consecuencia, el centro de curvatura de la circunferencia se ubica verticalmente debajo del punto de ingreso, en las coordenadas $(0, -R)$.

   La ecuación de la circunferencia es:
   $$(x - 0)^2 + (y - (-R))^2 = R^2 \implies x^2 + (y + R)^2 = R^2$$

3. **Condición de impacto en el extremo de la placa inferior:**  
   El electrón choca en el extremo final de la placa inferior, es decir, en el punto:
   $$(x,\, y) = \left(l,\, -\frac{d}{2}\right)$$

   Sustituyendo estas coordenadas en la ecuación de la circunferencia:
   $$l^2 + \left(-\frac{d}{2} + R\right)^2 = R^2$$
   $$l^2 + \frac{d^2}{4} - d R + R^2 = R^2$$

   Cancelando $R^2$ en ambos lados:
   $$l^2 + \frac{d^2}{4} - d R = 0 \implies d R = l^2 + \frac{d^2}{4} = \frac{4l^2 + d^2}{4}$$
   $$R = \frac{4l^2 + d^2}{4d}$$

4. **Cálculo de la rapidez $v$:**  
   Sustituyendo el radio geométrico $R$ en la relación dinámica $v = \frac{e B R}{m}$:
   $$v = \frac{e B}{m} \left( \frac{4l^2 + d^2}{4d} \right)$$

$$\boxed{v = \frac{e B}{m} \left(\frac{4l^2 + d^2}{4d}\right)}$$

**Verificación:**
- **Unidades:** $\left[\frac{e B}{m}\right] = \left[\frac{\text{C}\cdot\text{T}}{\text{kg}}\right] = \left[\text{s}^{-1}\right]$ (frecuencia ciclotrón). El factor geométrico tiene dimensiones $\left[\frac{\text{m}^2}{\text{m}}\right] = [\text{m}]$. Su producto tiene dimensiones de $[\text{m/s}]$, lo que corresponde a una rapidez.
- **Comportamiento límite:** Para que el choque ocurra a lo largo de placas muy largas ($l \gg d$), el radio $R \approx \frac{l^2}{d}$ debe ser muy grande, lo que requiere una velocidad $v \propto l^2$ extremadamente alta para que la deflexión vertical acumulada en la distancia $l$ no supere $d/2$. Si $l \to 0$, $R \to \frac{d}{4} < \frac{d}{2}$, indicando que chocaría antes de alcanzar la placa si la velocidad no es adecuada.

---

## Problema 3

Una partícula de masa $m$ con carga $q > 0$, ingresa horizontalmente a una región de largo $L$, donde existe un campo magnético $\vec{B} = B\,\hat{k}$, como se muestra en la figura:

a) Encuentre el valor crítico de $v$ tal que la partícula logre cruzar la zona de campo magnético.  
b) Dibuje las trayectorias para $v < v_{\text{crítico}}$, $v > v_{\text{crítico}}$ y $v = v_{\text{crítico}}$.

> **[Figura]:** Región vertical rectangular de ancho $L$ comprendida entre los planos verticales $x = 0$ y $x = L$. En el interior de la región existe un campo magnético uniforme constante $\vec{B} = B\,\hat{k}$.  
> El sistema de coordenadas indicado en la figura define:
> - Eje $X$ ($\hat{i}$): horizontal hacia la derecha.
> - Eje $Y$ ($\hat{j}$): vertical hacia abajo.
> - Eje $Z$ ($\hat{k}$): perpendicular al plano, con convención entrando a la hoja ($\otimes$).  
> Una partícula de masa $m$ y carga positiva $q > 0$ se aproxima desde la izquierda a lo largo de una línea recta horizontal e ingresa a la zona de campo magnético por el origen $(0,0)$ con velocidad inicial $\vec{v}_0 = v_0\,\hat{i}$.

### Solución

**Idea:** Al ingresar la partícula cargada a la zona con campo magnético uniforme, la fuerza de Lorentz perpendicular a su velocidad induce una aceleración centrípeta constante, generando un movimiento circular uniforme de radio $R = \frac{mv}{qB}$. La partícula penetra en la región una distancia horizontal máxima igual al radio de su órbita circular ($x_{\text{máx}} = R$). Para que logre atravesar completamente la región de ancho $L$ y salir por la cara derecha ($x = L$), el radio de giro debe ser al menos igual al espesor $L$. El valor crítico de la rapidez corresponde a la condición geométrica en la que el círculo es justamente tangente a la frontera exterior ($R = L$).

#### Parte a) Valor crítico de la rapidez $v_{\text{crítico}}$

1. **Sentido de la fuerza magnética:**  
   Con los ejes definidos en la figura ($\hat{i}$ hacia la derecha, $\hat{j}$ hacia abajo, $\hat{k}$ entrando a la hoja):
   $$\vec{v}_0 = v_0\,\hat{i}$$
   $$\vec{B} = B\,\hat{k}$$
   $$\vec{F} = q (\vec{v}_0 \times \vec{B}) = q v_0 B (\hat{i} \times \hat{k})$$

   Como $\hat{i} \times \hat{k} = -\hat{j}$, y dado que $\hat{j}$ apunta hacia abajo, el vector $-\hat{j}$ apunta **hacia arriba**:
   $$\vec{F} = -q v_0 B\,\hat{j}$$

   La fuerza desvía a la partícula hacia arriba (en dirección a valores decrecientes y negativos de $y$).

2. **Ecuaciones paramétricas de la trayectoria:**  
   Tomando el punto de ingreso como origen $(0,0)$, la trayectoria circular con velocidad inicial en $+\hat{i}$ y fuerza en $-\hat{j}$ tiene su centro en $(0, -R)$ y se parametriza como:
   $$x(t) = R \sin(\omega t)$$
   $$y(t) = -R(1 - \cos(\omega t))$$
   donde $\omega = \frac{q B}{m}$ es la frecuencia ciclotrón y $R = \frac{m v}{q B}$ es el radio de Larmor o radio de giro.

3. **Condición para cruzar la zona de largo $L$:**  
   La máxima coordenada en $X$ que la partícula puede alcanzar en su giro circular es:
   $$x_{\text{máx}} = R$$

   - Si $R < L$, la partícula alcanza su punto de retorno horizontal en $x = R < L$ y se devuelve completando una semicircunferencia, saliendo nuevamente por la cara de entrada ($x = 0$).
   - Para que la partícula alcance la frontera opuesta ($x = L$) y logre cruzar la región, se requiere que:
     $$R \ge L$$

   El valor crítico $v_{\text{crítico}}$ es aquel para el cual el radio de curvatura es exactamente igual al largo $L$:
   $$R_{\text{crítico}} = L \implies \frac{m v_{\text{crítico}}}{q B} = L$$

   Despejando $v_{\text{crítico}}$:
   $$v_{\text{crítico}} = \frac{q B L}{m}$$

$$\boxed{v_{\text{crítico}} = \frac{q B L}{m}}$$

---

#### Parte b) Descripción y análisis de las trayectorias

A continuación se detalla la trayectoria de la partícula en los tres regímenes requeridos:

1. **Caso subcrítico: $v < v_{\text{crítico}} \implies R < L$**  
   - **Trayectoria:** Semicircunferencia completa contenida íntegramente en la región $0 \le x \le R < L$.
   - **Comportamiento:** La partícula ingresa en $(0,0)$, se desvía hacia arriba alcanzando una penetración horizontal máxima $x_{\text{máx}} = R$ en $\omega t = \frac{\pi}{2}$ (donde $y = -R$). Luego gira hacia la izquierda y sale de la zona magnética a través de la misma cara de entrada ($x = 0$).
   - **Punto y velocidad de salida:** Sale en el punto $(0, -2R)$ con vector velocidad $\vec{v}_{\text{salida}} = -v\,\hat{i}$ (es decir, desviada $180^\circ$ respecto a su dirección inicial).

2. **Caso crítico: $v = v_{\text{crítico}} \implies R = L$**  
   - **Trayectoria:** Cuarto de circunferencia que alcanza tangencialmente el límite exterior de la zona de campo magnético.
   - **Comportamiento:** La partícula penetra en el campo hasta rozar justamente la frontera derecha en el punto $(x, y) = (L, -L)$. En dicho punto, el vector tangente a la trayectoria es puramente vertical ascendente ($\vec{v} = -v_{\text{crítico}}\,\hat{j}$), siendo tangente a la línea límite $x = L$.
   - **Salida:** En este punto límite $(L, -L)$, la partícula roza tangencialmente la frontera; si la zona termina en $x = L$, abandona la región en ese instante hacia $y < -L$. Si continúa confinada a la región $x \le L$, completa la semicircunferencia y regresa a la cara de entrada saliendo en $(0, -2L)$ con velocidad $-v_{\text{crítico}}\,\hat{i}$.

3. **Caso supercrítico: $v > v_{\text{crítico}} \implies R > L$**  
   - **Trayectoria:** Arco de circunferencia de radio $R > L$ que interseca la frontera derecha $x = L$.
   - **Comportamiento:** La partícula atraviesa con éxito la zona de campo magnético, saliendo por la cara derecha $x = L$ antes de completar un cuarto de vuelta.
   - **Ángulo y punto de salida:** El ángulo de deflexión $\alpha$ que forma el vector velocidad con la horizontal al cruzar la frontera $x = L$ satisface:
     $$\sin\alpha = \frac{L}{R} = \frac{v_{\text{crítico}}}{v} < 1$$
     La partícula emerge en la frontera $x = L$ a una altura vertical:
     $$y_{\text{salida}} = -R(1 - \cos\alpha) = -R\left(1 - \sqrt{1 - \left(\frac{L}{R}\right)^2}\right)$$
     con vector velocidad de salida:
     $$\vec{v}_{\text{salida}} = v \cos\alpha\,\hat{i} - v \sin\alpha\,\hat{j}$$
     Una vez fuera del campo magnético ($x > L$), la partícula prosigue en movimiento rectilíneo uniforme en esa misma dirección.

**Verificación:**
- **Unidades:** $[q B L / m] = [\text{C} \cdot \text{T} \cdot \text{m} / \text{kg}] = [\text{m/s}]$, dimensionalmente correcto.
- **Continuidad de regímenes:** Cuando $v \to v_{\text{crítico}}^+$, $\sin\alpha = \frac{v_{\text{crítico}}}{v} \to 1$, lo que da $\alpha \to 90^\circ$ (vector tangente vertical), empalmando de forma continua con la solución crítica. Para $v \to \infty$, $R \to \infty$ y $\alpha \to 0$, de modo que la partícula cruza prácticamente sin desviarse ($\vec{v}_{\text{salida}} \approx v\,\hat{i}$ y $y_{\text{salida}} \approx 0$).

---

## Resumen de resultados

| Problema | Inciso | Magnitud / Variable | Expresión / Resultado |
| :--- | :--- | :--- | :--- |
| **Problema 1** | Rama 1 | Carga $Q_1(t)$ | $\varepsilon C_1 \left(1 - e^{-t / (R_1 C_1)}\right)$ |
| | Rama 1 | Corriente $I_1(t)$ | $\dfrac{\varepsilon}{R_1} e^{-t / (R_1 C_1)}$ |
| | Rama 2 | Carga $Q_2(t)$ | $\varepsilon C_2 \left(1 - e^{-t / (R_2 C_2)}\right)$ |
| | Rama 2 | Corriente $I_2(t)$ | $\dfrac{\varepsilon}{R_2} e^{-t / (R_2 C_2)}$ |
| **Problema 2** | a) | Sentido de deflexión | Hacia abajo (hacia la placa inferior, en $-\hat{j}$) |
| | b) | Rapidez de impacto $v$ | $\dfrac{e B}{m} \left(\dfrac{4l^2 + d^2}{4d}\right)$ |
| **Problema 3** | a) | Rapidez crítica $v_{\text{crítico}}$ | $\dfrac{q B L}{m}$ |
| | b) | Régimen $v < v_{\text{crítico}}$ | Semicircunferencia ($R < L$), retorna a $x = 0$ en $y = -2R$ con $\vec{v} = -v\,\hat{i}$ |
| | b) | Régimen $v = v_{\text{crítico}}$ | Arco tangente a $x = L$ en $(L, -L)$ con $\vec{v} = -v_{\text{crítico}}\,\hat{j}$ |
| | b) | Régimen $v > v_{\text{crítico}}$ | Arco de radio $R > L$, cruza $x = L$ con deflexión $\sin\alpha = \frac{v_{\text{crítico}}}{v}$ |
