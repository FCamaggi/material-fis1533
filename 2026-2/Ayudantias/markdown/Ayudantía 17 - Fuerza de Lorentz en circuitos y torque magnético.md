# Ayudantía 17 — Fuerza de Lorentz en circuitos y torque magnético

> Clases relacionadas: [Clase 10 - Campo Magnetico](../../Clases/markdown/Clase%2010%20-%20Campo%20Magnetico.md)

---

## Problema 1

Suponga que la figura representa esencialmente los componentes de un espectrómetro de masas. Este aparato se usa para medir la masa de partículas cargadas. En una fuente se produce un ion de masa $m$ y carga $q$, el cual parte del reposo y es acelerado por una diferencia de potencial $\Delta V$, entrando en una sección con un campo magnético uniforme (entrando a la hoja), y un campo eléctrico deflector. Solo partículas con velocidad $\vec{v}$ constante abandonan la sección (es un selector de velocidades). Las partículas emergentes entran a una segunda región donde existe otro campo magnético (entrando a la hoja), donde ellas siguen una trayectoria circunferencial hasta estrellarse en un detector a distancia $2r$ del punto de entrada.

a) Encuentre la velocidad $\vec{v}$.  
b) Encuentre la relación entre $\vec{E}$ y $\vec{B}$.  
c) Finalmente, encuentre la masa $m$ de la partícula.

> **[Figura]:** Esquema vertical de un espectrómetro de masas dispuesto en tres etapas consecutivas de abajo hacia arriba:
> - **Región aceleradora (inferior):** Una fuente emite un ion positivo ($q > 0$) de masa $m$, inicialmente en reposo, que es acelerado hacia arriba ($+\hat{j}$) a través de una diferencia de potencial $\Delta V$.
> - **Selector de velocidades (intermedia):** Un canal recto vertical por el que ingresa el haz con velocidad $\vec{v} = v\,\hat{j}$. En él coexisten un campo magnético uniforme entrante a la hoja ($\vec{B} = -B\,\hat{k}$) y un campo eléctrico uniforme transversal hacia la derecha ($\vec{E} = E\,\hat{i}$). Las partículas que atraviesan sin desviarse emergen por una ranura colimadora superior.
> - **Cámara de deflexión / analizador (superior):** El ion ingresa a una región con un campo magnético uniforme entrante a la hoja ($\vec{B}_0 = -B_0\,\hat{k}$). La fuerza magnética curva la trayectoria en un semicírculo de radio $r$ hacia la izquierda, impactando en una placa detectora situada a una distancia $2r$ del punto de entrada.

### Solución

**Idea:** La conservación de la energía mecánica permite determinar la velocidad alcanzada tras la aceleración electrostática. En el selector de velocidades, la condición de aceleración nula (movimiento rectilíneo uniforme) exige que la fuerza eléctrica compense exactamente a la fuerza magnética de Lorentz ($\vec{F}_{\text{net}} = \vec{0}$). En la cámara de deflexión, la fuerza magnética actúa exclusivamente como fuerza centrípeta, determinando el radio de la trayectoria circular a partir del cual se despeja la masa del ion.

Se fija un sistema de coordenadas cartesiano donde $\hat{j}$ apunta en el sentido de movimiento inicial del ion (hacia arriba), $\hat{i}$ hacia la derecha y $\hat{k}$ saliendo perpendicularmente de la hoja ($\hat{k} = \hat{i} \times \hat{j}$). Por lo tanto, $\vec{B} = -B\,\hat{k}$ en el selector y $\vec{B}_0 = -B_0\,\hat{k}$ en la segunda región, con $q > 0$.

#### a) Velocidad $\vec{v}$ a la salida de la región aceleradora

Entre la fuente emisora y la entrada al selector de velocidades, el ion parte del reposo ($v_0 = 0$) y sobre él solo realiza trabajo el campo eléctrico conservativo asociado a la diferencia de potencial $\Delta V$:

$$W = \Delta K \implies q\Delta V = \frac{1}{2}mv^2 - 0$$

Despejando la rapidez $v$ y considerando que el movimiento es en dirección $+\hat{j}$:

$$\boxed{\vec{v} = \sqrt{\frac{2q\Delta V}{m}}\,\hat{j}}$$

---

#### b) Relación entre $\vec{E}$ y $\vec{B}$ en el selector de velocidades

Para que el ion continúe en línea recta con velocidad $\vec{v}$ constante, la fuerza neta de Lorentz sobre él debe ser idénticamente nula:

$$\vec{F}_{\text{net}} = q\left(\vec{E} + \vec{v} \times \vec{B}\right) = \vec{0} \implies \vec{E} = -\vec{v} \times \vec{B}$$

Calculamos el producto cruz con $\vec{v} = v\,\hat{j}$ y $\vec{B} = -B\,\hat{k}$:

$$\vec{v} \times \vec{B} = (v\,\hat{j}) \times (-B\,\hat{k}) = -vB\,(\hat{j} \times \hat{k}) = -vB\,\hat{i}$$

Por consiguiente:

$$\vec{E} = -(-vB\,\hat{i}) = vB\,\hat{i}$$

En términos de las magnitudes y reemplazando la rapidez obtenida en el inciso anterior:

$$\boxed{\vec{E} = vB\,\hat{i} \implies E = vB = B\sqrt{\frac{2q\Delta V}{m}}}$$

$$\boxed{v = \frac{E}{B}}$$

---

#### c) Determinación de la masa $m$ de la partícula

Al ingresar a la segunda región con velocidad $\vec{v} = v\,\hat{j}$ y campo magnético $\vec{B}_0 = -B_0\,\hat{k}$, la fuerza magnética ejercida sobre la partícula es:

$$\vec{F}_{B0} = q\vec{v} \times \vec{B}_0 = q(v\,\hat{j}) \times (-B_0\,\hat{k}) = -qvB_0\,\hat{i}$$

Esta fuerza apunta horizontalmente hacia la izquierda ($-\hat{i}$), perpendicular a la velocidad en todo instante, por lo que no realiza trabajo y actúa como fuerza centrípeta pura en un movimiento circular uniforme de radio $r$:

$$F_c = \frac{mv^2}{r} \implies qvB_0 = \frac{mv^2}{r} \implies r = \frac{mv}{qB_0}$$

El detector registra el impacto a una distancia diametral $2r$ del orificio de entrada. Despejando $m$:

$$m = \frac{qB_0 r}{v}$$

Reemplazando la expresión de la rapidez $v = \sqrt{\frac{2q\Delta V}{m}}$:

$$r = \frac{m}{qB_0}\sqrt{\frac{2q\Delta V}{m}} = \frac{1}{B_0}\sqrt{\frac{2m\Delta V}{q}}$$

Elevando al cuadrado y despejando la masa $m$:

$$r^2 = \frac{2m\Delta V}{qB_0^2} \implies \boxed{m = \frac{qB_0^2 r^2}{2\Delta V}}$$

Alternativamente, sustituyendo la velocidad del selector $v = \frac{E}{B}$:

$$\boxed{m = \frac{qBB_0 r}{E}}$$

**Verificación:**
- **Unidades:** En la expresión $m = \frac{qB_0^2 r^2}{2\Delta V}$, $[q] = \text{C}$, $[B_0] = \text{T} = \frac{\text{N}}{\text{A}\cdot\text{m}} = \frac{\text{N}\cdot\text{s}}{\text{C}\cdot\text{m}}$, $[r^2] = \text{m}^2$, $[\Delta V] = \text{J/C} = \text{N}\cdot\text{m/C}$.  
  $$\frac{\text{C} \cdot \left(\frac{\text{N}\cdot\text{s}}{\text{C}\cdot\text{m}}\right)^2 \cdot \text{m}^2}{\frac{\text{N}\cdot\text{m}}{\text{C}}} = \frac{\frac{\text{N}^2\cdot\text{s}^2}{\text{C}}}{\frac{\text{N}\cdot\text{m}}{\text{C}}} = \frac{\text{N}\cdot\text{s}^2}{\text{m}} = \frac{(\text{kg}\cdot\text{m/s}^2)\cdot\text{s}^2}{\text{m}} = \text{kg}$$
  La dimensión es estrictamente de masa.
- **Sentido físico:** Si la masa $m$ es mayor, la inercia del ion es mayor, el radio de curvatura $r$ aumenta a igual velocidad, lo que concuerda con $r \propto \sqrt{m}$.

---

## Problema 2

Una partícula carga $q$ y masa $m$ entra con una velocidad $v$ en un campo magnético uniforme $B$ como se muestra en la figura. ¿Cuánto tiempo transcurre entre que la carga entra y sale del campo magnético?

> **[Figura]:** Una región con campo magnético uniforme $\vec{B}$ delimitada entre las caras planas de dos piezas polares magnéticas inclinadas (polo N abajo a la izquierda y polo S arriba a la derecha). La línea de frontera forma un ángulo de $45^\circ$ respecto a la horizontal. Una partícula con carga negativa (rotulada $e^-$) viaja horizontalmente hacia la derecha con velocidad $\vec{v} = v\,\hat{i}$ e incide sobre la frontera de la región magnética formando un ángulo de $45^\circ$.

### Solución

**Idea:** La fuerza magnética $\vec{F} = q\vec{v} \times \vec{B}$ es en todo instante ortogonal al vector velocidad $\vec{v}$. Como consecuencia, la fuerza no realiza trabajo sobre la partícula ($\vec{F}\cdot\vec{v} = 0$), su energía cinética se conserva y la rapidez $v = |\vec{v}|$ permanece rigurosamente constante. En una región con campo magnético uniforme perpendicular al plano del movimiento, la trayectoria es un arco de circunferencia con rapidez constante (movimiento circular uniforme). El tiempo de tránsito es el cociente entre el ángulo total barrido $\varphi$ y la rapidez angular $\omega$.

#### 1. Cinemática del movimiento circular uniforme

La aceleración centrípeta es proporcionada exclusivamente por la fuerza magnética:

$$F_B = qvB = \frac{mv^2}{R}$$

De aquí se obtienen el radio de giro $R$, la frecuencia angular de ciclotrón $\omega$ y el período $T$:

$$R = \frac{mv}{qB}$$

$$\omega = \frac{v}{R} = \frac{qB}{m}$$

$$T = \frac{2\pi}{\omega} = \frac{2\pi m}{qB}$$

Si el arco recorrido dentro de la región magnética subtiende un ángulo $\varphi$ medido desde el centro de curvatura, el tiempo que tarda la partícula en recorrerlo es:

$$t = \frac{\varphi}{\omega} = \frac{\varphi m}{qB}$$

#### 2. Tiempo de tránsito (solución oficial)

De acuerdo con la resolución oficial, se considera que la partícula penetra perpendicularmente a la frontera rectilínea del campo magnético, describiendo una media circunferencia completa antes de reemerger al exterior por la misma frontera ($\varphi = \pi$ rad):

$$t = \frac{\pi}{\omega} = \frac{\pi m}{qB}$$

$$\boxed{t = \frac{\pi m}{qB}}$$

Nótese que este tiempo es estrictamente independiente de la velocidad $v$ de entrada.

> **Nota:** La solución oficial asume una geometría simplificada donde la partícula incide perpendicularmente a la frontera del campo, recorriendo media circunferencia ($\varphi = \pi$). En el diagrama geométrico de la Figura 2, sin embargo, la partícula ingresa con velocidad horizontal $\vec{v} = v\,\hat{i}$ incidiendo con un ángulo de $45^\circ$ respecto al plano de la frontera. Si el campo magnético estuviera saliendo/entrando a la hoja, el arco de deflexión circular entre la entrada y la salida de la frontera plana subtendería un ángulo $\varphi = 2(45^\circ) = 90^\circ = \pi/2$ (o bien $\varphi = 270^\circ = 3\pi/2$, según el signo de la carga y el sentido de $\vec{B}$), conduciendo a $t = \frac{\pi m}{2qB}$ (o $t = \frac{3\pi m}{2qB}$). Por fidelidad a la pauta oficial del curso, se conserva el resultado estándar de media circunferencia $\varphi = \pi$.

**Verificación:**
- **Unidades:** $[m] = \text{kg}$, $[q] = \text{C}$, $[B] = \frac{\text{N}\cdot\text{s}}{\text{C}\cdot\text{m}} = \frac{\text{kg}}{\text{C}\cdot\text{s}}$. Por ende, $\left[\frac{m}{qB}\right] = \frac{\text{kg}}{\text{C}\cdot (\text{kg}/(\text{C}\cdot\text{s}))} = \text{s}$, unidad de tiempo.
- **Independencia de la velocidad:** Si una partícula entra con mayor rapidez, recorre un arco de circunferencia de radio proporcionalmente mayor ($R \propto v$), de modo que la longitud del camino crece en la misma proporción que la velocidad, tardando exactamente el mismo intervalo temporal.

---

## Problema 3

Un circuito cuadrado rígido, de lado $L$ y masa $M$, está pivoteado en torno a uno de sus ejes en presencia de un campo magnético $\vec{B}$ uniforme, y el campo gravitatorio. El circuito lleva una corriente $I$ que es capaz de mantenerlo en equilibrio en un ángulo $\theta$. Encuentre el sentido y magnitud de dicha corriente.

> **[Figura]:** Una espira conductora cuadrada rígida de lado $L$ y masa $M$ suspendida en el espacio. Su lado superior coincide con un eje horizontal fijo $AA'$ sobre el cual puede rotar libremente sin roce. El plano vertical de referencia pasa por el eje $AA'$. La espira forma un ángulo $\theta$ con respecto a la vertical descendente. Un campo magnético uniforme $\vec{B} = -B\,\hat{j}$ apunta verticalmente hacia abajo, en la misma dirección que la aceleración de gravedad $\vec{g} = -g\,\hat{j}$. Se observa el sistema desde el extremo $A$ mirando hacia $A'$, de manera que el eje de giro colapsa en un punto $O$.

### Solución

**Idea:** Para que la espira permanezca en equilibrio estático en el ángulo de inclinación $\theta$, la suma de los torques de todas las fuerzas externas respecto al eje de rotación $AA'$ debe anularse ($\sum \vec{\tau}_{AA'} = \vec{0}$). Las fuerzas presentes son el peso de la espira (que genera un torque restaurador hacia la vertical) y las fuerzas magnéticas que actúan sobre cada tramo conductor con corriente sumergido en el campo $\vec{B}$.

#### 1. Sistema de coordenadas y vectores directores

Se define un sistema coordenado cartesiano adaptado a la vista de perfil (mirando desde $A$ hacia $A'$):
- El eje $O$ coincide con el eje de rotación $AA'$.
- $\hat{i}$ horizontal en el plano de la figura, apuntando hacia la derecha (hacia donde se separa la espira de la vertical).
- $\hat{j}$ vertical hacia arriba.
- $\hat{k} = \hat{i} \times \hat{j}$ paralelo al eje de rotación, apuntando hacia afuera de la hoja (de $A'$ hacia $A$).

Bajo esta convención:
$$\vec{g} = -g\,\hat{j}, \qquad \vec{B} = -B\,\hat{j}$$

El vector unitario $\hat{d}$ que recorre el plano de la espira desde el eje $AA'$ hacia el lado inferior es:
$$\hat{d} = \sin\theta\,\hat{i} - \cos\theta\,\hat{j}$$

---

#### 2. Torque debido al peso de la espira

La masa total $M$ se distribuye uniformemente en el perímetro de la espira (o en su cuerpo rígido), por lo que su centro de masa se encuentra exactamente en su centro geométrico:

$$\vec{r}_{\text{cm}} = \frac{L}{2}\hat{d} = \frac{L}{2}\left(\sin\theta\,\hat{i} - \cos\theta\,\hat{j}\right)$$

La fuerza de gravedad neta es $\vec{F}_g = -Mg\,\hat{j}$. El torque respecto al eje $AA'$ es:

$$\vec{\tau}_g = \vec{r}_{\text{cm}} \times \vec{F}_g = \left[ \frac{L}{2}\left(\sin\theta\,\hat{i} - \cos\theta\,\hat{j}\right) \right] \times (-Mg\,\hat{j})$$

Calculando el producto cruz ($\hat{i} \times \hat{j} = \hat{k}$ y $\hat{j} \times \hat{j} = \vec{0}$):

$$\vec{\tau}_g = -\frac{MgL}{2}\sin\theta\,\hat{k}$$

Este torque apunta en $-\hat{k}$ y tiende a devolver la espira a la posición vertical ($\theta \to 0$).

---

#### 3. Fuerzas y torques magnéticos sobre los cuatro lados de la espira

La fuerza magnética sobre un elemento de alambre que conduce una corriente estacionaria $I$ sumergido en un campo magnético uniforme es $d\vec{F} = I\,d\vec{\ell} \times \vec{B}$.

1. **Lado superior (a lo largo del eje $AA'$):**  
   Este alambre coincide con el propio eje de rotación ($\vec{r} = \vec{0}$). Por lo tanto, su brazo de palanca es nulo y no produce torque:
   $$\vec{\tau}_{\text{sup}} = \vec{0}$$

2. **Lados laterales:**  
   En los alambres laterales, los elementos de longitud son paralelos a la dirección inclinada: $d\vec{\ell} \parallel \hat{d}$. Como $\vec{B} = -B\,\hat{j}$, el producto vectorial es:
   $$d\vec{\ell} \times \vec{B} \propto \hat{d} \times (-\hat{j}) = (\sin\theta\,\hat{i} - \cos\theta\,\hat{j}) \times (-\hat{j}) = -\sin\theta\,\hat{k}$$
   Las fuerzas sobre ambos alambres laterales apuntan a lo largo del eje $\hat{k}$ (paralelas al propio eje de giro $AA'$). Además, como la corriente recorre un lado bajando y el otro subiendo, estas dos fuerzas son de igual magnitud y de sentidos opuestos, cancelándose mutuamente. Dado que sus líneas de acción intersecan o son paralelas al eje, no generan componente de torque a lo largo del eje de giro $AA'$:
   $$\vec{\tau}_{\text{lat}} = \vec{0}$$

3. **Lado inferior:**  
   Este segmento se encuentra a una posición fija $\vec{r}_{\text{inf}} = L\,\hat{d}$ respecto al eje. Para contrarrestar el torque del peso (que apunta en $-\hat{k}$), el torque magnético debe apuntar en $+\hat{k}$.  
   Esto requiere que la fuerza magnética sobre este segmento empuje hacia la derecha ($+\hat{i}$).  
   Para que $\vec{F} = I\,\vec{L}_{\text{inf}} \times (-B\,\hat{j})$ apunte en $+\hat{i}$, requerimos que la corriente fluya en la dirección $+\hat{k}$ (de $A'$ hacia $A$):
   $$\vec{F}_{\text{inf}} = I(L\,\hat{k}) \times (-B\,\hat{j}) = -ILB\,(\hat{k} \times \hat{j}) = -ILB\,(-\hat{i}) = ILB\,\hat{i}$$

   Calculamos el torque producido por esta fuerza respecto al eje $AA'$:
   $$\vec{\tau}_B = \vec{r}_{\text{inf}} \times \vec{F}_{\text{inf}} = \left( L\,\hat{d} \right) \times (ILB\,\hat{i}) = L(\sin\theta\,\hat{i} - \cos\theta\,\hat{j}) \times (ILB\,\hat{i})$$
   Dado que $\hat{i} \times \hat{i} = \vec{0}$ y $\hat{j} \times \hat{i} = -\hat{k}$:
   $$\vec{\tau}_B = -IL^2 B\cos\theta\,(-\hat{k}) = IL^2 B\cos\theta\,\hat{k}$$

---

#### 4. Condición de equilibrio estático

Igualando la suma de torques a cero:

$$\sum \vec{\tau} = \vec{\tau}_B + \vec{\tau}_g = \vec{0}$$

$$IL^2 B\cos\theta\,\hat{k} - \frac{MgL}{2}\sin\theta\,\hat{k} = \vec{0}$$

$$IL^2 B\cos\theta = \frac{MgL}{2}\sin\theta$$

Despejando la intensidad de corriente $I$:

$$I = \frac{MgL\sin\theta}{2L^2 B\cos\theta} = \frac{Mg\tan\theta}{2LB}$$

$$\boxed{I = \frac{Mg\tan\theta}{2LB}}$$

#### 5. Sentido de la corriente

En el lado inferior, la corriente debe dirigirse en el sentido $+\hat{k}$, es decir, desde $A'$ hacia $A$.  
Por lo tanto, al recorrer la espira cerrada, la corriente circula:
- A lo largo del eje superior: de $A$ hacia $A'$.
- Bajando por el lateral derecho hacia el lado inferior.
- A lo largo del lado inferior: de $A'$ hacia $A$.
- Subiendo por el lateral izquierdo de regreso a $A$.

Visto desde el punto de vista del perfil mostrado en la pauta (mirando desde $A$ hacia $A'$), la corriente entra al plano por el lado superior ($\otimes$) y sale del plano por el lado inferior ($\odot$), lo que equivale a un sentido horario alrededor del circuito.

---

#### 6. Verificación mediante momento dipolar magnético

El momento dipolar magnético de la espira plana de área $A_{\text{esp}} = L^2$ con corriente $I$ está dado por:

$$\vec{\mu} = I A_{\text{esp}}\,\hat{n} = IL^2\,\hat{n}$$

Por la regla de la mano derecha aplicada al sentido de circulación determinado, el vector normal unitario a la espira apunta en:

$$\hat{n} = -(\cos\theta\,\hat{i} + \sin\theta\,\hat{j})$$

El torque magnético sobre el dipolo es:

$$\vec{\tau}_B = \vec{\mu} \times \vec{B} = \left[ -IL^2(\cos\theta\,\hat{i} + \sin\theta\,\hat{j}) \right] \times (-B\,\hat{j})$$

$$\vec{\tau}_B = IL^2 B\cos\theta\,(\hat{i} \times \hat{j}) = IL^2 B\cos\theta\,\hat{k}$$

Este resultado es idéntico al calculado tramo a tramo, confirmando la validez del planteamiento.

**Verificación:**
- **Unidades:** $[I] = \frac{[M][g]}{[L][B]} = \frac{\text{kg}\cdot (\text{m/s}^2)}{\text{m}\cdot (\text{N}/(\text{A}\cdot\text{m}))} = \frac{\text{N}}{\text{N}/\text{A}} = \text{A}$. Dimensionalmente correcto.
- **Límites físicos:**
  - Si $\theta \to 0$, $\tan\theta \to 0 \implies I \to 0$: para mantener la espira vertical no se requiere corriente magnética, pues el peso no produce torque respecto al eje.
  - Si $\theta \to 90^\circ$, $\tan\theta \to \infty \implies I \to \infty$: es imposible sostener la espira horizontalmente con un campo puramente vertical, ya que a $\theta = 90^\circ$ la fuerza magnética en el lado inferior se vuelve paralela al brazo de palanca y su torque se anula.

---

## Resumen de resultados

| Problema / Inciso | Expresión / Resultado | Comentarios |
| :--- | :--- | :--- |
| **P1 a)** Rapidez del ion | $\vec{v} = \sqrt{\frac{2q\Delta V}{m}}\,\hat{j}$ | Obtenida por conservación de energía en la aceleración electrostática. |
| **P1 b)** Relación de campos en el selector | $\vec{E} = vB\,\hat{i} \implies E = vB = B\sqrt{\frac{2q\Delta V}{m}}$ | Condición de fuerza de Lorentz nula ($\vec{F}_{\text{net}} = \vec{0}$). |
| **P1 c)** Masa del ion | $m = \frac{qB_0^2 r^2}{2\Delta V} = \frac{qBB_0 r}{E}$ | Determinada a partir del radio de ciclotrón $r = \frac{mv}{qB_0}$. |
| **P2** Tiempo dentro del campo magnético | $t = \frac{\pi m}{qB}$ | Solución oficial para incidencia perpendicular ($\varphi = \pi$ rad); independiente de $v$. |
| **P3** Magnitud de la corriente de equilibrio | $I = \frac{Mg\tan\theta}{2LB}$ | Equilibrio de torques $\vec{\tau}_B + \vec{\tau}_g = \vec{0}$ respecto al eje $AA'$. |
| **P3** Sentido de la corriente | De $A'$ hacia $A$ en el lado inferior | Circulación horaria vista desde el perfil $A \to A'$. |
