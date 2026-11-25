# Clase 12 — Ley de Ampère

En la Clase 11 obtuvimos el campo magnético de corrientes mediante la ley de Biot-Savart, integrando elemento por elemento. Comenzamos aplicándola a un alambre con una parte curva. Luego introducimos la **ley de Ampère**, que cumple para el campo magnético un papel análogo al de la ley de Gauss para el campo eléctrico (Clases 03 y 04): permite calcular $\vec{B}$ de forma muy simple cuando la distribución de corriente tiene alta simetría. Terminamos con la corrección de Maxwell (corriente de desplazamiento).

## Ejemplo 1: alambre con una semicircunferencia

**Enunciado.** En el alambre de la figura, el radio de la semicircunferencia es $r$, y las dos ramas rectas se extienden hasta el infinito. Por el alambre circula una corriente $I$. Determine la magnitud y dirección del campo magnético en el centro $C$.

> **[Figura]:** Un alambre horizontal que viene desde $-\infty$ por la izquierda con corriente $I$ hacia la derecha, llega a un punto a distancia $r$ a la izquierda de $C$, sube y recorre una **semicircunferencia superior** de radio $r$ centrada en $C$ (pasando por arriba de $C$), baja en el punto a distancia $r$ a la derecha de $C$ y continúa horizontalmente hacia $+\infty$ con corriente $I$ hacia la derecha. El punto $C$ está sobre la recta que contiene ambas ramas rectas.

**Resolución**

*Idea.* Ley de Biot-Savart (Clase 11) y superposición: separamos el alambre en tres partes (rama recta izquierda, semicircunferencia, rama recta derecha) y sumamos sus contribuciones en $C$.

*Paso 1: ramas rectas.* Para cualquier elemento $d\vec{s}$ de las ramas rectas, el vector $\hat{r}$ que va del elemento a $C$ es **paralelo o antiparalelo** a $d\vec{s}$, porque $C$ está sobre la misma recta que esas ramas. Entonces

$$d\vec{s}\times\hat{r} = \vec{0}\quad\Longrightarrow\quad d\vec{B}_{\text{rectas}} = \vec{0}.$$

Las ramas rectas **no** contribuyen al campo en $C$ (aunque sean infinitas).

*Paso 2: semicircunferencia.* Para cada elemento del arco:

- la distancia a $C$ es siempre $r$ (constante);
- $d\vec{s}$ es tangente al arco y $\hat{r}$ es radial hacia $C$, luego $d\vec{s}\perp\hat{r}$ y $|d\vec{s}\times\hat{r}| = ds$;
- la corriente recorre el arco por arriba, de izquierda a derecha, es decir en **sentido horario** visto por el lector. Por la regla de la mano derecha (dedos según la corriente en la espira, pulgar según $\vec{B}$), todos los elementos aportan en la misma dirección: **entrando al papel**.

Como todas las contribuciones son paralelas, sumamos magnitudes:

$$B = \int\frac{\mu_0}{4\pi}\frac{I\,ds}{r^2} = \frac{\mu_0 I}{4\pi r^2}\int_{\text{arco}}ds = \frac{\mu_0 I}{4\pi r^2}\,(\pi r).$$

$$\boxed{B(C) = \frac{\mu_0 I}{4r}\quad\text{entrando al papel}}$$

*Verificación / interpretación.*

- Una espira circular completa da en su centro $\mu_0 I/(2R)$ (Clase 11); media espira da la mitad: $\mu_0 I/(4r)$. ✓
- Unidades: $(\text{T·m/A})\,\text{A}/\text{m} = \text{T}$. ✓
- Si la corriente circulara de derecha a izquierda, el campo saldría del papel con la misma magnitud.

## Ejercicio 2: resolución vectorial del mismo alambre

La diapositiva del Ejercicio 2 presenta la resolución formal (vectorial) del alambre anterior. Recordemos la fórmula de Biot-Savart para el cálculo de campo magnético, con $\vec{r}$ la posición del punto de campo y $\vec{R}$ la posición del elemento de corriente:

$$\vec{B}(\vec{r}) = \frac{\mu_0}{4\pi}\int\frac{I\,d\vec{R}\times(\vec{r}-\vec{R})}{\|\vec{r}-\vec{R}\|^3}$$

**Resolución**

*Idea.* Elegir coordenadas que simplifiquen los vectores: origen en el punto de campo y coordenadas polares $(\rho,\theta)$ en el plano del alambre.

*Paso 1: sistema de coordenadas.* En este caso $\vec{r} = \vec{0}$, tomando un sistema de coordenadas conveniente en el que el origen está en $C$ y el eje $Z$ sale del papel ($\hat{x}$ a la derecha, $\hat{y}$ hacia arriba, $\hat{k}$ hacia el lector).

*Paso 2: porciones rectas.* En las porciones rectas, los vectores $d\vec{R}$ y $\vec{R}$ son paralelos, pues están sobre una recta que pasa por el origen; por tanto el producto cruz $d\vec{R}\times(\vec{0}-\vec{R})$ se anula. Así, dichas porciones no crean campo magnético en $C$.

*Paso 3: segmento semicircular.* Parametrizamos con el ángulo polar $\theta\in[0,\pi]$:

$$\vec{R} = r\,\hat{\boldsymbol{\rho}},\qquad d\vec{R} = r\,d\theta\,\hat{\boldsymbol{\theta}},\qquad \|\vec{r}-\vec{R}\|^3 = r^3.$$

Al aumentar $\theta$ de $0$ a $\pi$ se recorre el arco en sentido **antihorario** (de derecha a izquierda), pero la corriente lo recorre de izquierda a derecha (de $\theta=\pi$ a $\theta=0$). Para integrar de $0$ a $\pi$ manteniendo el sentido físico de la corriente, se escribe el elemento como $-I\,r\,d\theta\,\hat{\boldsymbol{\theta}}$. Además $\vec{r}-\vec{R} = -r\,\hat{\boldsymbol{\rho}}$. Reemplazando:

$$\vec{B}(C) = \frac{\mu_0}{4\pi}\int_0^{\pi}\frac{-I\,r\,d\theta\,\hat{\boldsymbol{\theta}}\times(-r\,\hat{\boldsymbol{\rho}})}{r^3}.$$

*Paso 4: producto cruz.* Como $(\hat{\boldsymbol{\rho}},\hat{\boldsymbol{\theta}},\hat{k})$ es una base derecha, $\hat{\boldsymbol{\rho}}\times\hat{\boldsymbol{\theta}} = \hat{k}$ y por lo tanto $\hat{\boldsymbol{\theta}}\times\hat{\boldsymbol{\rho}} = -\hat{k}$:

$$(-I\,r\,d\theta\,\hat{\boldsymbol{\theta}})\times(-r\,\hat{\boldsymbol{\rho}}) = I\,r^2\,d\theta\,(\hat{\boldsymbol{\theta}}\times\hat{\boldsymbol{\rho}}) = -I\,r^2\,d\theta\,\hat{k}.$$

*Paso 5: integrar.*

$$\vec{B}(C) = \frac{\mu_0}{4\pi}\cdot\frac{-I\,r^2}{r^3}\int_0^{\pi}d\theta\;\hat{k} = -\frac{\mu_0 I\,\pi}{4\pi r}\hat{k}$$

$$\boxed{\vec{B}(C) = -\frac{\mu_0 I}{4r}\,\hat{k}}$$

y el campo **entra al papel**.

*Verificación / interpretación.* Coincide en magnitud y dirección con el Ejemplo 1, obtenido con la regla de la mano derecha. El método vectorial es más largo, pero el signo sale solo, sin depender de la intuición geométrica; es la forma recomendable cuando el cálculo no es tan evidente.

## Recordatorio: campo de un alambre y divergencia de $\vec{B}$

El campo magnético generado por un cable recto e infinito con corriente $I$ está dado por (Clase 11)

$$\vec{B} = \frac{\mu_0 I}{2\pi r}\,\hat{\theta}.$$

> **[Figura]:** Un alambre recto (amarillo) con corriente $I$ hacia la derecha atraviesa una caja (superficie cerrada) de la que se ha cortado una esquina. Las líneas de $\vec{B}$ son círculos azules alrededor del alambre, recorridos según la regla de la mano derecha (mano a la derecha con el pulgar en la dirección de $I$). En la cara superior interior las líneas salen de la página (puntos) y en la cara inferior entran (cruces); en los vértices se dibujan vectores $\vec{B}$ tangentes a los círculos. Toda línea de campo que entra a la caja vuelve a salir de ella.

Se observa que, para cualquier superficie cerrada, el flujo magnético neto es nulo:

$$\oint\vec{B}\cdot d\vec{A} = 0\qquad\Longleftrightarrow\qquad \nabla\cdot\vec{B} = 0$$

(la equivalencia se obtiene con el teorema de la divergencia, igual que en la ley de Gauss diferencial de la Clase 04). Es la **ley de Gauss del magnetismo**: las líneas de $\vec{B}$ son cerradas y no existen "cargas magnéticas" (monopolos) donde puedan nacer o terminar. Por eso, para calcular $\vec{B}$ a partir de sus fuentes, no sirve una integral de flujo; lo que sí da información es la **circulación** de $\vec{B}$ a lo largo de una curva cerrada.

## Ley de Ampère (forma integral)

### Circulación alrededor de un alambre recto

Calculemos $\oint\vec{B}\cdot d\vec{l}$ para el campo de un alambre infinito, sobre distintas curvas cerradas en un plano perpendicular al alambre.

**Caso 1: círculo concéntrico, recorrido en el sentido de $\vec{B}$.**

> **[Figura]:** Corriente $I$ saliendo del papel ($\odot$) en el centro de un círculo de radio $r$ recorrido en sentido antihorario. En cuatro puntos del círculo se dibujan $d\vec{l}$ (tangente, sentido del recorrido) y $\vec{B}$ (tangente, mismo sentido). Resultado: $\oint\vec{B}\cdot d\vec{l} = \mu_0 I$.

En cada punto $\vec{B}\parallel d\vec{l}$ y $B = \mu_0 I/(2\pi r)$ es constante sobre el círculo:

$$\oint\vec{B}\cdot d\vec{l} = B\oint dl = \frac{\mu_0 I}{2\pi r}\cdot 2\pi r = \mu_0 I.$$

El resultado **no depende del radio** $r$: el $1/r$ del campo se compensa exactamente con el largo $2\pi r$ del camino.

**Caso 2: el mismo círculo recorrido en sentido opuesto.**

> **[Figura]:** Igual que la anterior, pero el círculo se recorre en sentido horario: en cada punto $d\vec{l}$ es antiparalelo a $\vec{B}$. Resultado: $\oint\vec{B}\cdot d\vec{l} = -\mu_0 I$.

Ahora $\vec{B}\cdot d\vec{l} = -B\,dl$ en cada punto, y $\oint\vec{B}\cdot d\vec{l} = -\mu_0 I$.

**Caso 3: curva que no encierra la corriente.**

> **[Figura]:** Corriente $I$ saliendo del papel en el origen. La curva cerrada $abcd$ está formada por: el arco $ab$ de radio $r_1$ (exterior) que barre un ángulo $\theta$ en sentido antihorario; el tramo radial $bc$ hacia adentro; el arco $cd$ de radio $r_2<r_1$ recorrido en sentido horario; y el tramo radial $da$ hacia afuera. En los arcos, $\vec{B}$ es tangente; en los tramos radiales $\vec{B}\perp d\vec{l}$. Resultado: $\oint\vec{B}\cdot d\vec{l} = 0$.

- Tramos radiales $bc$ y $da$: $\vec{B}\perp d\vec{l}$ $\Rightarrow$ aporte nulo.
- Arco exterior $ab$ (a favor de $\vec{B}$): $\dfrac{\mu_0 I}{2\pi r_1}\cdot r_1\theta = \dfrac{\mu_0 I\theta}{2\pi}$.
- Arco interior $cd$ (en contra de $\vec{B}$): $-\dfrac{\mu_0 I}{2\pi r_2}\cdot r_2\theta = -\dfrac{\mu_0 I\theta}{2\pi}$.

$$\oint\vec{B}\cdot d\vec{l} = \frac{\mu_0 I\theta}{2\pi} - \frac{\mu_0 I\theta}{2\pi} = 0.$$

En general, $\vec{B}\cdot d\vec{l} = \dfrac{\mu_0 I}{2\pi}\,d\theta$ para **cualquier** curva en el plano; si la curva encierra la corriente el ángulo total barrido es $2\pi$, y si no la encierra es $0$.

### Enunciado general

> **[Figura]:** Una curva cerrada de forma arbitraria ("plano de la curva") recorrida en sentido antihorario. Dentro de ella atraviesan el plano tres corrientes: $I_1$ y $I_3$ saliendo del papel ($\odot$) e $I_2$ entrando ($\otimes$). En un punto de la curva se dibujan $d\vec{l}$ (tangente) y $\vec{B}$ (con cualquier orientación). Leyenda: $I_{\text{enc}} = I_1 - I_2 + I_3$.

Por superposición, para cualquier curva cerrada $C$ y cualquier distribución de corrientes estacionarias:

$$\boxed{\oint_C\vec{B}\cdot d\vec{l} = \mu_0\,I_{\text{enc}}}$$

donde $I_{\text{enc}}$ es la corriente neta que atraviesa **cualquier** superficie limitada por $C$. Convención de signos (regla de la mano derecha): si los dedos de la mano derecha siguen el sentido de recorrido de la curva, el pulgar indica el sentido positivo de la corriente. En la figura, con recorrido antihorario, las corrientes que salen del papel son positivas: $I_{\text{enc}} = I_1 - I_2 + I_3$.

Observaciones:

- Las corrientes **exteriores** a la curva sí contribuyen al campo $\vec{B}$ en cada punto de la curva, pero su contribución neta a la circulación es cero (Caso 3).
- La ley es siempre válida (para corrientes estacionarias), pero solo **permite despejar** $B$ cuando la simetría permite elegir una curva amperiana en la que $\vec{B}$ es tangente y de magnitud constante (o perpendicular a $d\vec{l}$, o nulo) por tramos. Es la misma lógica que con la ley de Gauss.

## Ley de Ampère (forma diferencial)

Partimos de

$$\oint\vec{B}\cdot d\vec{l} = \mu_0\,I_{\text{enc}}.$$

Si recordamos que la corriente a través de una superficie $S$ es el flujo de la densidad de corriente (Clase 08)

$$I = \int_S\vec{J}\cdot d\vec{S},$$

y mediante el **teorema de Stokes**

$$\oint_C\vec{B}\cdot d\vec{l} = \int_S\left(\nabla\times\vec{B}\right)\cdot d\vec{S},$$

obtenemos

$$\int_S\left(\nabla\times\vec{B}\right)\cdot d\vec{S} = \mu_0\int_S\vec{J}\cdot d\vec{S}.$$

Como esto vale para **toda** superficie $S$, los integrandos deben ser iguales. Finalmente:

$$\boxed{\nabla\times\vec{B} = \mu_0\,\vec{J}}\qquad\text{(ley de Ampère, forma diferencial)}$$

Junto con $\nabla\cdot\vec{B} = 0$, estas son las ecuaciones de la magnetostática. Compárese con la electrostática: $\nabla\cdot\vec{E} = \rho/\varepsilon_0$ y $\nabla\times\vec{E} = 0$. Las fuentes del campo eléctrico estático "divergen"; las del campo magnético "rotan".

## Aplicaciones de la ley de Ampère

La ley de Ampère se utiliza para calcular el campo magnético de distribuciones con alta simetría:

- alambres infinitos / cilindros infinitos;
- toroides;
- solenoides;
- planos infinitos.

> **[Figura]:** Cuatro ilustraciones: (1) un solenoide de cuatro vueltas visto en perspectiva, con las líneas de campo apretadas y casi paralelas en el **interior** y muy separadas en el **exterior**, cerrándose por fuera; alrededor de cada sección de alambre se ven pequeñas líneas circulares ($\odot$ a la izquierda, $\otimes$ a la derecha). (2) Un toroide con su devanado (rojo), radio interior $b$, radio exterior $c$, sección de ancho $a$, un "lazo 1" circular punteado de radio $r$ dentro del núcleo con $\vec{B}$ tangente y un elemento $d\vec{s}$, y un "lazo 2" punteado en un plano perpendicular a la página que rodea un costado del anillo. (3) Un cilindro conductor de radio $R$ con corriente $I$, con un círculo amperiano 1 exterior (radio $r>R$) y uno 2 interior. (4) Una cinta conductora plana de ancho $w$ sobre el eje $x$, con corriente $I$ y un punto $P$ en su mismo plano a distancia $b$ de su borde.

### Alambre cilíndrico con corriente uniforme

**Enunciado.** Un alambre recto largo de radio $R$ porta una corriente estable $I$ que se distribuye uniformemente a través de la sección transversal del alambre. Calcule el campo magnético a una distancia $r$ desde el centro del alambre en las regiones $r<R$ y $r>R$.

> **[Figura]:** Cilindro conductor de radio $R$ (visto en perspectiva, con su sección circular al frente) y corriente $I$ dirigida hacia el lector a lo largo del eje. Dos circunferencias punteadas concéntricas con el eje: la "1", de radio $r>R$, exterior al cilindro, con un elemento $d\vec{s}$ tangente; la "2", de radio $r<R$, dentro del conductor. Ambas se recorren en el mismo sentido (antihorario visto de frente).

**Resolución**

*Idea.* Ley de Ampère con curvas amperianas circulares concéntricas. Es exactamente el análogo de la esfera o cilindro cargado uniformemente resuelto con la ley de Gauss (Clase 03).

*Simetría.* La distribución es invariante ante rotaciones alrededor del eje y ante traslaciones a lo largo de él. Por lo tanto $B$ solo depende de $r$. Además, por Biot-Savart cada filamento de corriente produce un campo azimutal, y $\nabla\cdot\vec{B} = 0$ descarta una componente radial; así $\vec{B} = B(r)\,\hat{\theta}$, con líneas circulares. Sobre un círculo de radio $r$: $\vec{B}\parallel d\vec{l}$ y $B$ constante, luego

$$\oint\vec{B}\cdot d\vec{l} = B(r)\,2\pi r.$$

*Región $r>R$ (curva 1).* La curva encierra toda la corriente: $I_{\text{enc}} = I$.

$$B\,2\pi r = \mu_0 I\quad\Longrightarrow\quad \boxed{B = \frac{\mu_0 I}{2\pi r}\quad(r>R)}$$

*Región $r<R$ (curva 2).* La densidad de corriente es uniforme: $J = \dfrac{I}{\pi R^2}$. La corriente encerrada es la que pasa por el círculo de radio $r$:

$$I_{\text{enc}} = J\,\pi r^2 = I\,\frac{r^2}{R^2}.$$

$$B\,2\pi r = \mu_0 I\frac{r^2}{R^2}\quad\Longrightarrow\quad \boxed{B = \frac{\mu_0 I\,r}{2\pi R^2}\quad(r<R)}$$

El sentido de $\vec{B}$ en ambas regiones está dado por la regla de la mano derecha con el pulgar en la dirección de $I$.

> **[Figura]:** Gráfico de $B$ versus $r$: desde el origen $B$ crece **linealmente**, $B = \dfrac{\mu_0 I}{2\pi}\dfrac{r}{R^2}$, pasando por $\tfrac12\dfrac{\mu_0 I}{2\pi R}$ en $r = R/2$, hasta el máximo $\dfrac{\mu_0 I}{2\pi R}$ en $r=R$; luego decae como $B = \dfrac{\mu_0 I}{2\pi r}$, mostrado hasta $r = 4R$.

*Verificación / interpretación.*

- Continuidad en $r=R$: ambas expresiones dan $\mu_0 I/(2\pi R)$. ✓
- En $r=0$, $B=0$: por simetría, en el eje no hay dirección azimutal privilegiada. ✓
- Fuera del alambre, el campo es el mismo que el de un alambre delgado (Clase 11): la ley de Ampère lo reproduce en una línea, sin integrar Biot-Savart.

### Solenoide ideal

**Enunciado.** Calcule el campo magnético dentro de un solenoide ideal de largo $l$, $N$ vueltas y que lleva una corriente estacionaria $I$.

> **[Figura]:** Corte longitudinal de la parte central de un solenoide largo: arriba, una fila de secciones de alambre con corriente entrando al papel ($\otimes$); abajo, una fila con corriente saliendo ($\odot$). En el interior, líneas de $\vec{B}$ horizontales, paralelas y uniformes, dirigidas hacia la izquierda. La trayectoria de integración es un rectángulo $abcd$: el lado $ab$, de largo $L$, está dentro del solenoide, paralelo al eje y recorrido en el sentido de $\vec{B}$ (de $a$, a la derecha, hacia $b$, a la izquierda); los lados $bc$ y $da$ son perpendiculares al eje y atraviesan el devanado; el lado $cd$ está fuera, donde se indica $B=0$.

**Resolución**

*Idea.* Ley de Ampère con una curva rectangular, aprovechando que en el solenoide ideal (largo $\gg$ radio, vueltas muy juntas) el campo interior es uniforme y paralelo al eje, y el exterior es despreciable.

*Justificación de las hipótesis.* Como se ve en las líneas de campo de un solenoide real, en el interior los campos de las espiras se suman y las líneas son casi paralelas y densas; en el exterior se dispersan en una región muy amplia y el campo es muy débil. En el límite ideal (solenoide infinitamente largo), $\vec{B}_{\text{ext}} = 0$ y $\vec{B}_{\text{int}} = B\,\hat{u}_{\text{eje}}$ uniforme.

*Circulación sobre $abcd$.*

- $ab$ (dentro, paralelo a $\vec{B}$): $\displaystyle\int_a^b\vec{B}\cdot d\vec{l} = BL$.
- $bc$ y $da$: la parte interior es perpendicular a $\vec{B}$ y la exterior está en $B = 0$ $\Rightarrow$ aporte nulo.
- $cd$ (fuera): $B = 0$ $\Rightarrow$ aporte nulo.

$$\oint\vec{B}\cdot d\vec{l} = BL.$$

*Corriente encerrada.* El rectángulo es atravesado por las vueltas comprendidas en el largo $L$. Si $n = N/l$ es el número de vueltas por unidad de longitud, hay $nL$ vueltas, cada una con corriente $I$:

$$I_{\text{enc}} = nLI.$$

*Ley de Ampère:*

$$BL = \mu_0 nLI\quad\Longrightarrow\quad \boxed{B = \mu_0 nI = \frac{\mu_0 NI}{l}}$$

*Dirección.* Regla de la mano derecha para espiras: los dedos según la corriente en las vueltas, el pulgar indica $\vec{B}$ en el interior. En la figura, corriente entrando arriba y saliendo abajo $\Rightarrow$ $\vec{B}$ hacia la izquierda, consistente con el dibujo.

*Verificación / interpretación.*

- El resultado no depende de la posición del lado $ab$ dentro del solenoide: el campo interior es **uniforme**. Si $ab$ se pone fuera, $I_{\text{enc}} = 0$ y se confirma $B_{\text{ext}} = 0$ (consistente).
- Unidades: $(\text{T·m/A})(1/\text{m})\,\text{A} = \text{T}$. ✓
- Ejemplo numérico: $N = 1000$, $l = 0.50\,\text{m}$, $I = 2\,\text{A}$ $\Rightarrow$ $n = 2000\,\text{m}^{-1}$, $B = 4\pi\times10^{-7}\cdot2000\cdot2 = 5.0\times10^{-3}\,\text{T}$.

*Solenoide real (finito).*

> **[Figura]:** Solenoide de largo $4a$ y diámetro $2a$ (radio $a$) con corriente $I$; debajo, el gráfico de $B$ sobre el eje en función de $x$ (de $-4a$ a $4a$). $B$ es máximo en el centro, levemente menor que $\mu_0 nI$; en los extremos ($x=\pm2a$) vale aproximadamente $\tfrac12\mu_0 nI$, y fuera decae a cero hacia $x=\pm4a$.

Que en el extremo el campo sea la mitad se entiende por superposición: un solenoide semi-infinito es "medio" solenoide infinito, y en su boca aporta la mitad del campo.

### Toroide

**Enunciado.** Un dispositivo llamado toroide se usa con frecuencia para crear un campo magnético casi uniforme en algún área cerrada. El dispositivo consiste en un alambre conductor enrollado alrededor de un anillo (un toro) hecho de un material no conductor. Para un toroide que tiene $N$ vueltas de alambre muy juntas una de otra, calcule el campo magnético en la región ocupada por el toro, a una distancia $r$ del centro.

> **[Figura]:** a) Toroide en perspectiva: anillo de sección rectangular con $N$ vueltas de alambre (moradas) enrolladas alrededor del núcleo; la corriente $I$ entra y sale por dos terminales. b) Vista superior en corte: en el borde interior del anillo las secciones de alambre llevan corriente entrando ($\otimes$) y en el borde exterior saliendo ($\odot$). Tres trayectorias circulares concéntricas centradas en $O$: la **trayectoria 1**, de radio menor que el radio interior del anillo; la **trayectoria 2**, de radio $r$ dentro del núcleo (entre ambos bordes), donde se dibuja $\vec{B}$ tangente; y la **trayectoria 3**, de radio mayor que el radio exterior. Leyenda: "El campo magnético está confinado casi por completo en el espacio encerrado por los devanados (en azul)". En la otra vista del toroide se indican radio interior $b$, radio exterior $c$, ancho de la sección $a$, el lazo 1 de radio $r$ y un elemento $d\vec{s}$.

Resultado de la diapositiva:

$$B = \frac{\mu_0 NI}{2\pi r}$$

**Resolución**

*Idea.* Ley de Ampère con círculos concéntricos al toroide.

*Simetría.* El toroide es invariante ante rotaciones alrededor del eje que pasa por $O$ (perpendicular al plano del anillo). Por eso $B$ solo depende de $r$, y las líneas de campo son círculos concéntricos: sobre un círculo de radio $r$, $\vec{B}\parallel d\vec{l}$ y $B$ constante, luego $\oint\vec{B}\cdot d\vec{l} = B\,2\pi r$.

*Trayectoria 2 ($b<r<c$, dentro del núcleo).* El disco limitado por el círculo es atravesado por las $N$ vueltas, cada una por su lado interior (corriente $\otimes$), todas en el mismo sentido: $I_{\text{enc}} = NI$.

$$B\,2\pi r = \mu_0 NI\quad\Longrightarrow\quad \boxed{B = \frac{\mu_0 NI}{2\pi r}\quad(b<r<c)}$$

*Trayectoria 1 ($r<b$).* El círculo no es atravesado por ningún alambre: $I_{\text{enc}} = 0\Rightarrow B = 0$.

*Trayectoria 3 ($r>c$).* Cada vuelta atraviesa el disco dos veces: una entrando (borde interior) y otra saliendo (borde exterior). $I_{\text{enc}} = NI - NI = 0\Rightarrow B = 0$.

*Verificación / interpretación.*

- El campo queda **confinado** en el núcleo, como indica la figura. No es exactamente uniforme: varía como $1/r$, pero si la sección es pequeña ($a = c-b\ll r$), $B$ es casi constante.
- Si el radio medio es muy grande, con $n = N/(2\pi r)$ vueltas por unidad de longitud, $B = \mu_0 nI$: el toroide se comporta como un solenoide "doblado" sin extremos. ✓
- (En un toroide real el devanado avanza también alrededor del anillo, lo que equivale a una espira de una vuelta y produce un pequeño campo exterior; se desprecia en el modelo ideal.)

### Conductor plano (cinta) de ancho $w$

**Enunciado.** Considere un conductor plano de ancho $w$ e infinitamente largo, en el plano $x$-$y$. Éste lleva una corriente $I$ en el sentido del eje $x$, como se muestra en la figura. Encuentre el campo magnético en un punto $P$ en el plano del conductor, a una distancia $b$ de él.

(En el enunciado de las diapositivas la distancia se llama $s$, pero en la figura y en el resultado se llama $b$; usamos $b$.)

> **[Figura]:** Ejes $x$ (hacia el lector, abajo a la izquierda), $y$ (a la derecha) y $z$ (vertical). Una cinta conductora delgada de ancho $w$, infinitamente larga a lo largo del eje $x$, yace en el plano $xy$; la corriente $I$ va en $+\hat{x}$. El punto $P$ está sobre el eje $y$, en el plano de la cinta, a una distancia $b$ del borde más cercano de la cinta.

Resultados de las diapositivas:

$$\vec{B}(P) = \frac{\mu_0 I}{2\pi w}\ln\left(\frac{b+w}{b}\right)\hat{k},\qquad\text{y para } w\ll b:\quad \vec{B}(P)\approx\frac{\mu_0 I}{2\pi b}\,\hat{k}.$$

**Resolución**

*Idea.* La cinta no tiene la simetría suficiente para aplicar la ley de Ampère directamente sobre ella. Pero sí podemos descomponerla en **filamentos** (tiras de ancho infinitesimal), cada uno de los cuales es un alambre recto infinito cuyo campo ya conocemos, $B = \mu_0 I/(2\pi d)$ (obtenido con Biot-Savart en la Clase 11 o con Ampère en esta clase), y luego sumar por superposición.

*Paso 1: coordenadas.* Colocamos la cinta entre $y' = -w$ y $y' = 0$ (su borde más cercano a $P$ en el origen) y el punto en $P = (0, b, 0)$. Un filamento ubicado en $y'$, de ancho $dy'$, lleva la corriente

$$dI = \frac{I}{w}\,dy'\qquad(\text{densidad superficial } K = I/w\ \text{uniforme}).$$

*Paso 2: campo de un filamento.* Su distancia a $P$ es $d = b - y'$, que varía entre $b$ (borde cercano) y $b+w$ (borde lejano). Su campo en $P$:

$$dB = \frac{\mu_0\,dI}{2\pi(b-y')} = \frac{\mu_0 I}{2\pi w}\,\frac{dy'}{b-y'}.$$

*Dirección.* Para un filamento con corriente $+\hat{x}$ y el punto $P$ desplazado en $+\hat{y}$ respecto de él: $d\vec{l}\times\hat{r}\propto\hat{x}\times\hat{y} = \hat{k}$. Todos los filamentos aportan en $+\hat{k}$, así que sumamos magnitudes.

*Paso 3: integrar.*

$$B = \frac{\mu_0 I}{2\pi w}\int_{-w}^{0}\frac{dy'}{b-y'} = \frac{\mu_0 I}{2\pi w}\Big[-\ln(b-y')\Big]_{-w}^{0} = \frac{\mu_0 I}{2\pi w}\left[\ln(b+w) - \ln b\right]$$

$$\boxed{\vec{B}(P) = \frac{\mu_0 I}{2\pi w}\ln\left(\frac{b+w}{b}\right)\hat{k}}$$

*Paso 4: límite $w\ll b$.* Usando $\ln(1+u)\approx u$ para $u\ll1$:

$$\ln\left(\frac{b+w}{b}\right) = \ln\left(1+\frac{w}{b}\right)\approx\frac{w}{b}.$$

Entonces:

$$\vec{B}(P)\approx\frac{\mu_0 I}{2\pi w}\cdot\frac{w}{b}\,\hat{k} = \frac{\mu_0 I}{2\pi b}\,\hat{k}.$$

*Verificación / interpretación.*

- Lejos de la cinta ($b\gg w$) recuperamos el campo de un alambre delgado: vista de lejos, la cinta es un alambre. Esta es la expresión $\vec{B}(P) = \mu_0 I/(2\pi d)$ que aparece anticipada en la primera diapositiva del problema (con $d$ la distancia a la cinta).
- Nota sobre la diapositiva: allí se escribe $\ln(1+w/b)\approx\frac{1}{s}w$; con la notación del problema $s = b$, es decir $\approx w/b$, como se usó arriba.
- Cuando $b\to0$ (punto en el borde), $B\to\infty$ logarítmicamente, consecuencia de modelar la cinta con espesor nulo.
- Unidades: $\mu_0 I/w$ tiene unidades de $\text{T}$ y el logaritmo es adimensional. ✓

### Complemento: lámina infinita de corriente

**Enunciado.** Un plano infinito (el plano $xy$) lleva una corriente superficial uniforme de densidad $\vec{K} = K\hat{x}$ (corriente por unidad de ancho, en $\text{A/m}$). Calcule $\vec{B}$ a ambos lados.

**Resolución**

*Idea.* Ley de Ampère con un rectángulo que atraviesa la lámina. Es el análogo del plano infinito cargado resuelto con Gauss (Clase 03).

*Simetría.* La lámina es la cinta anterior con $w\to\infty$: cada par de filamentos simétricos respecto del punto cancela las componentes normales al plano, así que $\vec{B}$ es **paralelo a la lámina y perpendicular a $\vec{K}$** (dirección $\pm\hat{y}$). No depende de $x$ ni de $y$, y por simetría de reflexión tiene igual magnitud y sentido opuesto a cada lado: $\vec{B} = -B\,\hat{y}$ para $z>0$ y $\vec{B} = +B\,\hat{y}$ para $z<0$ (regla de la mano derecha: $\hat{x}\times\hat{z} = -\hat{y}$ sobre la lámina).

*Curva amperiana.* Rectángulo en el plano $yz$, con lados horizontales de largo $L$ (paralelos a $\hat{y}$) a alturas $+z$ y $-z$, y lados verticales que cruzan la lámina. Los lados verticales son perpendiculares a $\vec{B}$ y no aportan; cada lado horizontal aporta $BL$ (recorriendo el rectángulo de modo que su normal sea $+\hat{x}$):

$$\oint\vec{B}\cdot d\vec{l} = 2BL,\qquad I_{\text{enc}} = KL.$$

$$2BL = \mu_0 KL\quad\Longrightarrow\quad\boxed{B = \frac{\mu_0 K}{2}}$$

*Verificación / interpretación.* El campo es **uniforme** e independiente de la distancia, como el campo eléctrico de un plano infinito ($\sigma/2\varepsilon_0$). Dos láminas paralelas con corrientes opuestas dan $\mu_0 K$ entre ellas y $0$ afuera: es el corte de un solenoide (con $K = nI$ se recupera $B = \mu_0 nI$). ✓

## Ley de Ampère-Maxwell

### Forma diferencial: la ley de Ampère está incompleta

La ley de Ampère en su forma diferencial es:

$$\nabla\times\vec{B} = \mu_0\vec{J}.$$

Si se aplica la divergencia a ambos lados:

$$\nabla\cdot\left(\nabla\times\vec{B}\right) = \mu_0\,\nabla\cdot\vec{J}.$$

Como la divergencia de un rotor es idénticamente nula,

$$\nabla\cdot\left(\nabla\times\vec{B}\right) = 0,$$

la ley de Ampère exige $\nabla\cdot\vec{J} = 0$, lo que solo es cierto para corrientes estacionarias. Pero la ley de conservación de carga (ecuación de continuidad, Clase 08), junto con la ley de Gauss diferencial $\rho = \varepsilon_0\nabla\cdot\vec{E}$ (Clase 04), implica que en general

$$\nabla\cdot\vec{J} = -\frac{\partial\rho}{\partial t} = -\frac{\partial}{\partial t}\left(\varepsilon_0\nabla\cdot\vec{E}\right) = -\nabla\cdot\left(\varepsilon_0\frac{\partial\vec{E}}{\partial t}\right)\neq0.$$

Por lo que la ley de Ampère está incompleta y falta considerar las **corrientes de desplazamiento**. Si reemplazamos $\vec{J}$ por $\vec{J} + \varepsilon_0\,\partial\vec{E}/\partial t$, cuya divergencia sí es siempre nula, obtenemos:

$$\boxed{\nabla\times\vec{B} = \mu_0\vec{J} + \mu_0\varepsilon_0\frac{\partial\vec{E}}{\partial t}}\qquad\text{(ley de Ampère-Maxwell, forma diferencial)}$$

### Forma integral y corriente de desplazamiento

Integrando sobre una superficie $S$ limitada por la curva $C$ y usando Stokes:

$$\boxed{\oint_C\vec{B}\cdot d\vec{l} = \mu_0\left(I_C + \varepsilon_0\frac{d\Phi_E}{dt}\right)_{\text{enc}}}$$

donde $I_C$ es la corriente de conducción y

$$I_D \equiv \varepsilon_0\frac{d\Phi_E}{dt},\qquad \Phi_E = \int_S\vec{E}\cdot d\vec{A},$$

es la **corriente de desplazamiento**. Un campo eléctrico variable en el tiempo genera campo magnético, igual que una corriente.

### Ejemplo: condensador que se carga

> **[Figura]:** Un condensador de placas paralelas circulares se carga con una corriente $i_C$ que entra por el cable izquierdo a la placa $+Q$ y sale por el cable derecho desde la placa $-Q$; entre las placas hay un campo $\vec{E}$ hacia la derecha. Una circunferencia ("trayectoria para la ley de Ampère", con elemento $d\vec{l}$) rodea el cable izquierdo. Dos superficies limitadas por esa misma curva: una **superficie plana** (disco), atravesada por el cable, y una **superficie abombada** que se extiende hasta pasar entre las placas sin cortar ningún cable.

**Resolución (la paradoja y su solución)**

*Idea.* La ley de Ampère dice que $I_{\text{enc}}$ puede calcularse con **cualquier** superficie limitada por la curva; comprobamos si eso se cumple.

1. **Superficie plana:** la atraviesa el cable, $I_{\text{enc}} = i_C$, de modo que $\oint\vec{B}\cdot d\vec{l} = \mu_0 i_C$.
2. **Superficie abombada:** pasa entre las placas, donde no hay conducción: $I_{\text{enc}} = 0$, de modo que $\oint\vec{B}\cdot d\vec{l} = 0$.

Contradicción: la misma circulación no puede valer dos cosas. La solución de Maxwell es que a través de la superficie abombada pasa flujo eléctrico variable. Con placas de área $A$, $E = \dfrac{q}{\varepsilon_0 A}$ (Clase 06), así que $\Phi_E = EA = q/\varepsilon_0$ y

$$I_D = \varepsilon_0\frac{d\Phi_E}{dt} = \frac{dq}{dt} = i_C.$$

La corriente de desplazamiento entre las placas es exactamente igual a la corriente de conducción en los cables: con la ley de Ampère-Maxwell, ambas superficies dan $\mu_0 i_C$. ✓

**Campo magnético entre las placas**

> **[Figura]:** Condensador de placas circulares de radio $R$ (carga $q$ y $-q$), cargándose con corriente $i_C$. Entre las placas, $\vec{E}$ uniforme hacia la derecha. Líneas de $\vec{B}$ circulares, concéntricas con el eje del condensador, tanto dentro de la región entre placas (círculo de radio $r$ que pasa por los puntos $a$ y $b$) como fuera de ella.

*Idea.* Ley de Ampère-Maxwell con un círculo de radio $r$ coaxial, entre las placas; por simetría $\vec{B}$ es azimutal y constante sobre el círculo. No hay corriente de conducción entre las placas.

*Caso $r<R$:* el flujo eléctrico a través del círculo es una fracción $r^2/R^2$ del total, así que $I_{D,\text{enc}} = i_C\,\dfrac{r^2}{R^2}$:

$$B\,2\pi r = \mu_0 i_C\frac{r^2}{R^2}\quad\Longrightarrow\quad\boxed{B = \frac{\mu_0 i_C\,r}{2\pi R^2}\quad(r<R)}$$

*Caso $r>R$:* se encierra todo el flujo, $I_{D,\text{enc}} = i_C$:

$$\boxed{B = \frac{\mu_0 i_C}{2\pi r}\quad(r>R)}$$

*Verificación / interpretación.* Son exactamente las expresiones del alambre cilíndrico con corriente uniforme: la corriente de desplazamiento, uniforme entre las placas, "continúa" a la corriente del cable. Este término es el que, combinado con la ley de Faraday (Clase 13), permite la existencia de ondas electromagnéticas que viajan a $c = 1/\sqrt{\varepsilon_0\mu_0}$.

## Resumen de fórmulas

| Concepto | Fórmula |
|---|---|
| Semicircunferencia de radio $r$ (centro) | $B = \dfrac{\mu_0 I}{4r}$ (ramas rectas colineales no aportan) |
| Ley de Gauss del magnetismo | $\oint\vec{B}\cdot d\vec{A} = 0$, $\ \nabla\cdot\vec{B} = 0$ |
| Ley de Ampère (integral) | $\oint\vec{B}\cdot d\vec{l} = \mu_0 I_{\text{enc}}$ |
| Ley de Ampère (diferencial) | $\nabla\times\vec{B} = \mu_0\vec{J}$ |
| Alambre cilíndrico, corriente uniforme | $B = \dfrac{\mu_0 I r}{2\pi R^2}$ ($r<R$); $\ B = \dfrac{\mu_0 I}{2\pi r}$ ($r>R$) |
| Solenoide ideal | $B = \mu_0 nI = \dfrac{\mu_0 NI}{l}$ (dentro), $0$ fuera |
| Toroide | $B = \dfrac{\mu_0 NI}{2\pi r}$ ($b<r<c$), $0$ fuera del núcleo |
| Cinta de ancho $w$ (en su plano, a distancia $b$) | $B = \dfrac{\mu_0 I}{2\pi w}\ln\left(\dfrac{b+w}{b}\right)$; $\ \approx\dfrac{\mu_0 I}{2\pi b}$ si $w\ll b$ |
| Lámina infinita de corriente | $B = \dfrac{\mu_0 K}{2}$ |
| Ley de Ampère-Maxwell (diferencial) | $\nabla\times\vec{B} = \mu_0\vec{J} + \mu_0\varepsilon_0\dfrac{\partial\vec{E}}{\partial t}$ |
| Ley de Ampère-Maxwell (integral) | $\oint\vec{B}\cdot d\vec{l} = \mu_0\left(I_C + \varepsilon_0\dfrac{d\Phi_E}{dt}\right)$ |
| Corriente de desplazamiento | $I_D = \varepsilon_0\dfrac{d\Phi_E}{dt}$ |
| Entre placas circulares de un condensador | $B = \dfrac{\mu_0 i_C r}{2\pi R^2}$ ($r<R$) |
