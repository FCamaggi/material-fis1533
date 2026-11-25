# Ayudantía 07 — Conductores en equilibrio electrostático

> Clases relacionadas: [Clase 05 - Potencial electroestático](../../Clases/markdown/Clase%2005%20-%20Potencial%20electroest%C3%A1tico.md), [Clase 06 - Condensadores](../../Clases/markdown/Clase%2006%20-%20Condensadores.md)

---

## Problema 1

Dos cavidades esféricas, de radios $a$ y $b$ están contenidas en el interior de una esfera conductora neutra de radio $R$. En el centro de cada cavidad hay una carga puntual $q_a$ y $q_b$.

a) Encuentre las densidades de carga superficiales.  
b) Obtenga el campo eléctrico fuera del conductor.  
c) Obtenga el campo eléctrico dentro de cada cavidad.

> **[Figura]:** Esfera conductora maciza de radio exterior $R$ con carga neta total cero. En su interior se aprecian dos cavidades esféricas no concéntricas: una cavidad de radio $a$ con una carga puntual $q_a$ fija en su centro exacto, y otra cavidad de radio $b$ con una carga puntual $q_b$ fija en su centro. No hay contacto eléctrico entre las cargas puntuales y las paredes conductoras.

### Solución

**Idea:** En un conductor en equilibrio electrostático, el campo eléctrico en el interior de la masa conductora es estrictamente nulo ($\vec{E} = \vec{0}$). Aplicando la ley de Gauss a superficies cerradas que transcurren por el interior del conductor se determinan las cargas inducidas en las paredes de cada cavidad. Por conservación de carga (el conductor es neutro), la carga complementaria se ubica en la superficie exterior esférica. Por el principio de apantallamiento electrostático (teorema de Faraday), el campo en el exterior se distribuye como si toda la carga exterior residiera uniformemente en una esfera de radio $R$, mientras que dentro de cada cavidad el campo está determinado únicamente por la carga puntual central.

#### Parte a) Densidades de carga superficiales

1. **Cavidad de radio $a$:**  
   Trazamos una superficie gaussiana esférica $S_1$ contenida completamente dentro del metal conductor que encierra únicamente a la cavidad de radio $a$.  
   Dado que en el interior del conductor $\vec{E} = \vec{0}$:
   $$\oint_{S_1} \vec{E}\cdot d\vec{A} = 0 \implies \frac{Q_{\text{int}}}{\varepsilon_0} = 0 \implies Q_{\text{int}} = 0$$
   La carga neta en el interior de $S_1$ es la suma de la carga puntual central $q_a$ y la carga superficial inducida en la pared interna de la cavidad $Q_a$:
   $$Q_{\text{int}} = q_a + Q_a = 0 \implies Q_a = -q_a$$
   Como la cavidad es esférica y la carga $q_a$ está en su centro, por simetría esférica la carga se distribuye uniformemente sobre el área superficial $4\pi a^2$:
   $$\boxed{\sigma_a = -\frac{q_a}{4\pi a^2}}$$

2. **Cavidad de radio $b$:**  
   Aplicando análogamente la ley de Gauss con una superficie $S_2$ contenida en el conductor que encierra a la cavidad de radio $b$:
   $$q_b + Q_b = 0 \implies Q_b = -q_b$$
   Distribuyéndose de forma homogénea sobre el área $4\pi b^2$:
   $$\boxed{\sigma_b = -\frac{q_b}{4\pi b^2}}$$

3. **Superficie exterior del conductor (radio $R$):**  
   El conductor es eléctricamente neutro en su conjunto ($Q_{\text{conductor}} = 0$).  
   La carga total del conductor es la suma de las cargas en sus tres superficies (las dos paredes internas y la frontera exterior):
   $$Q_{\text{conductor}} = Q_a + Q_b + Q_R = 0$$
   $$-q_a - q_b + Q_R = 0 \implies Q_R = q_a + q_b$$
   En virtud del apantallamiento electrostático, el campo interno es nulo en el metal, lo cual desacopla la distribución exterior de la forma o posición de las cavidades internas. Dado que la superficie externa es una esfera perfecta de radio $R$, la carga $Q_R$ se distribuye uniformemente sobre dicha esfera de área $4\pi R^2$:
   $$\boxed{\sigma_R = \frac{q_a + q_b}{4\pi R^2}}$$

---

#### Parte b) Campo eléctrico fuera del conductor ($r > R$)

Tomamos como origen de coordenadas el centro de la esfera conductora exterior de radio $R$.  
Dado que la carga en la superficie exterior se distribuye con perfecta simetría esférica y la carga neta total encerrada por una esfera gaussiana concéntrica de radio $r > R$ es $Q_{\text{total}} = q_a + q_b + Q_a + Q_b + Q_R = q_a + q_b$:
$$\oint_S \vec{E}\cdot d\vec{A} = E(r) \cdot 4\pi r^2 = \frac{q_a + q_b}{\varepsilon_0}$$

$$\boxed{\vec{E}(\vec{r}) = \frac{q_a + q_b}{4\pi\varepsilon_0 r^2}\,\hat{r} \qquad (r > R)}$$

Donde $\hat{r}$ es el vector unitario radial que apunta alejándose del centro de la esfera conductora.

---

#### Parte c) Campo eléctrico dentro de cada cavidad

El material conductor apantalla completamente el interior de cada cavidad frente a los campos eléctricos originados por la otra cavidad y por la superficie exterior.  
Asimismo, la carga superficial inducida $-q_a$ en la pared esférica de la cavidad $a$ se distribuye uniformemente, por lo que su campo en el interior de la cavidad es idénticamente nulo (por el teorema de cascarón esférico de Newton / Gauss).

Por lo tanto, el único campo presente dentro de cada cavidad proviene exclusivamente de la carga puntual ubicada en su centro:
1. **Dentro de la cavidad $a$ ($r_a < a$):**
   $$\boxed{\vec{E}_a(\vec{r}_a) = \frac{q_a}{4\pi\varepsilon_0 r_a^2}\,\hat{r}_a}$$
   donde $r_a$ es la distancia desde el centro de la cavidad $a$ hasta el punto de observación y $\hat{r}_a$ apunta radialmente hacia afuera desde dicho centro.

2. **Dentro de la cavidad $b$ ($r_b < b$):**
   $$\boxed{\vec{E}_b(\vec{r}_b) = \frac{q_b}{4\pi\varepsilon_0 r_b^2}\,\hat{r}_b}$$
   donde $r_b$ es la distancia medida desde el centro de la cavidad $b$ y $\hat{r}_b$ es el vector unitario radial asociado.

**Verificación:**
- **Condición de borde en las cavidades:** Justo en la pared interior de la cavidad $a$ ($r_a \to a^-$), el campo eléctrico normal saliente es $E_n = \frac{q_a}{4\pi\varepsilon_0 a^2}$. En el metal ($r_a \to a^+$), $E_n = 0$. La discontinuidad $\Delta E_n = 0 - \frac{q_a}{4\pi\varepsilon_0 a^2} = -\frac{q_a}{4\pi\varepsilon_0 a^2} = \frac{\sigma_a}{\varepsilon_0}$, cumpliendo la condición de salto electrostático.
- **Condición en la superficie exterior:** El salto en $r = R$ es $E_n(R^+) - E_n(R^-) = \frac{q_a + q_b}{4\pi\varepsilon_0 R^2} - 0 = \frac{\sigma_R}{\varepsilon_0}$, plenamente verificado.

---

## Problema 2

Se tiene un sistema formado por dos cascarones esféricos perfectamente conductores. El interno de radios $a_1$ y $a_2$ y el externo de radios $b_1$ y $b_2$. Los conductores son concéntricos y se encuentran inicialmente aislados y descargados. En el centro del agujero interior se encuentra una carga puntual $q$.

a) Determine las densidades de carga eléctrica inducidas en los conductores.  
b) Determine el campo eléctrico en todos los puntos del espacio.  
c) Determine el potencial eléctrico en todos los puntos del espacio.  
d) Se conectan los dos conductores a través de un cable conductor. Una vez que se restablece el equilibrio, determine la nueva distribución de carga en cada uno de los conductores y el campo eléctrico en todo el espacio.  
e) ¿Cuánto varía la energía almacenada entre $a_2$ y $b_1$ los conductores como consecuencia de la conexión?

> **[Figura]:** Dos cascarones esféricos conductores concéntricos centrados en el origen de coordenadas, donde se ubica una carga puntual $+q$. El cascarón interno tiene radio interior $a_1$ y radio exterior $a_2$. El cascarón externo tiene radio interior $b_1$ y radio exterior $b_2$, satisfaciendo $a_1 < a_2 < b_1 < b_2$. A la izquierda se ilustra una vista en corte tridimensional mostrando un cable con interruptor conectando ambos cascarones. A la derecha se aprecia la sección ecuatorial indicando los cuatro radios y la carga central $q$.

### Solución

**Idea:** La condición de equilibrio electrostático exige que $\vec{E} = \vec{0}$ en el seno de todo conductor. Mediante superficies gaussianas esféricas concéntricas que pasen por el interior de cada masa conductora se determinan las cargas inducidas. El potencial se halla integrando el campo desde el infinito ($V(\infty) = 0$). Al conectar los conductores mediante un cable, ambos forman un único conductor equipotencial, cancelándose las cargas en las caras enfrentadas. La variación de energía electrostática se evalúa mediante la integral de la densidad volumétrica de energía $u = \frac{1}{2}\varepsilon_0 E^2$.

#### Parte a) Densidades de carga inducidas

Ambos conductores están inicialmente descargados (carga neta cero):
- **Conductor interno ($a_1 \le r \le a_2$):**
  Para que $\vec{E} = 0$ dentro del metal, una superficie gaussiana en $a_1 < r < a_2$ debe encerrar carga neta cero:
  $$q + q_{a1} = 0 \implies q_{a1} = -q$$
  $$\boxed{\sigma_{a1} = \frac{-q}{4\pi a_1^2}}$$
  Como el cascarón interno es neutro ($q_{a1} + q_{a2} = 0$):
  $$q_{a2} = -q_{a1} = +q$$
  $$\boxed{\sigma_{a2} = \frac{q}{4\pi a_2^2}}$$

- **Conductor externo ($b_1 \le r \le b_2$):**
  Una superficie gaussiana en $b_1 < r < b_2$ encierra la carga central $q$, el cascarón interior completo (cuya carga neta es cero: $-q + q = 0$) y la carga inducida en la superficie $r = b_1$:
  $$Q_{\text{enc}} = q + (-q + q) + q_{b1} = q + q_{b1} = 0 \implies q_{b1} = -q$$
  $$\boxed{\sigma_{b1} = \frac{-q}{4\pi b_1^2}}$$
  Como el cascarón exterior es neutro ($q_{b1} + q_{b2} = 0$):
  $$q_{b2} = -q_{b1} = +q$$
  $$\boxed{\sigma_{b2} = \frac{q}{4\pi b_2^2}}$$

---

#### Parte b) Campo eléctrico en todo el espacio

Por simetría esférica, aplicamos la ley de Gauss con superficies esféricas concéntricas de radio $r$:
$$\oint_S \vec{E}\cdot d\vec{A} = E(r) \cdot 4\pi r^2 = \frac{Q_{\text{enc}}}{\varepsilon_0}$$

Analizando cada región desde el centro hacia afuera:
1. **Para $r < a_1$:** $Q_{\text{enc}} = q \implies \boxed{\vec{E}_1 = \frac{q}{4\pi\varepsilon_0 r^2}\,\hat{r}}$
2. **Para $a_1 < r < a_2$ (metal conductor):** $\boxed{\vec{E}_2 = \vec{0}}$
3. **Para $a_2 < r < b_1$:** $Q_{\text{enc}} = q - q + q = q \implies \boxed{\vec{E}_3 = \frac{q}{4\pi\varepsilon_0 r^2}\,\hat{r}}$
4. **Para $b_1 < r < b_2$ (metal conductor):** $\boxed{\vec{E}_4 = \vec{0}}$
5. **Para $r > b_2$:** $Q_{\text{enc}} = q - q + q - q + q = q \implies \boxed{\vec{E}_5 = \frac{q}{4\pi\varepsilon_0 r^2}\,\hat{r}}$

---

#### Parte c) Potencial eléctrico en todo el espacio

Fijamos el origen de potencial en el infinito: $V(\infty) = 0$.  
El potencial en cualquier punto se calcula mediante la integral de línea:
$$V(r) = -\int_\infty^r \vec{E}\cdot d\vec{r}'$$

1. **Región $r > b_2$:**
   $$V(r) = -\int_\infty^r \frac{q}{4\pi\varepsilon_0 {r'}^2}\,dr' = \boxed{\frac{q}{4\pi\varepsilon_0 r}}$$

2. **Región $b_1 \le r \le b_2$ (conductor exterior):**  
   Al ser un conductor en equilibrio, es equipotencial y continuo con la frontera exterior $r = b_2$:
   $$V(r) = V(b_2) = \boxed{\frac{q}{4\pi\varepsilon_0 b_2}}$$

3. **Región $a_2 < r < b_1$:**
   $$V(r) = V(b_1) - \int_{b_1}^r \vec{E}_3\cdot d\vec{r}' = \frac{q}{4\pi\varepsilon_0 b_2} - \int_{b_1}^r \frac{q}{4\pi\varepsilon_0 {r'}^2}\,dr'$$
   $$V(r) = \frac{q}{4\pi\varepsilon_0 b_2} + \frac{q}{4\pi\varepsilon_0}\left(\frac{1}{r} - \frac{1}{b_1}\right) = \boxed{\frac{q}{4\pi\varepsilon_0}\left(\frac{1}{b_2} - \frac{1}{b_1} + \frac{1}{r}\right)}$$

4. **Región $a_1 \le r \le a_2$ (conductor interior):**  
   Es una región conductora equipotencial continua con $r = a_2$:
   $$V(r) = V(a_2) = \boxed{\frac{q}{4\pi\varepsilon_0}\left(\frac{1}{b_2} - \frac{1}{b_1} + \frac{1}{a_2}\right)}$$

5. **Región $r < a_1$:**
   $$V(r) = V(a_1) - \int_{a_1}^r \vec{E}_1\cdot d\vec{r}' = V(a_1) + \frac{q}{4\pi\varepsilon_0}\left(\frac{1}{r} - \frac{1}{a_1}\right)$$
   $$\boxed{V(r) = \frac{q}{4\pi\varepsilon_0}\left(\frac{1}{b_2} - \frac{1}{b_1} + \frac{1}{a_2} - \frac{1}{a_1} + \frac{1}{r}\right)}$$

---

#### Parte d) Conexión entre los dos conductores mediante un cable

Al unir los dos cascarones mediante un alambre conductor, se convierten en un único cuerpo conductor en equilibrio electrostático, debiendo encontrarse a un mismo potencial eléctrico.

1. **Nueva distribución de carga:**
   - La carga puntual central $+q$ no cambia, por lo que en la superficie más interna ($r = a_1$) debe permanecer exactamente la misma carga inducida para anular el campo en el conductor:
     $$q_{a1} = -q \implies \boxed{\sigma_{a1} = \frac{-q}{4\pi a_1^2}}$$
   - Las superficies intermedias $r = a_2$ y $r = b_1$ quedan conectadas eléctricamente. Como el volumen comprendido entre $a_2$ y $b_1$ no encierra ninguna carga libre independiente, para que el potencial sea constante y el campo eléctrico sea nulo entre ambos cascarones, no puede haber densidad superficial en estas caras enfrentadas:
     $$q_{a2} = 0 \implies \boxed{\sigma_{a2} = 0}$$
     $$q_{b1} = 0 \implies \boxed{\sigma_{b1} = 0}$$
     *(Las cargas $+q$ de $a_2$ y $-q$ de $b_1$ fluyeron a través del alambre y se neutralizaron mutuamente).*
   - Por conservación de la carga total del conjunto de los dos conductores ($Q_{\text{ambos}} = 0$):
     $$q_{a1} + q_{a2} + q_{b1} + q_{b2} = 0 \implies -q + 0 + 0 + q_{b2} = 0 \implies q_{b2} = +q$$
     $$\boxed{\sigma_{b2} = \frac{q}{4\pi b_2^2}}$$

2. **Campo eléctrico en todo el espacio tras la conexión:**
   - Para $r < a_1$: $\boxed{\vec{E} = \dfrac{q}{4\pi\varepsilon_0 r^2}\,\hat{r}}$
   - Para $a_1 < r < b_2$: $\boxed{\vec{E} = \vec{0}}$
   - Para $r > b_2$: $\boxed{\vec{E} = \dfrac{q}{4\pi\varepsilon_0 r^2}\,\hat{r}}$

---

#### Parte e) Variación de energía almacenada entre $a_2$ y $b_1$

La energía electrostática almacenada en un volumen $V$ con campo eléctrico $\vec{E}$ es:
$$U = \int_V \frac{1}{2}\varepsilon_0 E^2\,dV = \frac{\varepsilon_0}{2} \int_{a_2}^{b_1} E^2 \cdot (4\pi r^2\,dr)$$

- **Antes de la conexión ($U_i$):**  
  En la zona $a_2 < r < b_1$, el campo era $E_3 = \frac{q}{4\pi\varepsilon_0 r^2}$:
  $$U_i = \frac{4\pi\varepsilon_0}{2} \int_{a_2}^{b_1} \left(\frac{q}{4\pi\varepsilon_0 r^2}\right)^2 r^2\,dr = \frac{q^2}{8\pi\varepsilon_0} \int_{a_2}^{b_1} \frac{dr}{r^2} = \frac{q^2}{8\pi\varepsilon_0} \left[ -\frac{1}{r} \right]_{a_2}^{b_1}$$
  $$U_i = \frac{q^2}{8\pi\varepsilon_0}\left(\frac{1}{a_2} - \frac{1}{b_1}\right)$$

- **Después de la conexión ($U_f$):**  
  Tras la conexión, el campo eléctrico en la región $a_2 < r < b_1$ es idénticamente cero ($\vec{E} = \vec{0}$), por lo que:
  $$U_f = 0$$

Por lo tanto, la variación de energía almacenada en esta región es:
$$\Delta U = U_f - U_i = 0 - \frac{q^2}{8\pi\varepsilon_0}\left(\frac{1}{a_2} - \frac{1}{b_1}\right)$$

$$\boxed{\Delta U = -\frac{q^2}{8\pi\varepsilon_0}\left(\frac{1}{a_2} - \frac{1}{b_1}\right)}$$

**Verificación:**
- **Signo:** Como $b_1 > a_2$, $\left(\frac{1}{a_2} - \frac{1}{b_1}\right) > 0$, lo que implica $\Delta U < 0$. La energía del sistema disminuye. Físicamente, esta pérdida de energía electrostática corresponde al trabajo realizado por el campo para mover las cargas a través del cable y se disipa en forma de calor por efecto Joule en la resistencia finita del conductor de conexión.

---

## Problema 3

Un sistema consiste de dos cascarones conductores cilíndricos concéntricos de longitud $L \gg d$ ($a, b, c, d$ definidos en la figura). El cascarón interior contiene una carga total $+Q$ y el exterior una carga total $-Q$. Determine:

a) La densidad carga en cada una de las cuatro superficies conductoras.  
b) El potencial en todo el espacio.  
c) La diferencia de potencial de los conductores cilíndricos.

> **[Figura]:** Sistema de dos cascarones conductores cilíndricos coaxiales de gran longitud $L \gg d$ con eje a lo largo de $\hat{z}$.
> - (a) Vista exterior: muestra el cilindro de longitud finita pero muy grande $L$.
> - (b) Vista interior (sección transversal normal al eje): se definen cuatro radios concéntricos: el cascarón interior posee radio interno $a$ y radio externo $b$ ($a < b$), mientras que el cascarón exterior posee radio interno $c$ y radio externo $d$ ($b < c < d$). Las cuatro superficies son $r = a$, $r = b$, $r = c$ y $r = d$.

### Solución

**Idea:** Debido a que la longitud es mucho mayor que el radio exterior ($L \gg d$), despreciamos los efectos de borde y asumimos simetría cilíndrica ideal. El campo eléctrico dentro de los conductores debe ser cero en equilibrio. Aplicando la ley de Gauss con cilindros coaxiales de longitud $L$ determinamos las densidades superficiales inducidas y el campo eléctrico radial. Luego, integrando $\vec{E}$ determinamos el potencial $V(r)$ con referencia $V(r \ge c) = 0$ y la diferencia de potencial entre ambos conductores.

#### Parte a) Densidad de carga en las cuatro superficies conductoras

1. **Superficie $r = a$:**  
   En la región hueca interior $r < a$ no existe ninguna carga eléctrica. Aplicando la ley de Gauss a una superficie cilíndrica coaxial de radio $r \in [a, b]$ dentro del conductor interior:
   $$\oint \vec{E}\cdot d\vec{A} = 0 \implies \frac{Q_{\text{enc}}}{\varepsilon_0} = 0 \implies \sigma_a \cdot (2\pi a L) = 0$$
   $$\boxed{\sigma_a = 0}$$

2. **Superficie $r = b$:**  
   El cascarón interior posee una carga total $+Q$. Como $\sigma_a = 0$, toda la carga debe ubicarse sobre la superficie exterior $r = b$:
   $$Q_b = Q - Q_a = Q - 0 = Q$$
   $$\boxed{\sigma_b = \frac{Q}{2\pi b L}}$$

3. **Superficie $r = c$:**  
   Aplicamos la ley de Gauss a una superficie cilíndrica coaxial contenida en el cascarón exterior, es decir, de radio $r \in [c, d]$. Como el campo dentro del conductor es cero:
   $$\oint \vec{E}\cdot d\vec{A} = 0 \implies Q_{\text{enc}} = Q + Q_c = 0 \implies Q_c = -Q$$
   Dividiendo por el área de la superficie $2\pi c L$:
   $$\boxed{\sigma_c = -\frac{Q}{2\pi c L}}$$

4. **Superficie $r = d$:**  
   El cascarón exterior porta una carga total $-Q$. Por conservación de carga en dicho conductor:
   $$Q_c + Q_d = -Q \implies -Q + Q_d = -Q \implies Q_d = 0$$
   $$\boxed{\sigma_d = 0}$$

---

#### Parte b) Potencial en todo el espacio

Calculamos en primer lugar el campo eléctrico $\vec{E}(r) = E(r)\,\hat{r}$ mediante la ley de Gauss con un cilindro coaxial de radio $r$ y longitud $L$:
$$E(r) \cdot 2\pi r L = \frac{Q_{\text{enc}}}{\varepsilon_0}$$

- **Para $r < b$:** $Q_{\text{enc}} = 0 \implies \vec{E} = \vec{0}$.
- **Para $b < r < c$:** $Q_{\text{enc}} = +Q \implies E(r) \cdot 2\pi r L = \frac{Q}{\varepsilon_0} \implies \vec{E}(r) = \frac{Q}{2\pi\varepsilon_0 L r}\,\hat{r}$.
- **Para $r > c$:** $Q_{\text{enc}} = +Q + (-Q) = 0 \implies \vec{E} = \vec{0}$.

Fijando la referencia estándar para sistemas cilíndricos donde el exterior está libre de campo ($E = 0$ para $r \ge c$), tomamos $V(r \to \infty) = 0$. Dado que $\vec{E} = \vec{0}$ para todo $r > c$, el potencial es uniforme y constante en toda la región exterior:
$$V(r) = V(c) = 0 \qquad (r \ge c)$$

1. **Para $r \ge c$:**
   $$\boxed{V(r) = 0 \qquad (r \ge c)}$$

2. **Para $b \le r \le c$:**
   $$V(r) - V(c) = -\int_c^r \vec{E}\cdot d\vec{r}' = -\int_c^r \frac{Q}{2\pi\varepsilon_0 L r'}\,dr' = -\frac{Q}{2\pi\varepsilon_0 L}\ln\left(\frac{r}{c}\right) = \frac{Q}{2\pi\varepsilon_0 L}\ln\left(\frac{c}{r}\right)$$
   Como $V(c) = 0$:
   $$\boxed{V(r) = \frac{Q}{2\pi\varepsilon_0 L}\ln\left(\frac{c}{r}\right) \qquad (b \le r \le c)}$$

3. **Para $r < b$:**  
   Como $\vec{E} = \vec{0}$ para $r < b$, el potencial en todo el interior es constante e igual al valor en la superficie conductora $r = b$:
   $$\boxed{V(r) = V(b) = \frac{Q}{2\pi\varepsilon_0 L}\ln\left(\frac{c}{b}\right) \qquad (r < b)}$$

---

#### Parte c) Diferencia de potencial de los conductores cilíndricos

La diferencia de potencial entre el conductor interior (a mayor potencial, con carga $+Q$) y el conductor exterior (con carga $-Q$) es:
$$\Delta V = V(b) - V(c) = \frac{Q}{2\pi\varepsilon_0 L}\ln\left(\frac{c}{b}\right) - 0$$

$$\boxed{\Delta V = V(b) - V(c) = \frac{Q}{2\pi\varepsilon_0 L}\ln\left(\frac{c}{b}\right)}$$

> **Nota:** En la pauta oficial manuscrita/digitalizada (página 10) aparece la etiqueta escrita como "$V(c) - V(b) = \frac{Q}{2\pi\varepsilon_0 L}\ln\left(\frac{c}{b}\right)$". Puesto que $c > b$, el argumento del logaritmo es mayor que 1 y por tanto $\ln(c/b) > 0$. Al ser el conductor interior positivo ($+Q$) y el exterior negativo ($-Q$), las líneas de campo apuntan desde $b$ hacia $c$, por lo que el potencial es mayor en el cilindro interior ($V(b) > V(c)$). La diferencia de potencial intrínseca del condensador $\Delta V = V_{\text{int}} - V_{\text{ext}} = V(b) - V(c)$ es estrictamente positiva e igual a $\frac{Q}{2\pi\varepsilon_0 L}\ln(c/b)$; mientras que la resta $V(c) - V(b)$ sería estrictamente $-\frac{Q}{2\pi\varepsilon_0 L}\ln(c/b)$.

**Verificación:**
- **Unidades:** $[Q/(2\pi\varepsilon_0 L)] = \text{C}/ [(\text{C}^2/(\text{N}\cdot\text{m}^2))\cdot\text{m}] = \text{N}\cdot\text{m}/\text{C} = \text{J}/\text{C} = \text{V}$, correspondiente a voltios.
- **Capacidad cilíndrica:** La capacidad $C = Q/\Delta V = \frac{2\pi\varepsilon_0 L}{\ln(c/b)}$ reproduce con exactitud la fórmula clásica de la capacitancia de un condensador cilíndrico coaxial de radios $b$ y $c$.

---

## Resumen de resultados

| Problema | Parte | Parámetro / Condición | Resultado |
| :--- | :--- | :--- | :--- |
| **Problema 1** | a) Densidades de carga | Superficie cavidad $a$ | $\sigma_a = -\dfrac{q_a}{4\pi a^2}$ |
| | a) Densidades de carga | Superficie cavidad $b$ | $\sigma_b = -\dfrac{q_b}{4\pi b^2}$ |
| | a) Densidades de carga | Superficie exterior esfera | $\sigma_R = \dfrac{q_a + q_b}{4\pi R^2}$ |
| | b) Campo fuera del conductor | $r > R$ | $\vec{E}(\vec{r}) = \dfrac{q_a + q_b}{4\pi\varepsilon_0 r^2}\,\hat{r}$ |
| | c) Campo dentro de cavidades | Cavidad $a$ ($r_a < a$) <br> Cavidad $b$ ($r_b < b$) | $\vec{E}_a(\vec{r}_a) = \dfrac{q_a}{4\pi\varepsilon_0 r_a^2}\,\hat{r}_a$ <br> $\vec{E}_b(\vec{r}_b) = \dfrac{q_b}{4\pi\varepsilon_0 r_b^2}\,\hat{r}_b$ |
| **Problema 2** | a) Densidades iniciales | Superficies $a_1, a_2, b_1, b_2$ | $\sigma_{a1} = -\dfrac{q}{4\pi a_1^2},\quad \sigma_{a2} = \dfrac{q}{4\pi a_2^2}$ <br> $\sigma_{b1} = -\dfrac{q}{4\pi b_1^2},\quad \sigma_{b2} = \dfrac{q}{4\pi b_2^2}$ |
| | b) Campo eléctrico inicial | $r < a_1$, $a_2 < r < b_1$, $r > b_2$ <br> $a_1 < r < a_2$, $b_1 < r < b_2$ | $\vec{E} = \dfrac{q}{4\pi\varepsilon_0 r^2}\,\hat{r}$ <br> $\vec{E} = \vec{0}$ |
| | c) Potencial inicial | $r > b_2$ <br> $b_1 \le r \le b_2$ <br> $a_2 < r < b_1$ <br> $a_1 \le r \le a_2$ <br> $r < a_1$ | $V = \dfrac{q}{4\pi\varepsilon_0 r}$ <br> $V = \dfrac{q}{4\pi\varepsilon_0 b_2}$ <br> $V = \dfrac{q}{4\pi\varepsilon_0}\left(\dfrac{1}{b_2} - \dfrac{1}{b_1} + \dfrac{1}{r}\right)$ <br> $V = \dfrac{q}{4\pi\varepsilon_0}\left(\dfrac{1}{b_2} - \dfrac{1}{b_1} + \dfrac{1}{a_2}\right)$ <br> $V = \dfrac{q}{4\pi\varepsilon_0}\left(\dfrac{1}{b_2} - \dfrac{1}{b_1} + \dfrac{1}{a_2} - \dfrac{1}{a_1} + \dfrac{1}{r}\right)$ |
| | d) Conexión con cable | Distribución de carga <br> Campo eléctrico | $\sigma_{a1} = -\dfrac{q}{4\pi a_1^2},\quad \sigma_{a2} = 0,\quad \sigma_{b1} = 0,\quad \sigma_{b2} = \dfrac{q}{4\pi b_2^2}$ <br> $\vec{E} = \dfrac{q}{4\pi\varepsilon_0 r^2}\,\hat{r}$ en $r < a_1$ y $r > b_2$; $\vec{E} = \vec{0}$ en $a_1 < r < b_2$ |
| | e) Variación de energía | Entre $a_2$ y $b_1$ | $\Delta U = -\dfrac{q^2}{8\pi\varepsilon_0}\left(\dfrac{1}{a_2} - \dfrac{1}{b_1}\right) < 0$ |
| **Problema 3** | a) Densidades en 4 caras | $r = a, b, c, d$ | $\sigma_a = 0,\quad \sigma_b = \dfrac{Q}{2\pi b L},\quad \sigma_c = -\dfrac{Q}{2\pi c L},\quad \sigma_d = 0$ |
| | b) Potencial en el espacio | $r \ge c$ <br> $b \le r \le c$ <br> $r < b$ | $V(r) = 0$ <br> $V(r) = \dfrac{Q}{2\pi\varepsilon_0 L}\ln\left(\dfrac{c}{r}\right)$ <br> $V(r) = \dfrac{Q}{2\pi\varepsilon_0 L}\ln\left(\dfrac{c}{b}\right)$ |
| | c) Diferencia de potencial | Entre cilindros interior y exterior | $\Delta V = V(b) - V(c) = \dfrac{Q}{2\pi\varepsilon_0 L}\ln\left(\dfrac{c}{b}\right)$ |
