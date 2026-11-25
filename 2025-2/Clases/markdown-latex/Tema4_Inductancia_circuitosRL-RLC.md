---
title: "Inductancia y circuitos RL, LC y RLC"
source_pdf: "Electro/2025-2/Clases/Tema4_Inductancia_circuitosRL-RLC.pdf"
pages: 23
extraction_mode: "visual_latex_transcription"
---

# Inductancia y circuitos RL, LC y RLC

> **Nota sobre el título:** La portada de la presentación indica *"Circuitos RL RC y RLC"*, aunque las diapositivas desarrollan inductancia mutua, autoinductancia, inductores y circuitos $RL$, $LC$ y $RLC$.

## Inductancia mutua

> **[Figura]:** Dos bobinas coaxiales enfrentadas en el espacio. A la izquierda, la **Bobina 1** ($N_1$ espiras, representada como un arco grueso de múltiples conductores en perspectiva) conduce una corriente $i_1$ que asciende por su cara frontal (indicada con flechas moradas); esta corriente genera líneas de campo magnético $\vec{B}$ (en azul) que atraviesan el interior de la bobina de izquierda a derecha y se cierran por el exterior arriba y abajo. A la derecha, la **Bobina 2** ($N_2$ espiras, de menor diámetro y alineada sobre el mismo eje horizontal) es atravesada por una fracción de dichas líneas de campo, correspondiendo al flujo magnético $\Phi_{B2}$.

Si la corriente $i_1$ en la bobina 1 está cambiando, el flujo magnético cambiante $\Phi_{B2}$ a través de la bobina 2 induce una fuerza electromotriz (fem) en esta última. Se define la **inductancia mutua** $M_{21}$ mediante

$$M_{21} = \frac{N_2\Phi_{B2}}{i_1}$$

De manera general, la inductancia mutua cumple la simetría $M_{12} = M_{21} = M$, aun cuando las dos bobinas no sean simétricas. Así:

$$M = \frac{N_2\Phi_{B2}}{i_1} = \frac{N_1\Phi_{B1}}{i_2}$$

Las fem mutuamente inducidas en cada bobina por la variación de corriente en la otra están dadas por

$$\varepsilon_2 = -M\frac{di_1}{dt} \qquad \text{y} \qquad \varepsilon_1 = -M\frac{di_2}{dt}$$

La unidad de medida de la inductancia en el Sistema Internacional es el **henry** ($\text{H}$):

$$1\,\text{H} = 1\,\text{Wb/A} = 1\,\text{V}\cdot\text{s/A} = 1\,\Omega\cdot\text{s} = 1\,\text{J/A}^2$$

## Autoinductancia

> **[Figura]:** Circuito formado por una bobina helicoidal (solenoide de pocas espiras) conectada en serie a una batería (ubicada abajo a la derecha, con el terminal $+$ hacia la rama derecha y el $-$ hacia la rama inferior). Las flechas moradas indican el sentido de la corriente $i$: sale del polo positivo hacia la izquierda por la rama inferior, sube hacia las espiras por la rama derecha, recorre el enrollado y desciende por la rama izquierda. Las líneas azules de campo magnético $\vec{B}$ atraviesan el interior de la bobina de derecha a izquierda y retornan cerrándose por la parte superior e inferior del solenoide.

Si la corriente $i$ en la bobina está cambiando, el flujo magnético cambiante $\Phi_B$ a través de sus propias espiras induce una fem en la propia bobina. Partiendo de la definición de **autoinductancia** $L$:

$$L = \frac{N\Phi_B}{i}$$

Derivando respecto del tiempo (para geometría fija), resulta

$$N\frac{d\Phi_B}{dt} = L\frac{di}{dt}$$

Por la ley de Faraday-Lenz ($\varepsilon = -N\,d\Phi_B/dt$), la fem autoinducida es

$$\varepsilon = -L\frac{di}{dt}$$

## Inductor y energía almacenada

Si un circuito contiene una bobina, como un solenoide, su autoinductancia **impide que la corriente en el circuito aumente o disminuya de manera instantánea**, lo que resulta útil cuando se requiere una corriente estable frente a una fuente externa con fem fluctuante. Un elemento de circuito con una gran inductancia se denomina **inductor**.

En el análisis de circuitos ideales se asumen las siguientes idealizaciones:

- Un resistor no tiene inductancia.
- Un inductor no tiene resistencia.

### Convención de potencial en resistores e inductores

> **[Figura]:** Cuatro tramos horizontales de circuito entre los nodos $a$ (izquierda) y $b$ (derecha), todos recorridos por una corriente $i$ dirigida de $a$ hacia $b$ (flecha morada hacia la derecha):
> - **a) Resistor con corriente $i$ de $a$ a $b$:** Resistor $R$ (zigzag magenta). El potencial disminuye de $a$ a $b$ (signo $+$ en $a$, $-$ en $b$), con $V_{ab} = iR > 0$.
> - **b) Inductor con corriente constante $i$ de $a$ a $b$:** Inductor $L$ (espiral verde), $di/dt = 0$. No hay diferencia de potencial ($\varepsilon = 0$), por lo que $V_{ab} = L\frac{di}{dt} = 0$.
> - **c) Inductor con corriente $i$ creciente de $a$ a $b$:** Inductor $L$, $di/dt > 0$. La fem inducida $\varepsilon$ apunta hacia la izquierda (de $b$ hacia $a$, flecha azul opuesta a $i$); el potencial disminuye de $a$ a $b$ ($+$ en $a$, $-$ en $b$), resultando $V_{ab} = L\frac{di}{dt} > 0$.
> - **d) Inductor con corriente $i$ decreciente de $a$ a $b$:** Inductor $L$, $di/dt < 0$. La fem inducida $\varepsilon$ apunta hacia la derecha (de $a$ hacia $b$, flecha azul a favor de $i$); el potencial se incrementa de $a$ a $b$ ($-$ en $a$, $+$ en $b$), resultando $V_{ab} = L\frac{di}{dt} < 0$.

### Energía almacenada en un inductor

> **[Figura]:** Dos elementos individuales entre los nodos $a$ y $b$ con corriente $i$ de $a$ a $b$: arriba, un resistor $R$ donde la energía se *disipa*; abajo, un inductor $L$ donde la energía se *almacena*. A la izquierda se muestra el diagrama conceptual en cadena de la derivación energética desde $\varepsilon = -L\frac{di}{dt}$ hasta $U = \frac{1}{2}LI^2$.

Para calcular la energía almacenada en un inductor por el que circula una corriente, partimos de la diferencia de potencial entre sus terminales al recorrerlo en el sentido de la corriente ($V_{ab} = L\,di/dt$, asociada a $\varepsilon = -L\,di/dt$). La potencia entregada al inductor es

$$P = V_{ab}\,i = Li\frac{di}{dt}$$

Como $dU = P\,dt$, el diferencial de energía almacenada resulta

$$dU = Li\,di$$

Integrando desde corriente nula hasta una corriente final $I$:

$$U = L\int_0^I i\,di = \frac{1}{2}LI^2$$

> **[Figura]:** Circuito $RL$ con tres ramas horizontales en paralelo entre dos nodos verticales extremos:
> - **Rama superior:** Fuente de fem $\varepsilon$ (polo $+$ a la izquierda, $-$ a la derecha) en serie con un interruptor $S_1$ (mostrado abierto, con flecha punteada azul hacia abajo).
> - **Rama central:** Nodo $a$, resistor $R$, nodo $b$, inductor $L$ y nodo $c$, con corriente $i$ indicada por una flecha morada hacia la derecha debajo del tramo entre $R$ y $L$.
> - **Rama inferior:** Interruptor $S_2$ (mostrado abierto, con flecha punteada azul hacia arriba).

Cuando se desconecta la fuente y se deja circular la corriente únicamente por la malla $R$-$L$, **la energía disipada por la resistencia estaba previamente almacenada en el campo magnético generado por el inductor**.

## Circuitos RL

### Circuito RL conectado a una fuente de fem

> **[Figura]:** Mismo circuito $RL$ de tres ramas horizontales: al cerrar el interruptor $S_1$ (manteniendo abierto $S_2$) se conecta la combinación $R$-$L$ en serie con la fuente de fem $\varepsilon$; al cerrar $S_2$ al mismo tiempo que se abre $S_1$ se desconecta la combinación de la fuente.

Sea $i$ la corriente en cierto instante $t$ después de que se cerró el interruptor $S_1$, y sea $di/dt$ su tasa de cambio en ese instante. La diferencia de potencial $v_{ab}$ a través del resistor es

$$v_{ab} = iR$$

y la diferencia de potencial $v_{bc}$ a través del inductor es

$$v_{bc} = L\frac{di}{dt}$$

Aplicando la regla de mallas de Kirchhoff al lazo superior-central se obtiene

$$\varepsilon - iR - L\frac{di}{dt} = 0$$

> **Nota (errata):** En las diapositivas aparece escrita la ecuación $\varepsilon - ir - L\frac{di}{dt} = 0$ con $r$ minúscula; por consistencia con $v_{ab} = iR$ y con el paso siguiente, la resistencia del circuito es $R$.

Despejando la derivada temporal de la corriente:

$$\frac{di}{dt} = \frac{\varepsilon - iR}{L} = \frac{\varepsilon}{L} - \frac{R}{L}i$$

Analizando los instantes límite:

- **Cuando se cierra por primera vez el interruptor $S_1$** ($t = 0$, $i = 0$):

$$\left(\frac{di}{dt}\right)_{\text{inicial}} = \frac{\varepsilon}{L}$$

- **En estado estable** ($t \to \infty$, la corriente alcanza su valor constante $I$):

$$\left(\frac{di}{dt}\right)_{\text{final}} = 0 = \frac{\varepsilon}{L} - \frac{R}{L}I \qquad \Longrightarrow \qquad I = \frac{\varepsilon}{R}$$

La corriente final $I$ no depende de la inductancia $L$; es la misma que se tendría si solo se conectara la resistencia $R$ a la fuente con fem $\varepsilon$.

Para hallar la evolución temporal $i(t)$, se separan variables en la ecuación diferencial:

$$\frac{di}{i - (\varepsilon/R)} = -\frac{R}{L}\,dt$$

Integrando desde $t = 0$ (donde $i = 0$) hasta un instante arbitrario $t$ (con corriente $i$):

$$\ln\left(\frac{i - \varepsilon/R}{-\varepsilon/R}\right) = -\frac{R}{L}t \qquad \Longrightarrow \qquad i - \frac{\varepsilon}{R} = -\frac{\varepsilon}{R}e^{-(R/L)t}$$

De donde se obtiene la corriente en un circuito $R$-$L$ con fem:

$$i = \frac{\varepsilon}{R}\left(1 - e^{-(R/L)t}\right)$$

Se define la **constante de tiempo para un circuito $R$-$L$** como

$$\tau = \frac{L}{R}$$

La corriente aumenta desde cero hasta un valor límite dado por la resistencia ($I = \varepsilon/R$).

> **[Figura]:** Gráfica de la corriente $i$ (eje vertical) en función del tiempo $t$ (eje horizontal) desde el origen $O$. La curva morada parte de $(0,0)$ con pendiente inicial positiva $\varepsilon/L$, crece de forma cóncava hacia abajo y se aproxima asintóticamente a la recta horizontal discontinua $I = \varepsilon/R$. En el instante $t = \tau = L/R$, marcado sobre el eje $t$, la corriente alcanza el valor $I\left(1 - \frac{1}{e}\right)$ (aproximadamente el $63.2\,\%$ de $I$), señalado mediante una flecha vertical doble entre el eje $t$ y la curva.

### Balance de potencia en el circuito RL con fem

> **[Figura]:** Circuito $RL$ con el interruptor $S_1$ etiquetado como *cerrado* y $S_2$ abierto, junto con la ecuación de la malla y su desglose término a término de potencias mediante flechas.

Multiplicando la ecuación de la malla $\varepsilon - iR - L\frac{di}{dt} = 0$ por la corriente instantánea $i$ y reordenando:

$$\varepsilon i = i^2 R + L i \frac{di}{dt}$$

Cada término representa en cierto instante de tiempo:

- $\varepsilon i$: **potencia suministrada por la fuente**.
- $i^2 R$: **potencia disipada en el resistor**.
- $Li\frac{di}{dt}$: **potencia almacenada en el inductor**.

### Circuito RL desconectado de la fuente de fem

> **[Figura]:** Tres elementos visuales:
> 1. **Izquierda:** Circuito completo $RL$ con $S_1$ etiquetado *abierto* y $S_2$ etiquetado *cerrado*.
> 2. **Arriba derecha:** Circuito equivalente simplificado para $t \ge 0$, formado por una única malla cerrada con el resistor $R$ y el inductor $L$ en serie en la rama superior (corriente $i$ hacia la derecha) y el interruptor $S_2$ cerrado en la rama inferior (*"El interruptor $S_2$ se cierra en $t = 0$"*).
> 3. **Abajo derecha:** Gráfica de $i$ frente a $t$ desde el origen $O$. La curva morada parte en $t = 0$ del valor inicial $I_0$ y decrece exponencialmente de forma cóncava hacia arriba tendiendo asintóticamente a cero. En $t = \tau = L/R$, una flecha vertical señala que la corriente ha caído al valor $I_0/e$.

Supóngase que el interruptor $S_1$ ha permanecido cerrado durante un tiempo prolongado y la corriente ha alcanzado el valor $I_0$. Se reinicia el cronómetro para redefinir el tiempo inicial: en $t = 0$ se cierra el interruptor $S_2$ y se abre $S_1$.

Al quedar excluida la fuente de fem, la ecuación de la malla para $t > 0$ es

$$iR + L\frac{di}{dt} = 0$$

> **Nota (errata):** En la diapositiva la ecuación diferencial se escribe con $I$ mayúscula ($IR + L\frac{dI}{dt} = 0$), mientras que la solución inmediata emplea $i$ minúscula para la corriente instantánea y $I_0$ para la corriente inicial en $t = 0$.

Separando variables ($\frac{di}{i} = -\frac{R}{L}\,dt$) e integrando desde $i(0) = I_0$ hasta $i(t)$:

$$i = I_0 e^{-(R/L)t}$$

### Balance de potencia en el circuito RL sin fem

> **[Figura]:** Mismo conjunto de esquemas (circuito completo con $S_1$ abierto y $S_2$ cerrado, malla reducida y gráfica de decaimiento exponencial) junto a la ecuación de malla con el término $\varepsilon$ tachado por una flecha naranja diagonal.

Al desconectar la fuente ($\varepsilon = 0$) en $\varepsilon - iR - L\frac{di}{dt} = 0$ y multiplicar por $i$, resulta

$$0 = i^2 R + L i \frac{di}{dt} \qquad \Longrightarrow \qquad L i \frac{di}{dt} = -i^2 R$$

Es decir, **la energía almacenada en el inductor disminuye a una tasa igual a la tasa de disipación de la energía en el resistor**.

## Circuitos LC

### Ciclo de oscilación y transferencia de energía

> **[Figura]:** Arriba, esquema de un circuito $LC$ compuesto por un capacitor $C$ en la rama izquierda (con placa superior $+$ y placa inferior $-$, carga inicial $Q_{\text{máx}}$), un inductor $L$ en la rama derecha y un interruptor $S$ abierto en la rama inferior con una flecha curva azul indicando su cierre. Abajo, diagrama físico del estado inicial ($I = 0$): capacitor horizontal con placa superior naranja cargada con $+Q_{\text{máx}}$ (signos $+$), placa inferior celeste con $-Q_{\text{máx}}$ (signos $-$), flechas naranjas verticales hacia abajo que representan el campo eléctrico $\vec{E}$ entre las placas, y el inductor $L$ a la derecha sin campo magnético.

Supóngase un circuito formado por un capacitor $C$ inicialmente con carga $Q_{\text{máx}}$ que se conecta a una inductancia $L$.

1. **En $t = 0$:** El capacitor está totalmente cargado y la energía del circuito está almacenada íntegramente en el campo eléctrico del capacitor:

$$U = \frac{Q_{\text{máx}}^2}{2C}$$

En este momento la corriente en el circuito es cero ($I = 0$), por lo que no existe energía almacenada en el campo magnético de la inductancia.

> **[Figura]:** Dos diagramas de evolución en la primera mitad del ciclo:
> - **Superior ($Q = 0$, $I = I_{\text{máx}}$):** Las placas del capacitor están descargadas (color gris/lila). Las flechas moradas indican corriente en sentido horario (hacia la derecha arriba, hacia la izquierda abajo). Dentro del inductor $L$ aparecen flechas verdes verticales hacia abajo que representan el campo magnético $\vec{B}$.
> - **Inferior ($I = 0$, polaridad invertida):** El capacitor vuelve a estar completamente cargado, pero con la placa superior celeste ($-Q_{\text{máx}}$) y la placa inferior naranja ($+Q_{\text{máx}}$); las flechas naranjas del campo eléctrico $\vec{E}$ apuntan verticalmente hacia arriba, y no hay campo $\vec{B}$ en $L$.

2. **Primer cuarto de ciclo ($0 \to T/4$):** Al cerrar el interruptor, comienza a circular corriente, el capacitor se descarga y parte de la energía se transfiere a la inductancia. Cuando el capacitor está completamente descargado ($Q = 0$), la corriente alcanza su valor máximo $I_{\text{máx}}$ y toda la energía queda almacenada en el campo magnético de la inductancia.
3. **Segundo cuarto de ciclo ($T/4 \to T/2$):** La corriente continúa en la misma dirección, disminuyendo su magnitud hasta que el capacitor se vuelve a cargar por completo, pero con la polaridad de sus placas opuesta a la inicial. En este instante la corriente vuelve a ser cero.

> **[Figura]:** Dos diagramas de evolución en la segunda mitad del ciclo:
> - **Superior ($Q = 0$, $I = I_{\text{máx}}$ en sentido opuesto):** Las placas del capacitor están descargadas; la corriente (flechas moradas) circula ahora en sentido antihorario (hacia la izquierda arriba, hacia la derecha abajo) y el campo magnético $\vec{B}$ (flechas verdes) en el inductor $L$ apunta verticalmente hacia arriba.
> - **Inferior ($I = 0$, estado inicial recuperado):** Placa superior naranja con $+Q_{\text{máx}}$, placa inferior celeste con $-Q_{\text{máx}}$, campo eléctrico $\vec{E}$ hacia abajo y sin campo en $L$.

4. **Segunda mitad del ciclo ($T/2 \to T$):** A continuación, la corriente circula en sentido opuesto (pasando por un máximo $I_{\text{máx}}$ en $t = 3T/4$ cuando $Q = 0$) hasta que el capacitor se vuelve a cargar a su estado inicial.

En un instante $t > 0$ cualquiera, la energía total del sistema está dada por la suma de la energía eléctrica en el capacitor y la energía magnética en el inductor:

$$U = \frac{Q^2}{2C} + \frac{1}{2}LI^2$$

> **[Figura]:** Diagrama cíclico de resumen del circuito $LC$ con cuatro estados dispuestos en un bucle horario mediante flechas negras:
> - **Arriba-izquierda:** $I = 0$, capacitor con $+Q_{\text{máx}}$ arriba y $-Q_{\text{máx}}$ abajo ($\vec{E}$ hacia abajo); energía $U = \frac{Q_{\text{máx}}^2}{2C}$.
> - **Transición superior ($\to$):** $U = \frac{Q^2}{2C} + \frac{1}{2}LI^2$.
> - **Arriba-derecha:** $Q = 0$, $I = I_{\text{máx}}$ en sentido horario ($\vec{B}$ hacia abajo en $L$); energía $U = \frac{1}{2}LI^2$ (evaluada en $I_{\text{máx}}$).
> - **Abajo-derecha (tras $\downarrow$):** $I = 0$, capacitor con $-Q_{\text{máx}}$ arriba y $+Q_{\text{máx}}$ abajo ($\vec{E}$ hacia arriba); energía $U = \frac{Q_{\text{máx}}^2}{2C}$.
> - **Transición inferior ($\leftarrow$):** $U = \frac{Q^2}{2C} + \frac{1}{2}LI^2$.
> - **Abajo-izquierda:** $Q = 0$, $I = I_{\text{máx}}$ en sentido antihorario ($\vec{B}$ hacia arriba en $L$); energía $U = \frac{1}{2}LI^2$ (evaluada en $I_{\text{máx}}$), cerrando con una flecha ($\uparrow$) hacia el estado inicial.

### Ecuación diferencial y solución armónica

Suponiendo que no existen pérdidas de energía ($U = \text{cte}$), se cumple

$$\frac{dU}{dt} = \frac{Q}{C}\frac{dQ}{dt} + LI\frac{dI}{dt} = 0$$

Sustituyendo $I = \frac{dQ}{dt}$ y $\frac{dI}{dt} = \frac{d^2 Q}{dt^2}$ (y simplificando $I \neq 0$), la ecuación anterior queda

$$\frac{Q}{C} + L\frac{d^2 Q}{dt^2} = 0 \qquad \Longrightarrow \qquad \frac{d^2 Q}{dt^2} = -\frac{1}{LC}Q$$

Esta es la ecuación del oscilador armónico simple, cuya solución general es

$$Q = Q_{\text{máx}}\cos(\omega t + \phi)$$

donde la frecuencia angular natural es

$$\omega = \frac{1}{\sqrt{LC}}$$

y $\phi$ es la constante de fase, que depende de las condiciones iniciales del circuito. Derivando $Q(t)$ respecto del tiempo, la corriente está dada por

$$I = \frac{dQ}{dt} = -\omega Q_{\text{máx}}\sin(\omega t + \phi)$$

Si en $t = 0$ se tiene $Q = Q_{\text{máx}}$ e $I = 0$, entonces $\phi = 0$. Por lo tanto,

$$Q = Q_{\text{máx}}\cos(\omega t)$$

$$I = -\omega Q_{\text{máx}}\sin(\omega t) = -I_{\text{máx}}\sin(\omega t)$$

con $I_{\text{máx}} = \omega Q_{\text{máx}} = \frac{Q_{\text{máx}}}{\sqrt{LC}}$.

> **[Figura]:** Dos gráficas alineadas verticalmente en función del tiempo $t$, con líneas verticales punteadas azules que conectan los instantes $T/2$, $T$, $3T/2$ y $2T$:
> - **Gráfica superior ($Q$ vs. $t$):** Curva cosenoidal naranja que inicia en $+Q_{\text{máx}}$ en $t = 0$, alcanza $-Q_{\text{máx}}$ en $T/2$ y $3T/2$, y regresa a $+Q_{\text{máx}}$ en $T$ y $2T$.
> - **Gráfica inferior ($I$ vs. $t$):** Curva sinusoidal negativa naranja ($-\sin$) que parte de $0$ en $t = 0$, alcanza su mínimo $-I_{\text{máx}}$ en $T/4$, cruza por $0$ en $T/2$, alcanza su máximo $+I_{\text{máx}}$ en $3T/4$ (indicado con una línea horizontal discontinua hasta $I_{\text{máx}}$ en el eje vertical), cruza por $0$ en $T$, y repite el período en $2T$.

### Distribución de energía en el tiempo

Sustituyendo $Q(t)$ e $I(t)$ en la energía total del circuito $LC$:

$$U = U_C + U_L = \frac{Q_{\text{máx}}^2}{2C}\cos^2(\omega t) + \frac{1}{2}LI_{\text{máx}}^2\sin^2(\omega t)$$

Como la energía máxima eléctrica coincide con la energía máxima magnética,

$$\frac{Q_{\text{máx}}^2}{2C} = \frac{1}{2}LI_{\text{máx}}^2$$

(lo cual se verifica directamente usando $I_{\text{máx}} = Q_{\text{máx}}/\sqrt{LC}$), resulta

$$U = \frac{Q_{\text{máx}}^2}{2C}\left[\cos^2(\omega t) + \sin^2(\omega t)\right] = \frac{Q_{\text{máx}}^2}{2C}$$

> **[Figura]:** Dos gráficas alineadas verticalmente en función del tiempo $t$ ($0, T/2, T, 3T/2, 2T$):
> - **Gráfica superior ($U_C$ vs. $t$):** Curva $\cos^2(\omega t)$ naranja, siempre no negativa, que oscila con período $T/2$ entre su amplitud máxima $\frac{Q_{\text{máx}}^2}{2C}$ (en $t = 0, T/2, T, 3T/2, 2T$) y cero (en $T/4, 3T/4, \dots$).
> - **Gráfica inferior ($U_L$ vs. $t$):** Curva $\sin^2(\omega t)$ naranja, en oposición de fase respecto a $U_C$: es nula en $0, T/2, T, 3T/2, 2T$ y alcanza su máximo $\frac{LI_{\text{máx}}^2}{2}$ en $T/4, 3T/4, \dots$, de modo que la suma $U_C + U_L$ permanece constante en todo instante.

## Circuitos RLC

### Disipación de energía y ecuación diferencial

> **[Figura]:** Circuito con tres ramas verticales paralelas: la rama izquierda contiene una fuente de fem $\varepsilon$ (polo $+$ arriba, $-$ abajo); la rama derecha contiene un capacitor $C$; la rama central contiene un inductor $L$ en serie con un resistor $R$. En la parte superior se ubica un interruptor $S$ de dos posiciones: en la posición $a$ conecta el capacitor $C$ con la fuente $\varepsilon$; en la posición $b$ desconecta la fuente y conecta el capacitor $C$ en serie con $L$ y $R$, formando un lazo cerrado $RLC$.

Supóngase que inicialmente el interruptor $S$ está en la posición $a$, de modo que el capacitor adquiere una carga inicial $Q_{\text{máx}}$. Luego el interruptor se coloca en la posición $b$. Después de ese instante, la energía total almacenada en el capacitor y en el inductor en cualquier tiempo es

$$U = U_C + U_L = \frac{Q^2}{2C} + \frac{1}{2}LI^2$$

Sin embargo, esta energía total ya no es constante como en el circuito $LC$, porque el resistor disipa energía eléctrica transformándola en energía interna a una tasa $I^2 R$:

$$LI\frac{dI}{dt} + \frac{Q}{C}\frac{dQ}{dt} = \frac{dU}{dt} = -I^2 R$$

> **Nota (errata):** En las diapositivas se omitió el factor $I$ en el primer término (aparece escrito $L\frac{dI}{dt} + \frac{Q}{C}\frac{dQ}{dt} = \frac{dU}{dt} = -I^2 R$); al derivar $U_L = \frac{1}{2}LI^2$ respecto al tiempo se obtiene $LI\frac{dI}{dt}$, lo cual coincide además con el paso inmediato siguiente en la presentación.

Reemplazando $I = \frac{dQ}{dt}$ y $\frac{dI}{dt} = \frac{d^2 Q}{dt^2}$ y pasando todos los términos al primer miembro:

$$LI\frac{d^2 Q}{dt^2} + I^2 R + \frac{Q}{C}I = 0$$

Dividiendo entre $I$ (para $I \neq 0$) se obtiene la ecuación diferencial del circuito $RLC$ serie sin fuente:

$$L\frac{d^2 Q}{dt^2} + R\frac{dQ}{dt} + \frac{Q}{C} = 0$$

### Oscilaciones amortiguadas

En el régimen subamortiguado débil ($\frac{1}{LC} > \left(\frac{R}{2L}\right)^2$, es decir, $R < 2\sqrt{L/C}$, con amortiguamiento pequeño respecto de la frecuencia natural), la carga en el capacitor oscila con amplitud decreciente exponencialmente:

$$Q = Q_{\text{máx}} e^{-Rt/2L}\cos(\omega_d t)$$

donde la frecuencia angular de las oscilaciones amortiguadas es

$$\omega_d = \left[\frac{1}{LC} - \left(\frac{R}{2L}\right)^2\right]^{1/2}$$

> **[Figura]:** Gráfica de la carga $Q$ (eje vertical) en función del tiempo $t$ (eje horizontal) para un circuito $RLC$ subamortiguado. La curva naranja sólida parte de $(0, Q_{\text{máx}})$ y oscila alternando valores positivos y negativos alrededor del eje $t$, con amplitud decreciente contenida entre dos envolventes exponenciales simétricas punteadas en azul, $\pm Q_{\text{máx}} e^{-Rt/2L}$, que tienden asintóticamente a cero al aumentar $t$.

## Resumen de fórmulas

| Fórmula | Significado | Condiciones |
|---|---|---|
| $M = \dfrac{N_2\Phi_{B2}}{i_1} = \dfrac{N_1\Phi_{B1}}{i_2}$ | Inductancia mutua entre dos bobinas ($M_{12} = M_{21} = M$) | Geometría fija; unidad $\text{H} = \text{Wb/A} = \Omega\cdot\text{s}$ |
| $\varepsilon_2 = -M\dfrac{di_1}{dt},\quad \varepsilon_1 = -M\dfrac{di_2}{dt}$ | Fem mutuamente inducidas | Corriente variable en la bobina acoplada |
| $L = \dfrac{N\Phi_B}{i}$ | Autoinductancia de una bobina | Geometría y medio lineal fijos |
| $\varepsilon = -L\dfrac{di}{dt},\quad V_{ab} = L\dfrac{di}{dt}$ | Fem autoinducida y caída de potencial en el sentido de $i$ | Inductor ideal sin resistencia |
| $U = \dfrac{1}{2}LI^2$ | Energía magnética almacenada en un inductor | Corriente estacionaria o instantánea $I$ |
| $i(t) = \dfrac{\varepsilon}{R}\left(1 - e^{-t/\tau}\right)$ | Corriente en circuito $RL$ conectado a fem | $i(0) = 0$, fem $\varepsilon$ constante, $\tau = L/R$ |
| $i(t) = I_0 e^{-t/\tau}$ | Corriente en circuito $RL$ desconectado de la fem | $i(0) = I_0$, sin fuente ($\varepsilon = 0$), $\tau = L/R$ |
| $\varepsilon i = i^2 R + Li\dfrac{di}{dt}$ | Balance instantáneo de potencia en circuito $RL$ | Con fuente $\varepsilon$ (si $\varepsilon = 0$, $Li\frac{di}{dt} = -i^2 R$) |
| $\dfrac{d^2 Q}{dt^2} = -\dfrac{1}{LC}Q$ | Ecuación diferencial del circuito $LC$ ideal | $R = 0$, conservación de $U = \frac{Q^2}{2C} + \frac{1}{2}LI^2$ |
| $Q(t) = Q_{\text{máx}}\cos(\omega t + \phi)$ | Carga oscilante en circuito $LC$ | $\omega = 1/\sqrt{LC}$; si $Q(0)=Q_{\text{máx}}$ e $I(0)=0$, $\phi = 0$ |
| $I(t) = -\omega Q_{\text{máx}}\sin(\omega t + \phi)$ | Corriente oscilante en circuito $LC$ | $I_{\text{máx}} = \omega Q_{\text{máx}}$; $\frac{Q_{\text{máx}}^2}{2C} = \frac{1}{2}LI_{\text{máx}}^2$ |
| $L\dfrac{d^2 Q}{dt^2} + R\dfrac{dQ}{dt} + \dfrac{Q}{C} = 0$ | Ecuación diferencial del circuito $RLC$ serie libre | Sin fuente; disipación $\frac{dU}{dt} = -I^2 R$ |
| $Q(t) = Q_{\text{máx}} e^{-Rt/2L}\cos(\omega_d t)$ | Carga en circuito $RLC$ subamortiguado | $\omega_d = \left[\frac{1}{LC} - \left(\frac{R}{2L}\right)^2\right]^{1/2}$, $R < 2\sqrt{L/C}$ (amortiguamiento débil) |
