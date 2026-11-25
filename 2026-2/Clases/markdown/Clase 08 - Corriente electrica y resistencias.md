# Corriente eléctrica y resistencia

## Problema extra de dipolo

**Problema.** Considere un dipolo de momento dipolar $\vec{p}$ que forma un ángulo $\theta$ con la horizontal. Suponga que existe un campo eléctrico externo uniforme dado por $\vec{E}=E\,\hat{x}$.

a) Calcule la fuerza total y, explícitamente, el torque que se ejerce sobre el dipolo.
b) ¿Qué ocurre si el campo no es uniforme?

> **[Figura]:** Ejes $x$ (horizontal) e $y$ (vertical) con origen $O$ en el centro del dipolo. Líneas de campo $\vec{E}$ horizontales hacia la derecha ($+\hat{x}$). La carga $+q$ está en el extremo del vector $\vec{r}_+$, en el primer cuadrante, formando un ángulo $\theta$ con el eje $x$; la carga $-q$ está en $\vec{r}_-=-\vec{r}_+$, en el tercer cuadrante. Sobre $+q$ actúa $\vec{F}_+$ hacia la derecha y sobre $-q$ actúa $\vec{F}_-$ hacia la izquierda.

**Resolución**

*Idea / qué concepto usar.* Usamos la fuerza sobre una carga puntual en un campo, $\vec{F}=q\vec{E}$ (Clase 02), y la definición de torque respecto del origen, $\vec{\tau}=\vec{r}\times\vec{F}$. El momento dipolar es $\vec{p}=q\vec{d}$, con $\vec{d}$ el vector que va de $-q$ a $+q$.

*a) Fuerza total.* Sea $d$ la separación entre cargas. Entonces
$$\vec{r}_+=\frac{d}{2}\left(\cos\theta\,\hat{x}+\sin\theta\,\hat{y}\right),\qquad \vec{r}_-=-\vec{r}_+ .$$
Las fuerzas son
$$\vec{F}_+=qE\,\hat{x},\qquad \vec{F}_-=-qE\,\hat{x}.$$
Por lo tanto
$$\vec{F}_{tot}=\vec{F}_++\vec{F}_-=qE\,\hat{x}-qE\,\hat{x}=\vec{0}.$$
En un campo uniforme la fuerza neta sobre un dipolo es nula: el centro de masa no se acelera.

*a) Torque.* Respecto del origen:
$$\vec{\tau}=\vec{r}_+\times\vec{F}_++\vec{r}_-\times\vec{F}_-=\vec{r}_+\times(qE\,\hat{x})+(-\vec{r}_+)\times(-qE\,\hat{x})=2\,\vec{r}_+\times(qE\,\hat{x}).$$
Calculando el producto cruz, con $\hat{x}\times\hat{x}=0$ y $\hat{y}\times\hat{x}=-\hat{z}$:
$$2\,\vec{r}_+\times(qE\,\hat{x})=2\cdot\frac{d}{2}\,qE\left(\cos\theta\,\hat{x}\times\hat{x}+\sin\theta\,\hat{y}\times\hat{x}\right)=-qdE\sin\theta\,\hat{z}.$$
Como $p=qd$ y $\vec{p}=p(\cos\theta\,\hat{x}+\sin\theta\,\hat{y})$, el resultado coincide con
$$\vec{p}\times\vec{E}=pE(\cos\theta\,\hat{x}+\sin\theta\,\hat{y})\times\hat{x}=-pE\sin\theta\,\hat{z}.$$
$$\boxed{\vec{F}_{tot}=\vec{0},\qquad \vec{\tau}=\vec{p}\times\vec{E}=-pE\sin\theta\,\hat{z}}$$

*Verificación / interpretación.* El torque apunta en $-\hat{z}$ (sentido horario visto desde $+z$): tiende a hacer girar $\vec{p}$ hacia $\vec{E}$, es decir, a reducir $\theta$. Si $\theta=0$ (alineado) el torque es nulo y el equilibrio es estable; si $\theta=\pi$ también es nulo pero el equilibrio es inestable. Unidades: $[\text{C}\cdot\text{m}\cdot\text{N/C}]=[\text{N}\cdot\text{m}]$. Asociada a este torque está la energía potencial $U=-\vec{p}\cdot\vec{E}=-pE\cos\theta$, mínima para $\theta=0$.

*b) Campo no uniforme.* Si $\vec{E}$ depende de la posición, las cargas sienten campos distintos: $\vec{F}_{tot}=q\left[\vec{E}(\vec{r}_+)-\vec{E}(\vec{r}_-)\right]$. Expandiendo a primer orden en $\vec{d}$,
$$\vec{E}(\vec{r}_+)-\vec{E}(\vec{r}_-)\approx(\vec{d}\cdot\nabla)\vec{E}\quad\Rightarrow\quad \boxed{\vec{F}_{tot}=(\vec{p}\cdot\nabla)\vec{E}=\nabla(\vec{p}\cdot\vec{E})}$$
(la última igualdad vale para campos electrostáticos, $\nabla\times\vec{E}=0$). Además sigue existiendo el torque $\vec{\tau}\approx\vec{p}\times\vec{E}$. Resultado: el dipolo gira hacia la dirección del campo y además es arrastrado hacia las zonas de campo más intenso (por eso un objeto neutro polarizado es atraído por una carga).

## Corriente eléctrica

Una **corriente eléctrica** es todo movimiento de carga de una región a otra.

En situaciones electrostáticas el campo dentro de un conductor es cero y no hay corriente. Sin embargo, en un metal los electrones libres se mueven al azar con rapideces del orden de $10^6\,\text{m/s}$, sin flujo neto. Si se establece un campo $\vec{E}$ dentro del conductor, cada portador siente $\vec{F}=q\vec{E}$; por las colisiones con los iones de la red no se acelera indefinidamente, sino que adquiere un movimiento neto muy lento, la **deriva**, descrito por la velocidad de deriva $\vec{v}_d$ (del orden de $10^{-4}\,\text{m/s}$). La energía que el campo entrega a los portadores se transfiere a la red en las colisiones y calienta el conductor.

> **[Figura]:** Partículas con carga $+$ que atraviesan una superficie transversal de área $A$; las flechas rojas indican su velocidad, perpendicular a la superficie, y una flecha violeta indica el sentido de la corriente $I$, el mismo del movimiento de las cargas positivas.

La corriente se define como la tasa a la cual las cargas atraviesan una cierta área transversal. Si una cantidad de carga $\Delta Q$ pasa a través de una superficie en un intervalo de tiempo $\Delta t$, la **corriente promedio** es
$$I_{prom}=\frac{\Delta Q}{\Delta t}.$$
La unidad SI de corriente es el ampere: $1\,\text{A}=1\,\text{C/s}$.

En el límite $\Delta t\to 0$ se define la **corriente instantánea**:
$$I=\frac{dQ}{dt}.$$

Como el flujo tiene una dirección, se adopta la convención de **corriente convencional**: la dirección de la corriente es aquella en la que se moverían las cargas positivas. En un metal los portadores son electrones (negativos), que se mueven en sentido opuesto a la corriente.

> **[Figura]:** a) Conductor cilíndrico con cargas positivas que derivan con $\vec{v}_d$ hacia la derecha, en la misma dirección de $\vec{E}$; la corriente $I$ apunta a la derecha. b) Mismo conductor con cargas negativas que derivan hacia la izquierda, opuestas a $\vec{E}$; la corriente $I$ sigue apuntando a la derecha. Ambos casos producen la misma corriente.

Observaciones:
- En semiconductores (germanio, silicio) la conducción se debe en parte a electrones y en parte a **huecos** (vacantes que se comportan como cargas positivas). En gases ionizados y soluciones iónicas se mueven tanto electrones como iones positivos.
- **La corriente no es un vector**: aunque se habla de su "dirección", $I$ es un escalar que va siempre a lo largo del conductor, sea recto o curvo. Se indica su sentido con palabras o con un signo respecto de un sentido elegido como positivo.
- Órdenes de magnitud: linterna $0.5$–$1\,\text{A}$; motor de arranque de un automóvil $\sim200\,\text{A}$; $1\,\text{mA}=10^{-3}\,\text{A}$, $1\,\mu\text{A}=10^{-6}\,\text{A}$, $1\,\text{nA}=10^{-9}\,\text{A}$, $1\,\text{pA}=10^{-12}\,\text{A}$.

> **[Figura]:** Circuito simple: una pila (terminales $+$ y $-$) conectada con alambres a una ampolleta; la corriente $I$ circula del terminal $+$ por el circuito externo. Un tramo ampliado del alambre muestra cargas positivas derivando con $\vec{v}_d$ y un cilindro de largo $v_d\,dt$ y sección $A$.

## Modelo microscópico de la corriente

$v_d$ es la **velocidad de deriva** (o de arrastre): la velocidad promedio del portador, ya que este no viaja en línea recta sino que cambia de dirección en cada colisión.

> **[Figura]:** Trayectoria de un electrón dentro de un conductor. Sin campo, se mueve al azar desde $P_1$ hasta $P_2$ en un tiempo $\Delta t$ (trayectoria azul en zigzag). Con campo $\vec{E}$ (trayectoria magenta), el movimiento sigue siendo casi aleatorio, pero termina en $P_2'$, desplazado una distancia $v_d\Delta t$ respecto de $P_2$ en la dirección de la fuerza $\vec{F}=q\vec{E}$. Como $q<0$ para el electrón, la fuerza es opuesta a $\vec{E}$.

Suponga que hay $n$ partículas con carga $q$ en movimiento por unidad de volumen (concentración, en $\text{m}^{-3}$) y que todas derivan con la misma rapidez $v_d$. En un tiempo $dt$ cada partícula avanza
$$dx=v_d\,dt.$$
Las partículas que cruzan la sección $A$ durante $dt$ son las que estaban en el cilindro de volumen $A\,v_d\,dt$; su número es $n A v_d\,dt$. La carga que pasa es
$$dQ=q\,(n\,A\,v_d\,dt),$$
y la corriente
$$I=\frac{dQ}{dt}=n\,q\,A\,v_d .$$

### Densidad de corriente $\vec{J}$

La corriente por unidad de área de la sección transversal es la **densidad de corriente**:
$$J=\frac{I}{A}=nqv_d .$$
Se define además la densidad de corriente vectorial, que incluye la dirección de la deriva:
$$\vec{J}=nq\,\vec{v}_d .$$
$\vec{J}$ y $\vec{v}_d$ tienen la misma dirección para portadores positivos y direcciones opuestas para portadores negativos. En ambos casos $\vec{J}$ apunta en la dirección de la corriente convencional (y de $\vec{E}$). Unidad: $\text{A/m}^2$.

### Ejemplo 1

Un alambre de cobre del número 18 (el calibre que por lo general se utiliza en los cables para lámparas) tiene un diámetro nominal de $1.02\,\text{mm}$. Conduce una corriente constante de $1.67\,\text{A}$ para alimentar una ampolleta de $200\,\text{W}$. La densidad de electrones libres es $8.5\times10^{28}$ electrones por metro cúbico. Determine las magnitudes de:
a) la densidad de corriente;
b) la velocidad de deriva.

**Resolución**

*Idea / qué concepto usar.* Se usan las dos relaciones del modelo microscópico: $J=I/A$ (definición) y $J=n|q|v_d$. Con $I$ y la geometría se obtiene $J$; con $J$ y $n$ se despeja $v_d$. La potencia de la ampolleta no se necesita.

*Área de la sección.* Con $d=1.02\times10^{-3}\,\text{m}$:
$$A=\frac{\pi d^2}{4}=\frac{\pi\,(1.02\times10^{-3}\,\text{m})^2}{4}=8.17\times10^{-7}\,\text{m}^2 .$$

*a) Densidad de corriente.*
$$J=\frac{I}{A}=\frac{1.67\,\text{A}}{8.17\times10^{-7}\,\text{m}^2}=2.04\times10^{6}\,\text{A/m}^2 .$$

*b) Velocidad de deriva.* Despejando de $J=n|q|v_d$, con $|q|=e=1.60\times10^{-19}\,\text{C}$:
$$v_d=\frac{J}{n|q|}=\frac{2.04\times10^{6}\,\text{A/m}^2}{(8.5\times10^{28}\,\text{m}^{-3})(1.60\times10^{-19}\,\text{C})}=1.5\times10^{-4}\,\text{m/s}=0.15\,\text{mm/s}.$$

$$\boxed{J\approx2.04\times10^{6}\,\text{A/m}^2,\qquad v_d\approx1.5\times10^{-4}\,\text{m/s}}$$

*Verificación / interpretación.* Unidades: $\dfrac{\text{A/m}^2}{\text{m}^{-3}\cdot\text{C}}=\dfrac{\text{C/s}}{\text{C}}\cdot\text{m}=\text{m/s}$. A esta rapidez un electrón tarda $1/v_d\approx6700\,\text{s}$ (alrededor de 1 h 50 min) en recorrer $1\,\text{m}$ de alambre. Como la rapidez del movimiento aleatorio es $\sim10^6\,\text{m/s}$, la deriva es unas $10^{10}$ veces más lenta. La ampolleta se enciende de inmediato porque lo que se propaga casi a la velocidad de la luz es el campo eléctrico en el alambre, que pone en movimiento a todos los electrones casi a la vez.

*Pregunta de control.* Si se reemplaza el alambre por uno de calibre 12, con el doble de diámetro, y la corriente es la misma, el área se cuadruplica, $J$ se reduce a la cuarta parte y, como $v_d=J/(n|q|)$, **$v_d$ se reduce a la cuarta parte**.

### Corriente a través de una superficie arbitraria

Si $\vec{J}$ no es uniforme o la superficie no es perpendicular a ella, la corriente total que atraviesa una superficie $S$ es el flujo de $\vec{J}$:
$$I=\iint_S \vec{J}(\vec{x}\,')\cdot d\vec{s}(\vec{x}\,'),$$
donde $\vec{J}(\vec{x}\,')$ es la densidad de corriente en $\text{A/m}^2$. Para $\vec{J}$ uniforme y perpendicular a una sección plana se recupera $I=JA$.

## Continuidad de la carga eléctrica

Considere un volumen $V$ limitado por una superficie cerrada $S$ con normal $d\vec{s}$ hacia afuera. La carga que **entra** en $V$ por unidad de tiempo es menos el flujo saliente:
$$I_{entra}=-\oiint_S \vec{J}(\vec{x}\,')\cdot d\vec{s}(\vec{x}\,').$$
La carga encerrada en un instante dado es
$$Q=\iiint_V \rho(\vec{x}\,')\,d^3x' ,$$
de modo que su tasa de aumento es
$$\frac{dQ}{dt}=\iiint_V \frac{\partial\rho(\vec{x}\,')}{\partial t}\,d^3x' .$$
Como la carga se conserva, solo cambia si entra o sale por $S$: $I_{entra}=dQ/dt$. Aplicando el teorema de la divergencia (Clase 04) al flujo de $\vec{J}$:
$$-\oiint_S \vec{J}\cdot d\vec{s}=-\iiint_V \nabla'\cdot\vec{J}\,d^3x'=\iiint_V\frac{\partial\rho}{\partial t}\,d^3x'\quad\Longrightarrow\quad \iiint_V\left(\nabla'\cdot\vec{J}+\frac{\partial\rho}{\partial t}\right)d^3x'=0 .$$
Como esto vale para cualquier volumen $V$, el integrando debe anularse en todo punto:
$$\boxed{\nabla\cdot\vec{J}+\frac{\partial\rho}{\partial t}=0}$$
Esta es la **ecuación de continuidad** de la carga eléctrica: expresa localmente la conservación de la carga.

*Caso estacionario.* Si $\partial\rho/\partial t=0$ (corrientes estacionarias), $\nabla\cdot\vec{J}=0$: el flujo de $\vec{J}$ por cualquier superficie cerrada es nulo. En particular, la corriente es la misma en todas las secciones de un conductor sin ramificaciones; en los nodos de un circuito esto se convierte en la ley de nodos (Clase 09).

## Ley de Ohm

La densidad de corriente $\vec{J}=nq\vec{v}_d$ depende del campo eléctrico y de las propiedades del material. En general esa dependencia es muy compleja. Sin embargo, en muchos materiales (en especial los metales, a temperatura dada) la densidad de corriente depende linealmente del campo:
$$\vec{J}(\vec{x})=\sigma\,\vec{E}(\vec{x})=\frac{1}{\rho}\,\vec{E}(\vec{x}),$$
donde $\sigma$ es la **conductividad** del material y $\rho=1/\sigma$ su **resistividad**. Esta es la **ley de Ohm diferencial (microscópica)**. Un material que la cumple, con $\rho$ independiente de $E$, se denomina **óhmico** (o lineal); los demás son no óhmicos.

La resistividad se define como $\rho=E/J$. Sus unidades son $\dfrac{\text{V/m}}{\text{A/m}^2}=\text{V}\cdot\text{m/A}=\Omega\cdot\text{m}$, y las de la conductividad, $(\Omega\cdot\text{m})^{-1}$. Un conductor perfecto tendría $\rho=0$ y un aislante perfecto, $\rho\to\infty$. La ley de Ohm es un *modelo idealizado* que describe muy bien a ciertos materiales, pero no a toda la materia.

**Tabla de resistividades a temperatura ambiente ($20\,^\circ\text{C}$)**

| Sustancia | $\rho\ (\Omega\cdot\text{m})$ | Sustancia | $\rho\ (\Omega\cdot\text{m})$ |
|---|---|---|---|
| *Conductores (metales)* | | *Semiconductores* | |
| Plata | $1.47\times10^{-8}$ | Carbono puro (grafito) | $3.5\times10^{-5}$ |
| Cobre | $1.72\times10^{-8}$ | Germanio puro | $0.60$ |
| Oro | $2.44\times10^{-8}$ | Silicio puro | $2300$ |
| Aluminio | $2.75\times10^{-8}$ | *Aislantes* | |
| Tungsteno | $5.25\times10^{-8}$ | Ámbar | $5\times10^{14}$ |
| Acero | $20\times10^{-8}$ | Vidrio | $10^{10}$–$10^{14}$ |
| Plomo | $22\times10^{-8}$ | Lucita | $>10^{13}$ |
| Mercurio | $95\times10^{-8}$ | Mica | $10^{11}$–$10^{15}$ |
| *Aleaciones* | | Cuarzo (fundido) | $75\times10^{16}$ |
| Manganina (84% Cu, 12% Mn, 4% Ni) | $44\times10^{-8}$ | Azufre | $10^{15}$ |
| Constantán (60% Cu, 40% Ni) | $49\times10^{-8}$ | Teflón | $>10^{13}$ |
| Nicromel | $100\times10^{-8}$ | Madera | $10^{8}$–$10^{11}$ |

Las resistividades de los aislantes superan a las de los metales en un factor del orden de $10^{22}$; por eso es fácil confinar corrientes a trayectorias bien definidas (por ejemplo, las pistas de cobre de una placa de circuito impreso). Los semiconductores tienen resistividades intermedias, muy sensibles a la temperatura y a las impurezas.

### De la ley de Ohm microscópica a la macroscópica: resistencia

Considere un segmento de alambre recto de largo $L$ y sección uniforme $A$. Se aplica una diferencia de potencial $\Delta V$ entre sus extremos, lo que crea un campo $E$ (que suponemos uniforme) y una corriente $I$.

> **[Figura]:** Conductor cilíndrico de largo $L$ y sección $A$. El extremo izquierdo está a mayor potencial y el derecho a menor potencial; $V$ es la diferencia de potencial entre ellos. $\vec{E}$, $\vec{J}$ e $I$ apuntan a lo largo del eje, del extremo de mayor al de menor potencial. La densidad de corriente es uniforme en cada sección y el campo es constante en toda la longitud.

Con $E$ uniforme (Clase 05):
$$\Delta V=EL .$$
Por la ley de Ohm diferencial:
$$J=\sigma E=\sigma\frac{\Delta V}{L}.$$
Como $I=JA$:
$$I=\frac{\sigma A}{L}\,\Delta V\quad\Longrightarrow\quad \Delta V=\frac{L}{\sigma A}\,I=R\,I .$$
Así se obtiene la **ley de Ohm macroscópica** y la **resistencia** del conductor:
$$\boxed{V=IR,\qquad R=\frac{V}{I}=\frac{L}{\sigma A}=\frac{\rho L}{A}}$$
con unidad $1\,\Omega=1\,\text{V/A}$.

La corriente siempre va del extremo de mayor potencial al de menor potencial, porque fluye en la dirección de $\vec{E}$ y $\vec{E}$ apunta hacia potenciales decrecientes. La relación $R=V/I$ *define* la resistencia de cualquier conductor; solo cuando $R$ es constante (independiente de $V$) es correcto llamar a $V=IR$ "ley de Ohm".

*Complemento: sección variable.* Si la sección o la resistividad cambian a lo largo del camino de la corriente, se divide el conductor en tramos de largo $dl$ en serie, cada uno con resistencia $dR=\rho\,dl/A(l)$, y se suman:
$$\boxed{R=\int\frac{\rho\,dl}{A(l)}}$$
donde $A(l)$ es el área atravesada por la corriente, perpendicular a ella, a la distancia $l$ del recorrido. Este método se usa en los Ejemplos 2 y 3.

### Ejemplo 2

El cilindro hueco de la figura tiene una longitud $L$ y radios interior y exterior $a$ y $b$. Está hecho de un material cuya resistividad es $\rho$. Se establece una diferencia de potencial entre las superficies interior y exterior del cilindro (cada una de ellas es una superficie equipotencial), de manera que la corriente fluye en forma radial a través del cilindro. ¿Cuál es la resistencia a este flujo radial de corriente?

> **[Figura]:** Cilindro hueco (tubo) de eje común, longitud $L$, radio interior $a$ y radio exterior $b$, de material de resistividad $\rho$. La corriente sale de la superficie interior y fluye radialmente hacia la superficie exterior. Se considera una capa cilíndrica delgada de radio $r$ ($a<r<b$), espesor $dr$ y largo $L$.

**Resolución**

*Idea / qué concepto usar.* La corriente atraviesa capas cilíndricas concéntricas, una después de otra: cada capa de espesor $dr$ es un "resistor" en serie con las demás. Se aplica $R=\int\rho\,dl/A$ con $dl=dr$ y área perpendicular al flujo $A(r)=2\pi rL$ (la superficie lateral de la capa, no la sección del tubo). Como verificación, se rehace con $\vec{J}$, $\vec{E}$ y la definición de potencial.

*Método 1: suma de capas en serie.* Resistencia de la capa de radio $r$:
$$dR=\frac{\rho\,dr}{2\pi rL}.$$
Sumando de $a$ a $b$:
$$R=\int_a^b\frac{\rho\,dr}{2\pi rL}=\frac{\rho}{2\pi L}\int_a^b\frac{dr}{r}=\frac{\rho}{2\pi L}\ln\frac{b}{a}.$$

*Método 2: desde $\vec{J}$ y $\vec{E}$.* Por simetría cilíndrica, $\vec{J}=J(r)\,\hat{r}$. En régimen estacionario la misma corriente $I$ cruza toda superficie cilíndrica de radio $r$ (continuidad):
$$I=J(r)\,2\pi rL\quad\Rightarrow\quad J(r)=\frac{I}{2\pi rL}.$$
Por la ley de Ohm diferencial, $\vec{E}=\rho\vec{J}=\dfrac{\rho I}{2\pi rL}\hat{r}$. La diferencia de potencial entre la superficie interior y la exterior es
$$V=V(a)-V(b)=\int_a^b E\,dr=\frac{\rho I}{2\pi L}\ln\frac{b}{a},$$
de modo que
$$R=\frac{V}{I}=\frac{\rho}{2\pi L}\ln\frac{b}{a}.$$

$$\boxed{R=\frac{\rho}{2\pi L}\ln\frac{b}{a}}$$

*Verificación / interpretación.* Unidades: $\Omega\cdot\text{m}/\text{m}=\Omega$. Si $b\to a$, $R\to0$, lo que tiene sentido porque la corriente atraviesa un espesor nulo. Límite de pared delgada: con $b=a+t$, $t\ll a$, se tiene $\ln(b/a)\approx t/a$ y $R\approx\rho t/(2\pi aL)$, que es $\rho\cdot(\text{largo})/(\text{área})$ con largo $t$ y área $2\pi aL$, como debe ser. $R$ disminuye con $L$, porque un tubo más largo ofrece más área al flujo radial.

## Ejemplo 3

Dos esferas metálicas concéntricas, de radios $a$ y $b$ ($a<b$), están separadas por un material conductor de conductividad $\sigma$ constante.
a) Si las esferas se mantienen a una diferencia de potencial $V$ constante, encuentre la corriente que va de una a la otra.
b) Encuentre la resistencia entre las esferas.

> **[Figura]:** Dos circunferencias concéntricas: la interior de radio $a$ y la exterior de radio $b$. El espacio $a<r<b$ está lleno del material de conductividad $\sigma$. La geometría es la misma del capacitor esférico (Clase 06): corteza interior con carga $+Q$ y exterior con $-Q$, superficie gaussiana esférica de radio $r$ entre ambas.

**Resolución**

*Idea / qué concepto usar.* Igual que en el capacitor esférico (Clase 06): por simetría esférica, el campo entre las esferas se obtiene con la ley de Gauss (Clase 03) y la diferencia de potencial con $\phi_b-\phi_a=-\int_a^b\vec{E}\cdot d\vec{l}$ (Clase 05). Luego $\vec{J}=\sigma\vec{E}$ e $I=\oint\vec{J}\cdot d\vec{A}$. La carga $Q$ es auxiliar y se elimina usando $V$.

*a) Corriente.* Sea $V=\phi(a)-\phi(b)$. Con una superficie gaussiana esférica de radio $r$, $a<r<b$:
$$E\cdot4\pi r^2=\frac{Q}{\epsilon_0}\quad\Rightarrow\quad \vec{E}=\frac{Q}{4\pi\epsilon_0}\frac{1}{r^2}\hat{r},\qquad a<r<b.$$
Diferencia de potencial:
$$\phi_b-\phi_a=-\int_a^b E\,dr\quad\Rightarrow\quad V=\frac{Q}{4\pi\epsilon_0}\left[\frac{1}{a}-\frac{1}{b}\right].$$
Despejando $Q$:
$$Q=\frac{4\pi\epsilon_0 V}{\dfrac{1}{a}-\dfrac{1}{b}}.$$
Sustituyendo en el campo:
$$\vec{E}=\frac{V}{\dfrac{1}{a}-\dfrac{1}{b}}\cdot\frac{1}{r^2}\hat{r}=\frac{V\,ab}{b-a}\cdot\frac{1}{r^2}\hat{r}.$$
(El resultado no depende de $\epsilon_0$ ni de $Q$: lo que fija el campo es la diferencia de potencial impuesta.)

Densidad de corriente:
$$\vec{J}=\sigma\vec{E}=\frac{\sigma V ab}{b-a}\frac{1}{r^2}\hat{r}.$$
Corriente a través de una esfera de radio $r$, con $\vec{J}$ paralelo a $d\vec{A}$ y de módulo constante sobre ella:
$$I=\oint\vec{J}\cdot d\vec{A}=4\pi r^2 J=\frac{4\pi\sigma V ab}{b-a}.$$
$$\boxed{I=\frac{4\pi\sigma\,ab}{b-a}\,V}$$
La corriente no depende de $r$, como exige la ecuación de continuidad en régimen estacionario ($\nabla\cdot\vec{J}=0$).

*b) Resistencia.* Con $V=RI$:
$$R=\frac{V}{I}=\frac{b-a}{4\pi\sigma ab}=\frac{1}{4\pi\sigma}\left[\frac{1}{a}-\frac{1}{b}\right].$$

*Alternativamente:* capas esféricas en serie, con $dl=dr$ y $A=4\pi r^2$:
$$dR=\frac{1}{\sigma}\frac{dr}{4\pi r^2}\quad\Rightarrow\quad R=\frac{1}{4\pi\sigma}\int_a^b\frac{dr}{r^2}=\frac{1}{4\pi\sigma}\left[\frac{1}{a}-\frac{1}{b}\right].$$

$$\boxed{R=\frac{1}{4\pi\sigma}\left(\frac{1}{a}-\frac{1}{b}\right)=\frac{b-a}{4\pi\sigma ab}}$$

*Verificación / interpretación.* Unidades: $\dfrac{1}{(\Omega\cdot\text{m})^{-1}\cdot\text{m}}=\Omega$. Si $b\to\infty$, $R\to1/(4\pi\sigma a)$ (resistencia de un electrodo esférico enterrado en un medio infinito), que es finita. Cáscara delgada, $b=a+t$: $R\approx t/(4\pi\sigma a^2)=\rho t/A$ con $A=4\pi a^2$. Notar la analogía con el capacitor esférico, $C=4\pi\epsilon_0 ab/(b-a)$: se cumple $RC=\epsilon_0/\sigma$, una relación general para electrodos que tienen la misma geometría.

## Dependencia de la resistividad con la temperatura

La mayoría de los metales con buena conductividad (baja resistividad) son óhmicos; nos concentraremos en ellos. Recordemos que
$$\rho=\frac{1}{\sigma}.$$
La resistividad depende también de la temperatura. En un rango moderado se aproxima linealmente:
$$\boxed{\rho(T)=\rho_0\left[1+\alpha\,(T-T_0)\right]}$$
donde $\rho_0$ es la resistividad a la temperatura de referencia $T_0$ (típicamente $20\,^\circ\text{C}$) y $\alpha$ es el **coeficiente de temperatura de la resistividad**, en $(^\circ\text{C})^{-1}$ o $\text{K}^{-1}$.

- En los metales $\alpha>0$: al aumentar $T$, los iones vibran más, aumentan las colisiones y $\rho$ crece.
- En los semiconductores $\alpha<0$: al aumentar $T$ aumenta mucho la concentración de portadores y $\rho$ disminuye. Por ejemplo, si se reduce la temperatura de un semiconductor manteniendo $\vec{E}$ constante, $\rho$ aumenta y la densidad de corriente $J=E/\rho$ **disminuye**.
- Como $R=\rho L/A$ y la dilatación térmica es despreciable frente a este efecto, la resistencia sigue la misma ley: $R(T)=R_0[1+\alpha(T-T_0)]$.

## Resistencia equivalente

Cuando varios resistores se conectan en secuencia, con una sola trayectoria de corriente entre dos puntos, se dice que están conectados **en serie**. Los resistores están conectados **en paralelo** entre los puntos $a$ y $b$ cuando cada resistor ofrece una trayectoria alternativa entre esos puntos.

> **[Figura]:** Cuatro formas de conectar tres resistores entre los puntos $a$ y $b$, con la corriente $I$ entrando por $a$ y saliendo por $b$:
> a) $R_1$, $R_2$ y $R_3$ en serie: $a$–$R_1$–$x$–$R_2$–$y$–$R_3$–$b$.
> b) $R_1$, $R_2$ y $R_3$ en paralelo: los tres conectados directamente entre los nodos $a$ y $b$.
> c) $R_1$ en serie con la combinación en paralelo de $R_2$ y $R_3$: $a$–$R_1$–nodo, luego $R_2$ y $R_3$ en ramas paralelas hasta $b$.
> d) $R_1$ en paralelo con la combinación en serie de $R_2$ y $R_3$: rama superior $R_2$–$R_3$ y rama inferior $R_1$, ambas entre $a$ y $b$.

Para cualquier combinación de resistores siempre es posible encontrar un resistor único que podría reemplazarla y dar la misma corriente y diferencia de potencial totales. Su resistencia se llama **resistencia equivalente**:
$$V_{ab}=I\,R_{eq}\qquad\text{o}\qquad R_{eq}=\frac{V_{ab}}{I}.$$
Para calcularla se supone una diferencia de potencial $V_{ab}$ aplicada a la red, se calcula la corriente $I$ que entra por $a$ y se obtiene el cociente.

### Resistencias en serie (demostración)

Si los resistores están en serie (figura a), la corriente $I$ es la misma en todos ellos, porque la carga no se acumula ni "se gasta" en régimen estacionario (continuidad). Aplicando la ley de Ohm a cada uno:
$$V_{ax}=IR_1,\qquad V_{xy}=IR_2,\qquad V_{yb}=IR_3 .$$
Las diferencias de potencial individuales no tienen por qué ser iguales. La diferencia total es la suma, porque el potencial es una función de punto:
$$V_{ab}=V_{ax}+V_{xy}+V_{yb}=I(R_1+R_2+R_3)\quad\Rightarrow\quad \frac{V_{ab}}{I}=R_1+R_2+R_3=R_{eq}.$$
(En la diapositiva original aparece por error "$R_1+R_2+R_2$"; el término correcto es $R_3$.) En general, para cualquier número de resistores en serie:
$$\boxed{R_{eq}=\sum_i R_i}$$
$R_{eq}$ es mayor que cualquiera de las resistencias individuales.

### Resistencias en paralelo (demostración)

Si los resistores están en paralelo (figura b), la corriente en cada uno no tiene por qué ser la misma, pero la diferencia de potencial entre sus terminales sí lo es, e igual a $V_{ab}$, porque todos están conectados a los mismos dos nodos:
$$I_1=\frac{V_{ab}}{R_1},\qquad I_2=\frac{V_{ab}}{R_2},\qquad I_3=\frac{V_{ab}}{R_3}.$$
Por conservación de la carga en el nodo $a$, la corriente total se reparte entre las ramas:
$$I=I_1+I_2+I_3=V_{ab}\left(\frac{1}{R_1}+\frac{1}{R_2}+\frac{1}{R_3}\right)\quad\Rightarrow\quad \frac{I}{V_{ab}}=\frac{1}{R_1}+\frac{1}{R_2}+\frac{1}{R_3}=\frac{1}{R_{eq}}.$$
Para cualquier número de resistores en paralelo, el recíproco de la resistencia equivalente es la suma de los recíprocos:
$$\boxed{\frac{1}{R_{eq}}=\sum_i\frac{1}{R_i}}$$
$R_{eq}$ es menor que cualquiera de las resistencias individuales. Para dos resistores, $R_{eq}=\dfrac{R_1R_2}{R_1+R_2}$, y como $V_{ab}=I_1R_1=I_2R_2$:
$$\frac{I_1}{I_2}=\frac{R_2}{R_1},$$
es decir, las corrientes en dos resistores en paralelo son inversamente proporcionales a sus resistencias: por la rama de menor resistencia circula más corriente.

*Estrategia para resolver redes de resistores.* (1) Dibujar la red. (2) Identificar grupos que estén claramente en serie (misma corriente, un solo camino) o en paralelo (mismos dos nodos). (3) Reemplazar cada grupo por su equivalente y repetir hasta llegar a un solo resistor. (4) Para hallar corrientes y voltajes, recorrer el camino inverso: en serie la corriente es común y los voltajes se suman; en paralelo el voltaje es común y las corrientes se suman. (5) Verificar: en serie $R_{eq}$ es mayor que cada resistor y en paralelo es menor.

### Ejemplo: red de resistores

Calcule la resistencia equivalente de la red que se ilustra en la figura y obtenga la corriente en cada resistor. La fuente de fem tiene resistencia interna despreciable.

> **[Figura] (etapa a, circuito original):** Fuente de fem $\mathcal{E}=18\,\text{V}$, $r=0$, en la rama superior, con el terminal $+$ a la izquierda. Su terminal izquierdo baja hasta el punto $a$. Entre $a$ y $c$ hay un resistor de $4\,\Omega$. Entre $c$ y $b$ hay dos resistores en paralelo: $6\,\Omega$ en la rama superior y $3\,\Omega$ en la rama inferior. El punto $b$ sube y se conecta al terminal derecho de la fuente, cerrando el circuito.
> Etapas siguientes de la figura: b) el paralelo $6\,\Omega\parallel3\,\Omega$ se reemplaza por $2\,\Omega$ entre $c$ y $b$, en serie con $4\,\Omega$; c) $4\,\Omega+2\,\Omega=6\,\Omega$ entre $a$ y $b$; d) $18\,\text{V}$ sobre $6\,\Omega$ con corriente $3\,\text{A}$; e) de vuelta: $4\,\Omega$ con $12\,\text{V}$ y $2\,\Omega$ con $6\,\text{V}$, ambos con $3\,\text{A}$; f) en el circuito original, $3\,\text{A}$ por el resistor de $4\,\Omega$ ($12\,\text{V}$), $6\,\text{V}$ entre $c$ y $b$, $1\,\text{A}$ por el de $6\,\Omega$ y $2\,\text{A}$ por el de $3\,\Omega$.

**Resolución**

*Idea / qué concepto usar.* Es una combinación tipo "c)": un resistor en serie con un paralelo. Se reduce con las reglas de serie y paralelo recién demostradas, se usa $V=IR$ (ley de Ohm macroscópica) para la corriente total y luego se reconstruyen voltajes y corrientes. La fuente ideal fija $V_{ab}=18\,\text{V}$ entre $a$ y $b$.

*Paso 1: paralelo entre $c$ y $b$.* El resistor de $6\,\Omega$ y el de $3\,\Omega$ conectan ambos los nodos $c$ y $b$, así que están en paralelo:
$$\frac{1}{R_{cb}}=\frac{1}{6\,\Omega}+\frac{1}{3\,\Omega}=\frac{1+2}{6\,\Omega}=\frac{1}{2\,\Omega}\quad\Rightarrow\quad R_{cb}=2\,\Omega .$$

*Paso 2: serie entre $a$ y $b$.* El de $4\,\Omega$ y el equivalente de $2\,\Omega$ son recorridos por la misma corriente:
$$R_{eq}=4\,\Omega+2\,\Omega=6\,\Omega .$$

*Paso 3: corriente total.*
$$I=\frac{\mathcal{E}}{R_{eq}}=\frac{18\,\text{V}}{6\,\Omega}=3\,\text{A}.$$
Esta corriente pasa por la fuente y por el resistor de $4\,\Omega$.

*Paso 4: voltajes.*
$$V_{ac}=I\cdot4\,\Omega=12\,\text{V},\qquad V_{cb}=I\cdot2\,\Omega=6\,\text{V}.$$
Comprobación: $12\,\text{V}+6\,\text{V}=18\,\text{V}=\mathcal{E}$.

*Paso 5: corrientes en el paralelo.* Ambos resistores tienen $V_{cb}=6\,\text{V}$:
$$I_6=\frac{6\,\text{V}}{6\,\Omega}=1\,\text{A},\qquad I_3=\frac{6\,\text{V}}{3\,\Omega}=2\,\text{A}.$$

$$\boxed{R_{eq}=6\,\Omega;\quad I_{4\Omega}=3\,\text{A},\quad I_{6\Omega}=1\,\text{A},\quad I_{3\Omega}=2\,\text{A}}$$

*Verificación / interpretación.* En el nodo $c$: $I_6+I_3=1\,\text{A}+2\,\text{A}=3\,\text{A}=I$, de modo que la carga se conserva. Las corrientes del paralelo cumplen $I_6/I_3=3/6=1/2$, inversamente proporcionales a las resistencias. $R_{cb}=2\,\Omega$ es menor que $3\,\Omega$ (la menor del paralelo) y $R_{eq}=6\,\Omega$ es mayor que $4\,\Omega$, como deben ser.

## Resumen de fórmulas

| Concepto | Fórmula |
|---|---|
| Corriente promedio | $I_{prom}=\dfrac{\Delta Q}{\Delta t}$ |
| Corriente instantánea | $I=\dfrac{dQ}{dt}$, $\quad1\,\text{A}=1\,\text{C/s}$ |
| Modelo microscópico | $I=nqAv_d$ |
| Densidad de corriente | $\vec{J}=nq\vec{v}_d$, $\quad J=I/A$ |
| Corriente por una superficie | $I=\displaystyle\iint_S\vec{J}\cdot d\vec{s}$ |
| Ecuación de continuidad | $\nabla\cdot\vec{J}+\dfrac{\partial\rho}{\partial t}=0$ (estacionario: $\nabla\cdot\vec{J}=0$) |
| Ley de Ohm microscópica | $\vec{J}=\sigma\vec{E}=\vec{E}/\rho$, $\quad\rho=1/\sigma$ |
| Ley de Ohm macroscópica | $V=IR$, $\quad1\,\Omega=1\,\text{V/A}$ |
| Resistencia de un conductor uniforme | $R=\dfrac{\rho L}{A}=\dfrac{L}{\sigma A}$ |
| Resistencia con sección variable | $R=\displaystyle\int\frac{\rho\,dl}{A(l)}$ |
| Cilindro hueco, flujo radial | $R=\dfrac{\rho}{2\pi L}\ln\dfrac{b}{a}$ |
| Esferas concéntricas | $R=\dfrac{1}{4\pi\sigma}\left(\dfrac{1}{a}-\dfrac{1}{b}\right)$ |
| Dependencia térmica | $\rho(T)=\rho_0[1+\alpha(T-T_0)]$ |
| Resistencia equivalente | $R_{eq}=V_{ab}/I$ |
| Serie | $R_{eq}=\sum_i R_i$ (misma corriente) |
| Paralelo | $\dfrac{1}{R_{eq}}=\sum_i\dfrac{1}{R_i}$ (mismo voltaje); $\dfrac{I_1}{I_2}=\dfrac{R_2}{R_1}$ |
| Dipolo en campo uniforme | $\vec{F}=0$, $\quad\vec{\tau}=\vec{p}\times\vec{E}$, $\quad U=-\vec{p}\cdot\vec{E}$ |
| Dipolo en campo no uniforme | $\vec{F}=\nabla(\vec{p}\cdot\vec{E})$ |
