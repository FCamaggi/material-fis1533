# Inductancia

## Inductancia mutua

> **[Figura]:** Dos bobinas enfrentadas. La bobina 1 ($N_1$ espiras) conduce una corriente $i_1$ y genera líneas de campo $\vec{B}$ que salen de ella hacia la derecha; parte de esas líneas atraviesa la bobina 2 ($N_2$ espiras), que está a su derecha y alineada en el mismo eje. $\Phi_{B2}$ es el flujo del campo de la bobina 1 a través de cada espira de la bobina 2.

Si $i_1$ varía, el flujo $\Phi_{B2}$ cambia y, por la ley de Faraday (Clase 13), se induce en la bobina 2 la fem

$$\varepsilon_2=-N_2\frac{d\Phi_{B2}}{dt}$$

Como $B$ es proporcional a $i_1$ (Biot-Savart, Clase 11), el flujo total enlazado por la bobina 2 también lo es. Suponemos entonces

$$N_2\Phi_{B2}=M_{21}\,i_1\qquad\Longrightarrow\qquad M_{21}=\frac{N_2\Phi_{B2}}{i_1}$$

donde $M_{21}$ se denomina **inductancia mutua** de las dos bobinas. Derivando en el tiempo (con geometría fija):

$$N_2\frac{d\Phi_{B2}}{dt}=M_{21}\frac{di_1}{dt}\qquad\Longrightarrow\qquad\varepsilon_2=-M_{21}\frac{di_1}{dt}$$

Análogamente, una corriente variable $i_2$ en la bobina 2 induce en la bobina 1 la fem $\varepsilon_1=-M_{12}\,di_2/dt$. Se cumple que

$$M_{21}=M_{12}=M$$

de modo que

$$\varepsilon_2=-M\frac{di_1}{dt},\qquad\varepsilon_1=-M\frac{di_2}{dt}$$

$M$ depende solo de la geometría (tamaño, forma, número de espiras, distancia y orientación) y del material del núcleo. Unidad: el **henry**, $1\,\text{H}=1\,\text{Wb/A}=1\,\text{V}\cdot\text{s/A}=1\,\Omega\cdot\text{s}$.

**Complemento: solenoide con una bobina enrollada encima.** Un solenoide largo de longitud $l$, área $A$ y $N_1$ espiras, con una segunda bobina de $N_2$ espiras enrollada sobre él. El campo del solenoide es $B_1=\mu_0N_1i_1/l$ (Clase 12) y atraviesa por completo cada espira de la bobina 2:

$$M=\frac{N_2\Phi_{B2}}{i_1}=\frac{N_2(\mu_0N_1i_1/l)A}{i_1}=\frac{\mu_0N_1N_2A}{l}$$

## Autoinductancia

> **[Figura]:** Bobina de pocas espiras conectada en serie a una batería; la corriente $i$ recorre el circuito y genera líneas de $\vec{B}$ que pasan por el interior de la propia bobina.

De la misma forma, si la corriente $i$ en la bobina varía, el flujo cambiante a través de sus **propias** espiras inducirá una fem en la bobina. Definimos

$$N\Phi_B=Li\qquad\Longrightarrow\qquad L=\frac{N\Phi_B}{i}$$

donde $L$ es la **autoinductancia** del circuito (también en henry). Derivando:

$$N\frac{d\Phi_B}{dt}=L\frac{di}{dt}$$

Así, la fem autoinducida es

$$\varepsilon_L=-L\frac{di}{dt}$$

**Complemento: autoinductancia de un solenoide largo.** $N$ espiras, longitud $l$, área $A$: $B=\mu_0Ni/l$, $\Phi_B=BA$, luego

$$L=\frac{N\Phi_B}{i}=\frac{\mu_0N^2A}{l}=\mu_0n^2\,(Al)$$

(proporcional al volumen $Al$ y al cuadrado de la densidad de espiras $n=N/l$).

La autoinductancia del **toroide** se calcula en la sección de densidad de energía.

### Ejemplo complementario 1: inductancia de un solenoide

Un solenoide de 25.0 cm de largo tiene 500 espiras y área transversal de 4.00 cm². a) Calcule su autoinductancia. b) Si la corriente crece a 100 A/s, ¿qué fem autoinducida aparece?

**Resolución**

*Idea:* campo de un solenoide largo (Ampère, Clase 12), $B=\mu_0Ni/l$ uniforme en su interior; luego $L=N\Phi_B/i$ y $\varepsilon_L=-L\,di/dt$.

a)
$$L=\frac{\mu_0N^2A}{l}=\frac{(4\pi\times10^{-7}\,\text{T·m/A})(500)^2(4.00\times10^{-4}\,\text{m}^2)}{0.250\,\text{m}}=5.03\times10^{-4}\,\text{H}$$

$$\boxed{L\approx0.503\,\text{mH}}$$

b)
$$\varepsilon_L=-L\frac{di}{dt}=-(5.03\times10^{-4}\,\text{H})(100\,\text{A/s})=-5.03\times10^{-2}\,\text{V}$$

$$\boxed{|\varepsilon_L|\approx50\,\text{mV}}$$

*Interpretación:* el signo negativo indica que la fem se opone al aumento de corriente (ley de Lenz). Valores del orden de mH son típicos para bobinas pequeñas con núcleo de aire.

## Inductores en un circuito

Como

$$\varepsilon_L=-L\frac{di}{dt}$$

la fem autoinducida **se opone a los cambios en la corriente** (no a la corriente misma). Un inductor actúa como una "inercia" eléctrica: dificulta que la corriente cambie bruscamente.

Convención: $V_{ab}=V_a-V_b$, con la corriente $i$ fluyendo de $a$ a $b$.

> **[Figura]:** Cuatro elementos entre los puntos $a$ (izquierda) y $b$ (derecha), con corriente $i$ de $a$ a $b$:
> a) Resistor $R$: el potencial disminuye de $a$ a $b$; $V_{ab}=iR>0$ ($a$ positivo).
> b) Inductor con corriente constante ($di/dt=0$): $\varepsilon=0$, $V_{ab}=L\,di/dt=0$; no hay diferencia de potencial.
> c) Inductor con corriente creciente ($di/dt>0$): la fem apunta de $b$ hacia $a$ (contra la corriente); el potencial disminuye de $a$ a $b$, $V_{ab}=L\,di/dt>0$ ($a$ positivo).
> d) Inductor con corriente decreciente ($di/dt<0$): la fem apunta de $a$ hacia $b$ (a favor de la corriente); el potencial aumenta de $a$ a $b$, $V_{ab}=L\,di/dt<0$ ($b$ positivo).

En resumen, para recorrer un inductor en el sentido de la corriente, la caída de potencial es

$$V_{ab}=L\frac{di}{dt}$$

que es la regla que se usa en las leyes de Kirchhoff (Clase 09): al recorrer el inductor en el sentido de $i$ se suma el término $-L\,di/dt$.

## Energía del campo magnético

Establecer una corriente en un inductor requiere trabajo contra la fem autoinducida. La potencia que la fuente entrega al inductor es

$$P=V_{ab}\,i=L\,i\frac{di}{dt}$$

Recordando que $dU=P\,dt$:

$$dU=L\,i\,di$$

Integrando desde $i=0$ hasta $i=I$:

$$U=\int_0^I L\,i\,di=\frac{1}{2}LI^2$$

Esta energía queda almacenada en el **campo magnético** del inductor, y se devuelve al circuito cuando la corriente disminuye (a diferencia de un resistor, que la disipa). Es la analogía magnética de $U=\frac{1}{2}CV^2$ para el condensador (Clase 06).

## Densidad de energía magnética

> **[Figura]:** Toroide de sección transversal $A$ (cuadrada pequeña) y radio medio $r$, con $N$ espiras enrolladas uniformemente (solo se muestran algunas); la corriente $i$ entra y sale por los terminales.

Para un toroide de sección pequeña frente a $r$, el campo en su interior es (Ampère, Clase 12):

$$B=\mu_0\frac{NI}{2\pi r}$$

El flujo por cada espira es

$$\Phi_B=BA=\mu_0\frac{NIA}{2\pi r}$$

y la autoinductancia del toroide:

$$L=\frac{N\Phi_B}{I}=\mu_0\frac{N^2A}{2\pi r}$$

La energía almacenada es

$$U=\frac{LI^2}{2}=\frac{1}{2}\mu_0\frac{N^2I^2A}{2\pi r}$$

El campo está confinado al volumen interior del toroide, $V=2\pi rA$ (longitud media por área). La densidad de energía es

$$u_B=\frac{U}{V}=\frac{U}{2\pi rA}=\frac{1}{2}\mu_0\left(\frac{NI}{2\pi r}\right)^2=\frac{B^2}{2\mu_0}$$

Aunque se dedujo para el toroide, el resultado

$$u_B=\frac{B^2}{2\mu_0}$$

es general en el vacío: todo campo magnético almacena energía con esa densidad (análogo a $u_E=\frac{1}{2}\varepsilon_0E^2$, Clase 06).

## Circuitos R-L

> **[Figura]:** Rama horizontal $a$–$R$–$b$–$L$–$c$ con corriente $i$ de izquierda a derecha. Arriba, en paralelo con esa rama, una batería de fem $\varepsilon$ (borne $+$ a la izquierda) en serie con el interruptor $S_1$. Abajo, otra rama paralela que solo contiene el interruptor $S_2$. Al cerrar $S_1$ se conecta la combinación R-L en serie con la fuente; al cerrar $S_2$ al mismo tiempo que se abre $S_1$, la combinación R-L queda desconectada de la fuente y en cortocircuito sobre sí misma.

### Crecimiento de la corriente

> **[Figura]:** Circuito serie: batería $\varepsilon$, interruptor $S_1$ (cerrado en $t=0$), resistor $R$ e inductor $L$, con corriente $i$ en sentido horario.

Al cerrar el interruptor $S_1$ en $t=0$, la regla de las mallas de Kirchhoff (Clase 09) da:

$$\varepsilon-iR-L\frac{di}{dt}=0$$

Es una ecuación de variables separables para $i$:

$$\frac{di}{dt}=\frac{R}{L}\left(\frac{\varepsilon}{R}-i\right)\quad\Rightarrow\quad\frac{di}{\varepsilon/R-i}=\frac{R}{L}dt$$

Integrando con $i(0)=0$ (un inductor no permite saltos de corriente):

$$-\ln\!\left(\frac{\varepsilon/R-i}{\varepsilon/R}\right)=\frac{R}{L}t\quad\Rightarrow\quad\boxed{i(t)=\frac{\varepsilon}{R}\left(1-e^{-(R/L)t}\right)}$$

La **constante de tiempo** del circuito es

$$\tau=\frac{L}{R}$$

> **[Figura]:** Gráfica $i(t)$: parte de 0 en $t=0$ y crece asintóticamente hacia la línea punteada $I=\varepsilon/R$. En $t=\tau=L/R$ la corriente vale $I(1-1/e)\approx0.632\,I$.

Observaciones:

- En $t=0$: $i=0$ y $di/dt=\varepsilon/L$; toda la fem cae en el inductor (se comporta como circuito abierto).
- Para $t\gg\tau$: $i\to\varepsilon/R$, $di/dt\to0$; el inductor se comporta como un cable (sin caída de potencial).
- A mayor $L$ o menor $R$, el crecimiento es más lento.

### Decaimiento de la corriente

Luego de mucho tiempo (corriente $I_0=\varepsilon/R$) se abre $S_1$ y se cierra $S_2$:

> **[Figura]:** Malla con $R$ y $L$ en serie cerrada por $S_2$ (cerrado en $t=0$), corriente $i$ en el mismo sentido que antes. Gráfica $i(t)$: parte de $I_0$ y decae exponencialmente a cero; en $t=L/R$ vale $I_0/e$.

$$-iR-L\frac{di}{dt}=0\quad\Rightarrow\quad\frac{di}{i}=-\frac{R}{L}dt$$

$$\boxed{i(t)=I_0\,e^{-(R/L)t}}$$

En $t=\tau$ la corriente cae a $I_0/e\approx0.368\,I_0$. La energía $\frac12LI_0^2$ almacenada en el inductor se disipa en el resistor:

$$\int_0^\infty i^2R\,dt=I_0^2R\int_0^\infty e^{-2Rt/L}dt=I_0^2R\frac{L}{2R}=\frac{1}{2}LI_0^2\ \checkmark$$

### Ejemplo complementario 2: circuito R-L

Un circuito R-L serie tiene $\varepsilon=12.0\,\text{V}$, $R=6.00\,\Omega$ y $L=30.0\,\text{mH}$. Se cierra el interruptor en $t=0$. Calcule: a) la constante de tiempo; b) la corriente final; c) la corriente en $t=\tau$; d) la energía almacenada en el inductor en régimen permanente.

**Resolución**

*Idea:* usar la solución de crecimiento $i(t)=\frac{\varepsilon}{R}(1-e^{-t/\tau})$ con $\tau=L/R$, y $U=\frac12LI^2$.

a) $\tau=\dfrac{L}{R}=\dfrac{30.0\times10^{-3}\,\text{H}}{6.00\,\Omega}=5.00\times10^{-3}\,\text{s}$.

b) $I=\dfrac{\varepsilon}{R}=\dfrac{12.0\,\text{V}}{6.00\,\Omega}=2.00\,\text{A}$.

c) $i(\tau)=I(1-e^{-1})=(2.00\,\text{A})(0.632)=1.26\,\text{A}$.

d) $U=\frac12LI^2=\frac12(30.0\times10^{-3}\,\text{H})(2.00\,\text{A})^2=0.0600\,\text{J}$.

$$\boxed{\tau=5.00\,\text{ms},\quad I=2.00\,\text{A},\quad i(\tau)=1.26\,\text{A},\quad U=60.0\,\text{mJ}}$$

*Verificación:* $[\text{H}/\Omega]=[\Omega\cdot\text{s}/\Omega]=\text{s}$ ✓; $i(\tau)<I$ ✓.

## Circuito L-C

> **[Figura]:** Ciclo de oscilación de un circuito L-C ideal (sin resistencia), con barras de energía $E=U_B+U_E$:
> a) $t=0$ y $t=T$: condensador cargado por completo ($+Q_m$ a la izquierda, $-Q_m$ a la derecha, campo eléctrico $E_m$), corriente cero; toda la energía está en el campo eléctrico. El interruptor se cierra en $t=0$.
> b) $t=T/4$: condensador descargado, corriente máxima $I_m$, campo magnético $B_m$ en el inductor; toda la energía está en el campo magnético.
> c) $t=T/2$: condensador cargado por completo con polaridad invertida ($-Q_m$ a la izquierda, $+Q_m$ a la derecha), corriente cero; energía eléctrica.
> d) $t=3T/4$: condensador descargado, corriente máxima en sentido inverso; energía magnética.
> Entre estados: el condensador se descarga con $I$ en aumento, luego se recarga con $I$ en disminución, y el ciclo se repite.

> **[Figura]:** Circuito: condensador $C$ (placa izquierda $+q$, derecha $-q$) en serie con inductor $L$; la corriente $i$ circula por el inductor de derecha a izquierda; recorrido de la malla en sentido horario.

Al recorrer el circuito:

$$-\frac{Q}{C}-L\frac{dI}{dt}=0$$

Como $I=\dfrac{dQ}{dt}$:

$$\frac{d^2Q}{dt^2}+\frac{1}{LC}Q=0$$

Ecuación de **movimiento armónico simple**, con solución

$$\boxed{Q(t)=Q_{\text{máx}}\cos(\omega t+\phi),\qquad\omega^2=\frac{1}{LC}\ \Rightarrow\ \omega=\frac{1}{\sqrt{LC}}}$$

La corriente es

$$I(t)=\frac{dQ}{dt}=-\omega Q_{\text{máx}}\sin(\omega t+\phi)$$

desfasada 90° respecto de la carga: cuando $Q$ es máxima, $I=0$, y viceversa.

**Conservación de la energía.** Multiplicando la ecuación de malla por $I$:

$$\frac{Q}{C}\frac{dQ}{dt}+LI\frac{dI}{dt}=\frac{d}{dt}\left(\frac{Q^2}{2C}+\frac{1}{2}LI^2\right)=0\quad\Rightarrow\quad\frac{Q^2}{2C}+\frac{1}{2}LI^2=\frac{Q_{\text{máx}}^2}{2C}=\text{cte.}$$

La energía oscila entre el campo eléctrico del condensador y el campo magnético del inductor. De aquí, $I_{\text{máx}}=Q_{\text{máx}}/\sqrt{LC}=\omega Q_{\text{máx}}$.

### Analogía masa-resorte

| Sistema masa-resorte | Circuito L-C |
|---|---|
| Desplazamiento $x$ | Carga $Q$ |
| Velocidad $v=dx/dt$ | Corriente $I=dQ/dt$ |
| Masa $m$ | Inductancia $L$ |
| Constante elástica $k$ | Inverso de la capacitancia $1/C$ |
| $m\ddot{x}+kx=0$ | $L\ddot{Q}+Q/C=0$ |
| $\omega=\sqrt{k/m}$ | $\omega=1/\sqrt{LC}$ |
| Energía cinética $\frac12mv^2$ | Energía magnética $\frac12LI^2$ |
| Energía potencial $\frac12kx^2$ | Energía eléctrica $\frac{Q^2}{2C}$ |
| Roce viscoso $b\,\dot{x}$ | Resistencia $R\,\dot{Q}$ |

### Ejemplo complementario 3: circuito L-C

Un condensador de $C=1.00\,\mu\text{F}$ se carga a $10.0\,\text{V}$ y en $t=0$ se conecta a un inductor de $L=10.0\,\text{mH}$. Determine: a) la frecuencia angular y la frecuencia de oscilación; b) la carga máxima y la energía total; c) la corriente máxima.

**Resolución**

*Idea:* M.A.S. eléctrico con $\omega=1/\sqrt{LC}$; carga inicial $Q=CV$ (Clase 06); energía conservada $\frac{Q_{\text{máx}}^2}{2C}=\frac12LI_{\text{máx}}^2$.

a)
$$\omega=\frac{1}{\sqrt{(10.0\times10^{-3}\,\text{H})(1.00\times10^{-6}\,\text{F})}}=\frac{1}{10^{-4}\,\text{s}}=1.00\times10^4\,\text{rad/s},\qquad f=\frac{\omega}{2\pi}=1.59\times10^3\,\text{Hz}$$

b)
$$Q_{\text{máx}}=CV=(1.00\times10^{-6}\,\text{F})(10.0\,\text{V})=1.00\times10^{-5}\,\text{C},\qquad U=\frac{Q_{\text{máx}}^2}{2C}=\frac{(10^{-5})^2}{2\times10^{-6}}\,\text{J}=5.00\times10^{-5}\,\text{J}$$

c)
$$I_{\text{máx}}=\omega Q_{\text{máx}}=(1.00\times10^4\,\text{s}^{-1})(1.00\times10^{-5}\,\text{C})=0.100\,\text{A}$$

$$\boxed{\omega=1.00\times10^4\,\text{rad/s},\ f\approx1.59\,\text{kHz},\ U=50.0\,\mu\text{J},\ I_{\text{máx}}=0.100\,\text{A}}$$

*Verificación:* $\frac12LI_{\text{máx}}^2=\frac12(0.0100)(0.100)^2=5.00\times10^{-5}\,\text{J}$, igual a la energía inicial del condensador ✓.

## Circuito L-R-C

> **[Figura]:** Batería $\varepsilon$ en la rama superior; condensador $C$ ($+q$ a la izquierda, $-q$ a la derecha, conectado al nodo $d$) en la rama central; abajo, inductor $L$ entre los nodos $c$ y $b$, y resistor $R$ entre $b$ y $a$. El interruptor S, conectado en $d$, puede unir el condensador con la batería (lo carga) o con el punto $a$, en cuyo caso el condensador se descarga a través de $R$ y $L$ en serie; la corriente $i$ circula por el inductor de $b$ hacia $c$.

Con el condensador cargado, en $t=0$ se cierra el interruptor S en la posición $a$:

$$-\frac{Q}{C}-IR-L\frac{dI}{dt}=0$$

Como $I=\dfrac{dQ}{dt}$:

$$-\frac{Q}{C}-\frac{dQ}{dt}R-L\frac{d^2Q}{dt^2}=0$$

$$\frac{d^2Q}{dt^2}+\frac{R}{L}\frac{dQ}{dt}+\frac{1}{LC}Q=0$$

Ecuación de **movimiento armónico amortiguado** (la resistencia cumple el papel del roce viscoso).

### Solución

Probamos soluciones de la forma

$$Q(t)=A\,e^{\lambda t}\quad\Rightarrow\quad\dot{Q}(t)=A\lambda e^{\lambda t},\qquad\ddot{Q}(t)=A\lambda^2e^{\lambda t}$$

Al reemplazar y dividir por $Ae^{\lambda t}\neq0$ se obtiene la ecuación característica:

$$\lambda^2+\frac{R}{L}\lambda+\frac{1}{LC}=0\quad\Rightarrow\quad\lambda=-\frac{1}{2}\left(\frac{R}{L}\right)\pm\frac{1}{2}\sqrt{\left(\frac{R}{L}\right)^2-\frac{4}{LC}}$$

El tipo de solución queda determinado por el discriminante $\left(\frac{R}{L}\right)^2-\frac{4}{LC}$:

| Condición | Equivalente | Tipo |
|---|---|---|
| $\left(\frac{R}{L}\right)^2-\frac{4}{LC}>0$ | $R>2\sqrt{L/C}$ | **Sobreamortiguado**: dos raíces reales negativas; $Q$ decae sin oscilar, lentamente |
| $\left(\frac{R}{L}\right)^2-\frac{4}{LC}=0$ | $R=2\sqrt{L/C}$ | **Críticamente amortiguado**: raíz doble; $Q=(A+Bt)e^{-Rt/2L}$, el retorno a cero más rápido sin oscilar |
| $\left(\frac{R}{L}\right)^2-\frac{4}{LC}<0$ | $R<2\sqrt{L/C}$ | **Subamortiguado**: raíces complejas; $Q$ oscila con amplitud decreciente |

> **[Figura]:** Tres gráficas $q(t)$ que parten de $Q$ en $t=0$: a) subamortiguado ($R$ pequeña): oscilación alrededor de cero cuya amplitud decae dentro de una envolvente exponencial (líneas punteadas); b) críticamente amortiguado ($R$ grande): caída rápida a cero sin cruzar el eje; c) sobreamortiguado ($R$ muy grande): caída a cero sin oscilar, más lenta que en b).

### Caso subamortiguado

Si $\frac{1}{LC}>\frac{R^2}{4L^2}$, las raíces son $\lambda=-\frac{R}{2L}\pm i\omega'$ con

$$\omega'=\sqrt{\frac{1}{LC}-\frac{R^2}{4L^2}}$$

Combinando las dos exponenciales complejas ($e^{\pm i\omega't}$) en una solución real:

$$\boxed{Q(t)=A\,e^{-(R/2L)t}\cos(\omega't+\phi)}$$

> **[Figura]:** Gráfica del caso subamortiguado: $q(t)$ parte de $Q$, oscila con frecuencia angular $\omega'$ y su amplitud decrece siguiendo la envolvente $\pm Ae^{-Rt/2L}$ (líneas punteadas grises).

- La amplitud decae con la constante de tiempo $2L/R$: la energía se disipa en el resistor.
- $\omega'<\omega_0=1/\sqrt{LC}$: la resistencia hace la oscilación algo más lenta.
- Si $R\to0$, $\omega'\to1/\sqrt{LC}$ y se recupera el circuito L-C.

### Ejemplo complementario 4: circuito L-R-C

Al circuito del ejemplo complementario 3 ($L=10.0\,\text{mH}$, $C=1.00\,\mu\text{F}$) se le agrega en serie un resistor $R=50.0\,\Omega$. a) ¿Es el circuito subamortiguado? b) Calcule $\omega'$. c) ¿Qué resistencia produciría amortiguamiento crítico?

**Resolución**

*Idea:* comparar $R$ con $2\sqrt{L/C}$ (signo del discriminante) y aplicar la fórmula de $\omega'$.

a) $2\sqrt{L/C}=2\sqrt{\dfrac{10.0\times10^{-3}}{1.00\times10^{-6}}}\,\Omega=2\sqrt{10^4}\,\Omega=200\,\Omega$. Como $50.0\,\Omega<200\,\Omega$, el circuito es **subamortiguado**.

b)
$$\frac{1}{LC}=1.00\times10^8\,\text{s}^{-2},\qquad\frac{R^2}{4L^2}=\frac{(50.0)^2}{4(10.0\times10^{-3})^2}\,\text{s}^{-2}=6.25\times10^6\,\text{s}^{-2}$$
$$\omega'=\sqrt{1.00\times10^8-6.25\times10^6}\,\text{s}^{-1}=\sqrt{9.375\times10^7}\,\text{s}^{-1}=9.68\times10^3\,\text{rad/s}$$

c) $R_{\text{crít}}=2\sqrt{L/C}=200\,\Omega$.

$$\boxed{\text{subamortiguado},\quad\omega'\approx9.68\times10^3\,\text{rad/s},\quad R_{\text{crít}}=200\,\Omega}$$

*Interpretación:* $\omega'$ es solo un 3 % menor que $\omega_0=1.00\times10^4\,\text{rad/s}$; la amplitud decae con constante de tiempo $2L/R=0.4\,\text{ms}$, es decir, en unas pocas oscilaciones ($T'=2\pi/\omega'\approx0.65\,\text{ms}$).

## Resumen de fórmulas

| Concepto | Expresión |
|---|---|
| Inductancia mutua | $M=\dfrac{N_2\Phi_{B2}}{i_1}=\dfrac{N_1\Phi_{B1}}{i_2}$, $\ \varepsilon_2=-M\dfrac{di_1}{dt}$, $\ \varepsilon_1=-M\dfrac{di_2}{dt}$ |
| Autoinductancia | $L=\dfrac{N\Phi_B}{I}$, $\ \varepsilon_L=-L\dfrac{dI}{dt}$ |
| Solenoide | $L=\dfrac{\mu_0N^2A}{l}$ |
| Toroide | $L=\dfrac{\mu_0N^2A}{2\pi r}$ |
| Caída en el inductor (sentido de $i$) | $V_{ab}=L\dfrac{di}{dt}$ |
| Energía magnética | $U_B=\dfrac12LI^2$ |
| Densidad de energía | $u_B=\dfrac{B^2}{2\mu_0}$ |
| R-L, crecimiento | $\varepsilon-iR-L\dfrac{di}{dt}=0$, $\ i=\dfrac{\varepsilon}{R}\left(1-e^{-t/\tau}\right)$ |
| R-L, decaimiento | $i=I_0e^{-t/\tau}$, $\ \tau=\dfrac{L}{R}$ |
| L-C | $\ddot{Q}+\dfrac{Q}{LC}=0$, $\ Q=Q_{\text{máx}}\cos(\omega t+\phi)$, $\ \omega=\dfrac{1}{\sqrt{LC}}$ |
| Energía en L-C | $\dfrac{Q^2}{2C}+\dfrac12LI^2=\text{cte.}$ |
| L-R-C | $\ddot{Q}+\dfrac{R}{L}\dot{Q}+\dfrac{Q}{LC}=0$ |
| Clasificación | sobre: $R>2\sqrt{L/C}$; crítico: $R=2\sqrt{L/C}$; sub: $R<2\sqrt{L/C}$ |
| Subamortiguado | $Q=Ae^{-Rt/2L}\cos(\omega't+\phi)$, $\ \omega'=\sqrt{\dfrac{1}{LC}-\dfrac{R^2}{4L^2}}$ |
