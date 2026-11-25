---
title: "Corriente alterna"
source_pdf: "Electro/2025-2/Clases/Tema5_Corriente_Alterna.pdf"
pages: 35
extraction_mode: "visual_latex_transcription"
---

# Corriente alterna

> **Convención de notación:** A lo largo de este apunte se mantiene la notación de las diapositivas, que emplean $\mathrm{i} = \sqrt{-1}$ (letra «i» recta/romana) para la unidad imaginaria, diferenciándola de $i$ o $i(t)$ que representan la corriente instantánea. Asimismo, los valores máximos (amplitudes) se escriben con mayúsculas ($V$, $I$, $V_R$, $V_L$, $V_C$) y los valores eficaces o cuadráticos medios con el subíndice $\text{rms}$ ($V_{\text{rms}}$, $I_{\text{rms}}$).

## Introducción a la corriente alterna

### Corriente alterna frente a corriente continua

Cuando el voltaje y la corriente varían de forma **sinusoidal** en el tiempo hablamos de **corriente alterna (ca)**. Para suministrar una corriente alterna a un circuito se requiere una fuente de fem o voltaje alternos (recurso audiovisual citado en la presentación: `https://www.youtube.com/watch?v=9vIG51BtzsY`).

> **[Figura]:** Símbolo de fuente de corriente alterna (círculo amarillo con una onda sinusoidal `~` en su interior y dos terminales horizontales) acompañado de una fotografía de transformadores de alta tensión en una subestación eléctrica y una infografía comparativa entre corriente alterna (ca) y corriente continua (cc):
> - **Corriente alterna:** su valor varía periódicamente cambiando de dirección; su gráfica $v(t)$ es sinusoidal (se indican el voltaje pico-pico $V_{\text{pp}}$ y el voltaje eficaz $\text{RMS}$). Aplicaciones típicas: transformadores eléctricos, transporte de altos voltajes, electricidad residencial e industrial.
> - **Corriente continua:** tiene una sola dirección y se mantiene constante en el tiempo; su gráfica $v(t)$ es una línea horizontal constante. Aplicaciones típicas: electrónica digital, computación y redes, dispositivos de control y electrónica analógica.

### Voltaje y corriente sinusoidales

Una fuente sinusoidal produce un voltaje instantáneo $v$ y una corriente instantánea $i$ de la forma:

$$v = V\cos\omega t$$

$$i = I\cos\omega t$$

donde:
- $v$ e $i$ son el **voltaje y la corriente instantáneos** (dependientes del tiempo $t$).
- $V$ e $I$ son el **voltaje y la corriente máximos** (amplitudes o valores pico).
- $\omega = 2\pi f$ es la frecuencia angular (en $\text{rad/s}$) y $f$ la frecuencia (en $\text{Hz}$).

> **[Figura]:** Gráfica del voltaje instantáneo $v$ en función del tiempo $t$ para una señal sinusoidal con $f = 50\,\text{Hz}$ ($\omega = 314\,\text{rad/s}$), correlacionada con tres esquemas de la fuente de ca:
> 1. Durante el semiciclo positivo ($v > 0$, área sombreada sobre el eje $t$), la fuente tiene terminal izquierdo positivo ($+$) y derecho negativo ($-$).
> 2. En el cruce por cero ($v = 0$), el voltaje entre terminales es nulo.
> 3. Durante el semiciclo negativo ($v < 0$, área sombreada bajo el eje $t$), la polaridad se invierte: terminal izquierdo negativo ($-$) y derecho positivo ($+$).

### Amplitudes y frecuencias en redes eléctricas

> **[Figura]:** Mapamundi codificado por colores que muestra los estándares de voltaje eficaz (rms) y frecuencia de la red eléctrica residencial en el mundo. La leyenda distingue regiones con voltajes en torno a $100\,\text{V}$, $110\,\text{V}$, $115\,\text{V}$, $120\,\text{V}$ y $127\,\text{V}$ (predominantemente a $60\,\text{Hz}$, como en Norteamérica y parte del norte de Sudamérica, o a $50\,\text{Hz}$/mixto como en partes de Japón o Brasil), y regiones con $220\,\text{V}$, $230\,\text{V}$ y $240\,\text{V}$ (predominantemente a $50\,\text{Hz}$, como en el Cono Sur de Sudamérica, Europa, África, Asia y Oceanía, además de zonas a $220\text{--}240\,\text{V}$ y $60\,\text{Hz}$ como Perú o Corea del Sur).

## Fasores y representación compleja

### Diagramas fasoriales

Para representar voltajes y corrientes que varían en forma sinusoidal se pueden utilizar diagramas de **vectores giratorios**, denominados **fasores**, de forma análoga al movimiento armónico simple.

> **[Figura]:** Diagrama de fasor de corriente en un sistema de ejes cartesianos centrado en $O$: una flecha violeta (el fasor) de longitud igual a la corriente máxima $I$ forma un ángulo $\omega t$ con el eje horizontal positivo y gira en sentido antihorario con frecuencia $f$ y rapidez angular $\omega = 2\pi f$. La proyección del fasor sobre el eje horizontal en el instante $t$ (indicada con una flecha horizontal desde $O$ hasta el pie de la perpendicular punteada) es igual a la corriente instantánea $i = I\cos\omega t$.

### Representación compleja y fórmula de Euler

Otra manera equivalente y algebraicamente más cómoda es utilizar la **representación compleja**. En el plano complejo, un número $z$ se describe en forma cartesiana o polar mediante:

$$z = (x, y) = x + \mathrm{i}y, \qquad r = |z| = \sqrt{x^2 + y^2}$$

$$x = r\cos\theta, \qquad y = r\sin\theta$$

$$z = r e^{\mathrm{i}\theta}, \qquad |z| = r$$

y utilizando la identidad de Euler (referida en las diapositivas como «fórmula de Moivre»):

$$e^{\mathrm{i}\theta} = \cos\theta + \mathrm{i}\sin\theta$$

> **Nota:** En las diapositivas se denomina «fórmula de Moivre» a la fórmula de Euler $e^{\mathrm{i}\theta} = \cos\theta + \mathrm{i}\sin\theta$ (la fórmula de De Moivre propiamente dicha es $(\cos\theta + \mathrm{i}\sin\theta)^n = \cos(n\theta) + \mathrm{i}\sin(n\theta)$).

> **[Figura]:** Dos representaciones equivalentes de un número complejo en el plano:
> 1. Plano complejo con ejes $\text{Re}$ (horizontal) e $\text{Im}$ (vertical): punto $z = (x, y) = x + \mathrm{i}y$ en el primer cuadrante, unido al origen por un segmento de longitud $r = \sqrt{x^2 + y^2}$ con ángulo $\theta$ respecto al eje $\text{Re}$, y líneas punteadas hacia sus coordenadas $x$ e $y$.
> 2. Plano $(x, y)$ con el mismo vector de módulo $r$ y ángulo $\theta$ formando un rectángulo cuyas llaves muestran las proyecciones $x = r\cos(\theta)$ (horizontal) e $y = r\sin(\theta)$ (vertical).

Representamos las cantidades sinusoidales reales como la **parte real del número complejo**:

$$v(t) = V\cos\omega t = \operatorname{Re}\left\{V e^{\mathrm{i}\omega t}\right\}, \qquad \mathrm{i} = \sqrt{-1}$$

En general, trabajamos con las funciones complejas:

$$q(t) = Q e^{\mathrm{i}\omega t}$$

$$v(t) = V e^{\mathrm{i}\omega t}$$

$$i(t) = I e^{\mathrm{i}\omega t}$$

donde $Q$, $I$ y $V$ son **constantes complejas** (fasores o amplitudes complejas). Al final del cálculo, las cantidades físicas medibles se determinan tomando la **parte real** de las cantidades complejas.

> **[Figura]:** Dos gráficos complementarios sobre fase y fasores:
> 1. **Fasores en fase (resistor):** en el primer cuadrante, un fasor de corriente de longitud $I$ y un fasor de voltaje de longitud $V_R$ (superpuesto sobre la misma dirección) forman un ángulo $\omega t$ con el eje horizontal y giran juntos. Sus proyecciones horizontales representan los valores instantáneos $v_R$ e $i$.
> 2. **Desfase temporal entre ondas:** ejes vertical (amplitud $A$) y horizontal ($t$). Una curva continua $A\cos(\omega t)$ tiene su máximo en $t = 0$; una curva discontinua $A\cos(\omega t + \phi)$ está desplazada hacia la izquierda (adelantada) en un intervalo de tiempo $\phi/\omega$.

## Valor cuadrático medio o eficaz (rms)

En la corriente alterna, la intensidad cambia continuamente de magnitud y de sentido, por lo que su promedio simple en un ciclo completo es nulo:

$$V_{\text{prom}} = \frac{1}{T}\int_0^T v(t)\,dt = \frac{V}{T}\int_0^T \cos\omega t\,dt = 0$$

Para saber qué corriente o voltaje **continuos** producirían el mismo efecto (por ejemplo, la misma potencia media o el mismo calor disipado en un resistor), se define el **valor cuadrático medio o eficaz (rms)** integrando el cuadrado de la señal durante un período $T = 2\pi/\omega$:

$$V_{\text{rms}} = \sqrt{\frac{1}{T}\int_0^T \big(v(t)\big)^2\,dt} = \sqrt{\frac{V^2}{T}\int_0^T \cos^2\omega t\,dt} = \sqrt{\frac{V^2}{T}\int_0^T \frac{1 + \cos(2\omega t)}{2}\,dt} = \frac{V}{\sqrt{2}}$$

Para toda señal sinusoidal (corriente o voltaje):

$$I_{\text{rms}} = \frac{I}{\sqrt{2}} \qquad \text{(valor cuadrático medio de una corriente sinusoidal)}$$

$$V_{\text{rms}} = \frac{V}{\sqrt{2}} \qquad \text{(valor cuadrático medio de un voltaje sinusoidal)}$$

donde $I$ y $V$ son las **amplitudes** (valores pico) e $I_{\text{rms}}$ y $V_{\text{rms}}$ son los **valores eficaces**.

### Ejemplo 1: Voltaje eficaz y amplitud pico en la red domiciliaria

> **[Figura]:** Fotografía de un enchufe macho de tres clavijas alineadas junto a un tomacorriente hembra de tres orificios, indicando $V_{\text{rms}} = 220\,\text{V}$ y que el voltaje instantáneo entre las terminales varía entre $-311\,\text{V}$ y $311\,\text{V}$.

> **Nota (errata):** En la diapositiva 10 el subíndice $\text{rms}$ en $V_{\text{rms}} = 220\,\text{V}$ no se visualiza (aparece un espacio en blanco entre $V$ y $=$).

**Enunciado:** La red eléctrica domiciliaria suministra un voltaje alterno sinusoidal de valor eficaz $V_{\text{rms}} = 220\,\text{V}$. Determine la amplitud (valor pico) $V$ y el rango de variación del voltaje instantáneo $v(t)$.

**Resolución**

*Idea:* Para un voltaje sinusoidal $v(t) = V\cos\omega t$, el valor eficaz se relaciona con la amplitud mediante $V_{\text{rms}} = V/\sqrt{2}$.

*Desarrollo:* Despejando la amplitud $V$:

$$V = \sqrt{2}\,V_{\text{rms}} = \sqrt{2}\,(220\,\text{V}) \approx 1.4142 \times 220\,\text{V} \approx 311.1\,\text{V}$$

Como $\cos\omega t$ oscila entre $-1$ y $+1$, el voltaje instantáneo $v(t) = V\cos\omega t$ varía entre $-V$ y $+V$:

$$\boxed{V \approx 311\,\text{V}, \qquad -311\,\text{V} \le v(t) \le +311\,\text{V}}$$

*Verificación:* El resultado tiene unidades de volt ($\text{V}$) y cumple $V > V_{\text{rms}}$ por un factor $\sqrt{2} \approx 1.414$, pues la amplitud máxima siempre supera al valor eficaz; además, $311\,\text{V}/\sqrt{2} \approx 219.9\,\text{V} \approx 220\,\text{V}$.

## Elementos básicos en circuitos de corriente alterna

### Resistor en un circuito de ca

Consideremos un resistor de resistencia $R$ conectado a una fuente de corriente alterna.

> **[Figura]:** Tres paneles para el circuito puramente resistivo:
> - **Circuito:** fuente de ca arriba en lazo cerrado con un resistor $R$ abajo entre los puntos $a$ (izquierda) y $b$ (derecha). La corriente $i$ circula de $a$ hacia $b$, y el voltaje entre terminales $v_R = V_a - V_b$ se mide entre $a$ y $b$.
> - **Gráficas $i, v$ contra $t$:** $i = I\cos\omega t$ (curva morada de amplitud $I$) y $v_R = IR\cos\omega t = V_R\cos\omega t$ (curva roja de amplitud $V_R$). Ambas curvas alcanzan sus crestas, valles y cruces por cero simultáneamente (están **en fase**).
> - **Diagrama de fasores:** los fasores de corriente ($I$) y voltaje ($V_R$) son colineales con ángulo $\omega t$ respecto al eje horizontal y giran juntos; sus proyecciones horizontales dan $i$ y $v_R$.

Usando la notación compleja, la ecuación de malla es:

$$v_R(t) - i(t)R = 0 \quad\Longrightarrow\quad i(t) = \frac{V_R}{R}e^{\mathrm{i}\omega t} = I e^{\mathrm{i}\omega t}$$

donde la amplitud máxima de voltaje (y también la relación entre valores eficaces $V_{R,\text{rms}} = I_{\text{rms}}R$) satisface:

$$V_R = IR$$

Tomando la parte real, la corriente y el voltaje instantáneos en el resistor son:

$$i = I\cos\omega t$$

$$v_R = V_R\cos\omega t$$

En un resistor, la corriente y el voltaje están **en fase** ($\phi = 0$) y las amplitudes guardan la misma relación que en corriente continua.

### Inductor en un circuito de ca

> **[Figura]:** Tres paneles para el circuito puramente inductivo:
> - **a) Circuito con fuente de ca e inductor:** fuente de ca arriba conectada en lazo cerrado con una bobina de inductancia $L$ abajo entre los puntos $a$ (izquierda) y $b$ (derecha); corriente $i$ dirigida de $a$ a $b$ y voltaje $v_L$ medido entre $a$ y $b$.
> - **b) Gráficas de corriente y voltaje contra el tiempo:** $i = I\cos\omega t$ (curva morada con cresta $I$ en $t=0$) y $v_L = I\omega L\cos(\omega t + 90^\circ)$ (curva roja de amplitud $V_L$). La curva del voltaje **adelanta** a la de la corriente en un cuarto de ciclo ($\frac{1}{4}T$, correspondiente a $\phi = \pi/2\,\text{rad} = 90^\circ$): por ejemplo, $v_L$ cruza por cero hacia valores negativos en $t=0$, mientras que $i$ lo hace en $t = T/4$.
> - **c) Diagrama de fasores:** el fasor de corriente $I$ está en el primer cuadrante a ángulo $\omega t$ con proyección horizontal $i$; el fasor de voltaje $V_L$ está girado $90^\circ$ en sentido antihorario respecto a $I$ (en el segundo cuadrante, ángulo $\omega t + 90^\circ$), con proyección horizontal $v_L$ negativa en ese instante.

Aunque un inductor ideal no tiene resistencia, **sí existe una diferencia de potencial** entre sus terminales $a$ y $b$ porque la corriente varía con el tiempo. Esta fem autoinducida está dada por la ley de Faraday, pero el voltaje terminal $v_L = V_a - V_b$ tiene el signo opuesto:

- Si la corriente en el inductor fluye en el sentido positivo (antihorario, de $a$ hacia $b$) y va en aumento, entonces $\frac{di}{dt} > 0$ y la fem inducida apunta hacia la izquierda para oponerse al aumento de la corriente.
- Por lo tanto, el punto $a$ queda a un potencial más alto que el punto $b$, de modo que el potencial de $a$ respecto a $b$ es positivo (es el negativo de la fem inducida): $v_L = +L\frac{di}{dt}$.
- Este signo se mantiene válido incluso cuando $i$ circula en sentido horario (aumentando o disminuyendo).

> **Nota (errata):** En la diapositiva 14 aparece escrito «`di>dt` es positiva» por error tipográfico en lugar de $di/dt > 0$ (o «$di/dt$ es positiva»).

**Representación compleja**

Con $i(t) = I e^{\mathrm{i}\omega t}$:

$$v_L = L\frac{di}{dt} = \mathrm{i}I\omega L\, e^{\mathrm{i}\omega t} = V_L e^{\mathrm{i}\omega t}$$

donde la amplitud compleja de voltaje es:

$$V_L = \mathrm{i}I\omega L$$

Tomando la parte real (usando $\mathrm{i} = e^{\mathrm{i}\pi/2}$ y $e^{\mathrm{i}\theta} = \cos\theta + \mathrm{i}\sin\theta$):

$$\operatorname{Re}\{v_L\} = I\omega L\cos\left(\omega t + \frac{\pi}{2}\right)$$

**Cálculo directo con funciones reales**

Si se trabaja directamente con $i = I\cos\omega t$:

$$v_L = L\frac{di}{dt} = L\frac{d}{dt}(I\cos\omega t) = -I\omega L\sin\omega t = I\omega L\cos\left(\omega t + \frac{\pi}{2}\right)$$

de donde la amplitud real del voltaje en el inductor es:

$$V_L = I\omega L$$

### Impedancia y reactancia inductiva

De la forma compleja $V_L = \mathrm{i}I\omega L$ (donde $V_L$ e $I$ son fasores), podemos escribir la relación entre voltaje y corriente de manera análoga a la ley de Ohm:

$$V_L = Z_L I, \qquad \text{con } Z_L = \mathrm{i}\omega L$$

donde $Z_L$ se define como la **impedancia** del inductor. La parte imaginaria de la impedancia recibe el nombre de **reactancia**, en este caso **reactancia inductiva**:

$$X_L = \operatorname{Im}\{Z_L\} = \omega L$$

El hecho de que la impedancia sea compleja significa que la corriente no está en fase con el voltaje aplicado. Con esta definición, las **amplitudes** (y también los valores eficaces $V_{L,\text{rms}} = I_{\text{rms}} X_L$) satisfacen una relación formalmente similar a la del resistor:

$$V_L = I X_L \qquad (\text{análogo a } V_R = IR)$$

- Si se aplica un voltaje oscilante de amplitud $V_L$ dada entre los terminales del inductor, la corriente resultante tendrá una amplitud $I = V_L / X_L$ más pequeña para valores mayores de $X_L$ (es decir, a mayor $\omega$ o mayor $L$).
- Como la reactancia es el cociente entre un voltaje y una corriente, su unidad en el SI es el **ohm ($\Omega$)**, la misma que la de la resistencia.
- La reactancia inductiva $X_L$ describe el efecto de la fem autoinducida que se opone a cualquier cambio en la corriente a través del inductor.

> **Nota (errata):** En la segunda frase de la diapositiva 18 se omite el subíndice en «La reactancia inductiva $X$» en lugar de $X_L$.

**Convención de fase respecto a la corriente**

Por lo general describiremos la **fase del voltaje en relación con la corriente**, y no a la inversa. Si la corriente en el circuito es:

$$i = I\cos\omega t$$

y el voltaje entre dos puntos es:

$$v = V\cos(\omega t + \phi)$$

entonces:
- Para un **resistor**: $\phi = 0$.
- Para un **inductor**: $\phi = \frac{\pi}{2}$.

> **[Figura]:** Comparación lado a lado de los diagramas fasoriales del resistor (izquierda: $V_R$ e $I$ colineales a ángulo $\omega t$, en fase) y del inductor (derecha: $V_L$ adelantado un ángulo de fase $\phi = \pi/2\,\text{rad} = 90^\circ$ respecto a $I$).

### Capacitor en un circuito de ca y reactancia capacitiva

> **[Figura]:** Tres paneles para el circuito puramente capacitivo:
> - **a) Circuito con fuente de ca y capacitor:** fuente de ca arriba conectada en lazo cerrado con un capacitor de placas paralelas $C$ abajo entre $a$ (placa izquierda con carga $+q$) y $b$ (placa derecha con carga $-q$); la corriente $i$ entra hacia $a$ y sale desde $b$, y el voltaje entre placas es $v_C = V_a - V_b$.
> - **b) Gráficas de corriente y voltaje contra el tiempo:** $i = I\cos\omega t$ (curva morada con máximo $I$ en $t=0$) y $v_C = \frac{I}{\omega C}\cos(\omega t - 90^\circ)$ (curva roja de amplitud $V_C$). La curva del voltaje **se retrasa** respecto a la corriente en un cuarto de ciclo ($\frac{1}{4}T$, correspondiente a $\phi = -\pi/2\,\text{rad} = -90^\circ$): en $t=0$, $v_C = 0$ y alcanza su máximo en $t = T/4$.
> - **c) Diagrama de fasores:** el fasor de corriente $I$ está en el primer cuadrante a ángulo $\omega t$ con proyección horizontal $i$; el fasor de voltaje $V_C$ está girado $90^\circ$ en sentido horario respecto a $I$ (en el cuarto cuadrante, ángulo $\omega t - 90^\circ$), con proyección horizontal positiva $v_C$ en el instante mostrado.

En notación compleja, la corriente es la derivada temporal de la carga $q(t) = Q e^{\mathrm{i}\omega t}$:

$$i(t) = I e^{\mathrm{i}\omega t} = \frac{dq}{dt} = \mathrm{i}\omega Q e^{\mathrm{i}\omega t} \quad\Longrightarrow\quad Q = \frac{I}{\mathrm{i}\omega}$$

> **Nota (errata):** En la diapositiva 21 la unidad imaginaria delante de $\omega Q e^{\mathrm{i}\omega t}$ aparece impresa en cursiva ($i\omega Q e^{\mathrm{i}\omega t}$) en lugar de la letra recta $\mathrm{i}$ utilizada en el resto de la diapositiva.

El voltaje complejo en el capacitor es $v_C = q/C$:

$$v_C = \frac{q}{C} = \frac{I}{\mathrm{i}\omega C}e^{\mathrm{i}\omega t}$$

Tomando la parte real (usando $1/\mathrm{i} = -\mathrm{i} = e^{-\mathrm{i}\pi/2}$):

$$\operatorname{Re}\{v_C\} = \frac{I}{\omega C}\cos\left(\omega t - \frac{\pi}{2}\right)$$

El voltaje y la corriente del capacitor están fuera de fase por un cuarto de ciclo (el voltaje atrasa $90^\circ$ a la corriente). En forma fasorial, el voltaje complejo (amplitud compleja) y la impedancia del capacitor son:

$$V_C = \frac{I}{\mathrm{i}\omega C}, \qquad Z_C = \frac{1}{\mathrm{i}\omega C} = -\frac{\mathrm{i}}{\omega C}$$

Luego, la **reactancia capacitiva** definida como la parte imaginaria de la impedancia es:

$$X_C = \operatorname{Im}\{Z_C\} = -\frac{1}{\omega C}$$

*(Nota sobre convenciones: cuando se relaciona la amplitud real $V_C = I X_C$, suele usarse el valor positivo $X_C = \frac{1}{\omega C}$, reservando el signo negativo para la parte imaginaria de $Z_C = -\mathrm{i}/(\omega C)$, como se observa en la tabla resumen y en el circuito LRC más abajo).*

De $X_C$ se deduce que **a mayor capacitancia $C$ o mayor frecuencia $\omega$, menor magnitud de reactancia** $|X_C|$. Por eso, los capacitores permiten el paso de corrientes de alta frecuencia y bloquean las de baja frecuencia y la corriente continua, al contrario que los inductores. Un circuito que deja pasar preferentemente señales de alta frecuencia se denomina **filtro pasa-alto**.

### Resumen de elementos en un circuito de ca

| Elemento de circuito | Relación de amplitudes | Cantidad de circuito | Fase de $v$ respecto a $i$ | Impedancia $Z$ |
| :--- | :--- | :--- | :--- | :--- |
| Resistor | $V_R = I R$ | $R$ | En fase con $i$ ($\phi = 0$) | $R$ |
| Inductor | $V_L = I X_L$ | $X_L = \omega L$ | Se adelanta $90^\circ$ a $i$ ($\phi = +\pi/2$) | $\mathrm{i}\omega L$ |
| Capacitor | $V_C = I X_C$ | $X_C = \dfrac{1}{\omega C}$ | Se retrasa $90^\circ$ respecto a $i$ ($\phi = -\pi/2$) | $\dfrac{-\mathrm{i}}{\omega C}$ |

En todos los casos, en representación fasorial se cumple $V = Z I$ (válida tanto para amplitudes complejas como para valores eficaces complejos). Recuerde que el voltaje y la corriente **instantáneos** son proporcionales en un resistor ($v_R = i R$, desfase nulo), mientras que **no** son proporcionales en un inductor ni en un capacitor porque existe una diferencia de fase de $90^\circ$.

> **[Figura]:** Gráfica de $R$ y $X$ (magnitudes de reactancia) en función de la frecuencia angular $\omega$ a partir del origen $O$:
> - La resistencia $R$ es una línea recta horizontal constante (en color magenta).
> - La reactancia inductiva $X_L = \omega L$ es una recta creciente que parte del origen con pendiente $L$.
> - La reactancia capacitiva $X_C = 1/(\omega C)$ es una hipérbola decreciente que tiende a $+\infty$ cuando $\omega \to 0^+$ y a $0$ cuando $\omega \to \infty$, intersecando a la recta $X_L$ en una frecuencia determinada.

## Circuito LRC en serie e impedancias

### El circuito LRC en serie

> **[Figura]:** Circuito LRC en serie dispuesto en un lazo rectangular con vértices $a$ (arriba izquierda), $b$ (abajo izquierda), $c$ (abajo derecha) y $d$ (arriba derecha). En la rama superior se ubica la fuente de ca, con la corriente $i$ saliendo hacia la izquierda (sentido antihorario); en la rama izquierda $a\text{--}b$ hay un resistor $R$; en la rama inferior $b\text{--}c$ un inductor $L$; y en la rama derecha $c\text{--}d$ un capacitor $C$ con carga $+q$ en la placa inferior y $-q$ en la superior.

Aplicando la regla de Kirchhoff de mallas en el sentido de la corriente $i$:

$$v - iR - L\frac{di}{dt} - \frac{q}{C} = 0$$

Derivando respecto al tiempo (recordando que $i = dq/dt$):

$$\frac{dv}{dt} - R\frac{di}{dt} - L\frac{d^2 i}{dt^2} - \frac{1}{C}i = 0$$

Reemplazando $i(t) = I e^{\mathrm{i}\omega t}$ y $v(t) = V e^{\mathrm{i}\omega t}$ (de modo que $\frac{d}{dt} \leftrightarrow \mathrm{i}\omega$ y $\frac{d^2}{dt^2} \leftrightarrow -\omega^2$):

$$\mathrm{i}\omega V e^{\mathrm{i}\omega t} - \mathrm{i}\omega R I e^{\mathrm{i}\omega t} + \omega^2 L I e^{\mathrm{i}\omega t} - \frac{1}{C} I e^{\mathrm{i}\omega t} = 0$$

Dividiendo por $\mathrm{i}\omega e^{\mathrm{i}\omega t}$, se obtiene:

$$V = Z I \qquad \text{con } Z = R + \mathrm{i}\omega L - \frac{\mathrm{i}}{\omega C} = R + \mathrm{i}\left(\omega L - \frac{1}{\omega C}\right)$$

Es decir, **la impedancia total es la suma de las impedancias de cada elemento** ($Z = Z_R + Z_L + Z_C$).

Si se escribe la impedancia en forma polar:

$$Z = |Z|e^{\mathrm{i}\phi} \qquad \text{con } |Z| = \sqrt{R^2 + \left(\omega L - \frac{1}{\omega C}\right)^2}$$

$$\phi = \tan^{-1}\left(\frac{\omega L - 1/(\omega C)}{R}\right)$$

entonces la corriente compleja instantánea resulta:

$$i(t) = \frac{v(t)}{Z} = \frac{V e^{\mathrm{i}\omega t}}{|Z|e^{\mathrm{i}\phi}} = \frac{V}{|Z|}e^{\mathrm{i}(\omega t - \phi)}$$

cuya parte real es $i(t) = \frac{V}{|Z|}\cos(\omega t - \phi)$, con amplitud de corriente $I = \frac{V}{|Z|}$ (e igualmente $I_{\text{rms}} = \frac{V_{\text{rms}}}{|Z|}$).

> **Nota (errata):** En la diapositiva 25 aparece escrito $|z|$ en minúscula dentro de la fórmula del módulo $|Z|$, y en la expresión de $i(t)$ aparece $v/Z$ (en minúscula) igualado a $\frac{V}{|Z|}e^{\mathrm{i}(\omega t - \phi)}$; aquí se unifica la notación como $|Z|$ y $v(t) = V e^{\mathrm{i}\omega t}$.

### Impedancias en serie

Si se conectan elementos de impedancia $Z_i$ en serie, la misma corriente atraviesa a todos ellos, de modo que el voltaje y la impedancia equivalente son:

$$V = V_1 + V_2 + \dots = \sum_i V_i, \qquad Z = Z_1 + Z_2 + \dots = \sum_i Z_i$$

**Importante:** siempre se deben sumar las **impedancias (números complejos)**, no las magnitudes ni las reactancias por separado sin signo. Así, para dos impedancias $Z_1 = R_1 + \mathrm{i}X_1$ y $Z_2 = R_2 + \mathrm{i}X_2$:

$$Z = Z_1 + Z_2 = (R_1 + R_2) + \mathrm{i}(X_1 + X_2)$$

En forma polar, $Z = |Z|e^{\mathrm{i}\phi}$, donde:

$$|Z| = \sqrt{(R_1 + R_2)^2 + (X_1 + X_2)^2}, \qquad \phi = \tan^{-1}\left(\frac{X_1 + X_2}{R_1 + R_2}\right)$$

### Impedancias en paralelo y asociaciones mixtas

Si se conectan elementos de impedancia $Z_i$ en paralelo, comparten el mismo voltaje y las corrientes se suman:

$$V = V_1 = V_2 = \dots = V_i$$

$$I = I_1 + I_2 + \dots = \frac{V}{Z_1} + \frac{V}{Z_2} + \dots = V\left(\frac{1}{Z_1} + \frac{1}{Z_2} + \dots\right)$$

Por lo tanto, la impedancia equivalente en paralelo cumple:

$$\frac{1}{Z} = \frac{1}{Z_1} + \frac{1}{Z_2} + \dots$$

En resumen:
- **Serie:** $Z = Z_1 + Z_2 + \dots = \sum_i Z_i$
- **Paralelo:** $\dfrac{1}{Z} = \dfrac{1}{Z_1} + \dfrac{1}{Z_2} + \dots$

> **[Figura]:** Reducción paso a paso de un circuito mixto de impedancias:
> 1. Circuito original: impedancia $Z_1$ en serie con el paralelo de $Z_2$ y $Z_3$.
> 2. Circuito intermedio equivalente: $Z_1$ en serie con $Z_p$, donde $Z_p = \dfrac{Z_2 Z_3}{Z_2 + Z_3}$.
> 3. Impedancia equivalente total: un único bloque $Z_T = Z_1 + \dfrac{Z_2 Z_3}{Z_2 + Z_3}$.

## Potencia en circuitos de corriente alterna

La **potencia instantánea** entregada a un dispositivo o circuito es el producto de los valores físicos (reales) instantáneos del voltaje y la corriente:

$$p = v\,i \quad\longrightarrow\quad P(t) = \operatorname{Re}\{i(t)\}\operatorname{Re}\{v(t)\}$$

> **[Figura]:** Cuatro gráficas temporales de $v$ (curva azul), $i$ (curva morada) y la potencia instantánea $p = vi$ (curva negra) frente a $t$:
> - **a) Resistor:** $v$ e $i$ están en fase (ambos positivos o ambos negativos simultáneamente), por lo que $p = vi \ge 0$ en todo instante, oscilando entre $0$ y $VI$ al doble de frecuencia, con línea punteada de potencia media en $P_{\text{med}} = \frac{1}{2}VI$.
> - **b) Inductor:** $v$ adelanta a $i$ en $90^\circ$; $p$ oscila simétricamente tomando valores positivos y negativos iguales, de modo que $P_{\text{med}} = 0$.
> - **c) Capacitor:** $v$ retrasa a $i$ en $90^\circ$; $p$ oscila simétricamente entre valores positivos y negativos iguales, de modo que $P_{\text{med}} = 0$.
> - **d) Circuito de ca arbitrario:** existe un desfase $\phi$ entre $v$ e $i$; $p$ es mayormente positiva con breves intervalos negativos por ciclo, y la potencia media es positiva: $P_{\text{med}} = \frac{1}{2}VI\cos\phi$.

Sin embargo, suele ser más útil conocer la **potencia media** durante un período completo. Si $i(t) = |I|\cos\omega t$ y $v(t) = |V|\cos(\omega t + \phi)$, promediando sobre un ciclo se obtiene:

$$\langle P \rangle = \big\langle \operatorname{Re}\{i(t)\}\operatorname{Re}\{v(t)\} \big\rangle = \frac{1}{2}|I||V|\cos\phi = |I_{\text{rms}}||V_{\text{rms}}|\cos\phi$$

donde $\cos\phi$ es el factor de potencia.

- **Potencia en un resistor** ($\phi = 0$, $\cos 0 = 1$):

$$P_{\text{med}} = \frac{1}{2}VI = \frac{V}{\sqrt{2}}\frac{I}{\sqrt{2}} = V_{\text{rms}}I_{\text{rms}} = I_{\text{rms}}^2 R = \frac{V_{\text{rms}}^2}{R}$$

- **Potencia en un capacitor o un inductor ideales:** el desfase es $\phi = \pm\pi/2$, entonces $\cos(\pm\pi/2) = 0$, por lo que **la potencia media en un ciclo es cero** (la energía se almacena y se devuelve a la fuente en cada ciclo sin disiparse).

## Resonancia en circuitos LRC en serie

Gran parte de la importancia práctica de los circuitos LRC en serie radica en cómo responden a fuentes de distinta frecuencia angular $\omega$. Recordando que:

$$Z = |Z|e^{\mathrm{i}\phi}, \qquad |Z| = \sqrt{R^2 + \left(\omega L - \frac{1}{\omega C}\right)^2}, \qquad \phi = \tan^{-1}\left(\frac{\omega L - 1/(\omega C)}{R}\right)$$

$$i(t) = \frac{v(t)}{Z} = \frac{V}{|Z|}e^{\mathrm{i}(\omega t - \phi)}$$

La impedancia alcanza su valor mínimo cuando se cancelan las reactancias inductiva y capacitiva ($\omega L = \frac{1}{\omega C}$), es decir, cuando $Z = R$ (y $|Z| = R$). En ese punto se alcanza la **corriente máxima** para una amplitud de voltaje dada, fenómeno denominado **resonancia**, que ocurre a la frecuencia angular de resonancia:

$$\omega_0 = \frac{1}{\sqrt{LC}}$$

> **[Figura]:** Curvas de resonancia de la amplitud de corriente $I$ (eje vertical, en $\text{A}$, de $0$ a $0.5$) frente a la frecuencia angular $\omega$ (eje horizontal, en $\text{rad/s}$, de $0$ a $2000$) para tres resistencias distintas ($200\,\Omega$, $500\,\Omega$ y $2000\,\Omega$), todas centradas en $\omega_0 = 1000\,\text{rad/s}$:
> - Con $R = 200\,\Omega$, la curva presenta un pico alto y agudo hasta $I \approx 0.5\,\text{A}$.
> - Con $R = 500\,\Omega$, el pico alcanza $I \approx 0.2\,\text{A}$.
> - Con $R = 2000\,\Omega$, la curva es baja y ancha con un máximo de $I \approx 0.05\,\text{A}$.
> Cuanto menor es la resistencia $R$ del circuito, más alta y pronunciada es la curva de resonancia cerca de $\omega_0$.

## Transformadores

Un **transformador** es un dispositivo que cambia el voltaje de una señal de corriente alterna mediante inducción electromagnética. Una de las grandes ventajas de la corriente alterna sobre la continua en la distribución de energía eléctrica es que resulta mucho más sencillo elevar y reducir voltajes con ca que con cc.

El devanado al que se suministra energía se llama **primario** ($N_1$ espiras), y el devanado del que se toma energía recibe el nombre de **secundario** ($N_2$ espiras).

> **[Figura]:** Esquema tridimensional de un transformador ideal: un núcleo rectangular hueco de hierro canaliza líneas cerradas de flujo magnético $\Phi_B$ en su interior. En la rama izquierda está enrollado el devanado primario ($N_1$ espiras), alimentado por una fuente de ca con voltaje terminal $V_1$ y corriente $I_1$. En la rama derecha está enrollado el devanado secundario ($N_2$ espiras), conectado a una resistencia de carga $R$ entre cuyos terminales hay un voltaje $V_2$.

Suponiendo que todo el flujo magnético $\Phi_B$ queda confinado al núcleo de hierro, el flujo es el mismo en ambos devanados, por lo que las fem inducidas cumplen:

$$\mathcal{E}_1 = -N_1\frac{d\Phi_B}{dt} \qquad \text{y} \qquad \mathcal{E}_2 = -N_2\frac{d\Phi_B}{dt}$$

Dividiendo ambas expresiones (la fem inducida *por espira* es la misma en ambas bobinas):

$$\frac{\mathcal{E}_2}{\mathcal{E}_1} = \frac{N_2}{N_1}$$

Como ambos voltajes oscilan con la misma frecuencia (y despreciando la resistencia de los devanados):

$$\frac{V_2}{V_1} = \frac{N_2}{N_1}$$

donde $V_1$ y $V_2$ son las **amplitudes** o bien los **valores rms** de los voltajes terminales del primario y secundario, respectivamente.

Si se completa el circuito secundario con una resistencia $R$, entonces la amplitud (o el valor rms) de la corriente en el secundario es $I_2 = V_2/R$. En un transformador ideal (sin pérdidas ni resistencia en los devanados), la potencia media entregada al primario es igual a la potencia que sale del secundario:

$$V_1 I_1 = V_2 I_2 \qquad \text{(voltajes y corrientes terminales del primario y secundario; ambos en amplitud o ambos en rms)}$$

Combinando $V_1 I_1 = V_2 I_2$, $I_2 = V_2 / R$ y $V_2 / V_1 = N_2 / N_1$, se obtiene la resistencia equivalente vista desde el circuito primario:

$$\frac{V_1}{I_1} = \frac{V_1^2}{V_1 I_1} = \frac{V_1^2}{V_2 I_2} = \frac{V_1^2}{V_2 (V_2/R)} = \left(\frac{V_1}{V_2}\right)^2 R = \frac{R}{(N_2/N_1)^2}$$

$$\frac{V_1}{I_1} = \frac{R}{(N_2/N_1)^2}$$

## Resumen de fórmulas

| Fórmula | Significado | Condiciones |
| :--- | :--- | :--- |
| $v(t) = V\cos\omega t = \operatorname{Re}\{V e^{\mathrm{i}\omega t}\}$ | Voltaje sinusoidal instantáneo y representación compleja | Régimen estacionario sinusoidal; $V$ amplitud (pico) |
| $i(t) = I\cos\omega t = \operatorname{Re}\{I e^{\mathrm{i}\omega t}\}$ | Corriente sinusoidal instantánea y representación compleja | $\omega = 2\pi f$; tomar $\operatorname{Re}\{\cdot\}$ al final |
| $V_{\text{rms}} = \dfrac{V}{\sqrt{2}}, \quad I_{\text{rms}} = \dfrac{I}{\sqrt{2}}$ | Valores eficaces o cuadráticos medios (rms) | Señales puramente sinusoidales |
| $V_R = I R, \quad Z_R = R$ | Relación de amplitudes e impedancia de un resistor | $\phi = 0$ ($v_R$ e $i$ en fase) |
| $X_L = \omega L, \quad Z_L = \mathrm{i}\omega L, \quad V_L = I X_L$ | Reactancia inductiva, impedancia y amplitud en un inductor | $\phi = +\pi/2$ ($v_L$ adelanta $90^\circ$ a $i$) |
| $X_C = -\dfrac{1}{\omega C}$ ($\left|X_C\right| = \dfrac{1}{\omega C}$), $\quad Z_C = \dfrac{1}{\mathrm{i}\omega C} = -\dfrac{\mathrm{i}}{\omega C}$ | Reactancia capacitiva e impedancia de un capacitor | $\phi = -\pi/2$ ($v_C$ retrasa $90^\circ$ respecto a $i$); $V_C = I|X_C|$ |
| $Z = R + \mathrm{i}\left(\omega L - \dfrac{1}{\omega C}\right)$ | Impedancia compleja del circuito LRC en serie | Elementos $R, L, C$ ideales en serie a frecuencia $\omega$ |
| $\|Z\| = \sqrt{R^2 + \left(\omega L - \dfrac{1}{\omega C}\right)^2}, \quad \phi = \tan^{-1}\!\left(\dfrac{\omega L - 1/(\omega C)}{R}\right)$ | Módulo de impedancia y ángulo de fase en LRC serie | $i(t) = \operatorname{Re}\left\{\dfrac{V}{|Z|}e^{\mathrm{i}(\omega t - \phi)}\right\}$ |
| $Z_{\text{eq}} = \sum_i Z_i \quad \text{(serie)}, \qquad \dfrac{1}{Z_{\text{eq}}} = \sum_i \dfrac{1}{Z_i} \quad \text{(paralelo)}$ | Asociación de impedancias en serie y en paralelo | Deben sumarse impedancias complejas, no solo módulos |
| $\langle P \rangle = \dfrac{1}{2}|I||V|\cos\phi = |I_{\text{rms}}||V_{\text{rms}}|\cos\phi$ | Potencia media disipada en un ciclo completo | $\phi$ desfase entre $v$ e $i$; en $R$: $P_{\text{med}} = I_{\text{rms}}^2 R = V_{\text{rms}}^2/R$; en $L, C$: $0$ |
| $\omega_0 = \dfrac{1}{\sqrt{LC}}$ | Frecuencia angular de resonancia en LRC serie | Impedancia mínima $Z = R$ y corriente máxima |
| $\dfrac{V_2}{V_1} = \dfrac{N_2}{N_1}, \quad V_1 I_1 = V_2 I_2, \quad \dfrac{V_1}{I_1} = \dfrac{R}{(N_2/N_1)^2}$ | Relaciones de voltajes, potencia e impedancia reflejada en un transformador | Transformador ideal (mismo flujo $\Phi_B$, sin pérdidas, carga $R$ en secundario) |
