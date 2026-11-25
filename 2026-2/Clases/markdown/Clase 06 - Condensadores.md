# Condensadores

## ¿Qué es un condensador?

Los **condensadores** (o capacitores) son dispositivos que permiten almacenar carga eléctrica a un determinado potencial eléctrico (voltaje). Consisten en **dos cuerpos conductores** a potenciales distintos, separados por un aislante (o vacío) a una distancia fija. Generalmente tienen forma **plana, cilíndrica o esférica**.

En la práctica, cada conductor parte con carga neta cero y se transfieren electrones de uno al otro; a esto se le llama *cargar* el condensador. Así, ambos conductores quedan con cargas de **igual magnitud y signo contrario**, $+Q$ y $-Q$, y la carga neta del condensador sigue siendo cero. Cuando se dice que un condensador "tiene carga $Q$", significa que el conductor de mayor potencial tiene $+Q$ y el de menor potencial tiene $-Q$.

> **[Figura]:** Dos conductores cualesquiera $a$ (carga $+Q$, arriba) y $b$ (carga $-Q$, abajo) aislados entre sí. Las líneas de campo $\vec{E}$ salen de $a$ y llegan a $b$, concentrándose en la región entre ambos. Cualquier par de conductores aislados forma un condensador.

En los diagramas de circuito un condensador se representa con dos líneas paralelas (rectas, o una recta y una curva) que simbolizan los conductores, unidas a los alambres de conexión: $\dashv\vdash$.

Una forma común de cargarlo es conectar sus terminales a los bornes de una batería; una vez establecidas las cargas $\pm Q$ se desconecta la batería y queda una diferencia de potencial fija $V_{ab}$ entre los conductores, igual al voltaje de la batería.

## Capacitancia

El campo eléctrico en la región entre los conductores es proporcional a $Q$ (principio de superposición, Clase 02), por lo que la diferencia de potencial $\Delta V = -\int \vec{E}\cdot d\vec{l}$ (Clase 05) también es proporcional a $Q$. Si se duplica la carga, se duplican el campo y la diferencia de potencial, pero su **razón no cambia**. Esa razón es la **capacitancia**:

$$C=\frac{Q}{\left| \Delta V \right|}$$

La capacitancia indica cuánta carga puede contener el condensador para un voltaje dado. Su unidad SI es el **faradio** (en honor a Michael Faraday):

$$1\,\text{F} = 1\,\frac{\text{C}}{\text{V}} = 1\,\frac{\text{C}^2}{\text{N}\cdot\text{m}} = 1\,\frac{\text{C}^2}{\text{J}}$$

Los condensadores de aparatos electrónicos suelen ir desde picofaradios ($1\,\text{pF}=10^{-12}\,\text{F}$) hasta microfaradios ($1\,\mu\text{F}=10^{-6}\,\text{F}$). Como consecuencia, $\varepsilon_0 = 8.85\times10^{-12}\,\text{C}^2/(\text{N}\cdot\text{m}^2) = 8.85\times10^{-12}\,\text{F/m}$.

> **Cuidado:** no confundir el símbolo $C$ de capacitancia (en cursiva) con la unidad C de coulomb.

Cuanto mayor es $C$, más carga (y, como veremos, más energía) almacena el condensador a un voltaje dado.

> **¡La capacitancia es una propiedad que depende exclusivamente de la geometría del condensador** (formas, tamaños y separación de los conductores) **y del material aislante entre ellos!** No depende de $Q$ ni de $\Delta V$.

**Receta general para calcular $C$:**

1. Suponer cargas $+Q$ y $-Q$ en los conductores.
2. Encontrar $\vec{E}$ en la región entre ellos (normalmente con la ley de Gauss, Clase 03).
3. Calcular $\Delta V = -\int_{-}^{+}\vec{E}\cdot d\vec{l}$ entre los conductores (Clase 05).
4. Dividir: $C = Q/|\Delta V|$. La carga $Q$ siempre se cancela.

## Condensador de placas paralelas

**Problema.** Calcule la capacitancia de un condensador de placas paralelas de área $A$, separadas por una distancia $d$ (con $d$ pequeña comparada con las dimensiones de las placas).

> **[Figura]:** Dos placas conductoras horizontales de área $A$: la superior (placa $a$) con carga $+Q$ y la inferior (placa $b$) con carga $-Q$, separadas una distancia $d$; cada una conectada a un alambre. En la vista lateral, las líneas de $\vec{E}$ son verticales y uniformes entre las placas, apuntando de $+$ a $-$ (eje $-\hat{z}$ si $\hat z$ apunta hacia arriba; en la deducción se toma $\hat z$ apuntando de la placa positiva a la negativa). Cerca de los bordes las líneas se curvan (efecto de borde), despreciable cuando $d$ es pequeña frente al tamaño de las placas.

**Resolución**

*Idea:* usar la ley de Gauss (Clase 03) para el campo de un plano infinito y el principio de superposición (Clase 02); luego $\Delta V=-\int\vec E\cdot d\vec l$ (Clase 05).

*Paso 1 — Campo de una sola placa.* Para un plano infinito con densidad $\sigma$, tomamos como superficie gaussiana un cilindro ("pastillero") de tapas $A'$ que atraviesa el plano. Por simetría $\vec E$ es perpendicular al plano y de igual magnitud en ambas tapas; por el manto no hay flujo:

$$\oint \vec E\cdot d\vec A = 2EA' = \frac{\sigma A'}{\varepsilon_0}\quad\Rightarrow\quad E_{\text{placa}}=\frac{\sigma}{2\varepsilon_0}$$

*Paso 2 — Superposición (¡ojo con el factor 2!).* La placa positiva produce $\sigma/2\varepsilon_0$ alejándose de ella; la placa negativa produce $\sigma/2\varepsilon_0$ acercándose a ella.

- **Entre las placas** ambos campos apuntan en el mismo sentido (de $+$ a $-$) y se suman: $E=\dfrac{\sigma}{2\varepsilon_0}+\dfrac{\sigma}{2\varepsilon_0}=\dfrac{\sigma}{\varepsilon_0}$.
- **Fuera de las placas** apuntan en sentidos opuestos y se cancelan: $E=0$.

(Equivalentemente, con un pastillero que tenga una tapa *dentro* del conductor, donde $E=0$, el flujo sale sólo por una tapa: $EA'=\sigma A'/\varepsilon_0$, y se obtiene directamente $E=\sigma/\varepsilon_0$.)

Con $\hat z$ apuntando de la placa positiva hacia la negativa:

$$\vec{E}=\frac{\sigma}{\varepsilon_0}\hat{z},\qquad \sigma=\frac{Q}{A}$$

*Paso 3 — Diferencia de potencial.* Integrando desde la placa positiva ($z=0$) hasta la negativa ($z=d$):

$$\Delta V = V_- - V_+ = -\int_0^d \frac{\sigma}{\varepsilon_0}\hat{z}\cdot dz\,\hat{z}=-\frac{\sigma}{\varepsilon_0}d=-\frac{Q\,d}{\varepsilon_0 A}$$

El signo negativo indica que el potencial baja al ir de la placa $+$ a la $-$, como corresponde. (Nota: en la diapositiva el último término aparece como $-\frac{QA}{\varepsilon_0}d$; es una errata, pues $\sigma = Q/A$ da $-\frac{Q d}{\varepsilon_0 A}$, que además es el único dimensionalmente correcto.)

*Paso 4 — Capacitancia.*

$$C=\frac{Q}{|\Delta V|}=\frac{Q}{Qd/(\varepsilon_0A)}$$

$$\boxed{C=\frac{\varepsilon_0 A}{d}}$$

*Verificación / interpretación:* unidades $[\text{F/m}]\cdot[\text{m}^2]/[\text{m}]=[\text{F}]$ ✓. $C$ crece con el área (más espacio para la carga) y disminuye con la separación (a igual $Q$, mayor $d$ implica mayor voltaje). $Q$ se canceló: sólo depende de la geometría. Si una placa es flexible, $C$ varía con $d$: ése es el principio del micrófono de condensador. Con aire en vez de vacío, $C$ difiere en menos de un $0.06\,\%$.

> **[Figura]:** Fotografía de condensadores comerciales planos tipo "flat pack" (p. ej., $4400\,\mu\text{F}$/40 V, $330\,\mu\text{F}$/250 V, $820\,\mu\text{F}$/200 V), con dos terminales cada uno.

## Condensador cilíndrico

**Problema.** Calcule la capacitancia de un condensador formado por dos cilindros conductores coaxiales de radios $r_A$ (interior) y $r_B$ (exterior), $r_A<r_B$, y largo $L$ ($L\gg r_B$, se desprecian efectos de borde). El cilindro interior tiene carga $+Q$ y el exterior $-Q$.

> **[Figura]:** Cilindro conductor interior de radio $r_A$ con carga $+Q$ (densidad lineal $+\lambda = Q/L$), rodeado por una coraza cilíndrica coaxial de radio interior $r_B$ con carga $-Q$ ($-\lambda$). Entre ellos hay vacío y el campo es radial, saliendo del eje.

**Resolución**

*Idea:* simetría cilíndrica → ley de Gauss con un cilindro coaxial (Clase 03); luego integrar el campo radial (Clase 05).

*Paso 1 — Campo.* Superficie gaussiana: cilindro coaxial de radio $r$ ($r_A<r<r_B$) y largo $L$. Por simetría $\vec E = E(r)\hat r$; sólo el manto aporta flujo (en las tapas $\vec E\perp d\vec A$). La carga encerrada es la del cilindro interior, $+Q$ (la coraza exterior queda fuera):

$$E\,(2\pi r L)=\frac{Q}{\varepsilon_0}\quad\Rightarrow\quad \vec{E}=\frac{Q}{2\pi \varepsilon_0 rL} \hat{r}$$

*Paso 2 — Diferencia de potencial* entre el cilindro interior ($A$, positivo) y el exterior ($B$):

$$\Delta V = V_A - V_B=-\int_{r_B}^{r_A} \frac{Q}{2\pi \varepsilon_0 rL}\hat{r}\cdot dr\, \hat{r}=-\frac{Q}{2\pi\varepsilon_0L}\left[\ln r\right]_{r_B}^{r_A}=\frac{Q}{2\pi \varepsilon_0 L}\ln\left( \frac{r_B}{r_A} \right)$$

Es positiva porque $r_B>r_A$: el conductor interior (positivo) está a mayor potencial ✓.

*Paso 3 — Capacitancia.*

$$\boxed{C=\frac{Q}{|\Delta V|}=\frac{2\pi \varepsilon_0 L}{\ln\left(\dfrac{r_B}{r_A}\right)}}\qquad\text{o, por unidad de largo,}\qquad \frac{C}{L}=\frac{2\pi\varepsilon_0}{\ln(r_B/r_A)}$$

*Verificación / interpretación:* unidades F ✓; depende sólo de $L$, $r_A$, $r_B$. Si $r_B\to r_A$ ($r_B = r_A + d$, $d\ll r_A$): $\ln(1+d/r_A)\approx d/r_A$ y $C\approx \varepsilon_0(2\pi r_A L)/d = \varepsilon_0 A/d$, el resultado de placas paralelas con área igual al manto ✓. Ejemplo numérico: con $r_B/r_A = 2$, $C/L = 2\pi(8.85\times10^{-12})/\ln 2 \approx 80\,\text{pF/m}$, orden de magnitud típico de un cable coaxial.

> **[Figura]:** Fotografía de supercondensadores cilíndricos comerciales ($2.7\,\text{V}$, $15\,\text{F}$).

## Condensador esférico

**Problema.** Dos corazas conductoras esféricas y concéntricas están separadas por vacío. La interior tiene carga $+Q$ y radio exterior $r_A$; la exterior tiene carga $-Q$ y radio interior $r_B$. Determine la capacitancia.

> **[Figura]:** Corte de una esfera: coraza interior de radio $r_a$ (cargas $+$ en su superficie), coraza exterior de radio $r_b$ (cargas $-$ en su superficie interna), y entre ellas una superficie gaussiana esférica de radio $r$ ($r_a<r<r_b$). La coraza interior se sostiene con varillas aislantes de efecto despreciable.

**Resolución**

*Idea:* no es de placas paralelas, así que volvemos a la definición $C=Q/V_{ab}$. Simetría esférica → Gauss con una esfera concéntrica (Clase 03); el campo entre las corazas es el de una carga puntual $Q$ (la coraza exterior no aporta campo en su interior).

*Paso 1 — Campo.* Gaussiana esférica de radio $r$, $r_A<r<r_B$; por simetría $\vec E\parallel d\vec A$ y $|\vec E|$ constante sobre ella:

$$\oint\vec E\cdot d\vec A = E\,(4\pi r^2)=\frac{Q_{\text{enc}}}{\varepsilon_0}=\frac{Q}{\varepsilon_0}\quad\Rightarrow\quad\vec{E}=\frac{Q}{4\pi\varepsilon_0 r^2}\hat{r}$$

*Paso 2 — Diferencia de potencial.*

$$V_b-V_a=-\int_{r_a}^{r_b} \frac{Q}{4\pi \varepsilon_0}\frac{1}{r^{2}}\hat{r}\cdot dr\,\hat{r}=-\frac{Q}{4\pi\varepsilon_0}\left[-\frac1r\right]_{r_a}^{r_b}=-\frac{Q}{4\pi \varepsilon_0}\left( \frac{1}{r_a}-\frac{1}{r_b} \right)$$

Luego

$$V_{ab}=V_a-V_b=\frac{Q}{4\pi\varepsilon_0}\left(\frac1{r_a}-\frac1{r_b}\right)=\frac{Q}{4\pi\varepsilon_0}\,\frac{r_b-r_a}{r_a r_b}>0$$

*Paso 3 — Capacitancia.*

$$\boxed{C=\frac{Q}{V_{ab}}=4\pi\varepsilon_0\frac{r_A r_B}{r_B-r_A}}$$

*Ejemplo numérico* (libro): $r_a = 9.5\,\text{cm}$, $r_b = 10.5\,\text{cm}$:

$$C=4\pi\left(8.85\times10^{-12}\,\tfrac{\text{F}}{\text{m}}\right)\frac{(0.095\,\text{m})(0.105\,\text{m})}{0.010\,\text{m}}=1.1\times10^{-10}\,\text{F}=110\,\text{pF}$$

*Verificación / interpretación:* $4\pi r_ar_b$ es la media geométrica $A_{gm}$ de las áreas $4\pi r_a^2$ y $4\pi r_b^2$, y $d=r_b-r_a$, así que $C=\varepsilon_0A_{gm}/d$: la misma forma que placas paralelas. Si la separación es pequeña frente a los radios, las esferas se comportan como placas paralelas ✓. Límite $r_B\to\infty$: $C\to 4\pi\varepsilon_0 r_A$, la capacitancia de una esfera aislada ✓.

> **[Figura]:** Montaje de laboratorio: fuente de alto voltaje (kV) conectada a una esfera metálica sobre soporte aislante, con electrómetro y multímetro para medir carga y potencial (capacitancia de una esfera).

## Condensadores en serie

> **[Figura]:** Dos condensadores en serie entre los puntos $a$ y $b$: $C_1$ arriba (placas $+Q$ / $-Q$), conectado en el nodo intermedio $c$ a $C_2$ abajo (placas $+Q$ / $-Q$). $V_{ac}=V_1$ a través de $C_1$, $V_{cb}=V_2$ a través de $C_2$ y $V_{ab}=V$ a través de la combinación. Abajo, el condensador equivalente único $C_{eq}$ con la misma $Q$ y el mismo $V$.

**Demostración.**

1. **Misma carga.** Si se aplica $V_{ab}$, la placa superior de $C_1$ adquiere $+Q$ y la inferior de $C_2$ adquiere $-Q$. La placa inferior de $C_1$ y la superior de $C_2$ forman un conductor aislado (sólo conectadas entre sí), cuya carga neta debe seguir siendo cero por conservación de carga: si una tiene $-Q$, la otra tiene $+Q$. Así, **todos los condensadores en serie tienen la misma carga $Q$**.
2. **Voltajes individuales:**
$$V_{ac}=V_1=\frac{Q}{C_1},\qquad V_{cb}=V_2=\frac{Q}{C_2}$$
3. **Sus diferencias de potencial se suman** (el potencial es función de punto: $V_a-V_b=(V_a-V_c)+(V_c-V_b)$):
$$V_{ab}=V_1+V_2=Q\left( \frac{1}{C_1}+\frac{1}{C_2} \right)$$
4. **Equivalente.** Un único condensador $C_{eq}$ es equivalente si con el mismo $V$ almacena la misma $Q$: $C_{eq}=Q/V_{ab}$. Entonces
$$\frac{V_{ab}}{Q}=\frac{1}{C_{eq}}=\frac{1}{C_1}+\frac{1}{C_2}$$

Para $N$ condensadores en serie, el mismo argumento da

$$\boxed{\frac{1}{C_{eq}}=\sum_{i=1}^{N}\frac{1}{C_i}}$$

La capacitancia equivalente en serie es **menor** que cualquiera de las individuales. Ojo: la carga es la misma en todos, pero los voltajes individuales sólo son iguales si las capacitancias lo son; en general $V_{total}=V_1+V_2+\dots$

## Condensadores en paralelo

> **[Figura]:** Dos condensadores $C_1$ y $C_2$ conectados en paralelo entre $a$ y $b$: sus placas superiores unidas al nodo $a$ y las inferiores al nodo $b$, con cargas $Q_1$ y $Q_2$. Abajo, el condensador equivalente $C_{eq}$ con carga $Q=Q_1+Q_2$ y voltaje $V$.

**Demostración.**

1. **Mismo voltaje.** Las placas superiores están unidas por alambre conductor y forman una equipotencial; lo mismo las inferiores. Por tanto ambos condensadores tienen la misma diferencia de potencial $V_{ab}=V$.
2. **Cargas individuales** (dependen de cada capacitancia):
$$Q_1=C_1V,\qquad Q_2=C_2V$$
3. **La carga total es la suma** de las cargas individuales (la batería entrega $Q$ que se reparte):
$$Q=Q_1+Q_2=\left( C_1+C_2 \right)V$$
4. **Equivalente:**
$$\frac{Q}{V}=C_{eq}=C_1+C_2$$

Para $N$ condensadores en paralelo:

$$\boxed{C_{eq}=\sum_{i=1}^{N}C_i}$$

La capacitancia equivalente en paralelo es **mayor** que cualquiera de las individuales (equivale a sumar área de placas).

## Ejercicio: capacidad equivalente de una red

**Enunciado.** Considere la configuración de la figura. Encuentre la capacidad equivalente del circuito asumiendo que todos los condensadores tienen la misma capacidad $C$. *Respuesta:* $\frac{11}{6}C$.

> **[Figura]:** Dos terminales (izquierdo y derecho) unidos por un alambre horizontal que llega a dos nodos verticales, uno a la izquierda y otro a la derecha. Entre esos dos nodos hay **tres ramas en paralelo**: (1) rama superior con **un** condensador $C$; (2) rama central con **dos** condensadores $C$ en serie; (3) rama inferior con **tres** condensadores $C$ en serie. No hay conexiones intermedias entre las ramas.

**Resolución**

*Idea:* reducir paso a paso usando las reglas de serie (misma carga, $1/C_{eq}=\sum 1/C_i$) y paralelo (mismo voltaje, $C_{eq}=\sum C_i$) demostradas en esta clase.

*Paso 1 — Reducir cada rama (serie).*

- Rama 1: un solo condensador, $C_1' = C$.
- Rama 2: dos en serie, $\dfrac{1}{C_2'}=\dfrac1C+\dfrac1C=\dfrac2C\Rightarrow C_2'=\dfrac{C}{2}$.
- Rama 3: tres en serie, $\dfrac{1}{C_3'}=\dfrac1C+\dfrac1C+\dfrac1C=\dfrac3C\Rightarrow C_3'=\dfrac{C}{3}$.

*Paso 2 — Combinar las ramas (paralelo).* Las tres ramas comparten los mismos dos nodos, luego tienen el mismo voltaje:

$$C_{eq}=C+\frac{C}{2}+\frac{C}{3}=\frac{6C+3C+2C}{6}$$

$$\boxed{C_{eq}=\frac{11}{6}\,C}$$

*Verificación / interpretación:* coincide con la respuesta de la diapositiva ✓. Es mayor que $C$ (hay una rama con $C$ en paralelo con otras, y el paralelo siempre aumenta la capacitancia) y menor que $3C$ (lo que se obtendría si las tres ramas tuvieran un solo condensador) ✓. Por ejemplo, con $C=6\,\mu\text{F}$: $C_{eq}=11\,\mu\text{F}$.

## Energía almacenada en un condensador

La energía potencial eléctrica almacenada en un condensador cargado es exactamente igual al **trabajo requerido para cargarlo**.

**Deducción.** Supongamos que en un instante intermedio el condensador tiene carga $q$ y voltaje $v=q/C$. Para trasladar una carga adicional $dq$ desde la placa negativa a la positiva (contra el campo) hay que hacer un trabajo (Clase 05: $W = q\,\Delta V$):

$$dW=v\,dq=\frac{q}{C}\,dq$$

Integrando desde $q=0$ (descargado) hasta $q=Q$:

$$W= \int_0^Q \frac{q\,dq}{C}=\frac{1}{2}\frac{Q^{2}}{C}$$

Usando $Q = CV$ se obtienen tres formas equivalentes:

$$\boxed{U=\frac{1}{2}\frac{Q^{2}}{C}=\frac{1}{2} C V^{2}=\frac{1}{2} QV}$$

El factor $\tfrac12$ aparece porque el voltaje crece linealmente de $0$ a $V$ durante la carga: el trabajo equivale a trasladar toda la carga $Q$ a través del voltaje *promedio* $V/2$.

## Energía del campo eléctrico (densidad de energía)

Se puede pensar que la energía está almacenada **en el campo eléctrico** entre las placas. Se define la densidad volumétrica de energía:

$$u=\frac{U}{\text{Vol}}$$

Para un condensador de placas paralelas, el campo ocupa el volumen $A\cdot d$:

$$u=\frac{\frac{1}{2}CV^{2}}{A\cdot d}$$

Sustituyendo $C=\varepsilon_0A/d$ y $V=Ed$:

$$u=\frac{\frac12\,\frac{\varepsilon_0A}{d}\,(Ed)^2}{A\,d}=\frac{\frac12\varepsilon_0 A d\,E^2}{A\,d}$$

$$\boxed{u_E=\frac{1}{2}\varepsilon_0 E^{2}}$$

Aunque se dedujo para placas paralelas, este resultado es **válido para cualquier configuración de campo eléctrico en vacío**. Cuando el campo no es uniforme, la energía total se obtiene integrando:

$$U=\int u_E\,dV=\int\frac12\varepsilon_0E^2\,dV$$

## Ejemplo: energía de un condensador esférico

**Enunciado.** El condensador esférico de la figura tiene cargas $+Q$ y $-Q$ en sus conductores interior (radio $r_a$) y exterior (radio $r_b$). Calcule la energía potencial eléctrica almacenada en el condensador:

a) calculando la capacitancia $C$, y
b) integrando la densidad de energía del campo eléctrico.

> **[Figura]:** La misma geometría del condensador esférico anterior: coraza interior de radio $r_a$ con $+Q$, coraza exterior de radio $r_b$ con $-Q$, vacío entre ellas.

**Resolución**

*Idea:* (a) usar $C$ del condensador esférico y $U=Q^2/2C$; (b) usar $u_E=\tfrac12\varepsilon_0E^2$ con el campo obtenido por Gauss y sumar sobre cascarones esféricos. Ambos métodos deben coincidir.

**a) A partir de la capacitancia.** Ya obtuvimos $C=4\pi\varepsilon_0\dfrac{r_ar_b}{r_b-r_a}$. Como la carga es dato, conviene la forma $U=\frac{Q^2}{2C}$:

$$U=\frac{Q^2}{2}\cdot\frac{r_b-r_a}{4\pi\varepsilon_0\,r_ar_b}$$

$$\boxed{U=\frac{Q^2}{8\pi\varepsilon_0}\,\frac{r_b-r_a}{r_a r_b}}$$

**b) Integrando la densidad de energía.**

*Paso 1 — Campo y densidad.* Para $r_a<r<r_b$, $E=\dfrac{Q}{4\pi\varepsilon_0 r^2}$; fuera de esa región ($r<r_a$ dentro del conductor, y $r>r_b$ donde la carga encerrada es $Q-Q=0$) el campo es nulo y no hay energía. Entonces

$$u_E=\frac12\varepsilon_0\left(\frac{Q}{4\pi\varepsilon_0r^2}\right)^2=\frac{Q^2}{32\pi^2\varepsilon_0 r^4}$$

*Paso 2 — Elemento de volumen.* Como $u_E$ sólo depende de $r$, usamos cascarones esféricos de radio $r$ y espesor $dr$: $dV=4\pi r^2\,dr$. La energía en el cascarón es

$$dU=u_E\,dV=\frac{Q^2}{32\pi^2\varepsilon_0 r^4}\,4\pi r^2\,dr=\frac{Q^2}{8\pi\varepsilon_0}\frac{dr}{r^2}$$

*Paso 3 — Integrar entre las corazas.*

$$U=\int_{r_a}^{r_b}\frac{Q^2}{8\pi\varepsilon_0}\frac{dr}{r^2}=\frac{Q^2}{8\pi\varepsilon_0}\left[-\frac1r\right]_{r_a}^{r_b}=\frac{Q^2}{8\pi\varepsilon_0}\left(\frac1{r_a}-\frac1{r_b}\right)$$

$$\boxed{U=\frac{Q^2}{8\pi\varepsilon_0}\,\frac{r_b-r_a}{r_a r_b}}$$

*Verificación / interpretación:* ambos métodos dan el mismo resultado ✓, lo que confirma que la energía del condensador puede entenderse como energía almacenada en el campo. Unidades: $\text{C}^2/(\text{F/m}\cdot\text{m})=\text{C}^2/\text{F}=\text{J}$ ✓. $U>0$ y crece con la separación $r_b-r_a$ (hay más volumen con campo). Ilustración numérica: con los radios del ejemplo anterior ($r_a=9.5\,\text{cm}$, $r_b=10.5\,\text{cm}$, $C\approx110\,\text{pF}$) y $Q=1.0\,\text{nC}$, $U=\frac{(1.0\times10^{-9})^2}{2(1.11\times10^{-10})}\approx4.5\times10^{-9}\,\text{J}$.

## Resumen de fórmulas

| Concepto | Fórmula |
|---|---|
| Definición de capacitancia | $C = \dfrac{Q}{\lvert\Delta V\rvert}$, $\;1\,\text{F}=1\,\text{C/V}$ |
| Placas paralelas | $E=\dfrac{\sigma}{\varepsilon_0}$, $\;C=\dfrac{\varepsilon_0A}{d}$ |
| Cilíndrico (coaxial) | $E=\dfrac{Q}{2\pi\varepsilon_0 rL}$, $\;C=\dfrac{2\pi\varepsilon_0L}{\ln(r_B/r_A)}$ |
| Esférico | $E=\dfrac{Q}{4\pi\varepsilon_0r^2}$, $\;C=4\pi\varepsilon_0\dfrac{r_Ar_B}{r_B-r_A}$ |
| Esfera aislada ($r_B\to\infty$) | $C=4\pi\varepsilon_0 r_A$ |
| Serie (misma $Q$) | $\dfrac{1}{C_{eq}}=\sum_i\dfrac{1}{C_i}$ |
| Paralelo (mismo $V$) | $C_{eq}=\sum_i C_i$ |
| Energía almacenada | $U=\dfrac{Q^2}{2C}=\dfrac12CV^2=\dfrac12QV$ |
| Densidad de energía | $u_E=\dfrac12\varepsilon_0E^2$, $\;U=\int u_E\,dV$ |
| Energía condensador esférico | $U=\dfrac{Q^2}{8\pi\varepsilon_0}\dfrac{r_b-r_a}{r_ar_b}$ |
