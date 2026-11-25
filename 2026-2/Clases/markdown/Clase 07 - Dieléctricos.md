# Capacitores y dieléctricos

Electricidad y Magnetismo — FIS1533

## Capacitores con dieléctrico

La mayoría de los capacitores tienen un material no conductor, o **dieléctrico**, entre sus placas. Un tipo común usa tiras largas de hojas metálicas como placas, separadas por hojas de plástico (por ejemplo, Mylar); el conjunto se enrolla y forma una unidad de varios microfarads en un volumen pequeño.

> **[Figura]:** Capacitor enrollado: dos hojas metálicas (conductores) separadas por una hoja de plástico (dieléctrico), enrolladas en espiral.

Colocar un dieléctrico sólido entre las placas cumple tres funciones:

1. **Mantiene la separación entre las placas**: resuelve el problema mecánico de sostener dos hojas grandes muy cercanas sin que se toquen.
2. **Incrementa la máxima diferencia de potencial aplicable**: todo aislante se ioniza y conduce si el campo es suficientemente intenso (*ruptura del dieléctrico*); muchos dieléctricos toleran campos mayores que el aire, por lo que el capacitor soporta mayor $V$ y almacena más carga y energía.
3. **Incrementa la capacitancia**: para dimensiones dadas, $C$ es mayor con dieléctrico que con vacío.

### Constante dieléctrica

Se carga un capacitor con $\pm Q$ y se mide su diferencia de potencial $V_0$ con un electrómetro (que no permite flujo apreciable de carga). Al insertar una lámina dieléctrica sin carga, la diferencia de potencial **disminuye** a un valor $V$; al retirarla, vuelve a $V_0$, lo que muestra que la carga de las placas no cambió.

> **[Figura]:** a) Capacitor de placas paralelas en vacío con cargas $Q$ y $-Q$, conectado a un electrómetro que marca $V_0$. b) Mismo capacitor con una lámina dieléctrica entre las placas; la aguja del electrómetro marca un valor menor $V$: al agregar el dieléctrico se reduce la diferencia de potencial.

Como $C_0=Q/V_0$ y $C=Q/V$ con la misma $Q$ y $V<V_0$, se tiene $C>C_0$. Cuando el dieléctrico llena todo el espacio entre las placas, la razón se denomina **constante dieléctrica** $K$:

$$K=\frac{C}{C_0}\qquad\Longrightarrow\qquad C=KC_0.$$

Con carga constante, $Q=C_0V_0=CV$, de donde

$$V=\frac{V_0}{K}\qquad(Q\ \text{constante}).$$

$K$ es adimensional y siempre $K\ge1$ ($K=1$ para el vacío por definición). Se define la **permitividad** del material:

$$\varepsilon=K\varepsilon_0,\qquad\text{por ejemplo, placas paralelas: } C=\frac{K\varepsilon_0A}{d}=\frac{\varepsilon A}{d}.$$

**Tabla: valores de la constante dieléctrica $K$ a 20 °C**

| Material | $K$ | Material | $K$ |
|---|---|---|---|
| Vacío | 1 | Cloruro de polivinilo | 3.18 |
| Aire (1 atm) | 1.00059 | Plexiglás | 3.40 |
| Aire (100 atm) | 1.0548 | Vidrio | 5–10 |
| Teflón | 2.1 | Neopreno | 6.70 |
| Polietileno | 2.25 | Germanio | 16 |
| Benceno | 2.28 | Glicerina | 42.5 |
| Mica | 3–6 | Agua | 80.4 |
| Mylar | 3.1 | Titanato de estroncio | 310 |

Para fines prácticos, un capacitor con aire equivale a uno con vacío. El agua, pese a su $K$ grande, no es un dieléctrico práctico: es un buen solvente iónico y los iones disueltos descargarían el capacitor. Ningún dieléctrico real es un aislante perfecto: siempre existe una pequeña *corriente de fuga*.

### Ruptura del dieléctrico y rigidez dieléctrica

Si el campo es muy intenso, arranca electrones de las moléculas y estos ionizan otras moléculas en avalancha: se forma una chispa o arco y el dieléctrico se vuelve conductor. Por eso los capacitores tienen voltajes máximos nominales. La **rigidez dieléctrica** $E_m$ es el campo máximo que soporta un material sin ruptura. Para el aire seco, $E_m\approx3\times10^6$ V/m.

| Material | $K$ | Rigidez dieléctrica $E_m$ (V/m) |
|---|---|---|
| Policarbonato | 2.8 | $3\times10^7$ |
| Poliéster | 3.3 | $6\times10^7$ |
| Polipropileno | 2.2 | $7\times10^7$ |
| Poliestireno | 2.6 | $2\times10^7$ |
| Vidrio pyrex | 4.7 | $1\times10^7$ |

Ejemplo: una capa de policarbonato de 0.01 mm soporta como máximo $V_{max}=E_md=(3\times10^7\ \text{V/m})(1\times10^{-5}\ \text{m})=300$ V.

## Carga inducida y polarización

Con carga constante, $V$ disminuye en un factor $K$; como $E=V/d$, el campo entre las placas también se reduce:

$$E=\frac{E_0}{K}\qquad(Q\ \text{constante}).$$

Si el campo es menor, la densidad de carga que lo crea también debe serlo. La carga de las placas no cambió, así que en cada superficie del dieléctrico aparece una **carga inducida** de signo contrario a la de la placa adyacente. El dieléctrico sigue siendo neutro en total: las cargas inducidas resultan de la **redistribución** de cargas positivas y negativas dentro del material. Este fenómeno se llama **polarización**.

> **[Figura]:** a) Vacío: placa izquierda con $+\sigma$, derecha con $-\sigma$, campo uniforme $\vec{E}_0$ de izquierda a derecha. b) Con dieléctrico: en la cara del dieléctrico junto a la placa positiva aparece $-\sigma_i$ y en la cara junto a la negativa $+\sigma_i$; las líneas de campo dentro del dieléctrico son menos densas ($\vec{E}$ menor).

### Modelo molecular

- **Moléculas polares** (H$_2$O, N$_2$O): son dipolos permanentes. Sin campo se orientan al azar; con campo aplicado los pares de torsión (Clase 02, dipolo en un campo) tienden a alinearlas con $\vec{E}$, aunque la agitación térmica impide una alineación perfecta.
- **Moléculas no polares**: sin campo no son dipolos; el campo empuja las cargas positivas en su dirección y las negativas en sentido opuesto, creando **dipolos inducidos**.

> **[Figura]:** Moléculas polares (elipses con un extremo $+$ rojo y otro $-$ azul) orientadas al azar sin campo, y alineadas con el $+$ apuntando en la dirección de $\vec{E}$ cuando hay campo. Moléculas no polares (esferas) que, en presencia de $\vec{E}$, separan ligeramente sus cargas y se vuelven polares.

En ambos casos, la redistribución forma una capa de carga en cada superficie del material, de densidad $\pm\sigma_i$. Estas cargas no pueden moverse libremente (cada una está unida a su molécula): se llaman **cargas ligadas**, para distinguirlas de las **cargas libres** que se agregan o retiran de las placas conductoras. En el interior de un material uniformemente polarizado la carga neta por unidad de volumen sigue siendo cero.

> **[Figura]:** Bloque dieléctrico de espesor $d$ en un campo $\vec{E}$ hacia la derecha: filas de dipolos alineados ($-$ a la izquierda, $+$ a la derecha). En el interior las cargas de dipolos vecinos se cancelan; queda una capa $-\sigma_i$ en la cara izquierda y $+\sigma_i$ en la cara derecha.

> **[Figura]:** Secuencia de cuatro paneles entre placas $+\sigma$ (izquierda) y $-\sigma$ (derecha): a) sin dieléctrico, campo $E_0$; b) dieléctrico recién insertado, aún sin reacomodo de cargas; c) las cargas inducidas $-\sigma_i$ (izquierda) y $+\sigma_i$ (derecha) crean un campo opuesto (flechas delgadas hacia la izquierda) dentro del dieléctrico; d) campo resultante de magnitud $E_0/K$, más débil dentro del dieléctrico.

### Relación entre carga libre e inducida

Como la carga de las placas conductoras es la misma, $V=V_0/K$ y $E=E_0/K$. Para placas paralelas, el campo en vacío lo produce solo $\sigma$, y con dieléctrico lo produce la carga neta $\sigma-\sigma_i$ (superposición de dos láminas, Clase 03):

$$E_0=\frac{\sigma}{\varepsilon_0},\qquad E=\frac{\sigma-\sigma_i}{\varepsilon_0}.$$

Igualando $E=E_0/K$:

$$\frac{\sigma-\sigma_i}{\varepsilon_0}=\frac{\sigma}{K\varepsilon_0}\quad\Longrightarrow\quad\sigma_i=\sigma\left(1-\frac1K\right).$$

Para $K=1$ (vacío), $\sigma_i=0$; para $K\to\infty$ (comportamiento de conductor), $\sigma_i\to\sigma$ y $E\to0$. De esta forma

$$E=\frac{\sigma-\sigma_i}{\varepsilon_0}=\frac{\sigma}{K\varepsilon_0}=\frac{\sigma}{\varepsilon}.$$

## Vector polarización y cargas ligadas

*Complemento (desarrollo estándar FIS1533).* Se define el **vector polarización** $\vec{P}$ como el momento dipolar por unidad de volumen:

$$\vec{P}=\frac{d\vec{p}}{dV}=n\,\vec{p}\qquad[\text{C/m}^2],$$

donde $n$ es el número de dipolos por unidad de volumen. En un **dieléctrico lineal**, $\vec{P}$ es proporcional al campo total en el material:

$$\vec{P}=\varepsilon_0\chi_e\vec{E},\qquad K=1+\chi_e,$$

con $\chi_e$ la susceptibilidad eléctrica.

Las densidades de **carga ligada** que produce la polarización son:

$$\sigma_b=\vec{P}\cdot\hat{n}\qquad\text{(superficial, }\hat{n}\text{ normal exterior)},\qquad\rho_b=-\vec{\nabla}\cdot\vec{P}\qquad\text{(volumétrica)}.$$

Justificación: el potencial de un volumen polarizado es $V=k\int\frac{\vec{P}\cdot\hat{r}}{r^2}\,dV'$ (suma de dipolos). Usando $\vec{\nabla}'(1/r)=\hat{r}/r^2$ e integrando por partes (teorema de la divergencia),

$$V=k\oint\frac{\vec{P}\cdot\hat{n}}{r}\,dA'+k\int\frac{-\vec{\nabla}'\cdot\vec{P}}{r}\,dV',$$

que es el potencial de una carga superficial $\sigma_b=\vec{P}\cdot\hat{n}$ más una volumétrica $\rho_b=-\vec{\nabla}\cdot\vec{P}$. Si $\vec{P}$ es uniforme, $\rho_b=0$ y solo hay carga en las superficies, como en la figura del bloque.

**Conexión con el capacitor plano:** dentro del dieléctrico $\vec{P}$ es uniforme y apunta de la placa positiva a la negativa. En la cara junto a la placa negativa, $\hat{n}$ es paralelo a $\vec{P}$, luego $\sigma_b=+P$; en la otra cara, $\sigma_b=-P$. Así $P=\sigma_i$. Comprobación: $P=\varepsilon_0(K-1)E=\varepsilon_0(K-1)\dfrac{\sigma}{K\varepsilon_0}=\sigma\left(1-\dfrac1K\right)=\sigma_i$. ✓

## Vector desplazamiento eléctrico y ley de Gauss en dieléctricos

En presencia de un dieléctrico, la ley de Gauss involucra **toda** la carga, libre y ligada:

$$\vec{\nabla}\cdot(\varepsilon_0\vec{E})=\rho_{libre}+\rho_b=\rho_{libre}-\vec{\nabla}\cdot\vec{P}\quad\Longrightarrow\quad\vec{\nabla}\cdot(\varepsilon_0\vec{E}+\vec{P})=\rho_{libre}.$$

Se define el **vector desplazamiento eléctrico**

$$\vec{D}=\varepsilon_0\vec{E}+\vec{P}\qquad[\text{C/m}^2].$$

Para un dieléctrico lineal, $\vec{D}=\varepsilon_0\vec{E}+\varepsilon_0\chi_e\vec{E}=\varepsilon_0(1+\chi_e)\vec{E}=K\varepsilon_0\vec{E}=\varepsilon\vec{E}$.

La ley de Gauss generalizada (la versión de la diapositiva con $\varepsilon\vec{E}$) queda, en forma integral y diferencial:

$$\oint\varepsilon\vec{E}\cdot d\vec{A}=Q_{libre},\qquad\oint\vec{D}\cdot d\vec{A}=Q_{libre}\quad\Longleftrightarrow\quad\vec{\nabla}\cdot\vec{D}=\rho_{libre}.$$

Ventaja: solo se necesita la carga **libre** (la que controlamos en las placas), y las cargas ligadas quedan incluidas automáticamente. Receta habitual: (1) obtener $\vec{D}$ por Gauss con la carga libre; (2) $\vec{E}=\vec{D}/\varepsilon$ en cada región; (3) $V=-\int\vec{E}\cdot d\vec{l}$; (4) $C=Q/V$.

Verificación con placas paralelas: gaussiana tipo caja con una cara dentro de la placa positiva ($D=0$ dentro del conductor) y otra en el dieléctrico: $DA=\sigma A\Rightarrow D=\sigma$, $E=\sigma/(K\varepsilon_0)$, igual que antes.

## Energía almacenada con dieléctrico

La energía de un capacitor es (Clase 06)

$$U=\frac{Q^2}{2C}=\frac12CV^2=\frac12QV.$$

- Con **carga fija** (capacitor aislado), al insertar el dieléctrico $C\to KC_0$ y $U=\dfrac{Q^2}{2KC_0}=\dfrac{U_0}{K}$: la energía disminuye (el dieléctrico es atraído hacia el interior y el campo hace trabajo sobre él).
- Con **voltaje fijo** (conectado a una batería), $U=\tfrac12KC_0V^2=KU_0$: la energía aumenta (la batería entrega carga adicional).

La densidad de energía en un dieléctrico lineal es

$$u=\frac12\varepsilon E^2=\frac12K\varepsilon_0E^2=\frac12\vec{D}\cdot\vec{E}.$$

Para un capacitor plano: $u\,(Ad)=\tfrac12K\varepsilon_0\left(\tfrac{V}{d}\right)^2Ad=\tfrac12\left(\tfrac{K\varepsilon_0A}{d}\right)V^2=\tfrac12CV^2$. ✓

**Energía en el campo de un capacitor esférico (vacío).** Con $E=\dfrac{Q}{4\pi\varepsilon_0r^2}$ entre $r_a$ y $r_b$, $u=\tfrac12\varepsilon_0E^2=\dfrac{Q^2}{32\pi^2\varepsilon_0r^4}$; integrando sobre cascarones $dV=4\pi r^2dr$:

$$U=\int_{r_a}^{r_b}\frac{Q^2}{32\pi^2\varepsilon_0r^4}\,4\pi r^2\,dr=\frac{Q^2}{8\pi\varepsilon_0}\int_{r_a}^{r_b}\frac{dr}{r^2}=\frac{Q^2}{8\pi\varepsilon_0}\left(\frac1{r_a}-\frac1{r_b}\right)=\frac{Q^2}{8\pi\varepsilon_0}\,\frac{r_b-r_a}{r_ar_b}.$$

Coincide con $Q^2/(2C)$ usando $C=4\pi\varepsilon_0\dfrac{r_ar_b}{r_b-r_a}$: la energía puede asociarse a las cargas o al campo; el valor es el mismo.

**Preguntas conceptuales**

1. *Se conecta un capacitor de 4 μF con otro de 8 μF. ¿En qué conexión el de 4 μF almacena más energía que el de 8 μF? i) serie; ii) paralelo; iii) cualquiera; iv) ninguna.*
   **Resolución:** en serie ambos tienen la misma carga $Q$, y $U=Q^2/(2C)$ es mayor para el menor $C$. En paralelo tienen igual $V$, y $U=\tfrac12CV^2$ es mayor para el de 8 μF. $\boxed{\text{i) en serie}}$
2. *Un capacitor aislado de placas paralelas con cargas $\pm Q$ tiene un dieléctrico $K$. Si se retira el dieléctrico sin cambiar las cargas, ¿cómo cambia la energía? i) aumenta; ii) disminuye; iii) igual.*
   **Resolución:** $Q$ fija y $C$ disminuye de $KC_0$ a $C_0$; $U=Q^2/(2C)$ aumenta en un factor $K$. La energía extra la aporta el trabajo realizado para sacar el dieléctrico (que es atraído hacia adentro). $\boxed{\text{i) aumenta}}$

## Ejemplo 1: capacitor esférico lleno de aceite

En el capacitor esférico de la figura, el volumen entre las corazas conductoras esféricas está lleno de un aceite aislante cuya constante dieléctrica es igual a $K$. Use la ley de Gauss para encontrar la capacitancia.

> **[Figura]:** Dos corazas conductoras esféricas concéntricas. La interior tiene radio exterior $r_a$ y carga $+Q$; la exterior tiene radio interior $r_b$ y carga $-Q$. Entre ellas se dibuja una superficie gaussiana esférica de radio $r$, con $r_a<r<r_b$. (En el problema original el espacio es vacío; aquí está lleno de aceite de constante $K$.)

**Resolución**

*Idea:* no es un capacitor plano, así que se vuelve a la definición $C=Q/V_{ab}$. Se usa la ley de Gauss para dieléctricos, $\oint\vec{D}\cdot d\vec{A}=Q_{libre}$, luego $\vec{E}=\vec{D}/(K\varepsilon_0)$ y $V_{ab}=-\int\vec{E}\cdot d\vec{l}$ (Clase 05).

1. **Simetría:** la distribución es esférica, así que $\vec{D}$ es radial y su magnitud depende solo de $r$.
2. **Gauss con carga libre:** la gaussiana de radio $r$ ($r_a<r<r_b$) encierra la carga libre $+Q$ de la coraza interior (la carga ligada del aceite no se cuenta):
$$D\,(4\pi r^2)=Q\quad\Longrightarrow\quad D=\frac{Q}{4\pi r^2}.$$
3. **Campo:**
$$E=\frac{D}{K\varepsilon_0}=\frac{Q}{4\pi K\varepsilon_0r^2}.$$
Es el campo en vacío reducido por un factor $K$.
4. **Diferencia de potencial** (de la coraza interior, positiva, a la exterior):
$$V_{ab}=V_a-V_b=\int_{r_a}^{r_b}E\,dr=\frac{Q}{4\pi K\varepsilon_0}\int_{r_a}^{r_b}\frac{dr}{r^2}=\frac{Q}{4\pi K\varepsilon_0}\left(\frac1{r_a}-\frac1{r_b}\right)=\frac{Q}{4\pi K\varepsilon_0}\,\frac{r_b-r_a}{r_ar_b}.$$
5. **Capacitancia:**
$$C=\frac{Q}{V_{ab}}.$$

$$\boxed{C=4\pi K\varepsilon_0\,\frac{r_ar_b}{r_b-r_a}=K\,C_0}$$

*Verificación / interpretación:*
- Para $K=1$ se recupera el capacitor esférico en vacío, $C_0=4\pi\varepsilon_0\dfrac{r_ar_b}{r_b-r_a}$.
- Valor numérico de referencia: con $r_a=9.5$ cm y $r_b=10.5$ cm, $C_0=4\pi(8.85\times10^{-12})\dfrac{(0.095)(0.105)}{0.010}\approx1.1\times10^{-10}$ F $=110$ pF; con aceite, $C\approx K\cdot110$ pF.
- Si $d=r_b-r_a\ll r_a$, $4\pi r_ar_b\approx A$ (media geométrica de las áreas) y $C\approx K\varepsilon_0A/d$: el capacitor esférico se comporta como uno plano.
- Unidades: $\varepsilon_0\cdot$m = F. ✓

## Ejemplo 2: cilindros coaxiales parcialmente llenos

Considere dos cilindros coaxiales, el interior de radio $a$ y el exterior de radio $c$. El espacio $a<r<b$, donde $b<c$, se llena con un dieléctrico de constante $k$. Encuentre la capacidad del dispositivo por unidad de largo.

> **[Figura]:** Corte transversal: conductor cilíndrico interior de radio $a$; capa dieléctrica de constante $k$ entre $r=a$ y $r=b$; vacío entre $r=b$ y el conductor exterior de radio interior $c$. Ambos conductores son coaxiales.

**Resolución**

*Idea:* ley de Gauss para $\vec{D}$ con carga libre $\pm\lambda$ por unidad de largo en los conductores; $E=D/\varepsilon$ cambia de región a región; las caídas de potencial de cada región se suman (equivale a dos capacitores en serie, Clase 06).

1. **Simetría cilíndrica:** $\vec{D}$ es radial. Gaussiana cilíndrica de radio $r$ ($a<r<c$) y largo $L$; las tapas no aportan flujo:
$$D\,(2\pi rL)=\lambda L\quad\Longrightarrow\quad D=\frac{\lambda}{2\pi r}\qquad\text{(igual en ambas regiones)}.$$
2. **Campo por región:**
$$E_1=\frac{\lambda}{2\pi k\varepsilon_0r}\quad(a<r<b),\qquad E_2=\frac{\lambda}{2\pi\varepsilon_0r}\quad(b<r<c).$$
3. **Diferencia de potencial** entre el conductor interior y el exterior:
$$V=\int_a^bE_1\,dr+\int_b^cE_2\,dr=\frac{\lambda}{2\pi\varepsilon_0}\left[\frac1k\ln\frac ba+\ln\frac cb\right].$$
4. **Capacitancia por unidad de largo:** $\dfrac{C}{L}=\dfrac{\lambda}{V}$.

$$\boxed{\frac{C}{L}=\frac{2\pi\varepsilon_0}{\dfrac1k\ln\dfrac ba+\ln\dfrac cb}=\frac{2\pi k\varepsilon_0}{\ln\dfrac ba+k\ln\dfrac cb}}$$

*Verificación / interpretación:*
- $k=1$: $C/L=\dfrac{2\pi\varepsilon_0}{\ln(c/a)}$, el capacitor cilíndrico en vacío.
- $b=c$ (dieléctrico llena todo): $C/L=\dfrac{2\pi k\varepsilon_0}{\ln(c/a)}=kC_0/L$.
- $b=a$ (sin dieléctrico): se recupera el caso en vacío.
- La estructura $\dfrac{1}{C}=\dfrac{1}{C_1}+\dfrac{1}{C_2}$, con $C_1/L=\dfrac{2\pi k\varepsilon_0}{\ln(b/a)}$ y $C_2/L=\dfrac{2\pi\varepsilon_0}{\ln(c/b)}$, confirma que son dos capacitores en serie (misma carga, voltajes que se suman).

## Ejemplo 3: lámina dieléctrica de espesor parcial

Un capacitor de placas paralelas, con separación de placas $d$, tiene capacitancia $C_0$ en ausencia de un dieléctrico. ¿Cuál es la capacitancia cuando entre las placas se inserta una lámina de material dieléctrico con constante dieléctrica $k$ y grosor $fd$, donde $f$ es una fracción entre 0 y 1?

> **[Figura]:** a) Capacitor de placas paralelas horizontales separadas $d$; junto a la placa superior hay una lámina dieléctrica $k$ de espesor $fd$; el resto, de espesor $(1-f)d$, es aire. b) Circuito equivalente: dos capacitores en serie, $C_1$ (dieléctrico, separación $fd$) y $C_2$ (aire, separación $(1-f)d$).

**Resolución**

*Idea:* una hoja metálica infinitesimalmente delgada insertada paralela a las placas no altera la capacitancia (sus caras adquieren $\mp Q$ y el campo no cambia). Colocándola en la cara del dieléctrico, el sistema es una **combinación en serie** de dos capacitores planos (Clase 06), uno con dieléctrico ($C=kC_0$ según esta clase).

1. Capacitancias parciales:
$$C_1=\frac{k\varepsilon_0A}{fd},\qquad C_2=\frac{\varepsilon_0A}{(1-f)d}.$$
2. Serie:
$$\frac1C=\frac1{C_1}+\frac1{C_2}=\frac{fd}{k\varepsilon_0A}+\frac{(1-f)d}{\varepsilon_0A}=\frac{fd}{k\varepsilon_0A}+\frac{k(1-f)d}{k\varepsilon_0A}=\frac{f+k(1-f)}{k}\,\frac{d}{\varepsilon_0A}.$$
3. Invirtiendo y usando $C_0=\varepsilon_0A/d$:

$$\boxed{C=\frac{k}{f+k(1-f)}\,C_0}$$

*Verificación:* $f\to0$ (sin dieléctrico): $C\to C_0$. $f\to1$ (lleno): $C\to kC_0$. Para $0<f<1$, el denominador $f+k(1-f)$ está entre 1 y $k$, así que $C_0<C<kC_0$. El resultado no depende de la posición de la lámina, solo de su espesor. Alternativa con $\vec{D}$: $D=\sigma$ en todo el espacio, $V=\dfrac{\sigma}{\varepsilon_0}\left[\dfrac{fd}{k}+(1-f)d\right]$, y $C=\sigma A/V$ da el mismo resultado.

## Ejemplo 4: voltaje máximo de capacitores con dos dieléctricos

Un condensador de placas paralelas de área $A$ separadas a una distancia $d$ puede cargarse a un voltaje máximo de 30 kV cuando el material entre las placas es aire (permitividad $\varepsilon_0$). Un voltaje mayor produce ruptura en el aire. Cuando el mismo capacitor se llena con una sustancia dieléctrica de permitividad $\varepsilon_1=6\varepsilon_0$, el voltaje máximo al que se puede cargar es de 150 kV.

Calcule el voltaje máximo que se puede aplicar en cada uno de los condensadores de la figura.

> **[Figura]:** (1) Placas horizontales separadas $d$: mitad superior ($d/2$) con aire $\varepsilon_0$ y mitad inferior ($d/2$) con dieléctrico $\varepsilon_1$; las capas están **apiladas** entre las placas (en serie). (2) Placas horizontales separadas $d$: la mitad izquierda del área tiene aire $\varepsilon_0$ y la mitad derecha un bloque de dieléctrico $\varepsilon_1$ que ocupa todo el espesor $d$; las regiones están **lado a lado** (en paralelo).

**Resolución**

*Idea:* la ruptura ocurre cuando el campo en algún material supera su **rigidez dieléctrica**. Primero se obtienen los campos máximos de cada material a partir de los datos. Luego: en la configuración en serie, $D$ es continuo a través de la interfaz (Gauss con carga libre); en paralelo, ambas regiones tienen el mismo $V$ y el mismo espesor, por lo tanto el mismo $E$.

**Rigideces:** con campo uniforme $E=V/d$,
$$E_{0,max}=\frac{30\ \text{kV}}{d},\qquad E_{1,max}=\frac{150\ \text{kV}}{d}.$$

**Caso (1), capas en serie.** La componente normal de $\vec{D}$ es la misma en ambas capas ($D=\sigma_{libre}$):
$$\varepsilon_0E_0=\varepsilon_1E_1=6\varepsilon_0E_1\quad\Longrightarrow\quad E_0=6E_1.$$
El campo en el aire es 6 veces mayor. Hay que ver qué material rompe primero:
- Si el aire llega a su límite, $E_0=30\ \text{kV}/d$, entonces $E_1=5\ \text{kV}/d<150\ \text{kV}/d$: el dieléctrico resiste.
- Por lo tanto, el aire es el factor limitante.

$$V_{max}^{(1)}=E_0\frac d2+E_1\frac d2=\frac{30\ \text{kV}}{d}\cdot\frac d2+\frac{5\ \text{kV}}{d}\cdot\frac d2=15+2.5=17.5\ \text{kV}.$$

**Caso (2), regiones en paralelo.** Las dos regiones conectan las mismas placas: misma $V$, mismo espesor $d$, así que $E_0=E_1=V/d$. Rompe primero el material de menor rigidez, el aire:
$$V_{max}^{(2)}=E_{0,max}\,d=30\ \text{kV}.$$

$$\boxed{V_{max}^{(1)}=17.5\ \text{kV},\qquad V_{max}^{(2)}=30\ \text{kV}}$$

*Interpretación:* paradójicamente, agregar dieléctrico en serie **reduce** el voltaje máximo bajo los 30 kV del capacitor de aire, porque concentra el campo en la capa de aire ($E_0=6E_1$). En paralelo, el aire sigue expuesto al campo completo $V/d$ y el dieléctrico no ayuda a la ruptura (aunque sí aumenta la capacitancia). Sanity check: ambos resultados son menores que 150 kV (todo dieléctrico) y $\le30$ kV (todo aire).

## Resumen de fórmulas

| Concepto | Expresión |
|---|---|
| Constante dieléctrica | $K=C/C_0$, $\ C=KC_0$ |
| Permitividad | $\varepsilon=K\varepsilon_0$ |
| Con $Q$ constante | $V=V_0/K$, $\ E=E_0/K$ |
| Placas paralelas con dieléctrico | $C=K\varepsilon_0A/d$ |
| Carga inducida (placas) | $\sigma_i=\sigma(1-1/K)$, $\ E=(\sigma-\sigma_i)/\varepsilon_0=\sigma/(K\varepsilon_0)$ |
| Polarización (lineal) | $\vec{P}=\varepsilon_0\chi_e\vec{E}$, $\ K=1+\chi_e$ |
| Cargas ligadas | $\sigma_b=\vec{P}\cdot\hat{n}$, $\ \rho_b=-\vec{\nabla}\cdot\vec{P}$ |
| Desplazamiento eléctrico | $\vec{D}=\varepsilon_0\vec{E}+\vec{P}=\varepsilon\vec{E}$ |
| Gauss en dieléctricos | $\oint\vec{D}\cdot d\vec{A}=Q_{libre}$, $\ \vec{\nabla}\cdot\vec{D}=\rho_{libre}$ |
| Energía | $U=\dfrac{Q^2}{2C}=\tfrac12CV^2$; $\ u=\tfrac12\varepsilon E^2=\tfrac12\vec{D}\cdot\vec{E}$ |
| Esférico con dieléctrico | $C=4\pi K\varepsilon_0\dfrac{r_ar_b}{r_b-r_a}$ |
| Coaxial parcialmente lleno | $\dfrac CL=\dfrac{2\pi\varepsilon_0}{\frac1k\ln\frac ba+\ln\frac cb}$ |
| Lámina de espesor $fd$ | $C=\dfrac{k}{f+k(1-f)}C_0$ |
| Rigidez dieléctrica | $V_{max}=E_m d$ (aire: $E_m\approx3\times10^6$ V/m) |
