# Potencia, circuitos de resistencias y circuito RC

## Circuitos eléctricos

En esta clase se analizan circuitos eléctricos simples que contienen diversas combinaciones de baterías, resistores y capacitores (por ejemplo, las tarjetas de circuito impreso de los equipos electrónicos son redes de este tipo). El análisis de circuitos más complicados se simplifica si se utilizan las **leyes de Kirchhoff**, que son consecuencia de:

- la **ley de conservación de la energía** (ley de mallas), y
- la **ley de conservación de la carga eléctrica** en sistemas aislados (ley de nodos).

Se supone que la mayoría de los circuitos analizados está en **estado estacionario**: las corrientes son constantes en magnitud y dirección. La **corriente directa (CD)** es una corriente de dirección constante.

> **[Figura]:** a) Dos ampolletas $R_1$ y $R_2$ conectadas a los bornes $+$ y $-$ de una batería. b) Diagrama equivalente: $R_1$ y $R_2$ están en **paralelo** entre los nodos $a$ y $b$, alimentados por una batería $\Delta V$ (borne $+$ a la izquierda, unido a $a$). La corriente $I$ sale de la batería hacia $a$ y se divide en $I_1$ (por $R_1$) e $I_2$ (por $R_2$). Ambos resistores tienen la misma diferencia de potencial: $\Delta V_1=\Delta V_2=\Delta V$.

## Fuerza electromotriz

Cuando se usa una batería como fuente de energía se le llama **fuente de fuerza electromotriz** o, más comúnmente, **fuente de fem**. (El nombre "fuerza electromotriz" es un desafortunado equívoco histórico: no describe una fuerza, sino una diferencia de potencial, medida en volts.) La fem $\varepsilon$ de una batería es el **voltaje máximo posible** que puede suministrar entre sus terminales.

Todo circuito completo con corriente constante debe incluir algún dispositivo que provea una fem; tal dispositivo es una **fuente de fem**. Una fuente de fem obtiene energía eléctrica a partir de otra forma de energía, que puede ser:

- **Química** (batería o celda de combustible).
- **Mecánica** (generador).
- **Térmica** (termopila).
- **Radiante** (celda solar).

### Fuente real: resistencia interna

Una batería real tiene una **resistencia interna** $r$, en serie con la fem ideal.

> **[Figura]:** a) Circuito de una malla. Dentro de un recuadro (la batería real) están la fem $\varepsilon$ (borne $-$ en $a$, borne $+$ en $b$) y la resistencia interna $r$ (entre $c$ y $d$). Fuera del recuadro, la resistencia externa (carga) $R$ entre $e$ y $f$. La corriente $I$ circula en sentido horario: sube por el lado izquierdo, sale por $d$ y baja por el lado derecho hacia $R$. b) Gráfico del potencial $V$ al recorrer el circuito $a\to b\to c\to d\to e\to f$: en la fem el potencial sube bruscamente de $0$ a $\varepsilon$ ($a\to b$); se mantiene entre $b$ y $c$; cae una cantidad $Ir$ en la resistencia interna ($c\to d$) hasta el valor $IR$; se mantiene constante por el alambre ($d\to e$) y cae a cero a lo largo de $R$ ($e\to f$).

Como la resistencia interna y la externa están en serie, la ley de mallas da:

$$\varepsilon = Ir + IR \quad\Longrightarrow\quad I=\frac{\varepsilon}{r+R}$$

La diferencia de potencial entre los bornes de la batería (entre $a$ y $d$) es:

$$V_{ad}=\varepsilon-Ir$$

$$V_{ad}=\varepsilon-\frac{\varepsilon}{r+R}\,r$$

$$V_{ad}=\varepsilon\,\frac{R}{r+R}$$

Es decir, el **voltaje en terminales** de una fuente real es menor que su fem cuando entrega corriente; sólo coincide con $\varepsilon$ en circuito abierto ($I=0$). En general, para una fuente real entre los bornes $a$ (negativo) y $b$ (positivo) que entrega corriente $I$:

$$\boxed{V_{ab}=\varepsilon-Ir}$$

### Convención de signos al recorrer una malla

Al leer la malla desde $a$ hasta $b$ se calcula $V_b-V_a$ sumando los cambios de potencial de cada elemento (segunda ley de Kirchhoff, Serway, Fig. 28.13; cada elemento se recorre de $a$ hacia $b$, de izquierda a derecha):

> **[Figura]:** Cuatro casos de un elemento entre $a$ (izquierda) y $b$ (derecha): a) resistor con corriente $I$ hacia la derecha: $\Delta V=-IR$; b) resistor con corriente $I$ hacia la izquierda: $\Delta V=+IR$; c) fem con borne $-$ a la izquierda y $+$ a la derecha: $\Delta V=+\varepsilon$; d) fem con borne $+$ a la izquierda y $-$ a la derecha: $\Delta V=-\varepsilon$.

- Las cargas se mueven del extremo de potencial alto de un resistor hacia el de potencial bajo: si un resistor se atraviesa **en la dirección de la corriente**, $\Delta V=-IR$.
- Si un resistor se recorre **en dirección opuesta** a la corriente, $\Delta V=+IR$.
- Si una fem (sin resistencia interna) se recorre **en la dirección de la fem** (de $-$ a $+$), $\Delta V=+\varepsilon$.
- Si una fem se recorre **en dirección opuesta** (de $+$ a $-$), $\Delta V=-\varepsilon$.

La energía potencial de la carga disminuye cada vez que atraviesa una caída $-IR$ o una fem en sentido contrario, y aumenta cada vez que pasa del borne negativo al positivo de una batería. La ley de mallas expresa que, al dar una vuelta completa, la suma de los aumentos es igual a la suma de las disminuciones.

Observaciones (Serway):

- La **ley de nodos** puede usarse tantas veces como se necesite, siempre que cada nueva ecuación incluya una corriente no usada antes. En general se usa **una vez menos que el número de nodos**.
- La **ley de mallas** puede usarse tantas veces como haga falta, siempre que cada nueva ecuación incluya un elemento (resistor o batería) o una corriente nueva.
- **El número de ecuaciones independientes necesarias es igual al número de corrientes desconocidas.** Las redes grandes generan sistemas lineales que se resuelven con álgebra matricial o con computador.
- En estado estable, **cualquier capacitor funciona como una rama abierta**: la corriente en la rama que contiene al capacitor es cero.

**Estrategia para resolver problemas (leyes de Kirchhoff):**

1. *Conceptualizar:* identificar todos los elementos, la polaridad de cada batería e imaginar las direcciones de las corrientes.
2. *Categorizar:* ver si el circuito se reduce con combinaciones serie/paralelo; si no, aplicar Kirchhoff.
3. *Analizar:* rotular las cantidades conocidas y asignar símbolo **y dirección** a cada corriente desconocida (si la dirección supuesta es incorrecta, el resultado sale negativo, sin afectar la magnitud).

> **Convención de flechas de fem** (usada en las figuras de los Ejemplos 1 y 3, estilo Halliday–Resnick): la flecha junto a cada fuente apunta en el sentido en que la fem impulsa la carga positiva **dentro** de la fuente, es decir, del borne $-$ al borne $+$. Recorrer la fuente en el sentido de su flecha es $+\varepsilon$.

---

### Ejemplo 1

La figura muestra un circuito cuyos elementos tienen los valores siguientes: $\varepsilon_1=2.1\,[\text{V}]$, $\varepsilon_2=4.4\,[\text{V}]$, $r_1=1.8\,[\Omega]$, $r_2=2.3\,[\Omega]$ y $R=5.3\,[\Omega]$.

1. Encuentre la corriente $i$ del circuito.
2. Calcule la diferencia de potencial entre los puntos $a$ y $b$.
3. Calcule la diferencia de potencial entre los puntos $a$ y $c$.

> **[Figura]:** Circuito de una sola malla. En la rama superior, de izquierda a derecha: punto $c$, batería real 1 (resistencia interna $r_1$ y fem $\varepsilon_1$, con flecha de fem apuntando a la derecha, hacia $a$), punto $a$, batería real 2 (fem $\varepsilon_2$ y resistencia interna $r_2$, con flecha de fem apuntando a la izquierda, hacia $a$), punto $b$. La rama inferior une $c$ con $b$ a través de $R$; la corriente $i$ por $R$ apunta hacia la derecha (de $c$ hacia $b$). Las dos fem se **oponen**: ambas empujan carga hacia $a$.

**Resolución**

*Idea:* es una sola malla, así que la corriente es la misma en todos los elementos. Se aplica la ley de mallas con la convención de signos anterior. Como $\varepsilon_2>\varepsilon_1$, la fuente 2 "gana": la corriente recorre la rama superior de $b$ hacia $c$ (pasando por $a$) y vuelve por $R$ de $c$ a $b$, coherente con la flecha de $i$ dibujada. La fuente 1 es recorrida contra su fem (se está **cargando**).

*1. Corriente.* Se recorre la malla en el sentido de la corriente, partiendo de $b$: $b\to r_2\to\varepsilon_2\to a\to\varepsilon_1\to r_1\to c\to R\to b$.

- $r_2$ en el sentido de $i$: $-ir_2$.
- $\varepsilon_2$ en el sentido de su flecha: $+\varepsilon_2$.
- $\varepsilon_1$ contra su flecha: $-\varepsilon_1$.
- $r_1$ en el sentido de $i$: $-ir_1$.
- $R$ en el sentido de $i$: $-iR$.

$$-ir_2+\varepsilon_2-\varepsilon_1-ir_1-iR=0\quad\Longrightarrow\quad i=\frac{\varepsilon_2-\varepsilon_1}{r_1+r_2+R}$$

$$i=\frac{4.4-2.1}{1.8+2.3+5.3}\,[\text{A}]=\frac{2.3}{9.4}\,[\text{A}]$$

$$\boxed{i\approx 0.24\,[\text{A}]}$$

*2. $V_a-V_b$.* Se va de $b$ a $a$ por la batería 2 (camino más corto):

$$V_a-V_b=-ir_2+\varepsilon_2=4.4-(0.2447)(2.3)=4.4-0.563$$

$$\boxed{V_a-V_b\approx +3.8\,[\text{V}]}$$

*Comprobación por el otro camino* ($b\to R\to c\to r_1\to\varepsilon_1\to a$, todo contra la corriente salvo la fem recorrida en su sentido): $V_a-V_b=+iR+ir_1+\varepsilon_1=1.297+0.440+2.1=3.84\,[\text{V}]$. Coinciden.

*3. $V_a-V_c$.* De $c$ a $a$ por la batería 1: $r_1$ contra la corriente ($+ir_1$) y $\varepsilon_1$ en el sentido de su flecha ($+\varepsilon_1$):

$$V_a-V_c=ir_1+\varepsilon_1=(0.2447)(1.8)+2.1=0.440+2.1$$

$$\boxed{V_a-V_c\approx +2.5\,[\text{V}]}$$

*Verificación / interpretación:* el punto $a$ es el de mayor potencial. Balance de potencia (ver sección siguiente): la fuente 2 entrega $\varepsilon_2 i=1.077\,[\text{W}]$; la fuente 1 absorbe $\varepsilon_1 i=0.514\,[\text{W}]$; las resistencias internas disipan $i^2(r_1+r_2)=0.245\,[\text{W}]$ y $R$ disipa $i^2R=0.317\,[\text{W}]$. Suma: $0.514+0.245+0.317=1.076\,[\text{W}]$, igual a lo entregado (conservación de la energía).

---

## Potencia eléctrica

En los circuitos típicos la energía se transfiere desde una fuente (batería) a algún dispositivo (lámpara, radio, calefactor). Conviene una expresión para la **rapidez** de esa transferencia.

La rapidez con que el sistema pierde energía potencial eléctrica cuando la carga $Q$ atraviesa un resistor con diferencia de potencial $\Delta V$ es:

$$\frac{dU}{dt}=\frac{d}{dt}\left(Q\,\Delta V\right)=\frac{dQ}{dt}\,\Delta V=I\,\Delta V$$

donde $I$ es la corriente y $\Delta V$ el voltaje aplicado. La **potencia eléctrica** $P$ es esa rapidez; usando la ley de Ohm ($\Delta V=IR$, Clase 08):

$$\boxed{P=I\,\Delta V=I^2R=\frac{(\Delta V)^2}{R}}\qquad [\text{W}]=[\text{J/s}]$$

### Complemento: potencia en una fuente real

Multiplicando $V_{ab}=\varepsilon-Ir$ por $I$:

$$\underbrace{IV_{ab}}_{\text{potencia entregada al circuito externo}}=\underbrace{\varepsilon I}_{\text{potencia generada por la fem}}-\underbrace{I^2r}_{\text{disipada en } r}$$

- $\varepsilon I$: rapidez con que la fem convierte energía no eléctrica (química, etc.) en eléctrica.
- $I^2r$: energía disipada como calor dentro de la batería.
- $IV_{ab}=I^2R$: potencia entregada a la carga externa $R$.

Con $I=\varepsilon/(r+R)$, la potencia en la carga es $P_R=\dfrac{\varepsilon^2R}{(r+R)^2}$, que es máxima cuando $dP_R/dR=0\Rightarrow R=r$ (**máxima transferencia de potencia**), con $P_{R,\max}=\varepsilon^2/(4r)$. Si una corriente atraviesa una fuente de $+$ a $-$ (como la fuente 1 del Ejemplo 1), la fuente **recibe** energía $\varepsilon I$ (se carga).

---

### Ejemplo 2

Un calentador eléctrico se construye al aplicar una diferencia de potencial de $120\,[\text{V}]$ a través de un alambre de nicromo que tiene una resistencia total de $8.00\,[\Omega]$. Encuentre la corriente conducida por el alambre y la potencia de especificación del calentador.

**Resolución**

*Idea:* el nicromo tiene alta resistividad (Clase 08) y se usa en tostadores, planchas y calentadores, por lo que se espera una potencia alta. Es un problema de sustitución: ley de Ohm para la corriente y $P=I^2R$ para la potencia.

*Corriente* (ley de Ohm):

$$I=\frac{\Delta V}{R}=\frac{120\,[\text{V}]}{8.00\,[\Omega]}=15.0\,[\text{A}]$$

*Potencia nominal:*

$$P=I^2R=(15.0\,[\text{A}])^2(8.00\,[\Omega])=1.80\times10^{3}\,[\text{W}]$$

$$\boxed{I=15.0\,[\text{A}],\qquad P=1.80\,[\text{kW}]}$$

*Verificación:* por las otras formas, $P=I\,\Delta V=(15.0)(120)=1800\,[\text{W}]$ y $P=(\Delta V)^2/R=14400/8.00=1800\,[\text{W}]$. Coinciden. El valor es típico de un calefactor doméstico.

---

## Circuitos de mallas múltiples

> **[Figura] (circuito de dos mallas):** Rama superior con tres puntos $a$ (izquierda), $b$ (centro) y $c$ (derecha). Entre $a$ y $b$ hay una fem $\varepsilon_1$ con flecha apuntando a la izquierda (hacia $a$); entre $b$ y $c$ hay una fem $\varepsilon_2$ con flecha apuntando a la derecha (hacia $c$). Abajo hay un único punto $d$. Tres resistores verticales llegan a $d$: $R_1$ desde $a$ (corriente $i_1$ hacia abajo), $R_3$ desde $b$ (corriente $i_3$ hacia abajo) y $R_2$ desde $c$ (corriente $i_2$ hacia arriba, de $d$ a $c$). La **malla 1** es $a$-$b$-$d$ (izquierda) y la **malla 2** es $b$-$c$-$d$ (derecha).

El circuito tiene dos mallas. Para analizarlo hay que considerar sus **mallas** y sus **nodos**.

- Un **nodo** es un punto del circuito en el que se reúnen tres o más segmentos de alambre. En la figura, $b$ y $d$ son nodos; $a$ y $c$ **no** son nodos.
- Una **rama** es cualquier trayectoria que parte en un nodo y continúa hasta el siguiente nodo. En la figura hay tres ramas: $b$-$a$-$d$, $b$-$d$ y $b$-$c$-$d$. Cada rama lleva una única corriente ($i_1$, $i_3$ e $i_2$, respectivamente).

En este circuito **no** se pueden aplicar simplemente las equivalencias serie/paralelo (las fem están en ramas distintas); el análisis requiere las leyes de Kirchhoff.

### Ley de Corrientes de Kirchhoff (LCK, ley de nodos)

En cualquier nodo, la suma de las corrientes que **salen** del nodo es igual a la suma de las corrientes que **entran** al nodo:

$$\sum I_{\text{entran}}=\sum I_{\text{salen}}\qquad\Longleftrightarrow\qquad \sum_{\text{nodo}} I=0$$

Es consecuencia de la conservación de la carga: en estado estacionario la carga no se acumula en un nodo.

> **[Figura]:** Dos nodos $P$ con tres conductores 1, 2, 3. En ambos casos $i_1$ entra a $P$ desde el conductor 1, e $i_2$ e $i_3$ salen por los conductores 2 y 3 (en el segundo dibujo, el conductor 2 sale hacia arriba y el 3 continúa horizontalmente). En ambos casos: $i_1=i_2+i_3$.

### Ley de Voltajes de Kirchhoff (LVK, ley de mallas)

La suma algebraica de las diferencias de potencial a lo largo de cualquier malla cerrada es cero:

$$\sum_{\text{malla}}\Delta V=0$$

Es consecuencia de la conservación de la energía (el campo electrostático es conservativo, Clase 05: $\oint \vec E\cdot d\vec l=0$).

### Resolución del circuito de dos mallas

Con las leyes de Kirchhoff se plantean ecuaciones que permiten determinar todas las corrientes y diferencias de potencial. Con las direcciones de la figura:

*Por LCK en el nodo $b$:* entra $i_2$ (desde $c$) y salen $i_1$ (hacia $a$) e $i_3$ (hacia $d$):

$$i_2=i_1+i_3$$

*Por LVK en la malla 1* (recorrido $b\to a\to d\to b$): $\varepsilon_1$ en el sentido de su flecha ($+\varepsilon_1$); $R_1$ en el sentido de $i_1$ ($-i_1R_1$); $R_3$ de $d$ a $b$, contra $i_3$ ($+i_3R_3$):

$$\varepsilon_1-i_1R_1+i_3R_3=0$$

*Por LVK en la malla 2* (recorrido $b\to d\to c\to b$): $R_3$ en el sentido de $i_3$ ($-i_3R_3$); $R_2$ en el sentido de $i_2$ ($-i_2R_2$); $\varepsilon_2$ de $c$ a $b$, contra su flecha ($-\varepsilon_2$):

$$-i_3R_3-i_2R_2-\varepsilon_2=0$$

Son tres ecuaciones lineales para las tres incógnitas $i_1,i_2,i_3$. Escritas en forma matricial:

$$\begin{pmatrix}1&-1&1\\-R_1&0&R_3\\0&-R_2&-R_3\end{pmatrix}\begin{pmatrix}i_1\\i_2\\i_3\end{pmatrix}=\begin{pmatrix}0\\-\varepsilon_1\\\varepsilon_2\end{pmatrix}$$

(Una corriente que resulte negativa simplemente circula en sentido opuesto al supuesto.) La LVK aplicada a la malla exterior $a$-$b$-$c$-$d$ no aporta información nueva: es la suma de las otras dos.

---

### Ejemplo 3

La figura muestra un circuito cuyos elementos tienen los valores siguientes: $\varepsilon_1=2.1\,[\text{V}]$, $\varepsilon_2=6.3\,[\text{V}]$, $R_1=1.7\,[\Omega]$ y $R_2=3.5\,[\Omega]$.

1. Encuentre las corrientes de las tres ramas del circuito.
2. Calcule la diferencia de potencial entre los puntos $a$ y $b$.

> **[Figura]:** Dos nodos: $a$ (arriba, al centro) y $b$ (abajo, al centro). Tres ramas los unen:
> - **Rama izquierda:** desde $a$ hacia la izquierda por un $R_1$ superior, baja por el lado izquierdo atravesando la fem $\varepsilon_1$ (flecha hacia arriba) y vuelve hacia la derecha por un $R_1$ inferior hasta $b$. Corriente $i_1$: hacia la izquierda arriba, hacia abajo en el lado izquierdo y hacia la derecha abajo, es decir, de $a$ a $b$ por la izquierda.
> - **Rama central:** de $a$ baja por $R_2$ y luego por una fem $\varepsilon_2$ (flecha hacia arriba) hasta $b$. Corriente $i_2$ hacia abajo (de $a$ a $b$).
> - **Rama derecha:** desde $b$ hacia la derecha, sube por el lado derecho atravesando un $R_1$ (abajo) y una fem $\varepsilon_2$ (arriba, flecha hacia arriba) y vuelve hacia la izquierda por un $R_1$ superior hasta $a$. Corriente $i_3$: hacia arriba en el lado derecho y hacia la izquierda arriba, es decir, de $b$ a $a$ por la derecha.

**Resolución**

*Idea:* circuito de dos nodos y tres ramas: se necesitan 3 ecuaciones independientes, 1 de nodos (2 nodos − 1) y 2 de mallas. Se usan las direcciones supuestas de la figura y la convención de flechas de fem ($+\varepsilon$ si se recorre en el sentido de la flecha).

*LCK en el nodo $a$:* entra $i_3$, salen $i_1$ e $i_2$:

$$(1)\qquad i_3=i_1+i_2$$

*LVK en la malla izquierda* (recorrido $a\to$ izquierda $\to b\to$ subiendo por el centro $\to a$):

- $R_1$ superior, en el sentido de $i_1$: $-i_1R_1$.
- $\varepsilon_1$ recorrida hacia abajo, contra su flecha: $-\varepsilon_1$.
- $R_1$ inferior, en el sentido de $i_1$: $-i_1R_1$.
- $\varepsilon_2$ central recorrida hacia arriba, en el sentido de su flecha: $+\varepsilon_2$.
- $R_2$ recorrido hacia arriba, contra $i_2$: $+i_2R_2$.

$$(2)\qquad -2i_1R_1-\varepsilon_1+\varepsilon_2+i_2R_2=0$$

*LVK en la malla derecha* (recorrido $b\to$ derecha $\to$ sube $\to a\to$ baja por el centro $\to b$):

- $R_1$ derecho, en el sentido de $i_3$: $-i_3R_1$.
- $\varepsilon_2$ derecha, en el sentido de su flecha: $+\varepsilon_2$.
- $R_1$ superior derecho, en el sentido de $i_3$: $-i_3R_1$.
- $R_2$ hacia abajo, en el sentido de $i_2$: $-i_2R_2$.
- $\varepsilon_2$ central hacia abajo, contra su flecha: $-\varepsilon_2$.

$$(3)\qquad -2i_3R_1-i_2R_2=0$$

Las dos fuentes $\varepsilon_2$ se cancelan en la malla derecha.

*Sistema explícito:*

$$\begin{cases} i_1+i_2-i_3=0\\ -2R_1\,i_1+R_2\,i_2=\varepsilon_1-\varepsilon_2\\ -R_2\,i_2-2R_1\,i_3=0\end{cases}
\quad\Longrightarrow\quad
\begin{cases} i_1+i_2-i_3=0\\ -3.4\,i_1+3.5\,i_2=-4.2\\ -3.5\,i_2-3.4\,i_3=0\end{cases}$$

*Solución paso a paso.* De (3): $i_3=-\dfrac{R_2}{2R_1}\,i_2$, es decir, $2R_1i_3=-R_2i_2$. De (1): $i_1=i_3-i_2$. Sustituyendo en (2):

$$-2R_1(i_3-i_2)+R_2i_2=\varepsilon_1-\varepsilon_2$$

$$\underbrace{-2R_1i_3}_{=\,R_2i_2}+2R_1i_2+R_2i_2=\varepsilon_1-\varepsilon_2\quad\Longrightarrow\quad i_2\,(2R_1+2R_2)=\varepsilon_1-\varepsilon_2$$

$$i_2=\frac{\varepsilon_1-\varepsilon_2}{2(R_1+R_2)}=\frac{2.1-6.3}{2(1.7+3.5)}=\frac{-4.2}{10.4}=-0.404\,[\text{A}]$$

$$i_3=-\frac{R_2}{2R_1}\,i_2=-\frac{3.5}{3.4}(-0.404)=0.416\,[\text{A}]$$

$$i_1=i_3-i_2=0.416-(-0.404)=0.820\,[\text{A}]$$

$$\boxed{i_1\approx0.82\,[\text{A}],\quad i_2\approx-0.40\,[\text{A}],\quad i_3\approx0.42\,[\text{A}]}$$

El signo negativo de $i_2$ indica que en la rama central la corriente circula **hacia arriba** (de $b$ a $a$), con magnitud $0.40\,[\text{A}]$.

*2. $V_a-V_b$.* Se recorre de $a$ a $b$ por la rama central y se suman los cambios de potencial: $R_2$ hacia abajo en el sentido supuesto de $i_2$ ($-i_2R_2$) y $\varepsilon_2$ hacia abajo, contra su flecha ($-\varepsilon_2$):

$$V_b-V_a=-i_2R_2-\varepsilon_2=-(-0.404)(3.5)-6.3=1.41-6.3=-4.89\,[\text{V}]$$

Comprobación por la rama izquierda (de $a$ a $b$ en el sentido de $i_1$, con $\varepsilon_1$ recorrida contra su flecha): $V_b-V_a=-2i_1R_1-\varepsilon_1=-2(0.820)(1.7)-2.1=-2.79-2.1=-4.89\,[\text{V}]$. Ambos caminos dan $V_b-V_a=-4.89\,[\text{V}]$, es decir:

$$\boxed{V_a-V_b\approx4.9\,[\text{V}]\quad(\text{el punto } a \text{ está a mayor potencial})}$$

Tercer camino (rama derecha, de $a$ a $b$ contra $i_3$): $V_b-V_a=+i_3R_1-\varepsilon_2+i_3R_1=2(0.416)(1.7)-6.3=-4.89\,[\text{V}]$. Coincide.

*Verificación / interpretación:* (1) $i_1+i_2=0.820-0.404=0.416=i_3$ ✓. Las tres ramas dan la misma diferencia de potencial entre los nodos, como debe ser. La solución numérica del sistema con `numpy.linalg.solve` da $(i_1,i_2,i_3)=(0.8196,\,-0.4038,\,0.4157)\,[\text{A}]$.

---

## Circuitos RC

Se llama **circuito RC** a un circuito que contiene una combinación en serie de un resistor y un capacitor. A diferencia de los casos anteriores, la corriente **no** es constante: varía mientras el capacitor se carga o descarga.

> **[Figura]:** Circuito con una batería $\varepsilon$ (abajo, a la izquierda), un capacitor $C$ (arriba, a la derecha) y un resistor $R$ (lado derecho), todos en serie, y un interruptor de dos posiciones $a$/$b$ en la parte superior izquierda. En la posición $a$, la batería queda en serie con $C$ y $R$; en la posición $b$, la batería queda fuera y $C$ y $R$ forman un lazo cerrado por un alambre que baja desde $b$. a) Interruptor abierto ($t<0$). b) Interruptor en $a$: el capacitor se **carga** con corriente $I$ hacia abajo por $R$. c) Interruptor en $b$: el capacitor se **descarga** con corriente $I$ hacia arriba por $R$ (sentido opuesto al de carga).

### Carga de un condensador

Con el interruptor en $a$, usando la ley de voltajes de Kirchhoff (fem $+\varepsilon$, caída $q/C$ en el capacitor, caída $IR$ en el resistor):

$$\varepsilon-\frac{q}{C}-IR=0$$

En el instante en que se cierra el interruptor ($t=0$) el condensador está completamente descargado ($q=0$), por lo que se comporta como un cortocircuito:

$$I_0=\frac{\varepsilon}{R}$$

Una vez que el condensador está completamente cargado, la corriente deja de fluir ($I=0$) y toda la fem queda en el capacitor:

$$Q=C\varepsilon$$

Para encontrar la carga y la corriente en función del tiempo, se usa $I=dq/dt$:

$$\frac{dq}{dt}=\frac{\varepsilon}{R}-\frac{q}{RC}$$

Factorizando y reordenando términos:

$$\frac{dq}{dt}=-\frac{q-C\varepsilon}{RC}$$

¡Es una ecuación diferencial de **variables separables**!

$$\frac{dq}{q-C\varepsilon}=-\frac{1}{RC}\,dt$$

Integrando desde $t=0$ (con $q=0$) hasta un instante $t$ (con carga $q$):

$$\int_{0}^{q}\frac{dq'}{q'-C\varepsilon}=-\frac{1}{RC}\int_{0}^{t}dt'$$

Se obtiene:

$$\ln\!\left(\frac{q-C\varepsilon}{-C\varepsilon}\right)=-\frac{t}{RC}\qquad\Longrightarrow\qquad \frac{C\varepsilon-q}{C\varepsilon}=e^{-t/RC}$$

Entonces:

$$\boxed{q(t)=C\varepsilon\left(1-e^{-t/RC}\right)=Q\left(1-e^{-t/RC}\right)}$$

Utilizando la definición de corriente $I=dq/dt$:

$$\boxed{I(t)=\frac{\varepsilon}{R}\,e^{-t/RC}}$$

El producto $RC$ se denomina **constante de tiempo** $\tau$ del circuito:

$$\boxed{\tau=RC}\qquad [\Omega\cdot\text{F}]=\left[\tfrac{\text{V}}{\text{A}}\cdot\tfrac{\text{C}}{\text{V}}\right]=\left[\tfrac{\text{C}}{\text{C/s}}\right]=[\text{s}]$$

En $t=\tau$ la carga alcanza $Q(1-e^{-1})\approx0.632\,Q$ y la corriente cae a $I_0e^{-1}\approx0.368\,I_0$. El voltaje en el capacitor es $V_C(t)=q/C=\varepsilon(1-e^{-t/\tau})$ y en el resistor $V_R(t)=IR=\varepsilon e^{-t/\tau}$; en todo instante $V_C+V_R=\varepsilon$.

#### Complemento: análisis energético de la carga

- Energía entregada por la fuente durante toda la carga: la fem mueve la carga total $Q=C\varepsilon$ a través de la diferencia de potencial $\varepsilon$:
$$W_\varepsilon=\int_0^\infty \varepsilon I\,dt=\varepsilon Q=C\varepsilon^2$$
- Energía almacenada al final en el capacitor (Clase 06):
$$U_C=\frac{Q^2}{2C}=\frac12C\varepsilon^2$$
- Energía disipada en el resistor:
$$W_R=\int_0^\infty I^2R\,dt=\frac{\varepsilon^2}{R}\int_0^\infty e^{-2t/RC}\,dt=\frac{\varepsilon^2}{R}\cdot\frac{RC}{2}=\frac12C\varepsilon^2$$

Por lo tanto $W_\varepsilon=U_C+W_R$ y

$$\boxed{\text{la mitad de la energía entregada por la fuente se disipa en } R\text{, independientemente del valor de } R}$$

($R$ sólo determina la rapidez del proceso, a través de $\tau$.)

### Descarga de un condensador

Una vez completamente cargado, el condensador tiene una diferencia de potencial $Q/C$ entre sus placas y la diferencia de potencial en la resistencia es cero ($I=0$). Al mover el interruptor de $a$ a $b$, la batería sale del circuito y el capacitor comienza a descargarse a través de $R$. La ley de mallas, sin fem, da:

$$-\frac{q}{C}-IR=0\qquad\Longrightarrow\qquad -R\frac{dq}{dt}=\frac{q}{C}$$

Otra forma de verlo (descripción alternativa de la clase):

> **[Figura]:** Lazo con un condensador $C$ (lado derecho, placa superior $+q$ y placa inferior $-q$), un resistor $R$ (arriba) y un interruptor $I$ (abajo). El punto $a$ está entre $R$ y la placa positiva; el punto $b$, abajo a la izquierda, entre el interruptor y el otro extremo de $R$. La corriente $i$ sale de la placa positiva hacia arriba y recorre $R$ de $a$ hacia $b$.

Consideremos un circuito formado por un condensador inicialmente cargado con carga $Q$ y una resistencia $R$; se cierra el interruptor I. La ecuación del circuito es $V_{ab}+V_{ba}=0$:

- Como la corriente va de $a$ hacia $b$ por el resistor, el potencial de $a$ es mayor que el de $b$: por la ley de Ohm, $V_{ab}=iR$.
- En el condensador, la placa positiva ($a$) tiene más potencial que la negativa ($b$), de modo que $V_{ba}=-q/C$.

$$iR-\frac{q}{C}=0$$

Como la carga **disminuye** con el tiempo, $i=-dq/dt$, y la ecuación a integrar es la misma:

$$-R\frac{dq}{dt}=\frac{q}{C}\qquad\Longrightarrow\qquad\frac{dq}{q}=-\frac{1}{RC}\,dt$$

Integrando, considerando ahora que en $t=0$ se tiene $q=Q$:

$$\int_{Q}^{q}\frac{dq'}{q'}=-\frac{1}{RC}\int_{0}^{t}dt'$$

$$\ln\!\left(\frac{q}{Q}\right)=-\frac{t}{RC}$$

Luego:

$$\boxed{q(t)=Q\,e^{-t/RC}}$$

La carga disminuye exponencialmente. Derivando respecto del tiempo:

$$I(t)=\frac{dq}{dt}=-\frac{Q}{RC}\,e^{-t/RC}$$

donde la corriente inicial tiene magnitud

$$I_i=\frac{Q}{RC}$$

El **signo negativo** indica que la dirección de la corriente durante la descarga es opuesta a la dirección durante la carga. Si se mide en el sentido indicado en la figura alternativa ($i=-dq/dt$), la intensidad resulta positiva:

$$i=-\frac{dq}{dt}=\frac{Q}{RC}\,e^{-t/RC}$$

que también disminuye exponencialmente con el tiempo.

---

### Ejemplo 4

Considere un capacitor de capacitancia $C$ que se descarga a través de un resistor de resistencia $R$, como se muestra en la figura.

A) ¿Después de cuántas constantes de tiempo la carga en el capacitor es un cuarto de su valor inicial?

B) La energía almacenada en el capacitor disminuye con el tiempo conforme el capacitor se descarga. ¿Después de cuántas constantes de tiempo la energía almacenada es un cuarto de su valor inicial?

> **[Figura]:** El circuito RC con interruptor de la sección anterior, con el interruptor en la posición $b$: la batería $\varepsilon$ queda fuera y el capacitor $C$ se descarga a través de $R$, con corriente $I$ hacia arriba por $R$.

**Resolución**

*Idea:* al mover el interruptor a $b$ el capacitor se descarga, así que se usa $q(t)=Qe^{-t/RC}$. Para la energía se combina con la energía de un capacitor, $U=q^2/(2C)$ (Clase 06).

*A) Carga.* Se impone $q(t)=Q/4$:

$$\frac{Q}{4}=Qe^{-t/RC}\quad\Longrightarrow\quad\frac14=e^{-t/RC}$$

Tomando logaritmo natural a ambos lados:

$$-\ln4=-\frac{t}{RC}\quad\Longrightarrow\quad t=RC\ln4=1.39\,RC$$

$$\boxed{t=\tau\ln4\approx1.39\,\tau}$$

*B) Energía.* La energía almacenada en cualquier instante es

$$U(t)=\frac{q^2}{2C}=\frac{Q^2}{2C}\,e^{-2t/RC}$$

Imponiendo $U(t)=\tfrac14\,\dfrac{Q^2}{2C}$:

$$\frac14\,\frac{Q^2}{2C}=\frac{Q^2}{2C}e^{-2t/RC}\quad\Longrightarrow\quad\frac14=e^{-2t/RC}$$

$$-\ln4=-\frac{2t}{RC}\quad\Longrightarrow\quad t=\tfrac12RC\ln4=RC\ln2=0.693\,RC$$

$$\boxed{t=\tau\ln2\approx0.693\,\tau}$$

*Verificación / interpretación:* como la energía depende del **cuadrado** de la carga, decae con constante de tiempo efectiva $\tau/2$; por eso la energía cae más rápido que la carga (llega a 1/4 cuando la carga ha caído sólo a 1/2, lo que ocurre en $\tau\ln2$). Ambos resultados son adimensionales en unidades de $\tau$, independientes de $R$ y $C$ por separado.

---

### Ejercicio 1

Encuentre las corrientes $I_1$, $I_2$ e $I_3$ en el circuito que se muestra en la figura.

> **[Figura]:** Circuito rectangular con seis puntos: $e$ (arriba izquierda), $f$ (arriba derecha), $b$ (medio izquierda), $c$ (medio derecha), $a$ (abajo izquierda), $d$ (abajo derecha).
> - Rama superior $e$–$f$: batería de $14.0\,[\text{V}]$ con borne $+$ hacia $e$ y borne $-$ hacia $f$.
> - Lado izquierdo $e$–$b$: resistor de $4.0\,[\Omega]$. Lado izquierdo $b$–$a$: alambre.
> - Rama central $b$–$c$: batería de $10.0\,[\text{V}]$ con borne $-$ hacia $b$ y $+$ hacia la derecha, seguida de un resistor de $6.0\,[\Omega]$; corriente $I_1$ hacia la derecha (de $b$ a $c$).
> - Lado derecho $f$–$c$: alambre con corriente $I_2$ hacia abajo. Lado derecho $c$–$d$: alambre con corriente $I_3$ hacia abajo.
> - Rama inferior $a$–$d$: resistor de $2.0\,[\Omega]$.
>
> Nodos reales: $b$ y $c$. Ramas: $b$-$c$ (lleva $I_1$), $c$-$f$-$e$-$b$ (lleva $I_2$; con la dirección supuesta, la corriente sube de $b$ a $e$, va de $e$ a $f$ y baja de $f$ a $c$) y $c$-$d$-$a$-$b$ (lleva $I_3$, que baja por $c$-$d$, recorre el $2.0\,\Omega$ de $d$ a $a$ y sube de $a$ a $b$).

**Resolución**

*Idea:* tres corrientes desconocidas $\Rightarrow$ tres ecuaciones: 1 de nodos y 2 de mallas (hay tres espiras, $abcda$, $befcb$ y $aefda$, pero la tercera no da información nueva). Las mallas se recorren en sentido horario con la convención de signos de la clase.

*LCK en el nodo $c$:* entran $I_1$ (desde $b$) e $I_2$ (desde $f$); sale $I_3$ (hacia $d$):

$$(1)\qquad I_1+I_2-I_3=0$$

*LVK en la malla $abcda$* (horario: $a\to b\to c\to d\to a$): batería de $10\,\text{V}$ de $-$ a $+$ ($+10.0$); $6\,\Omega$ en el sentido de $I_1$ ($-6.0I_1$); $c\to d$ alambre; $2\,\Omega$ de $d$ a $a$ en el sentido de $I_3$ ($-2.0I_3$):

$$(2)\qquad 10.0-6.0\,I_1-2.0\,I_3=0$$

*LVK en la malla $befcb$* (horario: $b\to e\to f\to c\to b$): $4\,\Omega$ de $b$ a $e$ en el sentido de $I_2$ ($-4.0I_2$); batería de $14\,\text{V}$ de $+$ a $-$ ($-14.0$); $f\to c$ alambre; $6\,\Omega$ de $c$ a $b$ contra $I_1$ ($+6.0I_1$); batería de $10\,\text{V}$ de $+$ a $-$ ($-10.0$):

$$-4.0\,I_2-14.0+6.0\,I_1-10.0=0\quad\Longrightarrow\quad(3)\qquad -24.0+6.0\,I_1-4.0\,I_2=0$$

*Sistema explícito* (corrientes en A, resistencias en $\Omega$, fem en V):

$$\begin{cases}I_1+I_2-I_3=0\\ 6.0\,I_1+2.0\,I_3=10.0\\ 6.0\,I_1-4.0\,I_2=24.0\end{cases}$$

*Solución paso a paso.* De (1), $I_3=I_1+I_2$; sustituyendo en (2):

$$10.0-6.0I_1-2.0(I_1+I_2)=0\quad\Longrightarrow\quad(4)\qquad10.0-8.0I_1-2.0I_2=0$$

Multiplicando (3) por 4 y (4) por 3:

$$(5)\qquad -96.0+24.0I_1-16.0I_2=0$$
$$(6)\qquad 30.0-24.0I_1-6.0I_2=0$$

Sumando (5) y (6) se elimina $I_1$:

$$-66.0-22.0I_2=0\quad\Longrightarrow\quad I_2=-3.0\,[\text{A}]$$

Reemplazando en (3):

$$-24.0+6.0I_1-4.0(-3.0)=0\quad\Longrightarrow\quad-24.0+6.0I_1+12.0=0\quad\Longrightarrow\quad I_1=2.0\,[\text{A}]$$

Y de (1):

$$I_3=I_1+I_2=2.0-3.0=-1.0\,[\text{A}]$$

$$\boxed{I_1=2.0\,[\text{A}],\qquad I_2=-3.0\,[\text{A}],\qquad I_3=-1.0\,[\text{A}]}$$

*Verificación / interpretación:* los signos negativos indican que $I_2$ e $I_3$ circulan en sentido contrario al dibujado: $I_2=3.0\,\text{A}$ sube de $c$ a $f$, e $I_3=1.0\,\text{A}$ sube de $d$ a $c$. Comprobación en (2): $10-6(2)-2(-1)=10-12+2=0$ ✓. Malla exterior $aefda$ (horario: $a\to e\to f\to d\to a$): $-4.0I_2-14.0-2.0I_3=12-14+2=0$ ✓. La resolución con `numpy.linalg.solve` da $(2,\,-3,\,-1)\,[\text{A}]$.

---

### Ejercicio 2

El circuito de la figura se ha conectado durante mucho tiempo.

a) ¿Cuánto vale la carga del capacitor?

b) Si se desconecta la batería, ¿cuánto tiempo tarda el capacitor en descargarse hasta la décima parte de su voltaje inicial?

> **[Figura]:** Puente de resistencias en forma de rombo alimentado por una batería de $10.0\,[\text{V}]$ (a la izquierda, borne $+$ arriba) conectada entre el vértice superior y el vértice inferior del rombo. Lados del rombo: superior izquierdo $1.00\,[\Omega]$ y superior derecho $8.00\,[\Omega]$ (desde el vértice superior); inferior izquierdo $4.00\,[\Omega]$ e inferior derecho $2.00\,[\Omega]$ (desde el vértice inferior). Entre el vértice izquierdo y el vértice derecho hay un capacitor de $1.00\,[\mu\text{F}]$. Equivalentemente: dos divisores de voltaje en paralelo con la batería, uno izquierdo ($1\,\Omega$ arriba, $4\,\Omega$ abajo, punto medio $L$) y uno derecho ($8\,\Omega$ arriba, $2\,\Omega$ abajo, punto medio $R$), con el capacitor entre $L$ y $R$.

**Resolución**

*Idea:* después de mucho tiempo el capacitor está completamente cargado y funciona como **rama abierta** ($I=0$ por él). Entonces cada rama del puente es un **divisor de voltaje** en serie con la batería, y el voltaje del capacitor es la diferencia de potencial entre los puntos medios. Al desconectar la batería, el capacitor se descarga a través de las resistencias: es una descarga RC con la resistencia equivalente que "ve" el capacitor.

*a) Carga del capacitor.* Se toma el vértice inferior (borne $-$) como referencia $V=0$; el vértice superior está a $10.0\,\text{V}$.

Rama izquierda ($1\,\Omega+4\,\Omega$ en serie):

$$I_L=\frac{10.0\,[\text{V}]}{5.00\,[\Omega]}=2.00\,[\text{A}],\qquad V_L=10.0-(2.00)(1.00)=8.00\,[\text{V}]$$

Rama derecha ($8\,\Omega+2\,\Omega$ en serie):

$$I_R=\frac{10.0\,[\text{V}]}{10.0\,[\Omega]}=1.00\,[\text{A}],\qquad V_R=10.0-(8.00)(1.00)=2.00\,[\text{V}]$$

(o bien, por divisor de voltaje, $V_R=\dfrac{2.00}{2.00+8.00}(10.0)=2.00\,\text{V}$).

$$\Delta V_C=V_L-V_R=8.00-2.00=6.00\,[\text{V}]$$

$$Q=C\,\Delta V_C=(1.00\times10^{-6}\,[\text{F}])(6.00\,[\text{V}])$$

$$\boxed{Q=6.00\,[\mu\text{C}]}\quad(\text{placa positiva en el lado izquierdo})$$

*b) Descarga.* Al desconectar la batería, el vértice superior y el inferior ya no están unidos por la fuente. El capacitor (entre $L$ y $R$) se descarga por dos caminos:

- por arriba: $L\to1\,\Omega\to$ vértice superior $\to8\,\Omega\to R$: $1.00+8.00=9.00\,\Omega$ en serie;
- por abajo: $L\to4\,\Omega\to$ vértice inferior $\to2\,\Omega\to R$: $4.00+2.00=6.00\,\Omega$ en serie.

> **[Figura] (circuito redibujado):** el capacitor de $1.00\,\mu\text{F}$ en paralelo con un resistor de $9.00\,\Omega$ (arriba) y uno de $6.00\,\Omega$ (abajo).

Ambos caminos están en paralelo con el capacitor:

$$R_{eq}=\frac{1}{\dfrac{1}{9.00}+\dfrac{1}{6.00}}=3.60\,[\Omega],\qquad \tau=R_{eq}C=(3.60)(1.00\times10^{-6})=3.60\times10^{-6}\,[\text{s}]$$

Como $V_C=q/C$, el voltaje decae igual que la carga: $V_C(t)=V_0e^{-t/\tau}$. Imponiendo $V_C=V_0/10$:

$$e^{-t/\tau}=\frac1{10}\quad\Longrightarrow\quad t=\tau\ln10=(3.60\times10^{-6})(2.303)$$

$$\boxed{t\approx8.29\,[\mu\text{s}]}$$

*Verificación / interpretación:* $\ln10\approx2.30$, así que se necesitan unas 2.3 constantes de tiempo para bajar al 10 %, coherente con $e^{-2.3}\approx0.10$. El tiempo es muy corto porque $R_{eq}$ y $C$ son pequeños. El resultado coincide con la solución del texto (Serway P28.31: $\Delta V=6.00\,\text{V}$, $t=8.29\,\mu\text{s}$); la carga pedida en (a) es $Q=C\Delta V=6.00\,\mu\text{C}$.

---

## Resumen de fórmulas

| Concepto | Fórmula |
|---|---|
| Corriente en malla simple con fuente real | $I=\dfrac{\varepsilon}{r+R}$ |
| Voltaje en terminales de fuente real | $V_{ab}=\varepsilon-Ir=\varepsilon\dfrac{R}{r+R}$ |
| Convención de signos (recorrido) | Resistor a favor de $I$: $-IR$; en contra: $+IR$; fem de $-$ a $+$: $+\varepsilon$; de $+$ a $-$: $-\varepsilon$ |
| Potencia eléctrica | $P=I\,\Delta V=I^2R=\dfrac{(\Delta V)^2}{R}$ |
| Balance en fuente real | $IV_{ab}=\varepsilon I-I^2r$ |
| Máxima transferencia de potencia | $R=r$, $P_{\max}=\dfrac{\varepsilon^2}{4r}$ |
| Ley de nodos (LCK) | $\sum I_{\text{entran}}=\sum I_{\text{salen}}$ |
| Ley de mallas (LVK) | $\sum_{\text{malla}}\Delta V=0$ |
| N.º de ecuaciones | (nodos − 1) de LCK + resto de LVK = n.º de corrientes desconocidas |
| Carga RC: ecuación | $\dfrac{dq}{dt}=\dfrac{\varepsilon}{R}-\dfrac{q}{RC}$ |
| Carga RC: solución | $q(t)=C\varepsilon\left(1-e^{-t/RC}\right)$, $\;I(t)=\dfrac{\varepsilon}{R}e^{-t/RC}$ |
| Descarga RC | $q(t)=Q_0e^{-t/RC}$, $\;I(t)=-\dfrac{Q_0}{RC}e^{-t/RC}$ |
| Constante de tiempo | $\tau=RC$ |
| Energía en la carga | $W_\varepsilon=C\varepsilon^2$, $\;U_C=\tfrac12C\varepsilon^2$, $\;W_R=\tfrac12C\varepsilon^2$ |
| Energía en la descarga | $U(t)=\dfrac{Q_0^2}{2C}e^{-2t/RC}$ |
| Capacitor en estado estable | rama abierta ($I=0$) |
