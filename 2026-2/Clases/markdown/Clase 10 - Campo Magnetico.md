# Campo Magnético

## Un poco de historia

Muchos historiadores de la ciencia creen que la brújula, que usa una aguja magnética, ya se utilizaba en China en el siglo XIII a.C.; otros atribuyen su invención a un origen árabe o indio.

Se conocen muchas otras observaciones antiguas del fenómeno. Por ejemplo, los antiguos griegos manipulaban la **magnetita** ($\text{Fe}_3\text{O}_4$), un mineral que atrae limaduras de hierro. Más tarde, Pierre de Maricourt descubrió la existencia de los **polos** de un imán, sin saber todavía lo importantes que eran.

Otras manifestaciones naturales del magnetismo son la magnetósfera terrestre, que desvía el viento solar (partículas cargadas que vienen del Sol), y las auroras, que se producen cuando esas partículas quedan atrapadas por el campo terrestre y llegan a la alta atmósfera cerca de los polos.

La historia se vuelve realmente interesante en **1819**. Ese año **Hans Christian Oersted** descubrió la relación entre magnetismo y electricidad al experimentar con una brújula y un hilo por el que circulaba una corriente. Si se pone el hilo paralelo a la aguja y se hace circular corriente, la aguja se mueve.

La brújula de Oersted no se parece mucho a un circuito de corriente continua. Sin embargo, hoy sabemos, como sospechó Ampère, que el hierro imantado está lleno de cargas en movimiento incesante: corrientes eléctricas a escala atómica. **Toda fuente de campo magnético es, en el fondo, carga en movimiento.**

Hoy conocemos con certeza cómo se comportan las líneas de campo de una barra imantada. James Maxwell logró describirlo matemáticamente, y fue un gran avance.

> **[Figura]:** Barra imantada horizontal, con el polo N a la izquierda y el S a la derecha. Las líneas de campo salen del polo N, rodean la barra por arriba y por abajo y vuelven a entrar por el polo S. Dentro de la barra van de S a N, de modo que cada línea es una curva cerrada. Sobre las líneas hay brújulas pequeñas, y cada aguja apunta tangente a la línea, en el sentido del campo. Sobre la barra, la aguja apunta de N hacia S, y en los costados las agujas siguen la curvatura.

> **[Figura]:** La Tierra como un gran imán. Su eje de rotación (polos geográficos) está algo inclinado respecto del eje del dipolo magnético. Las líneas de campo salen cerca del **polo sur geográfico** y entran cerca del **polo norte geográfico**. Por eso el "polo norte magnético" terrestre, que atrae al polo N de las brújulas, es en realidad un polo S magnético. En el ecuador, las líneas son aproximadamente horizontales.

**Unidades:** en el S.I. el campo magnético se mide en **tesla** (T); en el sistema cgs se usa el **gauss** (G). Las unidades se detallan más abajo.

## Notación y definición

Usaremos el símbolo $\vec{B}$ para el **campo magnético**. Es una magnitud vectorial, y en cada punto tiene la dirección que indicaría una brújula ubicada ahí.

El campo magnético en un punto del espacio se puede definir a partir de la **fuerza magnética** $\vec{F}_B$ que ejerce sobre una partícula cargada que se mueve con velocidad $\vec{v}$. Los experimentos muestran que:

- La magnitud de $\vec{F}_B$ es proporcional a la carga $q$ y a la rapidez $v$ de la partícula.
- La magnitud y la dirección de $\vec{F}_B$ dependen de la velocidad de la partícula y de la magnitud y dirección de $\vec{B}$.
- Si la partícula se mueve **paralela** a $\vec{B}$, la fuerza magnética es **cero**.
- Si la velocidad forma un ángulo $\theta \neq 0$ con $\vec{B}$, la fuerza es perpendicular tanto a $\vec{v}$ como a $\vec{B}$.
- La fuerza sobre una carga positiva tiene sentido opuesto a la que actúa sobre una carga negativa que se mueve en la misma dirección.

Todo esto se resume en

$$\boxed{\vec{F}_B = q\,\vec{v}\times\vec{B}}$$

y su módulo es

$$F_B = |q|\,v\,B\,\sin\theta,$$

donde $\theta$ es el menor ángulo entre $\vec{v}$ y $\vec{B}$. La fuerza es máxima, $|q|vB$, cuando $\vec{v}\perp\vec{B}$, y nula cuando $\vec{v}\parallel\vec{B}$.

**Consecuencia importante:** como $\vec{F}_B\perp\vec{v}$ en todo instante, la fuerza magnética **no realiza trabajo**, porque $dW = \vec{F}_B\cdot\vec{v}\,dt = 0$. Puede cambiar la dirección de la velocidad, pero no su rapidez ni la energía cinética de la partícula.

### Fuerza de Lorentz

Si en la región hay además un campo eléctrico $\vec{E}$ (Clase 02, $\vec{F}_E = q\vec{E}$), la fuerza total sobre la carga es la **fuerza de Lorentz**:

$$\boxed{\vec{F} = q\left(\vec{E} + \vec{v}\times\vec{B}\right)}$$

Esta expresión se usa más adelante en el selector de velocidades.

### Diferencias entre fuerza eléctrica y fuerza magnética

| | Fuerza eléctrica $q\vec{E}$ | Fuerza magnética $q\vec{v}\times\vec{B}$ |
|---|---|---|
| Dirección | paralela (o antiparalela) a $\vec{E}$ | perpendicular a $\vec{B}$ y a $\vec{v}$ |
| Carga en reposo | actúa | no actúa |
| Trabajo | puede realizar trabajo | nunca realiza trabajo |

## Regla de la mano derecha

La fórmula de $\vec{F}_B$ usa el producto vectorial (producto cruz), cuyo resultado es perpendicular a los dos vectores originales, $\vec{v}$ y $\vec{B}$.

> **[Figura]:** Mano derecha con el pulgar hacia arriba. El vector $\vec{v}$ (rojo) apunta hacia la izquierda, el vector $\vec{B}$ (azul) apunta en diagonal hacia abajo y hacia el observador, y $\vec{F}_B$ (negro) apunta hacia arriba, en la dirección del pulgar. Los dedos se cierran desde $\vec{v}$ hacia $\vec{B}$.

**Regla 1 (dedos que se cierran):** se apuntan los dedos de la mano derecha en la dirección de $\vec{v}$ y se cierran hacia $\vec{B}$, por el ángulo menor. El pulgar indica la dirección de $\vec{v}\times\vec{B}$.

**Regla 2 (tres dedos):** el índice se extiende en la dirección del primer vector ($\vec{v}$) y el dedo medio en la dirección del segundo ($\vec{B}$). El pulgar da la dirección del resultado.

En ambos casos, el pulgar da la dirección de $\vec{v}\times\vec{B}$. **Si $q<0$, la fuerza apunta en el sentido opuesto al pulgar.**

Productos útiles entre los vectores unitarios cartesianos:
$$\hat{\imath}\times\hat{\jmath}=\hat{k},\quad \hat{\jmath}\times\hat{k}=\hat{\imath},\quad \hat{k}\times\hat{\imath}=\hat{\jmath},\quad \hat{\imath}\times\hat{\imath}=\hat{\jmath}\times\hat{\jmath}=\hat{k}\times\hat{k}=0,$$
y si se invierte el orden, cambia el signo (por ejemplo, $\hat{\jmath}\times\hat{\imath}=-\hat{k}$).

**Convención gráfica:** $\otimes$ (o $\times$) indica un campo que **entra** en la hoja, y $\odot$ (o $\bullet$) un campo que **sale** de la hoja.

## Unidades

En el Sistema Internacional, la unidad del campo magnético es el newton por coulomb-metro por segundo, llamado **tesla** (T):

$$1\,\frac{\text{N}}{\text{C}\cdot\text{m/s}} = 1\,\text{T}.$$

Como un coulomb por segundo es un ampere ($1\,\text{C/s}=1\,\text{A}$), también se puede escribir

$$1\,\frac{\text{N}}{\text{A}\cdot\text{m}} = 1\,\text{T}.$$

Otra unidad que vale la pena mencionar es el **gauss** (G), del sistema cgs:

$$1\,\text{T} = 10^{4}\,\text{G}.$$

Como referencia, el campo magnético terrestre en la superficie es del orden de $0{,}5\,\text{G} = 5\times10^{-5}\,\text{T}$, un imán de laboratorio produce entre $0{,}1$ y $1\,\text{T}$, y un resonador de imagen médica entre $1{,}5$ y $3\,\text{T}$.

## Ejemplo 1: electrón en un tubo de televisión (CRT)

Un electrón en un televisor de tubo (CRT) se mueve hacia el frente del tubo con una velocidad de $8{,}0\times10^{6}\,\text{m/s}$ a lo largo del eje $x$. Alrededor del cuello del tubo hay bobinas de alambre que crean un campo magnético de magnitud $0{,}025\,\text{T}$, dirigido a $60^\circ$ del eje $x$ y contenido en el plano $xy$.

a) Determine la magnitud de la fuerza magnética sobre el electrón.
b) Encuentre una expresión vectorial para esta fuerza magnética.

> **[Figura]:** Ejes $x$ (hacia el observador y a la izquierda), $y$ (hacia la derecha) y $z$ (hacia arriba), con el origen en el electrón ($-e$). El vector $\vec{v}$ va a lo largo de $+x$, y $\vec{B}$ está en el plano $xy$, a $60^\circ$ de $\vec{v}$, entre los ejes $+x$ y $+y$. La fuerza $\vec{F}_B$ apunta verticalmente hacia abajo ($-z$).

**Resolución**

*Idea:* se aplica directamente la definición $\vec{F}_B = q\vec{v}\times\vec{B}$, con $q=-e$. En (a) basta el módulo $|q|vB\sin\theta$. En (b) se descomponen los vectores en componentes cartesianas y se usa el álgebra del producto cruz.

**a) Magnitud.** El ángulo entre $\vec{v}$ y $\vec{B}$ es $\theta = 60^\circ$:
$$F_B = |q|vB\sin\theta = (1{,}6\times10^{-19}\,\text{C})(8{,}0\times10^{6}\,\text{m/s})(0{,}025\,\text{T})\sin 60^\circ.$$
Como $(1{,}6\times10^{-19})(8{,}0\times10^{6}) = 1{,}28\times10^{-12}$, luego $\times\, 0{,}025 = 3{,}2\times10^{-14}$, y finalmente $\times\,0{,}866 = 2{,}77\times10^{-14}$:
$$\boxed{F_B \approx 2{,}8\times10^{-14}\,\text{N}}$$

**b) Expresión vectorial.** Se escriben los vectores en componentes:
$$\vec{v} = (8{,}0\times10^{6}\,\hat{\imath})\,\text{m/s},$$
$$\vec{B} = (0{,}025\cos60^\circ\,\hat{\imath} + 0{,}025\sin60^\circ\,\hat{\jmath})\,\text{T} = (0{,}0125\,\hat{\imath} + 0{,}0217\,\hat{\jmath})\,\text{T}.$$

Se aplica la propiedad distributiva del producto cruz:
$$\vec{F}_B = (-e)\left[(8{,}0\times10^{6}\,\hat{\imath})\times(0{,}0125\,\hat{\imath}) + (8{,}0\times10^{6}\,\hat{\imath})\times(0{,}0217\,\hat{\jmath})\right].$$
Como $\hat{\imath}\times\hat{\imath}=0$, el primer término se anula. Como $\hat{\imath}\times\hat{\jmath}=\hat{k}$:
$$\vec{F}_B = (-1{,}6\times10^{-19}\,\text{C})(8{,}0\times10^{6}\,\text{m/s})(0{,}0217\,\text{T})\,\hat{k}.$$
$$\boxed{\vec{F}_B \approx (-2{,}8\times10^{-14}\,\text{N})\,\hat{k}}$$

*Verificación / interpretación:* el módulo coincide con el de la parte (a). Notar que solo la componente de $\vec{B}$ perpendicular a $\vec{v}$, es decir $B\sin60^\circ$, contribuye a la fuerza. La regla de la mano derecha da $\vec{v}\times\vec{B}$ en $+\hat{k}$, pero como la carga es negativa la fuerza apunta en $-\hat{k}$, hacia abajo, como en la figura. Unidades: $\text{C}\cdot\text{m/s}\cdot\text{T} = \text{C}\cdot\text{m/s}\cdot\frac{\text{N}}{\text{C}\cdot\text{m/s}} = \text{N}$.

## Problema extra: espectrómetro de masas

En la figura se muestran los componentes esenciales de un espectrómetro de masas, que se usa para medir la masa de partículas cargadas. En una fuente se produce un ion de masa $m$ y carga $q$, que parte del reposo y es acelerado por una diferencia de potencial $\Delta V$. Luego entra a una zona de selección donde hay un campo magnético $\vec{B}$ uniforme (entrando en la hoja) y un campo eléctrico deflector $\vec{E}$. Solo las partículas con velocidad $\vec{v}$ constante salen del selector (es un **selector de velocidades**). Las partículas que emergen entran a una segunda región donde existe otro campo magnético $\vec{B}_0$ (también entrando en la hoja). Ahí la partícula sigue una trayectoria circular y choca con un detector a una distancia $2r$ del punto de entrada.

a) Encuentre la velocidad $\vec{v}$.
b) Encuentre el campo $\vec{B}$.
c) Encuentre la masa $m$ de la partícula.

> **[Figura]:** Un ion positivo (+) se mueve verticalmente hacia arriba ($+\hat{\jmath}$). Primero atraviesa el selector, formado por dos placas verticales paralelas: la izquierda (naranja) y la derecha (celeste). Entre ellas hay un campo $\vec{E}$ horizontal hacia la derecha ($+\hat{\imath}$) y un campo $\vec{B}$ que entra en la hoja ($\times$, es decir $-\hat{k}$). La trayectoria dentro del selector es recta, por la línea punteada central. Al salir, el ion entra por una rendija a la región superior, donde $\vec{B}_0$ entra en la hoja ($\times$). Ahí describe una semicircunferencia de radio $r$, curvándose hacia la **izquierda**, y choca con la placa inferior de esa región a una distancia $2r$ (el diámetro) de la rendija de entrada.

**Resolución**

*Idea:* se combinan tres conceptos. (a) Conservación de la energía con potencial eléctrico (Clase 05): el trabajo del campo eléctrico, $q\Delta V$, se convierte en energía cinética. (b) Fuerza de Lorentz: para que la partícula atraviese el selector sin desviarse, la fuerza neta debe ser cero. (c) Movimiento circular en $\vec{B}$ uniforme: la fuerza magnética cumple el papel de fuerza centrípeta.

**a) Velocidad.** La partícula parte del reposo, de modo que la pérdida de energía potencial, $q\Delta V$, se transforma íntegramente en energía cinética:
$$\frac{1}{2}mv^{2} = q\,\Delta V \;\Longrightarrow\; v^{2} = \frac{2q\Delta V}{m}.$$
Como se mueve hacia arriba en la figura:
$$\boxed{\vec{v} = \sqrt{\frac{2q\,\Delta V}{m}}\;\hat{\jmath}}$$

**b) Campo en el selector.** Para que la velocidad sea constante, la partícula debe cruzar el selector en línea recta y sin acelerar, es decir, con fuerza de Lorentz nula:
$$\vec{F} = q\left(\vec{E} + \vec{v}\times\vec{B}\right) = 0,$$
con $\vec{E}=E\,\hat{\imath}$, $\vec{B}=-B\,\hat{k}$ y $\vec{v}=v\,\hat{\jmath}$. Se calcula el producto cruz:
$$\vec{v}\times\vec{B} = v\hat{\jmath}\times(-B\hat{k}) = -vB\,(\hat{\jmath}\times\hat{k}) = -vB\,\hat{\imath}.$$
Entonces
$$qE\,\hat{\imath} - qvB\,\hat{\imath} = 0 \;\Longrightarrow\; qE = qvB \;\Longrightarrow\; B = \frac{E}{v}.$$
Se reemplaza $v$ de la parte (a):
$$\boxed{B = \frac{E}{v} = E\sqrt{\frac{m}{2q\,\Delta V}}, \qquad \vec{B} = -E\sqrt{\frac{m}{2q\,\Delta V}}\;\hat{k}}$$

**c) Masa.** En la región de $\vec{B}_0$, con $\vec{v}\perp\vec{B}_0$, la fuerza magnética tiene módulo $qvB_0$ y es siempre perpendicular a $\vec{v}$, así que la trayectoria es una circunferencia de radio $r$. Por dinámica circular:
$$qvB_0 = m\frac{v^{2}}{r} \;\Longrightarrow\; qB_0 = \frac{m v}{r} = \frac{m}{r}\sqrt{\frac{2q\Delta V}{m}}.$$
Se eleva al cuadrado:
$$q^{2}B_0^{2} = \frac{m^{2}}{r^{2}}\cdot\frac{2q\Delta V}{m} = \frac{2mq\Delta V}{r^{2}}.$$
Se despeja $m$:
$$\boxed{m = \frac{q\,B_0^{2}\,r^{2}}{2\,\Delta V}}$$

*Verificación / interpretación:*
- **Selector:** la velocidad seleccionada $v=E/B$ no depende de $q$ ni de $m$. Una partícula más rápida tendría $qvB>qE$ y se desviaría hacia la izquierda; una más lenta se desviaría hacia la derecha.
- **Dirección de la curva:** en $\vec{B}_0$, $\vec{F}=q\,v\hat{\jmath}\times(-B_0\hat{k}) = -qvB_0\,\hat{\imath}$, hacia la izquierda, como en la figura.
- **Unidades de $m$:** $\dfrac{\text{C}\cdot\text{T}^{2}\cdot\text{m}^{2}}{\text{V}}$. Con $\text{T}=\text{N}\cdot\text{s}/(\text{C}\cdot\text{m})$ y $\text{V}=\text{J}/\text{C}=\text{N}\cdot\text{m}/\text{C}$ se obtiene $\dfrac{\text{C}\cdot\text{N}^{2}\text{s}^{2}/(\text{C}^{2}\text{m}^{2})\cdot\text{m}^{2}}{\text{N}\cdot\text{m}/\text{C}} = \dfrac{\text{N}\cdot\text{s}^{2}}{\text{m}} = \text{kg}$. ✓
- **Uso práctico:** midiendo la distancia $2r$ en el detector se obtiene $m$, porque $m\propto r^{2}$, y así se separan los isótopos.

## Líneas de campo y flujo magnético (complemento)

Las **líneas de campo magnético** se dibujan tangentes a $\vec{B}$ en cada punto, y su densidad indica la intensidad del campo. A diferencia de las líneas de $\vec{E}$, que nacen en cargas positivas y mueren en negativas, las líneas de $\vec{B}$ **no tienen principio ni fin**: son curvas cerradas. Fuera de un imán van de N a S, y dentro de él de S a N. Esto refleja que **no existen monopolos magnéticos**: si se corta un imán por la mitad, se obtienen dos imanes, cada uno con su polo N y su polo S.

El **flujo magnético** a través de una superficie se define en analogía con el flujo eléctrico de la Clase 03:
$$\Phi_B = \int \vec{B}\cdot d\vec{A}, \qquad [\Phi_B] = \text{T}\cdot\text{m}^{2} = \text{Wb (weber)}.$$
Para una superficie plana de área $A$ en un campo uniforme que forma un ángulo $\phi$ con la normal, $\Phi_B = BA\cos\phi$.

Como toda línea que entra a una superficie cerrada también sale de ella, el flujo neto a través de **cualquier superficie cerrada** es nulo. Esta es la **ley de Gauss para el magnetismo**:
$$\boxed{\oint_S \vec{B}\cdot d\vec{A} = 0}\qquad\Longleftrightarrow\qquad \nabla\cdot\vec{B}=0 \;\;(\text{forma diferencial, cf. Clase 04}).$$
Es el análogo de $\oint\vec{E}\cdot d\vec{A} = Q_{\text{enc}}/\varepsilon_0$, con "carga magnética encerrada" siempre igual a cero.

## Fuerza sobre conductores con corriente

Una corriente es un conjunto de cargas en movimiento (Clase 08), así que un conductor con corriente dentro de un campo magnético experimenta una fuerza: la suma de las fuerzas $q\vec{v}_d\times\vec{B}$ sobre los portadores.

**Deducción.** Se considera un tramo recto de longitud $L$ y sección $A$, con $n$ portadores por unidad de volumen, cada uno de carga $q$ y velocidad de deriva $\vec{v}_d$. El número de portadores es $nAL$, así que la fuerza total es
$$\vec{F}_B = (q\,\vec{v}_d\times\vec{B})\,nAL.$$
Como $I = nqv_dA$ (Clase 08), y definiendo $\vec{L}$ como el vector de módulo $L$ en la dirección de la corriente:

$$\boxed{\vec{F}_B = I\,\vec{L}\times\vec{B}}$$

donde $\vec{L}$ apunta en la dirección de la corriente y $|\vec{L}|=L$. El módulo es $F_B = ILB\sin\theta$.

> **[Figura]:** Un alambre vertical pasa entre los polos de un imán de herradura, con $\vec{B}$ horizontal. Los tres paneles siguientes muestran el alambre con $\vec{B}_{\text{in}}$ entrando en la hoja ($\times$). (1) Con $I=0$ el alambre queda recto. (2) Con la corriente hacia arriba, el alambre se curva hacia la **izquierda**, porque $\hat{\jmath}\times(-\hat{k}) = -\hat{\imath}$. (3) Con la corriente hacia abajo, se curva hacia la **derecha**.

### Forma general

Si un hilo de forma arbitraria con corriente $I$ está en un campo magnético cualquiera, la fuerza sobre un elemento muy pequeño de longitud $d\vec{s}$ es

$$d\vec{F}_B = I\,d\vec{s}\times\vec{B}.$$

Para obtener la fuerza sobre todo el hilo hay que integrar a lo largo de él:

$$\boxed{\vec{F}_B = I\int_a^b d\vec{s}\times\vec{B}}$$

donde $a$ y $b$ son los extremos del hilo. Hay que tener cuidado, porque a lo largo de la integración pueden variar tanto la magnitud como la dirección de $\vec{B}$. Esta expresión también se escribe $\vec{F}=\int I\,d\vec{l}\times\vec{B}$.

### Dos casos posibles en un campo uniforme

Si $\vec{B}$ es **uniforme**, sale de la integral.

**Caso 1: hilo con extremos distintos.**
$$\vec{F}_B = I\left(\int_a^b d\vec{s}\right)\times\vec{B}.$$
La integral es la suma vectorial de todos los desplazamientos a lo largo del hilo, es decir, el vector $\vec{L}'$ dirigido **de $a$ a $b$**:
$$\boxed{\vec{F}_B = I\,\vec{L}'\times\vec{B}}$$
Por lo tanto, la fuerza sobre un hilo curvo en un campo uniforme es igual a la fuerza sobre un hilo **recto** que une sus extremos.

> **[Figura]:** Un hilo curvo y ondulado va del punto $a$ al punto $b$ y lleva una corriente $I$. Los elementos $d\vec{s}$ son tangentes al hilo. Hay líneas paralelas de $\vec{B}$ uniforme que apuntan hacia la derecha y algo hacia arriba. El vector recto $\vec{L}'$ une $a$ con $b$.

**Caso 2: hilo cerrado.**
$$\vec{F}_B = I\left(\oint d\vec{s}\right)\times\vec{B}.$$
La suma vectorial de los lados de un polígono cerrado es cero, así que $\oint d\vec{s} = 0$ y
$$\boxed{\vec{F}_B = 0}$$
para **cualquier** espira cerrada en un campo uniforme, sin importar la corriente que lleve.

> **[Figura]:** Una espira cerrada de forma irregular, recorrida por la corriente $I$ y con elementos $d\vec{s}$ tangentes, dentro de un campo $\vec{B}$ uniforme de líneas paralelas oblicuas.

## Ejemplo 2: fuerza sobre un conductor semicircular

Un alambre doblado en forma de semicírculo de radio $R$ forma un circuito cerrado y lleva una corriente $I$. El alambre está en el plano $xy$, y hay un campo magnético constante en la dirección $+y$. Determine la magnitud y la dirección de la fuerza magnética sobre la porción semicircular del alambre, y muestre que la fuerza sobre el alambre completo es nula.

> **[Figura]:** Una espira formada por un diámetro horizontal de longitud $2R$, sobre el eje $x$ con el centro en el origen, y un arco semicircular de radio $R$ en el semiplano $y>0$. La corriente recorre el diámetro hacia la **derecha** ($+\hat{\imath}$) y el arco en sentido antihorario, de derecha a izquierda por arriba. El campo $\vec{B}$ es uniforme y vertical hacia arriba ($+\hat{\jmath}$).

**Resolución**

*Idea:* se usan $\vec{F}=I\vec{L}\times\vec{B}$ para el tramo recto y el Caso 1 (o la integral explícita) para el arco. Al final se comprueba el Caso 2: espira cerrada en campo uniforme implica fuerza nula.

**Tramo recto ($\vec{F}_1$).** Tiene $\vec{L} = 2R\,\hat{\imath}$, perpendicular a $\vec{B}$:
$$\vec{F}_1 = I(2R\,\hat{\imath})\times(B\,\hat{\jmath}) = 2IRB\,(\hat{\imath}\times\hat{\jmath}) = 2IRB\,\hat{k}\quad(\text{sale de la hoja}).$$

**Arco ($\vec{F}_2$).**
*Método rápido (Caso 1):* el arco va desde $(R,0)$ hasta $(-R,0)$, así que $\vec{L}' = -2R\,\hat{\imath}$ y
$$\vec{F}_2 = I(-2R\,\hat{\imath})\times(B\hat{\jmath}) = -2IRB\,\hat{k}.$$

*Método explícito (integral):* se parametriza el arco con el ángulo $\theta$, desde $\theta=0$ (extremo derecho) hasta $\theta=\pi$ (extremo izquierdo), en el sentido de la corriente. La posición es $\vec{r}=R(\cos\theta\,\hat{\imath}+\sin\theta\,\hat{\jmath})$, así que
$$d\vec{s} = R(-\sin\theta\,\hat{\imath}+\cos\theta\,\hat{\jmath})\,d\theta.$$
$$d\vec{s}\times\vec{B} = RB\,d\theta\left[-\sin\theta\,(\hat{\imath}\times\hat{\jmath}) + \cos\theta\,(\hat{\jmath}\times\hat{\jmath})\right] = -RB\sin\theta\,d\theta\,\hat{k}.$$
$$\vec{F}_2 = I\int_0^{\pi}(-RB\sin\theta)\,d\theta\,\hat{k} = -IRB\left[-\cos\theta\right]_0^{\pi}\hat{k} = -IRB\,(1+1)\,\hat{k} = -2IRB\,\hat{k}.$$

$$\boxed{\vec{F}_2 = -2IRB\,\hat{k}\quad(|\vec{F}_2| = 2IRB,\ \text{entrando a la hoja})}$$

**Fuerza total:**
$$\sum\vec{F} = \vec{F}_1+\vec{F}_2 = 2IRB\,\hat{k} - 2IRB\,\hat{k} = \boxed{0}$$

*Verificación / interpretación:* los dos métodos dan lo mismo. El resultado total es coherente con el Caso 2, porque la espira es cerrada y el campo uniforme. Notar que el arco tiene longitud $\pi R > 2R$, pero recibe la misma fuerza que el diámetro: los elementos cerca de los extremos, casi paralelos a $\vec{B}$, aportan poco. Las fuerzas se cancelan, pero como actúan en puntos distintos pueden producir un **torque**, que es el tema de la sección siguiente.

## Torque sobre una espira de corriente

Aunque la fuerza neta sobre una espira en un campo uniforme es cero, el **torque neto en general no lo es**. Esta es la base del motor eléctrico y del galvanómetro.

**Deducción para una espira rectangular.** Se considera una espira de lados $a$ y $b$ con corriente $I$, que puede girar en torno al eje $y$. Sea $\phi$ el ángulo entre la **normal** a la espira y $\vec{B}$ (uniforme, en $+z$).

> **[Figura]:** (a) Espira rectangular inclinada, con lados $a$ paralelos al eje $y$ de giro y lados $b$ perpendiculares a él. $\vec{B}$ apunta hacia arriba ($+z$), y el momento magnético $\vec{\mu}$ es normal a la espira y forma un ángulo $\phi$ con $\vec{B}$. Sobre los lados $a$ actúan $\vec{F}$ y $-\vec{F}$, horizontales, de sentidos opuestos y con líneas de acción distintas. Sobre los lados $b$ actúan $\vec{F}'$ y $-\vec{F}'$, colineales (a lo largo de $y$). (b) Si $\phi = 90^\circ$, $\vec{B}$ queda en el plano de la espira y el torque es máximo. (c) Si $\phi=0^\circ$, $\vec{\mu}\parallel\vec{B}$ y el torque es cero: es el equilibrio estable. Con $\phi=180^\circ$ el equilibrio es inestable.

1. Las fuerzas $\vec{F}'$ y $-\vec{F}'$ sobre los lados $b$ son colineales, así que no producen torque respecto de ningún punto.
2. Los lados $a$ son perpendiculares a $\vec{B}$, de modo que cada uno recibe una fuerza de módulo $F = IaB$, con sentidos opuestos y líneas de acción distintas.
3. El brazo de palanca de cada una respecto del eje $y$ es $(b/2)\sin\phi$. Ambos torques apuntan en $+y$, así que se suman:
$$\tau = 2F\,\frac{b}{2}\sin\phi = (IBa)(b\sin\phi).$$
4. Como el área es $A = ab$:
$$\boxed{\tau = IBA\sin\phi}$$

- El torque es **máximo** con $\phi = 90^\circ$, es decir, cuando $\vec{B}$ está en el plano de la espira.
- El torque es **cero** con $\phi = 0^\circ$ o $180^\circ$, es decir, cuando la normal es paralela o antiparalela a $\vec{B}$.
- $\phi=0^\circ$ es un equilibrio **estable**: si la espira se aparta un poco, el torque la devuelve.
- $\phi=180^\circ$ es un equilibrio **inestable**: si se aparta un poco, la espira se aleja aún más.
- Como la fuerza neta es cero, el resultado vale para **cualquier** elección de eje.

## Momento dipolar magnético

El **momento dipolar magnético** $\vec{\mu}$ de una espira con corriente $I$ se define como

$$\boxed{\vec{\mu} = I\vec{A}}$$

donde el vector área $\vec{A}$ es perpendicular al plano de la espira y su módulo es el área de la espira. Su sentido se obtiene con la regla de la mano derecha: si los dedos siguen la corriente, el pulgar indica $\hat{n}$. En el S.I., $\vec{\mu}$ se mide en $\text{A}\cdot\text{m}^{2}$.

Con esta definición, el resultado anterior ($\tau = IAB\sin\phi = \mu B\sin\phi$) toma forma vectorial. El **torque** sobre una espira de corriente en un campo $\vec{B}$ es

$$\boxed{\vec{\tau} = \vec{\mu}\times\vec{B}}$$

Esta forma es análoga a $\vec{\tau}=\vec{p}\times\vec{E}$ para un dipolo eléctrico (Clase 07).

La **energía potencial** de un dipolo magnético en un campo magnético depende de su orientación:

$$\boxed{U = -\vec{\mu}\cdot\vec{B} = -\mu B\cos\phi}$$

*Justificación:* el trabajo que hay que realizar para girar el dipolo de $\phi_0$ a $\phi$ es $\int_{\phi_0}^{\phi}\mu B\sin\phi'\,d\phi' = -\mu B\cos\phi + \mu B\cos\phi_0$. Si se elige $U=0$ en $\phi = 90^\circ$, resulta $U = -\mu B\cos\phi$. La energía es mínima, $-\mu B$, cuando $\vec{\mu}\parallel\vec{B}$ (equilibrio estable) y máxima, $+\mu B$, cuando son antiparalelos (equilibrio inestable).

**Bobinas.** Es común encontrar espiras de $N$ vueltas (bobinas). Cada vuelta aporta el mismo momento, así que el momento total se multiplica por $N$:
$$\vec{\mu}_{\text{bobina}} = N\,\vec{\mu}_{\text{espira}} = N I A\,\hat{n}.$$

## Ejemplo 3: momento dipolar de una bobina

Una bobina rectangular de $5{,}40\,\text{cm}\times 8{,}50\,\text{cm}$ tiene $25$ vueltas de alambre y lleva una corriente de $15{,}0\,\text{mA}$. Se aplica un campo magnético de magnitud $0{,}350\,\text{T}$ paralelo al plano de la espira.

a) Calcule la magnitud del momento dipolar.
b) ¿Cuál es la magnitud del torque que actúa sobre la espira?

**Resolución**

*Idea:* se usa la definición $\mu = NIA$ para una bobina de $N$ vueltas y luego $\vec{\tau}=\vec{\mu}\times\vec{B}$. Si $\vec{B}$ es paralelo al plano de la espira, entonces es **perpendicular** a $\hat{n}$, por lo que $\phi = 90^\circ$ y el torque es máximo.

**a)** Se convierten las unidades al S.I.: $I = 15{,}0\times10^{-3}\,\text{A}$ y $A = (0{,}0540\,\text{m})(0{,}0850\,\text{m}) = 4{,}59\times10^{-3}\,\text{m}^{2}$.
$$\mu = NIA = (25)(15{,}0\times10^{-3}\,\text{A})(4{,}59\times10^{-3}\,\text{m}^{2}) = 1{,}72\times10^{-3}\,\text{A}\cdot\text{m}^{2}.$$
$$\boxed{\mu_{\text{bobina}} \approx 1{,}72\times10^{-3}\,\text{A}\cdot\text{m}^{2}}$$

**b)** Con $\phi = 90^\circ$, $\sin\phi = 1$:
$$\tau = \mu B\sin90^\circ = (1{,}72\times10^{-3}\,\text{A}\cdot\text{m}^{2})(0{,}350\,\text{T}) = 6{,}02\times10^{-4}\,\text{N}\cdot\text{m}.$$
$$\boxed{\tau \approx 6{,}02\times10^{-4}\,\text{N}\cdot\text{m}}$$

*Verificación / interpretación:* unidades, $\text{A}\cdot\text{m}^{2}\cdot\text{T} = \text{A}\cdot\text{m}^{2}\cdot\frac{\text{N}}{\text{A}\cdot\text{m}} = \text{N}\cdot\text{m}$ ✓. Es el torque máximo posible para esta bobina en este campo. El torque tiende a girar la bobina hasta que $\vec{\mu}$ quede alineado con $\vec{B}$; en esa posición, el torque y la energía $U=-\mu B$ alcanzan su mínimo.

## Movimiento de una carga en un campo magnético uniforme

### Movimiento circular

Se considera una partícula de masa $m$ y carga $q$ cuya velocidad inicial es **perpendicular** a un campo $\vec{B}$ uniforme. La fuerza $q\vec{v}\times\vec{B}$ tiene módulo constante, $|q|vB$, y es siempre perpendicular a $\vec{v}$. Como no realiza trabajo, la rapidez es constante. Por lo tanto, la partícula describe una **circunferencia** en un plano perpendicular a $\vec{B}$, con rapidez constante.

> **[Figura]:** Un campo $\vec{B}$ entra en la hoja ($\times$). Una carga positiva parte del punto $O$ con $\vec{v}$ hacia la derecha y $\vec{F}$ hacia arriba. En los puntos $P$ y $S$ de la órbita, $\vec{v}$ es tangente y $\vec{F}$ apunta siempre al centro de la circunferencia de radio $R$. Para $q>0$, el giro es antihorario; para $q<0$ sería horario.

Por la segunda ley de Newton, con aceleración centrípeta $v^{2}/R$:
$$|q|vB = m\frac{v^{2}}{R}\;\Longrightarrow\;\boxed{R = \frac{mv}{|q|B}} = \frac{p}{|q|B}.$$

La rapidez angular, con $v = R\omega$, es
$$\boxed{\omega_c = \frac{v}{R} = \frac{|q|B}{m}}$$
y la llamamos **frecuencia del ciclotrón**. El periodo y la frecuencia son
$$\boxed{T = \frac{2\pi}{\omega_c} = \frac{2\pi m}{|q|B}}, \qquad f = \frac{\omega_c}{2\pi} = \frac{|q|B}{2\pi m}.$$

**Estas magnitudes no dependen del radio ni de la rapidez.** Una partícula más rápida describe un círculo más grande, pero tarda lo mismo en dar una vuelta. Este hecho se aprovecha en el **ciclotrón**, un acelerador en el que las partículas reciben un impulso dos veces por revolución: su energía y su radio aumentan, pero su frecuencia no cambia. También se aprovecha en el **magnetrón** de los hornos de microondas y los radares, que emite radiación con la frecuencia del movimiento circular de los electrones.

### Movimiento helicoidal

Si la velocidad tiene una componente **paralela** a $\vec{B}$, el movimiento es **helicoidal**. Se descompone $\vec{v} = \vec{v}_\parallel + \vec{v}_\perp$:

- $\vec{v}_\parallel$ no sufre fuerza, porque $\vec{v}_\parallel\times\vec{B}=0$, y se mantiene constante: es un movimiento uniforme a lo largo de $\vec{B}$.
- $\vec{v}_\perp$ produce un movimiento circular en el plano perpendicular, con
$$R = \frac{m v_\perp}{|q|B},\qquad \omega_c = \frac{|q|B}{m},\qquad T=\frac{2\pi m}{|q|B}.$$

La combinación de ambos es una hélice con eje paralelo a $\vec{B}$. La distancia que avanza la partícula a lo largo del eje en cada vuelta es el **paso (avance) de la hélice**:
$$\boxed{p = v_\parallel\,T = \frac{2\pi m\,v_\parallel}{|q|B}}$$

> **[Figura]:** Un campo $\vec{B}$ uniforme apunta a lo largo de $+x$. Una carga $q$ positiva tiene una velocidad $\vec{v}$ con componentes $v_\parallel$ (a lo largo de $x$) y $v_\perp$ (en el plano $yz$), y describe una hélice cuyo eje es paralelo al eje $x$.

En campos **no uniformes** el movimiento es más complejo. Por ejemplo, entre dos bobinas separadas las partículas pueden quedar rebotando de un extremo a otro (**botella magnética**), un mecanismo que se usa para confinar plasmas. Algo similar ocurre en los cinturones de Van Allen terrestres, que dan origen a las auroras.

**Estrategia de resolución:** si la partícula se mueve perpendicular a un $\vec{B}$ uniforme, se usan $R$ y $\omega_c$. Si la trayectoria es más compleja, por ejemplo con campos eléctricos y magnéticos a la vez, se aplica $\sum\vec{F} = m\vec{a}$ por componentes.

## Ejemplo: electrones en un horno de microondas

El magnetrón de un horno de microondas emite ondas electromagnéticas de frecuencia $f = 2450\,\text{MHz}$. ¿Qué intensidad de campo magnético se necesita para que los electrones describan trayectorias circulares con esta frecuencia?

**Resolución**

*Idea:* la frecuencia del ciclotrón, $\omega_c = |q|B/m$, relaciona directamente $f$ con $B$, sin necesidad de conocer la rapidez ni el radio.

Primero se calcula la rapidez angular:
$$\omega = 2\pi f = 2\pi(2450\times10^{6}\,\text{s}^{-1}) = 1{,}54\times10^{10}\,\text{s}^{-1}.$$
Se despeja $B$ de $\omega = |q|B/m$:
$$B = \frac{m\omega}{|q|} = \frac{(9{,}11\times10^{-31}\,\text{kg})(1{,}54\times10^{10}\,\text{s}^{-1})}{1{,}60\times10^{-19}\,\text{C}}.$$
$$\boxed{B \approx 0{,}0877\,\text{T}}$$

*Verificación / interpretación:* unidades, $\text{kg}\cdot\text{s}^{-1}/\text{C} = \text{T}$, ya que $\text{T} = \text{N}\cdot\text{s}/(\text{C}\cdot\text{m}) = \text{kg}/(\text{C}\cdot\text{s})$ ✓. Es un campo moderado, que un imán permanente produce con facilidad. Las ondas de 2450 MHz son absorbidas fuertemente por las moléculas de agua, por eso sirven para calentar alimentos.

## Ejemplo: movimiento helicoidal de un protón

En una situación como la de la figura de movimiento helicoidal, la partícula cargada es un protón ($q=1{,}60\times10^{-19}\,\text{C}$, $m=1{,}67\times10^{-27}\,\text{kg}$) y el campo magnético uniforme está dirigido a lo largo del eje $x$, con magnitud $0{,}500\,\text{T}$. Solo la fuerza magnética actúa sobre el protón. En $t=0$, el protón tiene componentes de velocidad $v_x = 1{,}50\times10^{5}\,\text{m/s}$, $v_y = 0$ y $v_z = 2{,}00\times10^{5}\,\text{m/s}$.

a) En $t=0$, calcule la fuerza sobre el protón y su aceleración.
b) Encuentre el radio de la trayectoria helicoidal, la rapidez angular del protón y el avance de la hélice (distancia recorrida a lo largo del eje de la hélice en cada revolución).

**Resolución**

*Idea:* se usan $\vec{F}=q\vec{v}\times\vec{B}$ y $\vec{F}=m\vec{a}$. Luego se descompone la velocidad respecto de $\vec{B}$: $v_\parallel = v_x$, que es constante, y $v_\perp = v_z$, que genera el giro. Con esto se aplican $R = mv_\perp/|q|B$, $\omega_c=|q|B/m$ y $p = v_\parallel T$.

**a) Fuerza y aceleración.** $\vec{v} = v_x\hat{\imath} + v_z\hat{k}$ y $\vec{B} = B\hat{\imath}$:
$$\vec{F} = q(v_x\hat{\imath} + v_z\hat{k})\times B\hat{\imath} = qv_xB\,(\hat{\imath}\times\hat{\imath}) + qv_zB\,(\hat{k}\times\hat{\imath}) = qv_zB\,\hat{\jmath}.$$
$$\vec{F} = (1{,}60\times10^{-19}\,\text{C})(2{,}00\times10^{5}\,\text{m/s})(0{,}500\,\text{T})\,\hat{\jmath}.$$
$$\boxed{\vec{F} = (1{,}60\times10^{-14}\,\text{N})\,\hat{\jmath}}$$
$$\vec{a} = \frac{\vec{F}}{m} = \frac{1{,}60\times10^{-14}\,\text{N}}{1{,}67\times10^{-27}\,\text{kg}}\,\hat{\jmath}$$
$$\boxed{\vec{a} \approx (9{,}58\times10^{12}\,\text{m/s}^{2})\,\hat{\jmath}}$$

**b) Radio.** La componente de la velocidad perpendicular a $\vec{B}$ es $v_z$:
$$R = \frac{m v_z}{|q|B} = \frac{(1{,}67\times10^{-27}\,\text{kg})(2{,}00\times10^{5}\,\text{m/s})}{(1{,}60\times10^{-19}\,\text{C})(0{,}500\,\text{T})} = \frac{3{,}34\times10^{-22}}{8{,}00\times10^{-20}}\,\text{m}.$$
$$\boxed{R \approx 4{,}18\times10^{-3}\,\text{m} = 4{,}18\,\text{mm}}$$

**Rapidez angular:**
$$\omega = \frac{|q|B}{m} = \frac{(1{,}60\times10^{-19}\,\text{C})(0{,}500\,\text{T})}{1{,}67\times10^{-27}\,\text{kg}}$$
$$\boxed{\omega \approx 4{,}79\times10^{7}\,\text{rad/s}}$$

**Avance de la hélice.** El periodo es
$$T = \frac{2\pi}{\omega} = \frac{2\pi}{4{,}79\times10^{7}\,\text{s}^{-1}} = 1{,}31\times10^{-7}\,\text{s}.$$
Durante ese tiempo, el protón avanza a lo largo de $x$ con $v_\parallel = v_x$ constante:
$$p = v_xT = (1{,}50\times10^{5}\,\text{m/s})(1{,}31\times10^{-7}\,\text{s})$$
$$\boxed{p \approx 1{,}97\times10^{-2}\,\text{m} = 19{,}7\,\text{mm}}$$

*Verificación / interpretación:* la fuerza, de apenas $10^{-14}\,\text{N}$, produce una aceleración enorme porque la masa del protón es muy pequeña. La fuerza es perpendicular a $\vec{v}$ y a $\vec{B}$: $\vec{F}\cdot\vec{v} = 0$ ✓. El avance es casi cinco veces el radio, así que la hélice está bastante "estirada". Unidades de $R$: $\dfrac{\text{kg}\cdot\text{m/s}}{\text{C}\cdot\text{T}} = \text{m}$, porque $\text{C}\cdot\text{T} = \text{kg}/\text{s}$ ✓.

## Campo magnético de una carga en movimiento (introducción a Biot-Savart)

Hasta aquí estudiamos el efecto de $\vec{B}$ sobre las cargas. Ahora vemos cómo las cargas en movimiento **generan** $\vec{B}$; el tema se desarrolla en la Clase 11.

Llamamos **punto de fuente** a la posición de la carga y **punto de campo** al punto $P$ donde se calcula el campo. Como ocurre con $\vec{E}$ (Clase 02), los experimentos muestran que la magnitud de $\vec{B}$ es proporcional a $|q|$ y a $1/r^{2}$. Pero la dirección de $\vec{B}$ **no** va a lo largo de la línea que une el punto de fuente con el punto de campo: $\vec{B}$ es perpendicular al plano que contiene esa línea y la velocidad $\vec{v}$. Además, $B$ es proporcional a $v\sin\phi$, donde $\phi$ es el ángulo entre $\vec{v}$ y $\vec{r}$:

$$B = \frac{\mu_0}{4\pi}\frac{|q|\,v\sin\phi}{r^{2}}, \qquad \boxed{\vec{B} = \frac{\mu_0}{4\pi}\,\frac{q\,\vec{v}\times\hat{r}}{r^{2}}}$$

donde $\hat{r} = \vec{r}/r$ apunta del punto de fuente al punto de campo.

> **[Figura]:** (a) Vista en perspectiva de una carga $+q$ que se mueve con $\vec{v}$. En varios puntos alrededor, $\vec{B}$ es perpendicular al plano formado por $\vec{r}$ y $\vec{v}$. Sobre la línea de $\vec{v}$ (delante y detrás de la carga), $B=0$, porque $\sin\phi=0$. El campo es máximo en el plano perpendicular a $\vec{v}$ que pasa por la carga. (b) Vista desde atrás de la carga, que se aleja del lector ($\otimes$): las líneas de $\vec{B}$ son **círculos concéntricos** centrados en la línea de movimiento y recorridos en sentido horario.

**Regla de la mano derecha para el campo generado:** se apunta el pulgar en la dirección de $\vec{v}$ (o de la corriente), y los dedos al cerrarse indican el sentido de las líneas de $\vec{B}$. Si la carga es negativa, el sentido se invierte.

### Ley de Biot-Savart

La ley de Biot-Savart da el campo $d\vec{B}$ en un punto $P$ debido a un elemento de longitud $d\vec{s}$ que lleva una corriente $I$. Se obtiene sustituyendo $q\vec{v}\to I\,d\vec{s}$:

$$\boxed{d\vec{B} = \frac{\mu_0}{4\pi}\,\frac{I\,d\vec{s}\times\hat{r}}{r^{2}}}$$

donde $\mu_0$ es la **permeabilidad del vacío**, $r$ es la distancia del elemento a $P$ y $\hat{r}$ es el vector unitario que apunta de $d\vec{s}$ hacia $P$. Con esta ley se puede calcular el campo de cualquier cable con corriente.

En el S.I., la permeabilidad vale
$$\mu_0 = 4\pi\times10^{-7}\,\text{T}\cdot\text{m/A},$$
y tiene la particularidad de que
$$\varepsilon_0\,\mu_0 = \frac{1}{c^{2}},$$
donde $c$ es la rapidez de la luz. Esta relación es un primer indicio de que la luz es una onda electromagnética.

## Ejemplo: campo de un conductor infinito con corriente

Calcule el campo magnético generado por un conductor rectilíneo infinito que lleva una corriente $I$.

**Resolución**

*Idea:* se aplica la ley de Biot-Savart, sumando las contribuciones $d\vec{B}$ de todos los elementos del hilo. Por simetría, todas apuntan en la misma dirección, así que basta integrar el módulo.

**Geometría.** El hilo está sobre el eje $z$, con la corriente en $+\hat{k}$. El punto $P$ está a una distancia perpendicular $s$ del hilo, sobre el eje $x$: $P=(s,0,0)$. Un elemento en $(0,0,z)$ tiene $d\vec{s} = dz\,\hat{k}$, y el vector del elemento a $P$ es
$$\vec{r} = s\,\hat{\imath} - z\,\hat{k}, \qquad r = \sqrt{s^{2}+z^{2}}.$$

**Producto cruz:**
$$d\vec{s}\times\vec{r} = dz\,\hat{k}\times(s\,\hat{\imath} - z\,\hat{k}) = s\,dz\,(\hat{k}\times\hat{\imath}) = s\,dz\,\hat{\jmath}.$$
Todos los elementos dan $d\vec{B}$ en $+\hat{\jmath}$, que en $P$ coincide con la dirección azimutal $\hat{\phi}$, tangente a una circunferencia centrada en el hilo.

**Integración.** Con $\hat{r}/r^{2} = \vec{r}/r^{3}$:
$$B = \frac{\mu_0 I}{4\pi}\int_{-\infty}^{\infty}\frac{s\,dz}{(s^{2}+z^{2})^{3/2}}.$$
Se usa la sustitución $z = s\tan\alpha$, de modo que $dz = s\sec^{2}\alpha\,d\alpha$ y $(s^{2}+z^{2})^{3/2} = s^{3}\sec^{3}\alpha$. Los límites pasan a ser $\alpha\in(-\pi/2,\pi/2)$:
$$\int_{-\infty}^{\infty}\frac{s\,dz}{(s^{2}+z^{2})^{3/2}} = \int_{-\pi/2}^{\pi/2}\frac{s\cdot s\sec^{2}\alpha}{s^{3}\sec^{3}\alpha}\,d\alpha = \frac{1}{s}\int_{-\pi/2}^{\pi/2}\cos\alpha\,d\alpha = \frac{2}{s}.$$
Por lo tanto,
$$\boxed{\vec{B} = \frac{\mu_0 I}{2\pi s}\,\hat{\phi}}$$

*Verificación / interpretación:* el campo disminuye como $1/s$, más lentamente que el de una carga puntual ($1/r^{2}$), como ocurría con el campo eléctrico de una línea infinita de carga, $\lambda/(2\pi\varepsilon_0 s)$ (Clase 03). Unidades: $\dfrac{\text{T}\cdot\text{m/A}\cdot\text{A}}{\text{m}} = \text{T}$ ✓. **Dirección (regla de la mano derecha):** con el pulgar en la dirección de la corriente, los dedos se cierran en el sentido de las líneas de $\vec{B}$, que son **circunferencias concéntricas** alrededor del hilo. Por ejemplo, con $I = 10\,\text{A}$ y $s = 1\,\text{cm}$: $B = \frac{(4\pi\times10^{-7})(10)}{2\pi(0{,}01)} = 2\times10^{-4}\,\text{T}$, unas cuatro veces el campo terrestre.

**Evidencia experimental:** si se espolvorean limaduras de hierro sobre una cartulina atravesada perpendicularmente por un conductor con corriente, las limaduras se ordenan en **círculos concéntricos** alrededor del conductor. Esto confirma que las líneas de campo magnético rodean la corriente.

## Resumen de fórmulas

| Concepto | Fórmula |
|---|---|
| Fuerza magnética sobre una carga | $\vec{F}_B = q\vec{v}\times\vec{B}$, $\;F_B = \lvert q\rvert vB\sin\theta$ |
| Fuerza de Lorentz | $\vec{F} = q(\vec{E}+\vec{v}\times\vec{B})$ |
| Unidades | $1\,\text{T} = 1\,\text{N}/(\text{A}\cdot\text{m}) = 10^{4}\,\text{G}$ |
| Flujo magnético / Gauss magnético | $\Phi_B=\int\vec{B}\cdot d\vec{A}$ [Wb], $\;\oint\vec{B}\cdot d\vec{A}=0$ |
| Fuerza sobre un conductor recto | $\vec{F}_B = I\vec{L}\times\vec{B}$ |
| Fuerza sobre un conductor arbitrario | $\vec{F}_B = I\int_a^b d\vec{s}\times\vec{B}$ |
| Campo uniforme: hilo abierto / espira cerrada | $\vec{F}_B = I\vec{L}'\times\vec{B}$ ($a\to b$) / $\vec{F}_B = 0$ |
| Torque sobre una espira | $\tau = IAB\sin\phi$, $\;\vec{\tau}=\vec{\mu}\times\vec{B}$ |
| Momento dipolar magnético | $\vec{\mu} = NIA\,\hat{n}$ [$\text{A}\cdot\text{m}^2$] |
| Energía potencial de un dipolo | $U = -\vec{\mu}\cdot\vec{B}$ |
| Radio de la órbita | $R = \dfrac{m v_\perp}{\lvert q\rvert B}$ |
| Frecuencia del ciclotrón y periodo | $\omega_c = \dfrac{\lvert q\rvert B}{m}$, $\;T = \dfrac{2\pi m}{\lvert q\rvert B}$, $\;f=\dfrac{\omega_c}{2\pi}$ |
| Paso de la hélice | $p = v_\parallel T$ |
| Selector de velocidades | $v = E/B$ |
| Espectrómetro de masas | $m = \dfrac{qB_0^{2}r^{2}}{2\Delta V}$ |
| Campo de una carga en movimiento | $\vec{B} = \dfrac{\mu_0}{4\pi}\dfrac{q\vec{v}\times\hat{r}}{r^{2}}$ |
| Ley de Biot-Savart | $d\vec{B} = \dfrac{\mu_0}{4\pi}\dfrac{I\,d\vec{s}\times\hat{r}}{r^{2}}$ |
| Conductor rectilíneo infinito | $\vec{B} = \dfrac{\mu_0 I}{2\pi s}\hat{\phi}$ |
| Constantes | $\mu_0 = 4\pi\times10^{-7}\,\text{T}\cdot\text{m/A}$, $\;\varepsilon_0\mu_0 = 1/c^{2}$ |
