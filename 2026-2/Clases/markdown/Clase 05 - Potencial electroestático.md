# Potencial electrostático

Electricidad y Magnetismo — FIS1533

## Trabajo realizado por el campo eléctrico

Se quiere mover una carga de prueba $q_0$ dentro de un campo eléctrico $\vec{E}(\vec{x})$. La fuerza que el campo ejerce sobre ella es $\vec{F}=q_0\vec{E}$, de modo que el trabajo realizado por el campo eléctrico al llevarla desde $a$ hasta $b$ es

$$W_{a\to b}=\int_a^b \left(q_0\,\vec{E}(\vec{x})\right)\cdot d\vec{l}.$$

> **[Figura]:** Una carga puntual positiva $q$ en el origen emite líneas de campo radiales hacia afuera. La carga de prueba $q_0$ se desplaza de $a$ (a distancia $r_a$ de $q$) a $b$ (a distancia $r_b$) por una trayectoria arbitraria (curva discontinua). En un punto intermedio a distancia $r$ se muestran $\vec{F}$ (radial, hacia afuera), el desplazamiento $d\vec{l}$ tangente a la trayectoria, el ángulo $\phi$ entre ambos y su proyección radial $dr=dl\cos\phi$.

Como $\vec{E}\cdot d\vec{l}=E\,dl\cos\phi=E\,dr$ para un campo radial, el trabajo depende solo de $r_a$ y $r_b$, no del camino:

$$W_{a\to b}=\int_{r_a}^{r_b}\frac{kq\,q_0}{r^2}\,dr=kq\,q_0\left(\frac{1}{r_a}-\frac{1}{r_b}\right).$$

Por superposición, esto vale para cualquier distribución estática de cargas: **el campo electrostático es conservativo**. Por lo tanto se puede definir una energía potencial $U$ tal que

$$dU=-dW \qquad\Longrightarrow\qquad \Delta U=U_b-U_a=-q_0\int_a^b \vec{E}(\vec{x})\cdot d\vec{l}.$$

## Energía potencial de una carga puntual

La energía potencial de una carga de prueba $q_0$ en el campo de una carga puntual $q$ (tomando $U=0$ cuando $r\to\infty$) es

$$U=\frac{1}{4\pi\varepsilon_0}\,\frac{q_0\,q}{r}.$$

> **[Figura]:** Dos gráficos de $U$ versus $r$.
> - Cargas de igual signo ($q$ y $q_0$ ambas positivas o ambas negativas): $U>0$; cuando $r\to0$, $U\to+\infty$; cuando $r\to\infty$, $U\to0$. La curva es una hipérbola positiva decreciente (repulsión: hay que hacer trabajo para acercarlas).
> - Cargas de signo opuesto: $U<0$; cuando $r\to0$, $U\to-\infty$; cuando $r\to\infty$, $U\to0$. La curva es una hipérbola negativa creciente (atracción: el sistema libera energía al acercarse).

## Energía potencial de un sistema de cargas puntuales

> **[Figura]:** Carga de prueba $q_0$ en el punto $a$, con tres cargas $q_1,q_2,q_3$ a distancias $r_1,r_2,r_3$ de $a$.

La energía potencial de $q_0$ en presencia de varias cargas es la suma (escalar) de las contribuciones:

$$U=\frac{q_0}{4\pi\varepsilon_0}\sum_i\frac{q_i}{r_i}.$$

Para la energía de **todo el arreglo** (el trabajo necesario para traer todas las cargas desde el infinito) se suma sobre cada par una sola vez:

$$U=\frac{1}{4\pi\varepsilon_0}\sum_{i<j}\frac{q_i\,q_j}{r_{ij}}=k\sum_{i<j}\frac{q_iq_j}{r_{ij}}.$$

La condición $i<j$ evita contar dos veces el mismo par (el par $1$–$2$ es el mismo que el $2$–$1$).

## Potencial eléctrico

Es útil definir el **potencial eléctrico** como la energía potencial por unidad de carga:

$$\Delta V=V_B-V_A=\frac{\Delta U}{q_0}=-\int_A^B \vec{E}(\vec{x})\cdot d\vec{l}.$$

- Su unidad en el SI es el J/C = volt (V). De aquí que el campo también se exprese en V/m (1 N/C = 1 V/m).
- Como la energía potencial es escalar, el potencial eléctrico también es una cantidad **escalar**.
- Solo las diferencias de potencial tienen significado físico; el cero se elige por conveniencia (usualmente $V(\infty)=0$, o la "tierra" de un circuito).
- El campo eléctrico apunta en la dirección en que $V$ **disminuye**.

### El electrón volt

El **electrón volt** (eV) es la energía cinética que gana un electrón al acelerarse a través de una diferencia de potencial de 1 V. Como $1\,\text{V}=1\,\text{J/C}$ y $e=1.60\times10^{-19}\,\text{C}$:

$$1\ \text{eV}=1.60\times10^{-19}\,\text{C}\cdot\text{V}=1.60\times10^{-19}\,\text{J}.$$

Los electrones en los átomos tienen energías de decenas de eV; los rayos X, miles de eV; los rayos gamma nucleares, millones de eV.

**Pregunta rápida.** Un electrón inicialmente en reposo se acelera a través de una diferencia de potencial de $+1$ V, obteniendo energía cinética $EC_e$; un protón, también en reposo, se acelera a través de $-1$ V, obteniendo $EC_p$. ¿Qué relación se cumple? a) $EC_e=EC_p$; b) $EC_e<EC_p$; c) $EC_e>EC_p$; d) no se puede determinar.

**Resolución.** Por conservación de energía, $\Delta K=-\Delta U=-q\,\Delta V$. Electrón: $-(-e)(+1\,\text{V})=+1$ eV. Protón: $-(+e)(-1\,\text{V})=+1$ eV. Ambos ganan 1 eV, sin importar su masa.

$$\boxed{\text{a) } EC_e=EC_p=1\ \text{eV}}$$

*Interpretación:* la masa determina la rapidez final, no la energía ganada.

## Principio de superposición

El potencial eléctrico de dos o más cargas se obtiene aplicando el principio de superposición: **el potencial eléctrico total en un punto $P$ debido a varias cargas puntuales es la suma algebraica de los potenciales debidos a cada carga individual**. A diferencia del campo (suma vectorial), aquí se suman escalares, lo que simplifica mucho los cálculos.

$$V_P=k\sum_i\frac{q_i}{r_i}.$$

## Potencial eléctrico debido a cargas puntuales

Recordemos que el campo de una carga puntual es $E=\dfrac{kq}{r^2}$ (radial). Si el desplazamiento es desde el infinito hasta la posición $r$:

$$V(r)-V(\infty)=-\int_\infty^r\frac{kq}{r'^2}\,dr'=kq\left[\frac{1}{r'}\right]_\infty^r=\frac{kq}{r}\quad\Longrightarrow\quad V=\frac{kq}{r}.$$

$V$ es el trabajo por unidad de carga que un agente externo debe hacer para traer una carga de prueba positiva desde el infinito hasta $r$. Disminuye como $1/r$, mientras que $E$ disminuye como $1/r^2$.

> **[Figura]:** Gráfico de $E$ (V/m) y $V$ (V) versus $r$ (m, de 0 a 6) para una carga puntual de $1.11\times10^{-10}$ C. Ambas curvas decrecen; la de $E=kq/r^2$ cae más rápido que la de $V=kq/r$.

**Signo de la carga y energía potencial.** A diferencia de la gravedad (un solo tipo de masa, siempre atractiva), en electrostática el signo de la carga importa:

> **[Figura]:** Placas paralelas, la superior positiva y la inferior negativa; campo $\vec E$ apuntando hacia abajo. Una carga negativa entre ellas siente la fuerza $q\vec E$ hacia arriba. El punto $A$ está abajo y el punto $B$ arriba.

Como $\Delta U=q\,\Delta V$ y el potencial aumenta al moverse en contra de $\vec E$ ($V_B>V_A$):

- una carga **positiva** que va de $A$ a $B$ (contra el campo) **gana** energía potencial: un agente externo hace trabajo contra $q\vec E$;
- una carga **negativa** que hace el mismo recorrido **pierde** energía potencial, porque el trabajo lo hace el propio campo.

El trabajo contra la fuerza eléctrica depende solo del desplazamiento efectivo a lo largo de $\vec E$ (por ejemplo, $L\sin\theta-d$ en la figura del libro) y no de la trayectoria, lo que confirma de nuevo que el campo es conservativo.

**Ejercicio complementario.** En un tubo de televisión los electrones se aceleran desde el reposo a través de una diferencia de potencial de $2.00\times10^4$ V, desde el cátodo hasta la pantalla (ánodo), a 25.0 cm de distancia. a) ¿Con qué rapidez chocan con la pantalla (sin efectos relativistas)? b) ¿Cuál es la magnitud del campo eléctrico, suponiéndolo uniforme? Respuestas: a) $8.38\times10^7$ m/s; b) $8.00\times10^4$ V/m.

**Resolución**

*Idea:* conservación de energía con $\Delta U=q\Delta V$; para campo uniforme, $\Delta V=Ed$.

a) El electrón ($q=-e$) va de menor a mayor potencial, $\Delta V=+2.00\times10^4$ V:

$$\Delta K=-q\Delta V=e\,\Delta V\;\Rightarrow\;\tfrac12 m v^2=e\,\Delta V\;\Rightarrow\; v=\sqrt{\frac{2e\Delta V}{m}}=\sqrt{\frac{2(1.60\times10^{-19})(2.00\times10^4)}{9.11\times10^{-31}}}.$$

b) $E=\dfrac{\Delta V}{d}=\dfrac{2.00\times10^4\,\text{V}}{0.250\,\text{m}}$.

$$\boxed{v\approx8.38\times10^{7}\ \text{m/s},\qquad E=8.00\times10^{4}\ \text{V/m}}$$

*Verificación:* $v\approx0.28c$, por lo que la aproximación no relativista es aceptable; las unidades $\sqrt{\text{J/kg}}=\text{m/s}$ y V/m son correctas. Coincide con las respuestas dadas.

## Potencial eléctrico debido a una distribución continua de carga

Cuando la carga está distribuida de forma continua a lo largo de una línea, sobre una superficie o en un volumen, se divide en elementos $dq$ (cada uno se trata como carga puntual) y se integra:

$$V(\vec{r})=\frac{1}{4\pi\varepsilon_0}\int\frac{dq}{|\vec{r}-\vec{r}\,'|},\qquad dq=\lambda\,dl,\ \ \sigma\,dA,\ \ \rho\,dV.$$

Esta expresión supone $V(\infty)=0$, válido solo si la distribución es finita. Otra vía es calcular primero $\vec{E}$ (por ejemplo con Gauss) y luego $V_B-V_A=-\int_A^B\vec{E}\cdot d\vec{l}$.

### Complemento: línea infinita de carga

Fuera de una línea recta muy larga con densidad $\lambda$, $E_r=\dfrac{\lambda}{2\pi\varepsilon_0 r}$ (Clase 03, Gauss). Entonces

$$V_a-V_b=\int_{r_a}^{r_b}E_r\,dr=\frac{\lambda}{2\pi\varepsilon_0}\ln\frac{r_b}{r_a}.$$

Si se intenta poner $V_b=0$ en $r_b\to\infty$, resulta $V_a=\infty$: como la carga se extiende al infinito, no se puede usar el infinito como referencia. Se fija $V=0$ en una distancia arbitraria $r_0$:

$$V=\frac{\lambda}{2\pi\varepsilon_0}\ln\frac{r_0}{r}.$$

> **[Figura]:** a) Alambre largo con carga positiva y $E_r$ radial a distancia $r$. b) Cilindro conductor largo de radio $R$ con carga positiva en su superficie; $E_r$ en un punto a distancia $r>R$ del eje.

Para un **cilindro conductor** de radio $R$ con carga $\lambda$ por unidad de largo, eligiendo $r_0=R$ ($V=0$ en la superficie): $V=\dfrac{\lambda}{2\pi\varepsilon_0}\ln\dfrac{R}{r}$ para $r\ge R$; en el interior $\vec{E}=0$ y $V=0$ (igual que en la superficie). Si $\lambda>0$, $V$ disminuye al aumentar $r$, es decir, en la dirección de $\vec{E}$.

### Complemento: disco uniformemente cargado (sobre su eje)

Disco de radio $R$ y densidad $\sigma$; punto $P$ a distancia $x$ sobre el eje. Se divide el disco en anillos de radio $r'$ y ancho $dr'$: $dq=\sigma\,2\pi r'\,dr'$, todos a distancia $\sqrt{x^2+r'^2}$ de $P$:

$$V=\frac{1}{4\pi\varepsilon_0}\int_0^R\frac{\sigma\,2\pi r'\,dr'}{\sqrt{x^2+r'^2}}=\frac{\sigma}{2\varepsilon_0}\left[\sqrt{x^2+r'^2}\right]_0^R=\frac{\sigma}{2\varepsilon_0}\left(\sqrt{x^2+R^2}-|x|\right).$$

Verificación: $E_x=-\dfrac{dV}{dx}=\dfrac{\sigma}{2\varepsilon_0}\left(1-\dfrac{x}{\sqrt{x^2+R^2}}\right)$ para $x>0$, el resultado de Clase 03. Para $x\gg R$: $\sqrt{x^2+R^2}\approx x+\frac{R^2}{2x}$, luego $V\approx\dfrac{\sigma\pi R^2}{4\pi\varepsilon_0 x}=\dfrac{kQ}{x}$ (carga puntual).

### Complemento: esferas

- **Cascarón esférico (o esfera conductora) de radio $R$ y carga $Q$:** $E=kQ/r^2$ fuera y $E=0$ dentro, por lo que
  $$V(r)=\frac{kQ}{r}\ (r\ge R),\qquad V(r)=\frac{kQ}{R}\ (r\le R).$$
- **Esfera aislante maciza de radio $R$ con carga $Q$ uniforme:** fuera $V=kQ/r$; dentro $E=\dfrac{kQr}{R^3}$, y
  $$V(r)=V(R)-\int_R^r\frac{kQr'}{R^3}dr'=\frac{kQ}{R}+\frac{kQ}{2R^3}(R^2-r^2)=\frac{kQ}{2R}\left(3-\frac{r^2}{R^2}\right)\quad(r\le R).$$
  En el centro $V(0)=\tfrac32\,kQ/R$.

## Líneas y superficies equipotenciales

Una **superficie equipotencial** es aquella en que todos los puntos tienen el mismo potencial. La diferencia de potencial entre dos puntos de ella es cero, por lo que **no se requiere trabajo para mover una carga (a velocidad constante) sobre una superficie equipotencial**.

**El campo eléctrico en cada punto de una superficie equipotencial es perpendicular a ella.** Si $\vec{E}$ tuviera una componente tangente a la superficie, ejercería una fuerza sobre una carga colocada allí y haría trabajo al moverla sobre la superficie, lo que contradice la definición.

En un diagrama bidimensional las intersecciones de estas superficies con el plano se llaman **equipotenciales**. Para una carga puntual $V=kq/r$ es constante cuando $r$ es constante: sus equipotenciales son esferas concéntricas.

> **[Figura]:** a) Carga puntual positiva: líneas de campo radiales hacia afuera (naranjas) y equipotenciales circulares concéntricas (azules discontinuas). b) Dipolo (cargas de igual magnitud y signo contrario): líneas de campo que salen de la positiva y llegan a la negativa; equipotenciales que rodean a cada carga, con la equipotencial $V=0$ siendo el plano bisector entre ellas (línea recta vertical). En todos los casos las equipotenciales son perpendiculares a las líneas de campo.

## Ejemplo 1: potencial de un dipolo

Un dipolo eléctrico consiste en dos cargas puntuales, $q_1=+12$ nC y $q_2=-12$ nC, colocadas a 10 cm una de la otra. Calcule los potenciales en los puntos $a$, $b$ y $c$ sumando los potenciales debidos a cada carga.

> **[Figura]:** Las cargas están sobre una recta horizontal: $q_1$ a la izquierda y $q_2$ a la derecha, separadas 10 cm. El punto $b$ está a la izquierda de $q_1$, a 4.0 cm de ella. El punto $a$ está entre las cargas, a 6.0 cm de $q_1$ y 4.0 cm de $q_2$. El punto $c$ está por encima del segmento, a 13.0 cm de $q_1$ y a 13.0 cm de $q_2$ (sobre la mediatriz).

Respuesta (diapositiva): $V_a=-900$ V, $V_b=1930$ V, $V_c=0$.

**Resolución**

*Idea:* principio de superposición escalar con el potencial de carga puntual $V=kq/r$ (referencia $V(\infty)=0$). No hay que sumar vectores, solo cuidar el signo de cada carga.

Con $k=8.99\times10^9\ \text{N·m}^2/\text{C}^2$, $kq_1=(8.99\times10^9)(12\times10^{-9})=107.9\ \text{V·m}$ y $kq_2=-107.9\ \text{V·m}$.

*Punto $a$* ($r_1=0.060$ m, $r_2=0.040$ m):
$$V_a=\frac{kq_1}{r_1}+\frac{kq_2}{r_2}=107.9\left(\frac{1}{0.060}-\frac{1}{0.040}\right)=107.9\,(16.67-25.00)=-899\ \text{V}.$$

*Punto $b$* ($r_1=0.040$ m, $r_2=0.040+0.100=0.140$ m):
$$V_b=107.9\left(\frac{1}{0.040}-\frac{1}{0.140}\right)=107.9\,(25.00-7.14)=1926\ \text{V}.$$

*Punto $c$* ($r_1=r_2=0.130$ m):
$$V_c=\frac{k}{0.130}(q_1+q_2)=0.$$

$$\boxed{V_a\approx-900\ \text{V},\qquad V_b\approx1.93\times10^3\ \text{V},\qquad V_c=0}$$

*Interpretación:* $a$ está más cerca de la carga negativa, luego $V_a<0$; $b$ está más cerca de la positiva, luego $V_b>0$. El punto $c$ está sobre el plano bisector, equidistante de cargas opuestas: es la equipotencial $V=0$ del dipolo, aunque allí $\vec{E}\ne0$ (potencial nulo no implica campo nulo). Coincide con la respuesta dada.

## Ejemplo 2: anillo de carga

Una carga eléctrica está distribuida de manera uniforme alrededor de un anillo delgado de radio $a$ con carga total $Q$. Determine el potencial en un punto $P$ sobre el eje del anillo a una distancia $x$ del centro.

> **[Figura]:** Anillo de radio $a$ centrado en $O$, en un plano perpendicular al eje $x$. El punto $P$ está sobre el eje a distancia $x$ de $O$. Desde cualquier punto del anillo hasta $P$ la distancia es $r=\sqrt{x^2+a^2}$ (hipotenusa de un triángulo rectángulo con catetos $a$ y $x$).

Respuesta (diapositiva): $V=\dfrac{1}{4\pi\varepsilon_0}\dfrac{Q}{\sqrt{x^2+a^2}}$.

**Resolución**

*Idea:* potencial de una distribución continua, $V=k\int dq/r$. Es mucho más simple que integrar $\vec{E}$, porque $V$ es escalar y no hay que descomponer.

1. Se divide el anillo en elementos $dq$. Todos están a la **misma** distancia de $P$: $r=\sqrt{x^2+a^2}$.
2. Como $r$ es constante, sale de la integral:
$$V=\frac{1}{4\pi\varepsilon_0}\int\frac{dq}{\sqrt{x^2+a^2}}=\frac{1}{4\pi\varepsilon_0}\frac{1}{\sqrt{x^2+a^2}}\int dq.$$
3. $\int dq=Q$:

$$\boxed{V=\frac{1}{4\pi\varepsilon_0}\,\frac{Q}{\sqrt{x^2+a^2}}}$$

*Verificación:* para $x\gg a$, $V\to kQ/x$ (carga puntual). En el centro ($x=0$), $V=kQ/a\neq0$ aunque allí $E=0$. Derivando, $E_x=-\dfrac{dV}{dx}=\dfrac{kQx}{(x^2+a^2)^{3/2}}$, que es el campo del anillo obtenido en Clase 03. Coincide con la respuesta dada.

## Ejemplo 3: línea de carga finita, punto sobre su eje

Una línea de largo $L$ tiene densidad de carga $\lambda$ y carga total $Q$. Determine el potencial eléctrico en el punto $P$ ubicado a lo largo del eje de esta línea.

> **[Figura]:** Eje $x$ horizontal con $P$ en el origen. La barra ocupa desde $x=a$ hasta $x=a+L$ (separación $a$ entre $P$ y el extremo cercano). Un elemento $dx$ a distancia $x$ de $P$ tiene carga $dq=\lambda\,dx$. El campo en $P$ (dibujado) apunta hacia $-x$, alejándose de la barra.

Respuesta (diapositiva): $V=\dfrac{1}{4\pi\varepsilon_0}\,\lambda\,\ln\!\left(\dfrac{a+L}{a}\right)$.

**Resolución**

*Idea:* $V=k\int dq/r$ con $dq=\lambda\,dx$; la distancia del elemento a $P$ es simplemente $x$.

$$V=\frac{1}{4\pi\varepsilon_0}\int_a^{a+L}\frac{\lambda\,dx}{x}=\frac{\lambda}{4\pi\varepsilon_0}\big[\ln x\big]_a^{a+L}=\frac{\lambda}{4\pi\varepsilon_0}\left[\ln(a+L)-\ln a\right].$$

$$\boxed{V=\frac{\lambda}{4\pi\varepsilon_0}\ln\!\left(\frac{a+L}{a}\right)=\frac{Q}{4\pi\varepsilon_0 L}\ln\!\left(1+\frac{L}{a}\right)}$$

*Verificación:* si $a\gg L$, $\ln(1+L/a)\approx L/a$, y $V\approx\dfrac{Q}{4\pi\varepsilon_0 a}$ (carga puntual). Además, si $P$ se desplaza a la posición $x_P$ (con la barra fija), $a$ disminuye cuando $x_P$ aumenta ($da=-dx_P$), así que $E_x=-\dfrac{dV}{dx_P}=\dfrac{dV}{da}=k\lambda\left(\dfrac{1}{a+L}-\dfrac1a\right)=-\dfrac{kQ}{a(a+L)}$: el campo de la barra visto en Clase 03, dirigido hacia $-x$. Coincide con la respuesta dada.

## Ejemplo 4: esfera maciza y cascarón concéntricos

Considere dos esferas concéntricas: una maciza de radio $R_1$ con densidad volumétrica uniforme $\rho$, y una superficie esférica de radio $R_2$ ($R_2>R_1$) con densidad superficial $\sigma$. Calcule:

a) la diferencia de potencial entre las superficies de ambas esferas;
b) el potencial sobre la superficie de la esfera de radio $R_1$.

Respuesta (diapositiva): a) $\dfrac{1}{4\pi\varepsilon_0}\left(\rho\frac{4}{3}\pi R_1^3\right)\left(\dfrac{1}{R_2}-\dfrac{1}{R_1}\right)$; b) $\dfrac{1}{4\pi\varepsilon_0}\left(\sigma4\pi R_2+\rho\frac{4}{3}\pi R_1^2\right)$.

**Resolución**

*Idea:* ley de Gauss (Clase 03) para obtener $\vec{E}$ por regiones, luego $V_B-V_A=-\int\vec{E}\cdot d\vec{l}$; o superposición de los potenciales de cada esfera.

Cargas: $Q_1=\rho\,\tfrac43\pi R_1^3$ (esfera maciza) y $Q_2=\sigma\,4\pi R_2^2$ (cascarón).

**a)** Para $R_1<r<R_2$ una gaussiana esférica de radio $r$ encierra solo $Q_1$; por simetría $\vec{E}$ es radial:
$$E(4\pi r^2)=\frac{Q_1}{\varepsilon_0}\;\Rightarrow\;E=\frac{Q_1}{4\pi\varepsilon_0 r^2}.$$
Entonces
$$V(R_2)-V(R_1)=-\int_{R_1}^{R_2}\frac{Q_1}{4\pi\varepsilon_0r^2}\,dr=\frac{Q_1}{4\pi\varepsilon_0}\left[\frac1r\right]_{R_1}^{R_2}=\frac{Q_1}{4\pi\varepsilon_0}\left(\frac{1}{R_2}-\frac{1}{R_1}\right).$$

$$\boxed{V(R_2)-V(R_1)=\frac{1}{4\pi\varepsilon_0}\left(\rho\,\frac43\pi R_1^3\right)\left(\frac{1}{R_2}-\frac{1}{R_1}\right)}$$

La carga $Q_2$ no influye: dentro del cascarón su campo es nulo.

**b)** Por superposición, con $V(\infty)=0$. El potencial de la esfera maciza en su propia superficie es $kQ_1/R_1$. El cascarón produce, en todo su interior, el potencial constante $kQ_2/R_2$:
$$V(R_1)=\frac{1}{4\pi\varepsilon_0}\left(\frac{Q_1}{R_1}+\frac{Q_2}{R_2}\right)=\frac{1}{4\pi\varepsilon_0}\left(\frac{\rho\frac43\pi R_1^3}{R_1}+\frac{\sigma4\pi R_2^2}{R_2}\right).$$

$$\boxed{V(R_1)=\frac{1}{4\pi\varepsilon_0}\left(\sigma\,4\pi R_2+\rho\,\frac43\pi R_1^2\right)}$$

*Verificación:* para $\rho>0$, $V(R_2)-V(R_1)<0$: el potencial disminuye hacia afuera, en el sentido de $\vec{E}$. Unidades: $\rho R_1^2/\varepsilon_0$ y $\sigma R_2/\varepsilon_0$ tienen unidades de (C/m)/(C²/N·m²)= N·m/C = V. Ambos resultados coinciden con la diapositiva.

## Potencial eléctrico en conductores

Como el campo eléctrico dentro de un conductor en equilibrio es cero, el potencial permanece constante.

> **[Figura]:** Conductor de forma arbitraria con carga positiva en exceso. Toda la carga está en la superficie, con mayor densidad (signos $+$ más juntos) en la zona más puntiaguda. Las flechas de $\vec{E}$ salen perpendiculares a la superficie. Sobre la superficie se marcan dos puntos $A$ y $B$ unidos por una trayectoria que recorre la superficie.

Argumento: el trabajo realizado por el campo sobre una carga es $W=-q(V_B-V_A)$.
- En la superficie, $\vec{E}$ es perpendicular a cualquier desplazamiento a lo largo de ella (si tuviera componente tangente, movería las cargas y no habría equilibrio). Así $W=0$ y $V_B=V_A$: **la superficie de un conductor en equilibrio es equipotencial**.
- En el interior $\vec{E}=0$, luego tampoco se hace trabajo entre dos puntos interiores: **el potencial es constante en todo el interior e igual al de la superficie**.
- El potencial dentro de un conductor no es necesariamente cero, aunque el campo sí lo sea.

## Campo eléctrico como gradiente del potencial

Como el campo eléctrico es conservativo, el trabajo en una trayectoria cerrada es nulo:

$$0=q_0\oint\vec{E}(\vec{x})\cdot d\vec{l}\quad\Longrightarrow\quad\oint\vec{E}(\vec{x})\cdot d\vec{l}=0.$$

Por el teorema de Stokes,

$$\oint\vec{E}\cdot d\vec{l}=\iint\left(\vec{\nabla}\times\vec{E}\right)\cdot d\vec{S}=0\quad\text{para toda superficie}\quad\Longrightarrow\quad\vec{\nabla}\times\vec{E}=0\;\Longleftrightarrow\;\vec{E}=-\vec{\nabla}V.$$

En componentes cartesianas:
$$E_x=-\frac{\partial V}{\partial x},\qquad E_y=-\frac{\partial V}{\partial y},\qquad E_z=-\frac{\partial V}{\partial z}.$$

Esto se obtiene de $dV=-\vec{E}\cdot d\vec{l}$. Para simetría esférica, $E_r=-dV/dr$. El signo menos indica que $\vec{E}$ apunta hacia donde $V$ decrece más rápido, perpendicular a las equipotenciales.

## Ecuaciones de Poisson y Laplace

Recordemos la forma diferencial de la ley de Gauss (Clase 04):
$$\vec{\nabla}\cdot\vec{E}=\frac{\rho}{\varepsilon_0}.$$

Sustituyendo $\vec{E}=-\vec{\nabla}V$:
$$\vec{\nabla}\cdot(-\vec{\nabla}V)=\frac{\rho}{\varepsilon_0}\quad\Longrightarrow\quad\nabla^2V=-\frac{\rho}{\varepsilon_0}\qquad\text{(ecuación de Poisson)}.$$

En una región sin carga ($\rho=0$, el "vacío"):
$$\nabla^2V=0\qquad\text{(ecuación de Laplace)},\qquad\nabla^2=\frac{\partial^2}{\partial x^2}+\frac{\partial^2}{\partial y^2}+\frac{\partial^2}{\partial z^2}.$$

> **Nota sobre el signo:** la diapositiva escribe $\nabla^2\phi=\rho/\varepsilon_0$; el signo correcto es negativo, porque $\vec{E}=-\vec{\nabla}V$ introduce un signo menos al reemplazar en $\vec{\nabla}\cdot\vec{E}=\rho/\varepsilon_0$.

*Verificación rápida:* entre las placas de un capacitor plano ($\rho=0$), $V(x)=V_0-Ex$ satisface $d^2V/dx^2=0$. Dentro de una esfera con $\rho$ uniforme, $V=\dfrac{kQ}{2R}\left(3-\dfrac{r^2}{R^2}\right)$ da $\nabla^2V=\dfrac{1}{r^2}\dfrac{d}{dr}\left(r^2\dfrac{dV}{dr}\right)=-\dfrac{3kQ}{R^3}=-\dfrac{\rho}{\varepsilon_0}$, con $\rho=\dfrac{3Q}{4\pi R^3}$.

## Resumen de fórmulas

| Concepto | Expresión |
|---|---|
| Trabajo del campo | $W_{a\to b}=q_0\int_a^b\vec{E}\cdot d\vec{l}$ |
| Energía potencial | $\Delta U=-W=-q_0\int_a^b\vec{E}\cdot d\vec{l}$ |
| $U$ de dos cargas | $U=\dfrac{kq_0q}{r}$ |
| $U$ de un sistema | $U=k\sum_{i<j}\dfrac{q_iq_j}{r_{ij}}$ |
| Diferencia de potencial | $V_B-V_A=-\int_A^B\vec{E}\cdot d\vec{l}$ |
| Carga puntual | $V=\dfrac{kq}{r}$ |
| Superposición | $V=k\sum_i q_i/r_i$; $\ V=k\int dq/r$ |
| Anillo (eje) | $V=\dfrac{kQ}{\sqrt{x^2+a^2}}$ |
| Disco (eje) | $V=\dfrac{\sigma}{2\varepsilon_0}\left(\sqrt{x^2+R^2}-\lvert x\rvert\right)$ |
| Barra (eje, extremo a distancia $a$) | $V=k\lambda\ln\dfrac{a+L}{a}$ |
| Línea infinita | $V=\dfrac{\lambda}{2\pi\varepsilon_0}\ln\dfrac{r_0}{r}$ |
| Cascarón / conductor esférico | $V=kQ/r$ fuera, $kQ/R$ dentro |
| Esfera maciza uniforme (dentro) | $V=\dfrac{kQ}{2R}\left(3-\dfrac{r^2}{R^2}\right)$ |
| Campo desde el potencial | $\vec{E}=-\vec{\nabla}V$, $\ \vec{\nabla}\times\vec{E}=0$ |
| Poisson / Laplace | $\nabla^2V=-\rho/\varepsilon_0$; $\ \nabla^2V=0$ |
| Electrón volt | $1\ \text{eV}=1.60\times10^{-19}$ J |
| Conductores | $V$ constante en todo el conductor; $\vec{E}\perp$ superficie |
