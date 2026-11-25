# Inducción Magnética

## Experimentos de inducción magnética

En los experimentos clásicos de inducción (Faraday, Henry) se observa que aparece una fem —y por lo tanto una corriente, si el circuito está cerrado— en una espira cuando:

- se acerca o aleja un imán de la espira;
- se acerca o aleja otra bobina que conduce corriente;
- se varía la corriente de una bobina cercana (al cerrar o abrir un interruptor);
- se gira, deforma o desplaza la espira dentro de un campo magnético.

No aparece fem cuando el imán y la espira están en reposo relativo con un campo constante. **¿Qué tienen en común los casos en que sí se genera fem? En todos ellos el flujo magnético a través de la espira varía en el tiempo.**

## Flujo magnético

Para un elemento de área infinitesimal $d\vec{A}$ (vector perpendicular a la superficie) en un campo $\vec{B}$, el flujo magnético es

$$d\Phi_B=\vec{B}\cdot d\vec{A}=B_\perp\,dA=B\,dA\cos\phi$$

donde $B_\perp$ es la componente de $\vec{B}$ perpendicular a la superficie y $\phi$ es el ángulo entre $\vec{B}$ y $d\vec{A}$. El flujo total sobre un área finita es

$$\Phi_B=\int\vec{B}\cdot d\vec{A}=\int B\,dA\cos\phi$$

Si $\vec{B}$ es uniforme sobre un área plana $\vec{A}$:

$$\Phi_B=\vec{B}\cdot\vec{A}=BA\cos\phi$$

Unidad: $1\,\text{Wb}=1\,\text{T}\cdot\text{m}^2$.

Casos particulares (área plana en campo uniforme):

| Orientación | Ángulo entre $\vec{B}$ y $\vec{A}$ | Flujo |
|---|---|---|
| Superficie de frente al campo ($\vec{B}\parallel\vec{A}$) | $\phi=0$ | $\Phi_B=BA$ |
| Superficie inclinada | $\phi$ | $\Phi_B=BA\cos\phi$ |
| Superficie de perfil ($\vec{B}\perp\vec{A}$) | $\phi=90^\circ$ | $\Phi_B=0$ |

**Cuidado con la dirección de $d\vec{A}$:** toda superficie tiene dos normales posibles; el signo del flujo depende de cuál se elija como positiva. Cualquier elección es válida, pero una vez hecha debe respetarse en todo el problema.

## Ley de inducción de Faraday

> La fem inducida en una espira cerrada es igual al negativo de la tasa de cambio del flujo magnético a través de la espira con respecto al tiempo.

$$\varepsilon=-\frac{d\Phi_B}{dt},\qquad \Phi_B=\int\vec{B}\cdot d\vec{A}$$

Si se tiene una bobina con $N$ espiras idénticas y el flujo varía a la misma tasa en cada una, las fem se suman:

$$\varepsilon=-N\frac{d\Phi_B}{dt}$$

Lo que induce la fem es el **cambio** del flujo en el tiempo, no el flujo en sí: si el flujo es constante (positivo, negativo o cero), no hay fem inducida. El flujo puede cambiar porque cambia $B$, porque cambia el área, o porque cambia el ángulo entre $\vec{B}$ y $\vec{A}$.

### Regla de signos para la fem

1. Elija la dirección del vector de área $\vec{A}$.
2. Calcule $\Phi_B$ y $d\Phi_B/dt$ con esa elección.
3. Doble los dedos de la mano derecha alrededor de $\vec{A}$ con el pulgar en la dirección de $\vec{A}$. Si $\varepsilon>0$, la fem (o corriente) circula en el sentido de los dedos doblados; si $\varepsilon<0$, en sentido opuesto.

> **[Figura]:** Cuatro espiras horizontales con $\vec{A}$ apuntando hacia arriba:
> a) $\vec{B}$ forma un ángulo agudo con $\vec{A}$ y crece: $\Phi_B>0$, $d\Phi_B/dt>0$, $\varepsilon<0$ (sentido horario visto desde arriba).
> b) $\vec{B}$ agudo y decreciente: $\Phi_B>0$, $d\Phi_B/dt<0$, $\varepsilon>0$ (antihorario).
> c) $\vec{B}$ apunta hacia abajo (ángulo obtuso) y crece: $\Phi_B<0$ y se hace más negativo, $d\Phi_B/dt<0$, $\varepsilon>0$ (antihorario).
> d) $\vec{B}$ hacia abajo y decreciente: $\Phi_B<0$ y se hace menos negativo, $d\Phi_B/dt>0$, $\varepsilon<0$ (horario).

### Estrategia para resolver problemas con la ley de Faraday

- **Identificar:** debe existir un área (normalmente la limitada por una espira) a través de la cual el flujo cambia. ¿Se mueve el conductor? ¿Cambia su orientación? ¿Cambia el campo?
- **Plantear:** elegir la dirección de $\vec{A}$ (perpendicular al plano del área) y usarla de forma consistente.
- **Ejecutar:** calcular $\Phi_B$ (con $BA\cos\phi$ si $\vec{B}$ es uniforme, o integrando si no lo es); calcular $\varepsilon=-N\,d\Phi_B/dt$; si se conoce la resistencia, $I=\varepsilon/R$.
- **Evaluar:** revisar unidades ($1\,\text{V}=1\,\text{Wb/s}=1\,\text{T}\cdot\text{m}^2/\text{s}$) y los signos.

## Forma integral y diferencial de la ley de Faraday-Lenz

La fem es el trabajo por unidad de carga que realiza el campo eléctrico (inducido) a lo largo de la espira, de modo que

$$\varepsilon=\oint\vec{E}\cdot d\vec{l}=-\frac{d}{dt}\iint\vec{B}\cdot d\vec{A}$$

Si la trayectoria de integración (la espira) está fija, la derivada temporal puede entrar a la integral:

$$\oint\vec{E}\cdot d\vec{l}=-\iint\frac{\partial\vec{B}(\vec{x},t)}{\partial t}\cdot d\vec{A}$$

Aplicando el teorema de Stokes al lado izquierdo:

$$\oint\vec{E}\cdot d\vec{l}=\iint\left(\nabla\times\vec{E}\right)\cdot d\vec{A}=-\iint\frac{\partial\vec{B}(\vec{x},t)}{\partial t}\cdot d\vec{A}$$

Como esto vale para cualquier superficie, los integrandos deben ser iguales:

$$\nabla\times\vec{E}+\frac{\partial\vec{B}(\vec{x},t)}{\partial t}=0\qquad\Longleftrightarrow\qquad\nabla\times\vec{E}=-\frac{\partial\vec{B}}{\partial t}$$

Esta es la **ecuación de Faraday-Lenz** en forma diferencial (una de las ecuaciones de Maxwell). En electrostática (Clase 05) teníamos $\nabla\times\vec{E}=0$ (campo conservativo); ahora, un campo magnético variable genera un campo eléctrico con rotor no nulo.

## Ejemplo 1: Magnitud y dirección de una fem inducida

Se coloca una bobina de alambre que contiene 500 espiras circulares con radio de 4.00 cm entre los polos de un electroimán grande, donde el campo magnético es uniforme y tiene un ángulo de 60° con respecto al plano de la bobina. El campo disminuye a razón de 0.200 T/s. ¿Cuáles son la magnitud y dirección de la fem inducida?

> **[Figura]:** Polo N a la izquierda y polo S a la derecha; líneas de $\vec{B}$ horizontales de izquierda a derecha. La bobina (vista de canto, diámetro marcado "4.00 cm") está inclinada formando 60° con las líneas de campo. El vector de área $\vec{A}$, perpendicular al plano de la bobina, apunta hacia abajo a la derecha formando $\phi=30^\circ$ con $\vec{B}$.

**Resolución**

*Idea:* el flujo a través de la bobina cambia porque disminuye la magnitud de $B$; se aplica la ley de Faraday para $N$ espiras con el flujo de un campo uniforme, $\Phi_B=BA\cos\phi$.

*Cuidado con el ángulo:* $\phi$ es el ángulo entre $\vec{B}$ y $\vec{A}$ (la normal), **no** entre $\vec{B}$ y el plano de la bobina. Como $\vec{B}$ forma 60° con el plano, forma $90^\circ-60^\circ=30^\circ$ con la normal: $\phi=30^\circ$.

1. Área de cada espira:
$$A=\pi r^2=\pi(0.0400\,\text{m})^2=5.03\times10^{-3}\,\text{m}^2$$

2. Solo $B$ cambia en el tiempo, así que
$$\frac{d\Phi_B}{dt}=\frac{dB}{dt}A\cos30^\circ=(-0.200\,\text{T/s})(5.03\times10^{-3}\,\text{m}^2)(0.866)=-8.71\times10^{-4}\,\text{Wb/s}$$

3. Fem total en las $N=500$ espiras:
$$\varepsilon=-N\frac{d\Phi_B}{dt}=-(500)(-8.71\times10^{-4}\,\text{Wb/s})=0.435\,\text{V}$$

$$\boxed{\varepsilon=0.435\,\text{V}}$$

*Dirección:* la fem es positiva, por lo que circula en el sentido de los dedos doblados de la mano derecha cuando el pulgar apunta según $\vec{A}$ (30° respecto de $\vec{B}$). Vista la bobina desde la izquierda, en la dirección de $\vec{A}$, la fem va en **sentido horario**.

*Verificación (ley de Lenz):* si se conectan los extremos, la corriente circula en sentido horario (visto desde la izquierda) y genera un campo en la misma dirección que el del electroimán, oponiéndose a la **disminución** del flujo. Unidades: $\text{T}\cdot\text{m}^2/\text{s}=\text{V}$.

### Ejemplo conceptual: la bobina exploradora

Una bobina pequeña de $N$ espiras y área $A$ se coloca con $\vec{A}$ alineado con un campo $B$ (flujo inicial $NBA$) y luego se gira rápidamente un cuarto de vuelta, o se saca del campo, de modo que el flujo cae a cero. Mientras el flujo disminuye aparece una fem momentánea; como $I=\varepsilon/R=-\frac{N}{R}\frac{d\Phi_B}{dt}$, integrando en el tiempo la carga total que circula es $Q=\frac{N\,\Delta\Phi_B}{R}=\frac{NBA}{R}$. Midiendo $Q$ se obtiene $B$ (en rigor, el campo medio sobre el área de la bobina).

## Alternador simple

En la figura se muestra una versión simplificada de un alternador (dispositivo que genera fem). Se hace girar una espira rectangular con velocidad angular constante $\omega$ alrededor del eje que se indica. El campo magnético $\vec{B}$ es uniforme y constante. En el momento $t=0$, $\phi=0$. Determine la fem inducida.

> **[Figura]:** a) Espira rectangular que gira con velocidad angular $\omega$ en torno a un eje contenido en su plano, en un campo $\vec{B}$ horizontal uniforme. $\vec{A}$ es perpendicular a la espira y forma un ángulo $\phi=\omega t$ con $\vec{B}$ (dibujada para $\phi=90^\circ$). Cada extremo de la espira está conectado a un anillo colector; dos escobillas fijas tocan los anillos y llevan la fem a los terminales externos $a$ y $b$.
> b) Gráfica de $\Phi_B$ (coseno) y de $\varepsilon=-d\Phi_B/dt$ (seno) durante una vuelta: cuando la espira está perpendicular a $\vec{B}$ el flujo es máximo (o mínimo) y la fem es cero; cuando la espira está paralela a $\vec{B}$ el flujo cambia con máxima rapidez y la fem es máxima (positiva cuando el flujo disminuye, negativa cuando aumenta).

**Resolución**

*Idea:* $\vec{B}$ es constante; el flujo cambia porque la dirección de $\vec{A}$ gira. Se usa $\Phi_B=BA\cos\phi$ con $\phi=\omega t$ y la ley de Faraday.

1. Flujo en función del tiempo:
$$\Phi_B=BA\cos(\omega t)$$

2. Fem:
$$\varepsilon=-\frac{d\Phi_B}{dt}=-BA\frac{d}{dt}\cos(\omega t)=\omega BA\sin(\omega t)$$

3. Con $N$ espiras:
$$\boxed{\varepsilon(t)=NBA\omega\sin(\omega t),\qquad \varepsilon_{\text{máx}}=NBA\omega}$$

*Interpretación:* la fem es sinusoidal (corriente alterna). Es máxima en $\omega t=90^\circ$ y $270^\circ$, cuando $\vec{B}$ está en el plano de la espira y el flujo cambia más rápido; es cero en $\omega t=0^\circ$ y $180^\circ$, cuando $\vec{B}$ es perpendicular al plano. Con $\omega=2\pi f$; la red eléctrica usa $f=50\,\text{Hz}$ (Chile, Europa) o $60\,\text{Hz}$ (EE. UU.).

**Generador de CD y motores.** Si los anillos colectores se reemplazan por un anillo dividido (conmutador), los contactos se intercambian cada medio ciclo y la fem de salida es $|\varepsilon|=NBA\omega|\sin\omega t|$: siempre de la misma polaridad, pulsante. Su valor medio en medio ciclo es

$$\left(|\sin\omega t|\right)_{\text{med}}=\frac{\int_0^{\pi/\omega}\sin\omega t\,dt}{\pi/\omega}=\frac{2}{\pi}\quad\Rightarrow\quad\varepsilon_{\text{med}}=\frac{2N\omega BA}{\pi}$$

Un motor es un generador funcionando al revés: una fuente impulsa corriente por la bobina y el torque magnético la hace girar (Clase 10). Al girar, el flujo cambiante induce una **fuerza contraelectromotriz** que, por la ley de Lenz, se opone a la corriente suministrada y crece con la rapidez de rotación.

## Ejemplo 2: Fem inducida en un generador

La bobina en un generador CA consiste en ocho vueltas de alambre, cada una de área $A=0.0900\,\text{m}^2$, y la resistencia total del alambre es de 12.0 Ω. La bobina da vueltas en un campo magnético de 0.500 T con una frecuencia constante de 60.0 Hz.

a) Encuentre la máxima fem inducida en la bobina.
b) ¿Cuál es la máxima corriente inducida en la bobina cuando las terminales de salida se conectan a un conductor de baja resistencia?

**Resolución**

*Idea:* es exactamente el alternador recién analizado, con $N$ vueltas: $\varepsilon_{\text{máx}}=NBA\omega$, $\omega=2\pi f$. Para la corriente se usa la ley de Ohm (Clase 08); "conductor de baja resistencia" significa que la única resistencia relevante es la de la bobina.

a) Rapidez angular: $\omega=2\pi f=2\pi(60.0\,\text{Hz})=377\,\text{rad/s}$.
$$\varepsilon_{\text{máx}}=NBA\omega=(8)(0.500\,\text{T})(0.0900\,\text{m}^2)(377\,\text{s}^{-1})=136\,\text{V}$$

$$\boxed{\varepsilon_{\text{máx}}\approx136\,\text{V}}$$

b)
$$I_{\text{máx}}=\frac{\varepsilon_{\text{máx}}}{R}=\frac{136\,\text{V}}{12.0\,\Omega}=11.3\,\text{A}$$

$$\boxed{I_{\text{máx}}\approx11.3\,\text{A}}$$

*Verificación:* unidades $\text{T}\cdot\text{m}^2\cdot\text{s}^{-1}=\text{V}$. Duplicar $N$, $B$ o $f$ duplicaría la fem; cambiar la resistencia del alambre cambia la corriente pero **no** la fem.

## Ley de Lenz

La ley de Lenz es un método alternativo conveniente para determinar la dirección de una corriente o fem inducida:

> La dirección de cualquier efecto de la inducción magnética es la que se opone a la causa del efecto.

Si el flujo en un circuito fijo cambia, la corriente inducida establece un campo magnético propio. Dentro del área limitada por el circuito, este campo es **opuesto** al campo original si éste se incrementa, pero tiene la **misma dirección** que el campo original si éste disminuye. Es decir, la corriente inducida se opone al **cambio** en el flujo a través del circuito (no al flujo en sí).

La ley de Lenz es consecuencia de la conservación de la energía: si la corriente inducida reforzara el cambio, el flujo crecería sin límite y se obtendría energía de la nada.

**Ejemplos de sentido** (espira horizontal, vista desde arriba):

- Se acerca el polo norte de un imán desde arriba: el flujo hacia abajo aumenta; la corriente inducida crea un campo hacia arriba → circula en sentido **antihorario**. (La espira se comporta como un polo norte enfrentado al imán y lo repele.)
- Se aleja el mismo polo norte: el flujo hacia abajo disminuye; la corriente crea un campo hacia abajo → sentido **horario** (la espira atrae al imán).
- Espira en campo constante que se inclina o comprime de modo que disminuye el flujo hacia arriba: la corriente refuerza el campo hacia arriba → sentido **antihorario**.
- Barra deslizante sobre rieles en un campo entrante (sección siguiente): el área y el flujo entrante aumentan; la corriente crea campo saliente → sentido **antihorario**, y la fuerza magnética sobre la barra la frena.

## Fuerza electromotriz de conductores en movimiento

### Generador de conductor corredizo

> **[Figura]:** Conductor fijo en forma de U (brazos horizontales separados una distancia $L$) dentro de un campo $\vec{B}$ uniforme que entra en la página (cruces). Una varilla metálica vertical de longitud $L$ cierra el circuito y se mueve hacia la derecha con velocidad $\vec{v}$; en un tiempo $dt$ avanza $v\,dt$. $\vec{A}$ se elige entrando en la página. La fem $\varepsilon$ en la varilla apunta hacia arriba y la corriente $I$ circula en sentido antihorario (hacia arriba en la varilla, hacia la izquierda por el brazo superior).

De la ley de Faraday, con $x$ la posición de la varilla (distancia desde el extremo de la U):

$$\Phi_B=\int\vec{B}\cdot d\vec{A}=B\,L\,x$$

$$\varepsilon=-\frac{d}{dt}(BLx)=-BL\frac{dx}{dt}=-BLv$$

El signo negativo indica que, con $\vec{A}$ entrando en la página (positivo = horario), la fem va en **sentido antihorario**, igual que la corriente inducida. Su magnitud es

$$|\varepsilon|=BLv$$

Si $v$ es constante la fem es constante: el dispositivo actúa como un generador de corriente continua (hasta que la varilla sale de los rieles).

### Forma general

Las cargas de la varilla se mueven con $\vec{v}$ en el campo $\vec{B}$ y sienten la fuerza magnética $q\vec{v}\times\vec{B}$ (Clase 10). El trabajo por unidad de carga en una vuelta completa es la **fem de movimiento**:

$$\varepsilon=\oint\left(\vec{v}\times\vec{B}\right)\cdot d\vec{l}$$

Para la varilla, $\vec{v}\times\vec{B}$ tiene magnitud $vB$ y apunta a lo largo de la varilla (hacia arriba), y solo la varilla se mueve, de modo que $\varepsilon=vBL$, coherente con lo anterior.

**Potencia.** Con resistencia total $R$, la corriente es $I=BLv/R$ y la varilla siente una fuerza magnética $F_B=ILB$ opuesta a $\vec{v}$. Para mantener $v$ constante se necesita una fuerza externa igual y opuesta, cuya potencia es

$$P=F_{\text{aplicada}}\,v=(ILB)v=\frac{B^2L^2v^2}{R}=\frac{\varepsilon^2}{R}$$

que coincide con la potencia disipada en la resistencia (Clase 09): la energía mecánica se convierte en energía eléctrica.

## Ejemplo 3: Fuerza magnética sobre una barra deslizante

La barra conductora de la figura se mueve sobre dos rieles paralelos sin fricción en presencia de un campo magnético uniforme dirigido hacia la página. La barra tiene masa $m$ y su longitud es $L$. A la barra se le da una velocidad inicial $\vec{v}_i$ hacia la derecha y se libera en $t=0$.

a) Con las leyes de Newton encuentre la velocidad de la barra como función del tiempo.
b) Demuestre que se encuentra el mismo resultado al usar un planteamiento energético.

> **[Figura]:** Dos rieles horizontales separados una distancia $L$, unidos a la izquierda por una resistencia $R$. Campo $\vec{B}$ uniforme entrando en la página. Barra vertical sobre los rieles con velocidad inicial $\vec{v}_i$ hacia la derecha ($+x$). La corriente inducida $I$ circula en sentido antihorario (hacia arriba en la barra) y la fuerza magnética $\vec{F}_B$ sobre la barra apunta hacia la izquierda.

**Resolución**

*Idea:* al moverse la barra aparece la fem de movimiento $\varepsilon=BLv$ y una corriente $I=BLv/R$ (antihoraria por la ley de Lenz). Sobre la barra con corriente actúa $\vec{F}=I\vec{L}\times\vec{B}$ (Clase 10), que apunta a la izquierda: la barra debe frenar.

a) **Planteamiento de Newton.** La fuerza magnética es la única fuerza horizontal:
$$F_x=m\frac{dv}{dt}=-ILB$$

Sustituyendo $I=BLv/R$:
$$m\frac{dv}{dt}=-\frac{B^2L^2}{R}v$$

Separando variables:
$$\frac{dv}{v}=-\left(\frac{B^2L^2}{mR}\right)dt$$

Integrando con $v=v_i$ en $t=0$ (el factor $B^2L^2/mR$ es constante):
$$\int_{v_i}^{v}\frac{dv'}{v'}=-\frac{B^2L^2}{mR}\int_0^t dt'\quad\Rightarrow\quad\ln\!\left(\frac{v}{v_i}\right)=-\left(\frac{B^2L^2}{mR}\right)t$$

Definiendo $\tau=\dfrac{mR}{B^2L^2}$:

$$\boxed{v(t)=v_i\,e^{-t/\tau},\qquad\tau=\frac{mR}{B^2L^2}}$$

b) **Planteamiento energético.** El circuito es un sistema aislado: la energía cinética que pierde la barra se transfiere eléctricamente a la resistencia. Igualando potencias:
$$P_{\text{resistencia}}=-P_{\text{barra}}\quad\Rightarrow\quad I^2R=-\frac{d}{dt}\left(\tfrac12mv^2\right)$$

Con $I=BLv/R$ y derivando:
$$\frac{B^2L^2v^2}{R}=-mv\frac{dv}{dt}\quad\Rightarrow\quad\frac{dv}{v}=-\left(\frac{B^2L^2}{mR}\right)dt$$

que es la misma ecuación diferencial de a), y por lo tanto la misma solución $v=v_i e^{-t/\tau}$. ∎

*Verificación:* $[\tau]=\dfrac{\text{kg}\cdot\Omega}{\text{T}^2\text{m}^2}$; como $\text{T}=\text{N}/(\text{A}\cdot\text{m})$ y $\Omega=\text{V}/\text{A}$, resulta $\dfrac{\text{kg}\cdot\text{V}\cdot\text{A}}{\text{N}^2}=\dfrac{\text{kg}\cdot\text{W}}{\text{N}^2}=\text{s}$. ✓ La velocidad decrece exponencialmente y tiende a cero, como se esperaba.

*¿Qué pasaría si...? (distancia recorrida).* Integrando la velocidad:
$$x=\int_0^\infty v_ie^{-t/\tau}dt=-v_i\tau e^{-t/\tau}\Big|_0^\infty=v_i\tau=v_i\frac{mR}{B^2L^2}$$
Duplicar $v_i$ o $R$ duplica la distancia, pero reducir $B$ a la mitad la **cuadruplica**: es el cambio más efectivo.

## Campos eléctricos inducidos

> **[Figura]:** a) Solenoide largo de sección transversal $A$ y $n$ espiras por unidad de longitud, con corriente $I$ que crece a tasa $dI/dt$; el campo $\vec{B}$ está confinado al interior (cilindro azul). Una espira circular de alambre rodea el solenoide en su centro y está conectada a un galvanómetro G que mide la corriente inducida $I'$. b) Vista transversal: $\vec{B}$ entrando en la página dentro del círculo del solenoide; la espira de radio $r$ lo rodea; el campo eléctrico inducido $\vec{E}$ es tangente a la espira en cada punto (sentido antihorario cuando $B$ entrante aumenta) y la corriente $I'$ circula en el mismo sentido.

El campo magnético del solenoide es (Clase 12):
$$B=\mu_0 nI$$

De esta forma, el flujo magnético por la espira (el campo fuera del solenoide es despreciable, $\vec{A}\parallel\vec{B}$) es:
$$\Phi_B=BA=\mu_0 nIA$$

Cuando la corriente $I$ en el solenoide cambia con el tiempo, el flujo magnético también cambia, entonces la fem inducida es:
$$\varepsilon=-\frac{d\Phi_B}{dt}=-\mu_0 nA\frac{dI}{dt}$$

Si la resistencia total de la espira es $R$, entonces:
$$I'=\frac{\varepsilon}{R}$$

**¿Qué fuerza hace que las cargas se muevan alrededor de la espira?** No puede ser una fuerza magnética: el conductor no se mueve y ni siquiera está dentro del campo magnético. **Tiene que haber un campo eléctrico inducido en el conductor causado por el flujo magnético cambiante.**

Cuando una carga $q$ completa una vuelta alrededor de la espira, el trabajo total realizado sobre ella por el campo eléctrico debe ser igual al producto de $q$ por la fem $\varepsilon$, esto es:

$$\oint\vec{E}\cdot d\vec{l}=\varepsilon=-\frac{d\Phi_B}{dt}\qquad\text{(trayectoria de integración constante)}$$

Este campo eléctrico **no es conservativo**: su integral de línea en una trayectoria cerrada no es cero (a diferencia del campo electrostático de la Clase 05). No proviene de cargas, sino de un campo magnético variable. La forma general $\varepsilon=-d\Phi_B/dt$ siempre es válida; la forma con $\oint\vec{E}\cdot d\vec{l}$ requiere una trayectoria fija.

Para la espira circular de radio $r$, por simetría cilíndrica $\vec{E}$ tiene la misma magnitud en todos los puntos y es tangente a la circunferencia (no puede ser radial, pues la ley de Gauss exigiría carga neta encerrada, y no la hay). Entonces $\oint\vec{E}\cdot d\vec{l}=2\pi rE$ y

$$E=\frac{1}{2\pi r}\left|\frac{d\Phi_B}{dt}\right|$$

## Ejemplo 4: Campos eléctricos inducidos

Un solenoide largo tiene 500 espiras por metro, y la corriente en éstas crece a razón de 100 A/s. El área de la sección transversal del solenoide es de 4.00 cm².

a) Encuentre la magnitud de la fem inducida en la espira de alambre afuera del solenoide.
b) Calcule la magnitud del campo eléctrico inducido dentro de la espira si su radio es de 2.0 cm.

**Resolución**

*Idea:* el campo del solenoide (Ampère, Clase 12) es $B=\mu_0 nI$ solo en su interior, así que el flujo por la espira es $\mu_0 nIA$ con $A$ el área del **solenoide** (no de la espira). Faraday da la fem; la simetría cilíndrica permite despejar $E$ de $\oint\vec{E}\cdot d\vec{l}=2\pi rE$.

a)
$$\varepsilon=-\frac{d\Phi_B}{dt}=-\mu_0 nA\frac{dI}{dt}=-(4\pi\times10^{-7}\,\text{Wb/A·m})(500\,\text{m}^{-1})(4.0\times10^{-4}\,\text{m}^2)(100\,\text{A/s})$$
$$\varepsilon=-2.5\times10^{-5}\,\text{V}$$

$$\boxed{|\varepsilon|=25\,\mu\text{V}}$$

b) Por simetría, $|\oint\vec{E}\cdot d\vec{l}|=2\pi rE=|\varepsilon|$:
$$E=\frac{|\varepsilon|}{2\pi r}=\frac{25\times10^{-6}\,\text{V}}{2\pi(2.0\times10^{-2}\,\text{m})}=2.0\times10^{-4}\,\text{V/m}$$

$$\boxed{E=2.0\times10^{-4}\,\text{V/m}}$$

*Dirección e interpretación:* con $\vec{A}$ en el sentido del flujo entrante (hacia el plano de la vista transversal), una fem positiva iría en sentido horario; el signo negativo indica que la fem (y $\vec{E}$) van en **sentido antihorario**. Por la ley de Lenz: el flujo entrante aumenta, así que la corriente inducida debe crear un campo saliente dentro de la espira, lo que exige circulación antihoraria. ✓ El resultado de $E$ no depende de si $r$ es mayor que el radio del solenoide, mientras la espira lo encierre (el flujo encerrado es el mismo).

## Corrientes parásitas (de Foucault)

Cuando masas de metal se mueven en campos magnéticos, o están en campos magnéticos variables, aparecen corrientes inducidas que circulan por todo el volumen del material, con patrones que recuerdan remolinos: las **corrientes parásitas** o corrientes de Foucault.

> **[Figura]:** a) Disco metálico que gira en sentido horario (centro $O$) en un campo $\vec{B}$ entrante confinado a una región pequeña cerca del borde inferior; se marcan los sectores $Oa$, $Ob$ y $Oc$, con $Ob$ atravesando la región de campo. b) Corrientes parásitas resultantes: lazos de corriente a ambos lados del sector $Ob$, que bajan por la zona con campo y regresan por fuera de ella; la fuerza $\vec{F}$ sobre la corriente en la zona del campo apunta hacia la derecha, opuesta al movimiento del disco en esa zona.

El sector $Ob$ se desplaza a través del campo y tiene una fem inducida; los sectores $Oa$ y $Oc$ (fuera del campo) son trayectorias de retorno. Por la ley de Lenz, la fuerza $\vec{F}=I\vec{L}\times\vec{B}$ sobre la corriente en la región del campo se **opone** a la rotación: las corrientes parásitas producen un **frenado**. Las corrientes de retorno quedan fuera del campo y no sienten fuerza.

Aplicaciones y efectos: frenos magnéticos (trenes, máquinas), detectores de metales, cocinas de inducción; y pérdidas de energía (calentamiento) en núcleos de transformadores y motores, que se reducen usando núcleos laminados.

## Resumen de fórmulas

| Concepto | Expresión |
|---|---|
| Flujo magnético | $\Phi_B=\int\vec{B}\cdot d\vec{A}$; uniforme y plano: $\Phi_B=BA\cos\phi$ |
| Ley de Faraday ($N$ espiras) | $\varepsilon=-N\dfrac{d\Phi_B}{dt}$ |
| Ley de Lenz | La corriente inducida se opone al **cambio** de flujo |
| Alternador | $\Phi_B=BA\cos\omega t$, $\ \varepsilon=NBA\omega\sin\omega t$, $\ \varepsilon_{\text{máx}}=NBA\omega$, $\ \omega=2\pi f$ |
| Generador de CD (fem media) | $\varepsilon_{\text{med}}=\dfrac{2N\omega BA}{\pi}$ |
| Fem de movimiento | $\varepsilon=\oint(\vec{v}\times\vec{B})\cdot d\vec{l}$; barra: $|\varepsilon|=BLv$ |
| Potencia en la barra | $P=\dfrac{B^2L^2v^2}{R}=\dfrac{\varepsilon^2}{R}$ |
| Barra frenada | $v=v_ie^{-t/\tau}$, $\ \tau=\dfrac{mR}{B^2L^2}$, $\ x_{\text{total}}=v_i\tau$ |
| Campo eléctrico inducido | $\oint\vec{E}\cdot d\vec{l}=-\dfrac{d\Phi_B}{dt}$; simetría circular: $E=\dfrac{1}{2\pi r}\left|\dfrac{d\Phi_B}{dt}\right|$ |
| Forma diferencial | $\nabla\times\vec{E}=-\dfrac{\partial\vec{B}}{\partial t}$ |
| Solenoide y espira | $\varepsilon=-\mu_0 nA\dfrac{dI}{dt}$ |
| Bobina exploradora | $Q=\dfrac{NBA}{R}$ |
