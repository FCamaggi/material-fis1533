# Clase 11 — Fuentes de campo magnético: ley de Biot-Savart

En la Clase 10 estudiamos el efecto de un campo magnético $\vec{B}$ **sobre** cargas y corrientes (fuerza de Lorentz, fuerza sobre conductores, torque sobre espiras y momento dipolar $\vec{\mu}$). En esta clase damos el paso inverso: cómo las cargas en movimiento y las corrientes **generan** campo magnético. Antes, cerramos el tema de dipolos con su comportamiento en campos no uniformes.

## Dipolos magnéticos en campos no uniformes

En un campo **uniforme**, una espira con corriente (dipolo magnético de momento $\vec{\mu} = I\vec{A}$) experimenta un torque $\vec{\tau} = \vec{\mu}\times\vec{B}$, pero la **fuerza neta es nula**. En un campo **no uniforme** la fuerza neta en general no se anula.

La energía potencial de un dipolo en un campo magnético es (Clase 10)

$$U = -\vec{\mu}\cdot\vec{B}.$$

Como la fuerza es menos el gradiente de la energía potencial (con $\vec{\mu}$ constante):

$$\boxed{\vec{F} = -\nabla U = \nabla\left(\vec{\mu}\cdot\vec{B}\right)}$$

Consecuencias:

- Si $\vec{\mu}$ es **paralelo** a $\vec{B}$, $\vec{\mu}\cdot\vec{B} = \mu B$ crece hacia donde $B$ es más intenso: el dipolo es **atraído** hacia la región de campo fuerte.
- Si $\vec{\mu}$ es **antiparalelo** a $\vec{B}$, $\vec{\mu}\cdot\vec{B} = -\mu B$: el dipolo es **repelido** hacia la región de campo débil.
- Si $\vec{B}$ es uniforme, $\nabla(\vec{\mu}\cdot\vec{B}) = 0$ y no hay fuerza neta (solo torque).

**Interpretación microscópica.** Cerca del polo de un imán las líneas de campo divergen. Sobre cada elemento de la bobina actúa $d\vec{F} = I\,d\vec{l}\times\vec{B}$. Como $\vec{B}$ no es paralelo al eje de la bobina, cada $d\vec{F}$ tiene una componente radial y una axial: las componentes radiales se cancelan por simetría al recorrer toda la espira, pero las axiales se suman, dando una fuerza neta a lo largo del eje.

> **[Figura]:** a) Un imán de barra con su polo S a la izquierda y su polo N a la derecha; a la derecha del polo N hay una bobina circular coaxial. Las líneas de $\vec{B}$ salen del polo N y se abren (divergen) al llegar a la bobina. El momento magnético $\vec{\mu}$ de la bobina apunta hacia el imán (antiparalelo a $\vec{B}$). En cuatro puntos de la espira se dibujan las fuerzas $d\vec{F}$, perpendiculares a $\vec{B}$ local; sus componentes axiales apuntan hacia la derecha. Leyenda: "La fuerza neta sobre esta bobina se aleja del polo norte del imán" ($\vec{F}_{\text{neta}}$ hacia la derecha).
>
> b) La misma bobina, con el mismo sentido de corriente $I$ y el mismo $\vec{\mu}$ (hacia la izquierda), pero con el imán invertido (N a la izquierda, S frente a la bobina). Ahora $\vec{B}$ cerca de la bobina apunta hacia el polo S, es decir, paralelo a $\vec{\mu}$. Las $d\vec{F}$ tienen componentes axiales hacia la izquierda. Leyenda: "La fuerza neta sobre la misma bobina va hacia el polo sur del imán".

Ambos casos se resumen en $\vec{F} = \nabla(\vec{\mu}\cdot\vec{B})$: en a) $\vec{\mu}\cdot\vec{B}<0$ y la bobina se aleja del campo intenso; en b) $\vec{\mu}\cdot\vec{B}>0$ y se acerca. Este mismo mecanismo explica por qué un imán atrae un trozo de hierro: los dipolos atómicos del hierro se alinean paralelos al campo y son atraídos hacia la región de campo más intenso.

## Campo magnético de una carga en movimiento

Igual que en el caso eléctrico, llamamos **punto de fuente** a la ubicación de la carga en movimiento en un instante dado y **punto de campo** al punto $P$ donde queremos calcular el campo. Recordemos que el campo eléctrico de una carga puntual es proporcional a $|q|$ y a $1/r^2$, y su dirección (para $q>0$) va a lo largo de la línea que une el punto de fuente con el punto de campo.

Los experimentos demuestran que la magnitud de $\vec{B}$ también es proporcional a $|q|$ y a $1/r^2$. Pero la **dirección** de $\vec{B}$ **no** es a lo largo de la línea que va del punto de fuente al punto de campo. En vez de ello, $\vec{B}$ es perpendicular al plano que contiene esta línea y al vector velocidad $\vec{v}$ de la partícula. Además, la magnitud es proporcional a la rapidez $v$ y al seno del ángulo $\phi$ entre $\vec{v}$ y la línea fuente–campo:

$$B = \frac{\mu_0}{4\pi}\,\frac{|q|\,v\sin\phi}{r^2}$$

donde $\mu_0/4\pi$ es una constante de proporcionalidad ($\mu_0$ se lee "mu subcero"). Introduciendo el vector unitario $\hat{r} = \vec{r}/r$ que apunta **desde el punto de fuente hacia el punto de campo**, magnitud y dirección se resumen en una sola ecuación vectorial:

$$\boxed{\vec{B} = \frac{\mu_0}{4\pi}\,\frac{q\,\vec{v}\times\hat{r}}{r^2}}\qquad\text{(carga puntual con velocidad constante)}$$

Propiedades:

- En todos los puntos de la recta que pasa por la carga y es paralela a $\vec{v}$, el campo es **cero**, porque $\sin\phi = 0$.
- A una distancia $r$ dada, $B$ es máximo en el plano perpendicular a $\vec{v}$ que pasa por la carga ($\phi = 90^\circ$).
- Si $q<0$, todas las direcciones se invierten.
- **Líneas de campo:** son **círculos** centrados en la recta de $\vec{v}$, contenidos en planos perpendiculares a ella (muy distinto de las líneas radiales del campo eléctrico).
- **Regla de la mano derecha:** apunte el pulgar derecho en la dirección de $\vec{v}$; los dedos se cierran alrededor de la carga en el sentido de las líneas de $\vec{B}$ (para $q>0$).

Estas expresiones valen para velocidad constante (y $v\ll c$); si la carga acelera, el campo es mucho más complicado.

> **[Figura]:** a) Vista en perspectiva: una carga positiva $q$ se mueve con velocidad $\vec{v}$ (flecha verde hacia la derecha) y una mano derecha con el pulgar a lo largo de $\vec{v}$ indica el sentido de giro de $\vec{B}$. Se dibujan dos planos que contienen la recta de $\vec{v}$: uno vertical (beige) y uno horizontal (dorado). Para un punto $P$ del plano beige, el vector $\vec{r}$ va de $q$ a $P$ formando un ángulo $\phi$ con $\vec{v}$, y $\vec{B}$ en $P$ es perpendicular a ese plano. Para puntos del plano dorado, $\vec{B}$ es vertical hacia abajo, perpendicular a ese plano. En los puntos sobre la recta de $\vec{v}$ (delante y detrás de la carga) se indica $B=0$.
>
> b) Vista desde atrás de la carga: la carga se aleja del lector (símbolo $\otimes$, entra a la página) y las líneas de $\vec{B}$ son círculos concéntricos alrededor de ella recorridos en sentido **horario**.

## Ley de Biot-Savart

Una corriente es un conjunto de cargas en movimiento. Un elemento de conductor de largo $d\vec{s}$ con corriente $I$ contiene una carga $dQ$ que se mueve con velocidad de arrastre $\vec{v}_d$, de modo que $dQ\,\vec{v}_d = I\,d\vec{s}$. Reemplazando $q\vec{v}\to I\,d\vec{s}$ en el campo de la carga puntual obtenemos la **ley de Biot-Savart**, que relaciona el campo magnético $d\vec{B}$ en un punto $P$ producido por un elemento de largo $d\vec{s}$ que porta una corriente $I$:

$$\boxed{d\vec{B} = \frac{\mu_0}{4\pi}\,\frac{I\,d\vec{s}\times\hat{r}}{r^2}}$$

donde

- $\mu_0$ es la **permeabilidad del vacío**,
- $r$ es la distancia desde el elemento hasta el punto $P$,
- $\hat{r}$ es el vector unitario que apunta desde $d\vec{s}$ hacia $P$.

Su magnitud es $dB = \dfrac{\mu_0}{4\pi}\dfrac{I\,ds\,\sin\phi}{r^2}$, con $\phi$ el ángulo entre $d\vec{s}$ y $\hat{r}$. El campo total de un conductor se obtiene por **superposición**, integrando sobre todo el circuito:

$$\vec{B} = \frac{\mu_0 I}{4\pi}\int \frac{d\vec{s}\times\hat{r}}{r^2}
\qquad\text{o bien}\qquad
\vec{B}(\vec{r}) = \frac{\mu_0}{4\pi}\int \frac{I\,d\vec{r}\,'\times(\vec{r}-\vec{r}\,')}{\|\vec{r}-\vec{r}\,'\|^3}$$

donde en la segunda forma $\vec{r}$ es la posición del punto de campo y $\vec{r}\,'$ la del elemento de corriente (usar $\hat{r}/r^2 = (\vec{r}-\vec{r}\,')/\|\vec{r}-\vec{r}\,'\|^3$). Esta ley permite determinar el campo de cualquier cable que conduce corriente. Es el análogo magnético de la integración de la ley de Coulomb para distribuciones continuas (Clase 03), con la diferencia de que aparece un **producto cruz**.

La permeabilidad tiene en SI el valor

$$\mu_0 = 4\pi\times10^{-7}\,\text{T·m/A}$$

y tiene la particularidad de que

$$\varepsilon_0\,\mu_0 = \frac{1}{c^2},$$

donde $c\approx 3.00\times10^{8}\,\text{m/s}$ es la rapidez de la luz en el vacío. (Verificación: $\varepsilon_0\mu_0 = 8.854\times10^{-12}\cdot 4\pi\times10^{-7} = 1.113\times10^{-17}\,\text{s}^2/\text{m}^2$ y $1/c^2 = 1.11\times10^{-17}\,\text{s}^2/\text{m}^2$.) Esta relación anticipa que la luz es una onda electromagnética.

> **[Figura]:** Un elemento de corriente $I\,d\vec{l}$ (segmento de alambre a lo largo de un eje horizontal, "eje de $d\vec{l}$") y una mano derecha cuyo pulgar apunta en la dirección de la corriente: "Regla de la mano derecha para el campo magnético debido a un elemento de corriente: apunte el pulgar de su mano derecha en dirección de la corriente. Ahora cierre sus dedos alrededor del elemento de corriente en dirección de las líneas de campo magnético". Igual que para la carga puntual, para puntos de campo en el plano beige (que contiene a $\vec{r}$ y a $d\vec{l}$) el vector $d\vec{B}$ es perpendicular a ese plano; para puntos en el plano dorado, $d\vec{B}$ es perpendicular al plano dorado. Sobre el eje de $d\vec{l}$ el campo es nulo.

## Ejemplo: campo de un conductor recto (finito e infinito)

**Enunciado.** Calcular el campo magnético generado por un conductor infinito que transporta corriente $I$.

**Resolución**

*Idea.* Usamos la ley de Biot-Savart recién vista y superposición: dividimos el alambre en elementos $d\vec{s}$, calculamos $d\vec{B}$ de cada uno y sumamos. Conviene resolver primero el caso de un tramo **finito**, que es más general, y luego tomar el límite de largo infinito.

*Planteamiento geométrico.* Ponemos el alambre sobre el eje $x$, con la corriente en $+\hat{x}$, y el punto de campo $P$ sobre el eje $y$ a distancia perpendicular $R$ del alambre: $P=(0,R,0)$. Un elemento genérico está en $(x,0,0)$, con $d\vec{s} = dx\,\hat{x}$.

- Vector del elemento a $P$: $\vec{r} = -x\,\hat{x} + R\,\hat{y}$, de módulo $r = \sqrt{x^2+R^2}$.
- Producto cruz: $d\vec{s}\times\vec{r} = dx\,\hat{x}\times(-x\,\hat{x}+R\,\hat{y}) = R\,dx\,(\hat{x}\times\hat{y}) = R\,dx\,\hat{z}$.

Todos los elementos aportan en la **misma dirección** $\hat{z}$ (regla de la mano derecha), así que basta sumar magnitudes:

$$d\vec{B} = \frac{\mu_0 I}{4\pi}\,\frac{d\vec{s}\times\vec{r}}{r^3} = \frac{\mu_0 I}{4\pi}\,\frac{R\,dx}{(x^2+R^2)^{3/2}}\,\hat{z}.$$

*Cambio de variable.* Sea $\theta$ el ángulo que forma la recta elemento–$P$ con la perpendicular al alambre que pasa por $P$ (medido positivo hacia $+x$): $x = R\tan\theta$. Entonces

$$dx = R\sec^2\theta\,d\theta,\qquad x^2+R^2 = R^2\sec^2\theta,\qquad (x^2+R^2)^{3/2} = R^3\sec^3\theta.$$

Sustituyendo:

$$dB = \frac{\mu_0 I}{4\pi}\,\frac{R\cdot R\sec^2\theta\,d\theta}{R^3\sec^3\theta} = \frac{\mu_0 I}{4\pi R}\cos\theta\,d\theta.$$

*Alambre finito.* Si el alambre va desde el ángulo $\theta_1$ hasta $\theta_2$ (vistos desde $P$):

$$B = \frac{\mu_0 I}{4\pi R}\int_{\theta_1}^{\theta_2}\cos\theta\,d\theta$$

$$\boxed{B = \frac{\mu_0 I}{4\pi R}\left(\sin\theta_2 - \sin\theta_1\right)}$$

Equivalentemente, si el alambre va de $x=x_1$ a $x=x_2$, como $\sin\theta = x/\sqrt{x^2+R^2}$:

$$B = \frac{\mu_0 I}{4\pi R}\left(\frac{x_2}{\sqrt{x_2^2+R^2}} - \frac{x_1}{\sqrt{x_1^2+R^2}}\right).$$

Para un tramo simétrico de largo $2a$ centrado frente a $P$ ($x_1=-a$, $x_2=a$): $B = \dfrac{\mu_0 I}{2\pi R}\dfrac{a}{\sqrt{a^2+R^2}}$.

*Alambre infinito.* Hacemos $x_1\to-\infty$, $x_2\to+\infty$, es decir $\theta_1 = -\pi/2$, $\theta_2 = +\pi/2$:

$$B = \frac{\mu_0 I}{4\pi R}\left[1-(-1)\right]$$

$$\boxed{B = \frac{\mu_0 I}{2\pi R}}$$

En forma vectorial, usando coordenadas cilíndricas con el eje del alambre como eje $z$ y $s$ la distancia al alambre:

$$\vec{B} = \frac{\mu_0 I}{2\pi s}\,\hat{\phi}.$$

*Dirección.* Las líneas de campo son **círculos concéntricos** al alambre. Se usa la regla de la mano derecha: el pulgar derecho apunta en el sentido de la corriente y los dedos, al cerrarse alrededor del alambre, indican el sentido de $\vec{B}$.

> **[Figura]:** (Geometría usada en las diapositivas, tomada del texto guía.) Un alambre recto vertical sobre el eje $y$, de largo $2a$ (de $y=-a$ a $y=a$), con corriente $I$ hacia arriba. Un elemento $d\vec{l}$ (en rojo) a la altura $y$; desde él, el vector $\vec{r}$ (azul) llega al punto de campo $P$, ubicado sobre el eje $x$ a distancia $x$ del alambre, con $r=\sqrt{x^2+y^2}$; se marca el ángulo $\phi$ entre $d\vec{l}$ y $\vec{r}$ y el vector unitario $\hat{r}$ (negro). En $P$, el campo $d\vec{B}$ entra al plano del dibujo. Debajo, el mismo alambre atravesando una caja con líneas de $\vec{B}$ circulares y una mano derecha con el pulgar según $I$ y los dedos curvados según $\vec{B}$.
>
> Es exactamente el cálculo anterior con los ejes rotados ($x\leftrightarrow y$, $R\to x$): para el tramo simétrico de largo $2a$, $B = \dfrac{\mu_0 I}{4\pi}\dfrac{2a}{x\sqrt{x^2+a^2}}$, y con $a\to\infty$, $B = \dfrac{\mu_0 I}{2\pi x}$.

*Verificación / interpretación.*

- Unidades: $\dfrac{(\text{T·m/A})\,\text{A}}{\text{m}} = \text{T}$. ✓
- $B\propto 1/R$: decae más lento que el campo de una carga puntual ($1/r^2$), igual que el campo eléctrico de una línea infinita de carga $E = \lambda/(2\pi\varepsilon_0 R)$ (Clase 03). La analogía es formal: $\lambda/\varepsilon_0 \leftrightarrow \mu_0 I$, pero $\vec{E}$ es radial y $\vec{B}$ es azimutal.
- Si $R\gg a$ en el tramo finito simétrico, $B\approx \dfrac{\mu_0 I\,(2a)}{4\pi R^2}$: el tramo se ve como un solo elemento $I\,d\vec{s}$ de largo $2a$, como predice Biot-Savart directamente. ✓
- Valor típico: $I = 10\,\text{A}$, $R = 5\,\text{cm}$ $\Rightarrow$ $B = \dfrac{4\pi\times10^{-7}\cdot10}{2\pi\cdot0.05} = 4.0\times10^{-5}\,\text{T}$, del orden del campo magnético terrestre.

**Evidencia experimental.** Las líneas de campo magnético circulares que rodean un conductor de corriente pueden desplegarse mediante limaduras de hierro.

> **[Figura]:** Dos fotografías de un alambre vertical que atraviesa una lámina horizontal espolvoreada con limaduras de hierro. Las limaduras se ordenan formando círculos concéntricos centrados en el alambre, confirmando que $\vec{B}$ es azimutal y de igual magnitud a igual distancia.

## Complemento: fuerza entre conductores paralelos y definición del ampere

Combinamos el resultado anterior con la fuerza sobre un conductor en un campo magnético (Clase 10), $\vec{F} = I\,\vec{L}\times\vec{B}$.

Consideremos dos alambres rectos, largos y paralelos, separados una distancia $d$, con corrientes $I_1$ e $I_2$.

1. El alambre 1 produce en la posición del alambre 2 un campo de magnitud $B_1 = \dfrac{\mu_0 I_1}{2\pi d}$, tangente al círculo centrado en el alambre 1 que pasa por el alambre 2; es decir, perpendicular tanto al alambre 2 como a la recta que une ambos alambres.
2. Sobre un largo $L$ del alambre 2 actúa $\vec{F}_2 = I_2\,\vec{L}\times\vec{B}_1$. Como $\vec{L}\perp\vec{B}_1$:

$$F_2 = I_2 L B_1 = \frac{\mu_0 I_1 I_2 L}{2\pi d}\quad\Longrightarrow\quad \boxed{\frac{F}{L} = \frac{\mu_0 I_1 I_2}{2\pi d}}$$

3. Por la tercera ley de Newton (y repitiendo el cálculo con los índices intercambiados), el alambre 1 recibe una fuerza igual y opuesta.

*Dirección.* Tomemos el alambre 1 en el eje $z$ con $I_1$ en $+\hat{z}$ y el alambre 2 en $x=d$. En $x=d$, $\vec{B}_1 = \dfrac{\mu_0 I_1}{2\pi d}\hat{y}$. Si $I_2$ también va en $+\hat{z}$: $\vec{F}_2 \propto \hat{z}\times\hat{y} = -\hat{x}$, es decir hacia el alambre 1.

- Corrientes en el **mismo sentido** $\Rightarrow$ los conductores se **atraen**.
- Corrientes en **sentidos opuestos** $\Rightarrow$ los conductores se **repelen**.

(Notar el contraste con cargas eléctricas, donde "iguales se repelen".)

**Definición del ampere.** Históricamente el ampere se definió así: si dos conductores rectos, largos y paralelos, separados $1\,\text{m}$ en el vacío, portan la misma corriente y la fuerza por unidad de longitud entre ellos es $2\times10^{-7}\,\text{N/m}$, la corriente en cada uno es de $1\,\text{A}$. En efecto, con $I_1=I_2=1\,\text{A}$ y $d=1\,\text{m}$:

$$\frac{F}{L} = \frac{4\pi\times10^{-7}\cdot1\cdot1}{2\pi\cdot1} = 2\times10^{-7}\,\text{N/m}.$$

Esta definición fijaba $\mu_0 = 4\pi\times10^{-7}\,\text{T·m/A}$ exactamente. Desde 2019 el SI define el ampere fijando el valor de la carga elemental $e$, y $\mu_0$ pasó a ser un valor medido, igual a $4\pi\times10^{-7}$ con una precisión de $\sim10^{-10}$; para efectos del curso se usa este valor.

## Ejemplo: campo magnético de una espira circular

**Enunciado.** Una espira circular de radio $R$, en el plano $xy$ y centrada en el origen, transporta una corriente $I$. Calcular el campo magnético en un punto $P$ del eje de la espira, a una altura $z$.

> **[Figura]:** Espira circular (anillo) de radio $R$ en el plano $xy$, centrada en el origen; ejes $x$ (hacia el lector), $y$ (a la derecha) y $z$ (vertical). La corriente $I$ circula en sentido antihorario visto desde $+z$ (flechas moradas). El punto $P$ está sobre el eje $z$, con vector posición $\vec{r} = z\hat{z}$. Un elemento $I\,d\vec{l}$ se ubica en la espira en la posición $\vec{r}\,'$, que forma un ángulo $\phi$ con el eje $x$; el vector $\vec{r}-\vec{r}\,'$ va desde el elemento hasta $P$.

Resultado que se muestra en la diapositiva:

$$B_z = \frac{\mu_0 I R^2}{2\left(z^2+R^2\right)^{3/2}}$$

**Resolución**

*Idea.* Ley de Biot-Savart en forma vectorial, $d\vec{B} = \dfrac{\mu_0 I}{4\pi}\dfrac{d\vec{l}\times(\vec{r}-\vec{r}\,')}{\|\vec{r}-\vec{r}\,'\|^3}$, parametrizando la espira con el ángulo $\phi$. La simetría de rotación alrededor del eje $z$ hará que las componentes perpendiculares al eje se cancelen.

*Paso 1: vectores.*

$$\vec{r} = z\,\hat{z},\qquad \vec{r}\,' = R\cos\phi\,\hat{x} + R\sin\phi\,\hat{y},\qquad d\vec{l} = \frac{d\vec{r}\,'}{d\phi}d\phi = R\,d\phi\left(-\sin\phi\,\hat{x} + \cos\phi\,\hat{y}\right)$$

$$\vec{r}-\vec{r}\,' = -R\cos\phi\,\hat{x} - R\sin\phi\,\hat{y} + z\,\hat{z},\qquad \|\vec{r}-\vec{r}\,'\| = \sqrt{R^2+z^2}\ \ (\text{constante}).$$

*Paso 2: producto cruz.*

$$d\vec{l}\times(\vec{r}-\vec{r}\,') = R\,d\phi\begin{vmatrix}\hat{x} & \hat{y} & \hat{z}\\ -\sin\phi & \cos\phi & 0\\ -R\cos\phi & -R\sin\phi & z\end{vmatrix}
= R\,d\phi\left(z\cos\phi\,\hat{x} + z\sin\phi\,\hat{y} + R(\sin^2\phi+\cos^2\phi)\,\hat{z}\right)$$

$$= R\,d\phi\left(z\cos\phi\,\hat{x} + z\sin\phi\,\hat{y} + R\,\hat{z}\right).$$

*Paso 3: integrar de $0$ a $2\pi$.* Como $\int_0^{2\pi}\cos\phi\,d\phi = \int_0^{2\pi}\sin\phi\,d\phi = 0$, las componentes $x$ e $y$ se anulan (cada elemento tiene un "opuesto" diametral cuyo aporte perpendicular cancela el suyo). Queda:

$$\vec{B} = \frac{\mu_0 I}{4\pi}\,\frac{1}{(R^2+z^2)^{3/2}}\int_0^{2\pi}R^2\,d\phi\;\hat{z} = \frac{\mu_0 I}{4\pi}\,\frac{2\pi R^2}{(R^2+z^2)^{3/2}}\,\hat{z}$$

$$\boxed{\vec{B} = \frac{\mu_0 I R^2}{2\left(z^2+R^2\right)^{3/2}}\,\hat{z}}$$

que coincide con la expresión de la diapositiva. (Con la notación habitual de los textos, eje $x$ y radio $a$: $B_x = \dfrac{\mu_0 I a^2}{2(x^2+a^2)^{3/2}}$.)

*Casos límite.*

- **Centro de la espira** ($z=0$):
$$\boxed{B_{\text{centro}} = \frac{\mu_0 I}{2R}}$$
Para $N$ vueltas apretadas, se multiplica por $N$.
- **Lejos de la espira** ($|z|\gg R$): $(z^2+R^2)^{3/2}\approx |z|^3$, así que
$$B \approx \frac{\mu_0 I R^2}{2|z|^3} = \frac{\mu_0}{2\pi}\,\frac{\mu}{|z|^3},\qquad \mu = I\pi R^2.$$
Es el campo de un **dipolo magnético** de momento $\vec{\mu} = I\pi R^2\,\hat{z}$ sobre su eje, con la misma forma que el campo eléctrico de un dipolo eléctrico en su eje, $E = \dfrac{1}{4\pi\varepsilon_0}\dfrac{2p}{|z|^3}$ (cambiando $p/\varepsilon_0\to\mu_0\mu$). Esto justifica llamar "dipolo magnético" a la espira (Clase 10).

*Dirección (regla de la mano derecha para una espira).* Si los dedos de la mano derecha se doblan en la dirección de $I$, el pulgar apunta en la dirección de $\vec{B}$ en el eje (y de $\vec{\mu}$).

> **[Figura]:** Dos espiras horizontales con una mano derecha cuyos dedos siguen el sentido de la corriente: en la primera, corriente antihoraria vista desde arriba y $\vec{B}$ hacia arriba; en la segunda, corriente horaria y $\vec{B}$ hacia abajo. Leyenda: "Cuando los dedos de la mano derecha se doblan en la dirección de $I$, el pulgar apunta en la dirección de $\vec{B}$".

*Verificación / interpretación.*

- Unidades: $\dfrac{(\text{T·m/A})\,\text{A}\,\text{m}^2}{\text{m}^3} = \text{T}$. ✓
- $B$ es máximo en el centro y decae simétricamente en $\pm z$ (función par de $z$). ✓
- Ejemplo numérico: $R = 5\,\text{cm}$, $I = 2\,\text{A}$: $B_{\text{centro}} = \dfrac{4\pi\times10^{-7}\cdot2}{2\cdot0.05} = 2.51\times10^{-5}\,\text{T}$; a $z = 5\,\text{cm}$: $B = B_{\text{centro}}\cdot\dfrac{R^3}{(2R^2)^{3/2}} = \dfrac{B_{\text{centro}}}{2\sqrt2} = 8.9\times10^{-6}\,\text{T}$.

## Resumen de fórmulas

| Concepto | Fórmula |
|---|---|
| Fuerza sobre un dipolo en campo no uniforme | $\vec{F} = \nabla(\vec{\mu}\cdot\vec{B})$, con $U = -\vec{\mu}\cdot\vec{B}$ |
| Campo de una carga puntual en movimiento | $\vec{B} = \dfrac{\mu_0}{4\pi}\dfrac{q\,\vec{v}\times\hat{r}}{r^2}$ |
| Ley de Biot-Savart | $d\vec{B} = \dfrac{\mu_0}{4\pi}\dfrac{I\,d\vec{s}\times\hat{r}}{r^2}$; $\ \vec{B}(\vec{r}) = \dfrac{\mu_0}{4\pi}\displaystyle\int\dfrac{I\,d\vec{r}\,'\times(\vec{r}-\vec{r}\,')}{\|\vec{r}-\vec{r}\,'\|^3}$ |
| Permeabilidad del vacío | $\mu_0 = 4\pi\times10^{-7}\,\text{T·m/A}$; $\ \varepsilon_0\mu_0 = 1/c^2$ |
| Alambre recto finito | $B = \dfrac{\mu_0 I}{4\pi R}(\sin\theta_2-\sin\theta_1)$ |
| Alambre recto infinito | $\vec{B} = \dfrac{\mu_0 I}{2\pi R}\hat{\phi}$ |
| Fuerza entre conductores paralelos | $\dfrac{F}{L} = \dfrac{\mu_0 I_1 I_2}{2\pi d}$ (mismo sentido: atracción; opuesto: repulsión) |
| Espira circular, en su eje | $B_z = \dfrac{\mu_0 I R^2}{2(z^2+R^2)^{3/2}}$ |
| Centro de la espira | $B = \dfrac{\mu_0 I}{2R}$ ($N$ vueltas: $\times N$) |
| Espira lejos ($|z|\gg R$): dipolo | $B \approx \dfrac{\mu_0}{2\pi}\dfrac{\mu}{|z|^3}$, $\mu = I\pi R^2$ |
