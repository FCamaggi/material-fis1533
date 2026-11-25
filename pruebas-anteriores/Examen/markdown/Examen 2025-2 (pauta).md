# Pauta Examen — Capacitores con dieléctricos, inducción electromagnética y circuitos RLC en corriente alterna

> **Curso:** FIS1533 — Electricidad y Magnetismo (Segundo semestre 2025) · **Fecha:** 5 de diciembre de 2025 · **Forma:** 1

---

## Problema 1

Tres placas conductoras paralelas de área $A$ muy grande, se colocan separadas una distancia $d$ y de manera consecutiva, tal como se muestra en la figura. El espacio entre las placas está lleno con materiales dieléctricos de permitividad $\varepsilon_1$ y $\varepsilon_2$, como se muestra en la figura. Las placas externas están conectadas eléctricamente por medio de un cable conductor que tiene un extremo denotado con la letra $b$. La placa central está conectada a un cable conductor eléctrico de extremo $a$. Las placas están cargadas de tal forma que la carga de la placa central es $+Q$ y los extremos $a$ y $b$ tienen una diferencia de potencial $V_{ab}$, ambas conocidas. Se pueden ignorar los efectos de los bordes.

- **a) (2 ptos.)** Calcular la capacitancia total, $C_T$, entre los extremos $a$ y $b$ en términos de los parámetros mostrados en la figura ($A, \varepsilon_1, \varepsilon_2, d, V_{ab}$).
- **b) (2 ptos.)** Calcular la densidad de carga libre, $\sigma_1$, en la superficie de contacto entre la placa conductora central y el material dieléctrico con permitividad $\varepsilon_1$ (En este punto puede considerar conocida $C_T$).
- **c) (2 ptos.)** Calcular la densidad de carga ligada, $\sigma_b$, en la superficie de contacto entre la placa conductora central y el material dieléctrico con permitividad $\varepsilon_1$ (En este punto puede considerar conocida $C_T$ y/o $\sigma_1$).

> **[Figura]:** Sistema de tres placas conductoras planas horizontales paralelas de área $A$ apiladas verticalmente. La placa superior y la placa central están separadas una distancia $d$, con un dieléctrico de permitividad $\varepsilon_1$ ocupando todo el espacio entre ellas. La placa central (etiquetada con carga $+Q$) y la placa inferior también están separadas una distancia $d$, con un dieléctrico de permitividad $\varepsilon_2$ llenando el espacio entre ambas. De la placa central sale hacia la izquierda un cable conductor que termina en el borne $a$. Las dos placas externas (superior e inferior) están conectadas entre sí mediante un cable conductor a la derecha que termina en el borne $b$. Entre los extremos $a$ y $b$ se indica la diferencia de potencial $V_{ab}$.

### Solución

**Idea:** La placa central está al potencial del extremo $a$ y ambas placas externas comparten el potencial del extremo $b$, de modo que los dos espacios dieléctricos conforman dos capacitores planos de igual área $A$ y separación $d$ conectados en paralelo entre $a$ y $b$. La carga $+Q$ se reparte entre las dos caras de la placa central en proporción a sus capacitancias, mientras que el campo eléctrico en ambas regiones es uniforme e igual a $V_{ab}/d$, lo que permite hallar directamente la polarización $\vec{P}_1$ y la densidad superficial de carga ligada $\sigma_{b_1} = \vec{P}_1\cdot\hat{n}$ sobre la superficie del dieléctrico $\varepsilon_1$.

---

#### Parte a) Capacitancia total $C_T$

La placa central forma dos condensadores planos con el conductor exterior (las placas superior e inferior conectadas al borne $b$): uno relleno con el dieléctrico $\varepsilon_1$ (capacitancia $C_1$) y otro relleno con el dieléctrico $\varepsilon_2$ (capacitancia $C_2$):
$$C_1 = \frac{\varepsilon_1 A}{d} \quad \text{(0.5 pts)}, \qquad C_2 = \frac{\varepsilon_2 A}{d} \quad \text{(0.5 pts)}$$

*(Nota: la pauta oficial se refiere coloquialmente a estos dos condensadores como «uno a la izquierda» y «otro a la derecha» de la placa central, aunque en el dibujo estén dispuestos verticalmente arriba y abajo de ella.)*

Como ambos condensadores conectan la misma placa central ($a$) con el mismo conductor exterior ($b$), están sometidos a la misma diferencia de potencial $V_{ab}$ y, por lo tanto, están conectados en paralelo:
$$C_T = C_{\text{total}} = C_1 + C_2 \qquad \text{(0.5 pts)}$$
$$C_T = \frac{\varepsilon_1 A}{d} + \frac{\varepsilon_2 A}{d} = \frac{(\varepsilon_1 + \varepsilon_2)A}{d} \qquad \text{(0.5 pts)}$$

$$\boxed{C_T = \frac{(\varepsilon_1 + \varepsilon_2)A}{d}}$$

---

#### Parte b) Densidad de carga libre $\sigma_1$

La carga libre $+Q$ de la placa conductora central se reparte entre sus dos caras (en contacto con $\varepsilon_1$ y $\varepsilon_2$) proporcionalmente a las capacitancias respectivas:
$$Q_1 = C_1 V_{ab} \qquad \text{(0.5 pts)}$$
donde la diferencia de potencial entre $a$ y $b$ es:
$$V_{ab} = \frac{Q}{C_{\text{total}}} \qquad \text{(0.5 pts)}$$

Sustituyendo $V_{ab}$ en $Q_1$:
$$Q_1 = \frac{C_1}{C_{\text{total}}}\,Q$$

Por definición, la densidad superficial de carga libre $\sigma_1$ sobre el área $A$ de la cara en contacto con $\varepsilon_1$ es:
$$\sigma_1 = \frac{Q_1}{A} \qquad \text{(0.5 pts)}$$
$$\sigma_1 = \frac{C_1}{C_{\text{total}}}\frac{Q}{A} \qquad \text{(0.5 pts)}$$

Sustituyendo las expresiones de $C_{\text{total}}$ y $C_1$ obtenidas en a):
$$\sigma_1 = \frac{\varepsilon_1 A / d}{(\varepsilon_1 + \varepsilon_2)A / d}\,\frac{Q}{A} = \frac{\varepsilon_1}{\varepsilon_1 + \varepsilon_2}\frac{Q}{A}$$

$$\boxed{\sigma_1 = \frac{C_1}{C_T}\frac{Q}{A} = \frac{\varepsilon_1}{\varepsilon_1 + \varepsilon_2}\frac{Q}{A}}$$

---

#### Parte c) Densidad de carga ligada $\sigma_b$ para el material $\varepsilon_1$

La densidad superficial de carga ligada en la superficie del material dieléctrico $\varepsilon_1$ en contacto con la placa conductora central está dada por:
$$\sigma_{b_1} = \vec{P}_1 \cdot \hat{n} \qquad \text{(0.5 pts)}$$

La polarización eléctrica para el material lineal de permitividad $\varepsilon_1$ se define como:
$$\vec{P}_1 = \varepsilon_0 (\varepsilon_{r_1} - 1)\vec{E}_1 \qquad \text{(0.5 pts)}$$
con $\varepsilon_{r_1} = \varepsilon_1 / \varepsilon_0$. En la interfaz dieléctrico-conductor, donde el conductor central está cargado positivamente ($+Q$), el campo eléctrico $\vec{E}_1$ sale de la placa central hacia el interior del dieléctrico, mientras que el vector unitario normal saliente del dieléctrico $\hat{n}$ apunta hacia la placa conductora, en sentido contrario al campo eléctrico:
$$\vec{E}_1 \cdot \hat{n} = -E_1$$

Por tanto:
$$\sigma_{b_1} = \varepsilon_0(\varepsilon_{r_1} - 1)\vec{E}_1 \cdot \hat{n} = -\varepsilon_0(\varepsilon_{r_1} - 1)E_1$$

Ignorando efectos de borde, el campo eléctrico entre la placa central y cada placa exterior es uniforme y su magnitud es idéntica en ambas regiones:
$$E_1 = E_2 = \frac{V_{ab}}{d} \qquad \text{(0.5 pts)}$$

Sustituyendo $E_1 = V_{ab}/d$ se obtiene:
$$\sigma_{b_1} = -\varepsilon_0(\varepsilon_{r_1} - 1)\frac{V_{ab}}{d} = -(\varepsilon_1 - \varepsilon_0)\frac{V_{ab}}{d} \qquad \text{(0.5 pts)}$$

Expresada alternativamente en términos de $C_{\text{total}}$ (usando $V_{ab} = Q/C_{\text{total}}$) o de $\sigma_1$ (usando $E_1 = \sigma_1/\varepsilon_1$):
$$\sigma_{b_1} = -\varepsilon_0(\varepsilon_{r_1} - 1)\frac{Q}{d\,C_{\text{total}}} = -\left(1 - \frac{\varepsilon_0}{\varepsilon_1}\right)\sigma_1$$

$$\boxed{\sigma_{b_1} = -\varepsilon_0(\varepsilon_{r_1} - 1)\frac{V_{ab}}{d} = -\varepsilon_0(\varepsilon_{r_1} - 1)\frac{Q}{d\,C_T}}$$

**Verificación:**
- **Balance eléctrico en la interfaz:** La densidad total de carga en la interfaz es $\sigma_{\text{tot}} = \sigma_1 + \sigma_{b_1} = \sigma_1 - \left(1 - \frac{\varepsilon_0}{\varepsilon_1}\right)\sigma_1 = \frac{\varepsilon_0}{\varepsilon_1}\sigma_1 = \varepsilon_0 E_1$, verificando exactamente $\vec{E}_1 = \frac{\sigma_{\text{tot}}}{\varepsilon_0}\hat{u}$ en el vacío microscópico equivalente.
- **Límite vacío ($\varepsilon_1 \to \varepsilon_0$, $\varepsilon_{r_1} \to 1$):** $\sigma_{b_1} \to 0$, como corresponde a la ausencia de material polarizable.

---

## Problema 2

Considere una espira cuadrada de lado $a$ y masa $m$ en el plano $yz$, colocada en un campo magnético $\vec{B} = (B_0 - \alpha z)\,\hat{x}$, con $\alpha > 0$. Considere que la espira, de resistencia $R$ y autoinducción despreciable, cae en la dirección vertical debido a la gravedad.

- **a) (1 pto.)** Determine el flujo magnético a través de la espira.
- **b) (2 ptos.)** Encuentre la fuerza electromotriz y la corriente inducida en función de la velocidad $v$ de la espira.
- **c) (1 pto.)** Indique el sentido de la corriente inducida y justifique su respuesta según la ley de Lenz.
- **d) (1 pto.)** Determine la fuerza que experimenta la espira.
- **e) (1 pto.)** ¿Cuál es la velocidad terminal de la espira?

> **[Figura]:** Espira cuadrada conductora de masa $m$ y lado $a$ situada en el plano vertical $yz$, inmersa en una región punteada con campo magnético $\vec{B}$ y aceleración de gravedad $\vec{g}$ vertical hacia abajo. El borde inferior de la espira está a una altura $z$ sobre el suelo (línea horizontal inferior de referencia) y su borde superior está a altura $z + a$. A la derecha se muestra la terna cartesiana: $\hat{z}$ vertical hacia arriba, $\hat{y}$ horizontal hacia la derecha y $\hat{x}$ saliendo perpendicularmente de la página ($\odot\,\hat{x}$).

### Solución

**Idea:** El campo magnético apunta en $+\hat{x}$ y decrece linealmente con la altura $z$. Al integrar $\vec{B}\cdot d\vec{A}$ sobre el área $a\times a$ de la espira se obtiene el flujo magnético $\Phi_B(z)$ en función de la altura $z$ del borde inferior. Cuando la espira cae ($v = dz/dt < 0$), entra en regiones de mayor $B_x$, incrementando el flujo saliente; por la ley de Faraday-Lenz se induce una corriente horaria cuyo efecto magnético sobre los lados horizontales produce una fuerza magnética neta hacia arriba que se opone a la caída hasta equilibrar el peso $mg$ en la velocidad terminal.

---

#### Parte a) Flujo magnético a través de la espira

Tomamos el vector diferencial de área normal al plano $yz$ apuntando en $+\hat{x}$:
$$d\vec{A} = dy\,dz'\,\hat{x}$$

El flujo magnético a través de la superficie plana de la espira (con $y \in [0, a]$ y $z' \in [z, z + a]$) es:
$$\Phi_B = \int \vec{B}\cdot d\vec{A} = \int_{y=0}^a \int_{z'=z}^{z+a} (B_0 - \alpha z')\,dy\,dz' = \int_{y=0}^a dy \int_{z'=z}^{z+a} (B_0 - \alpha z')\,dz' \qquad \text{(0.5 pts)}$$

Evaluando las integrales:
$$\Phi_B = a \left[ B_0 z' - \frac{\alpha {z'}^2}{2} \right]_{z}^{z+a} = a \left[ B_0 a - \frac{\alpha}{2}\left((z + a)^2 - z^2\right) \right]$$
Como $(z + a)^2 - z^2 = 2az + a^2 = a(2z + a)$, resulta:
$$\Phi_B = a^2 B_0 - \frac{\alpha a^2 (2z + a)}{2} \qquad \text{(0.5 pts)}$$

$$\boxed{\Phi_B = a^2 B_0 - \frac{\alpha a^2 (2z + a)}{2}}$$

---

#### Parte b) Fuerza electromotriz y corriente inducida en función de $v$

Aplicamos la ley de Faraday usando $\Phi_B(z)$:
$$\varepsilon = -\frac{d\Phi_B}{dt} = -\frac{d}{dt}\left( a^2 B_0 - \frac{\alpha a^2 (2z + a)}{2} \right) \qquad \text{(0.25 pts)}$$
$$\varepsilon = +\alpha a^2 \frac{dz}{dt} \qquad \text{(0.25 pts)}$$
$$\varepsilon = +\alpha a^2 v \qquad \text{(0.5 pts)}$$

Como la espira cae en la dirección $-\hat{z}$, su velocidad vertical es negativa ($v = -\lvert v \rvert < 0$), por lo que la fem inducida (con la orientación $d\vec{A} \parallel +\hat{x}$) también es negativa:
$$\varepsilon = -\alpha a^2 \lvert v \rvert \qquad \text{(0.5 pts)}$$

La magnitud de la corriente inducida en la espira de resistencia $R$ es:
$$I = \frac{\lvert \varepsilon \rvert}{R} = \frac{\alpha a^2 \lvert v \rvert}{R} \qquad \text{(0.5 pts)}$$

$$\boxed{\varepsilon = \alpha a^2 v = -\alpha a^2 \lvert v \rvert, \qquad I = \frac{\alpha a^2 \lvert v \rvert}{R}}$$

---

#### Parte c) Sentido de la corriente inducida según la ley de Lenz

Mientras la espira cae ($z$ disminuye), el campo magnético $B_x(z) = B_0 - \alpha z$ aumenta linealmente al descender (a menor altura $z$, mayor es el campo magnético en $+\hat{x}$), por lo que el flujo magnético saliente a través de la espira aumenta *(0.5 pts)*.

> **Nota:** La pauta oficial describe coloquialmente que «el campo magnético es inversamente proporcional a la altura» para expresar que disminuye al subir y aumenta al bajar; en estricto rigor matemático, $B_x(z) = B_0 - \alpha z$ decrece linealmente con $z$.

De acuerdo con la ley de Lenz, la corriente inducida debe generar un campo magnético propio en la dirección $-\hat{x}$ (entrante a la página) para oponerse a este aumento de flujo en $+\hat{x}$. Aplicando la regla de la mano derecha (con el plano $yz$ visto desde $+\hat{x}$: $\hat{y}$ a la derecha y $\hat{z}$ hacia arriba), la corriente inducida debe circular en **sentido horario** *(0.5 pts)*: sube por el lado vertical izquierdo, avanza hacia $+\hat{y}$ por el lado superior, baja por el lado vertical derecho y regresa hacia $-\hat{y}$ por el lado inferior.

$$\boxed{\text{Sentido horario (visto desde } +\hat{x}\text{)}}$$

---

#### Parte d) Fuerza que experimenta la espira

Calculamos la fuerza magnética sobre cada uno de los cuatro segmentos rectilíneos de la espira mediante $\vec{F} = I\int d\vec{\ell}\times\vec{B}$:

1. **Segmentos verticales izquierdo ($\vec{F}_1$, corriente en $+\hat{z}$) y derecho ($\vec{F}_2$, corriente en $-\hat{z}$):**
   $$\vec{F}_1 = I \int d\vec{\ell}_1 \times \vec{B} = I \int_z^{z+a} dz'\,\hat{z} \times (B_0 - \alpha z')\,\hat{x}$$
   Usando $\hat{z}\times\hat{x} = \hat{y}$:
   $$\vec{F}_1 = I \int_z^{z+a} (B_0 - \alpha z')\,dz'\,\hat{y} = I \left[ B_0 z' - \alpha \frac{{z'}^2}{2} \right]_z^{z+a} \hat{y} = I \left[ B_0 a - \frac{\alpha}{2}\left((z + a)^2 - z^2\right) \right] \hat{y} \qquad \text{(0.2 pts)}$$

   Mientras que para el segmento vertical derecho (recorrido desde $z+a$ hasta $z$):
   $$\vec{F}_2 = I \int d\vec{\ell}_2 \times \vec{B} = I \int_{z+a}^z dz'\,\hat{z} \times (B_0 - \alpha z')\,\hat{x} = -I \left[ B_0 a - \frac{\alpha}{2}\left((z + a)^2 - z^2\right) \right] \hat{y} \qquad \text{(0.2 pts)}$$

   Por tanto, $\vec{F}_1 + \vec{F}_2 = \vec{0}$ *(alternativamente, por simetría, 0.4 pts)*.

2. **Segmentos horizontales superior ($\vec{F}_3$ en $z + a$, corriente en $+\hat{y}$) e inferior ($\vec{F}_4$ en $z$, corriente en $-\hat{y}$):**  
   A lo largo de cada tramo horizontal la altura es fija y $\vec{B}$ es uniforme sobre el segmento de longitud $a$ (usando $\hat{y}\times\hat{x} = -\hat{z}$):
   $$\vec{F}_3 = I\vec{L}_3 \times \vec{B} = I(a\hat{y}) \times \left[B_0 - \alpha(z + a)\right]\hat{x} = -Ia\left[B_0 - \alpha(z + a)\right]\hat{z} \qquad \text{(0.2 pts)}$$
   $$\vec{F}_4 = I\vec{L}_4 \times \vec{B} = I(-a\hat{y}) \times (B_0 - \alpha z)\hat{x} = Ia(B_0 - \alpha z)\hat{z} \qquad \text{(0.2 pts)}$$

   Sumando ambas contribuciones verticales, la fuerza magnética neta sobre la espira es:
   $$\vec{F}_B = \vec{F}_3 + \vec{F}_4 = -Ia\left[B_0 - \alpha(z + a)\right]\hat{z} + Ia(B_0 - \alpha z)\hat{z} \qquad \text{(0.1 pts)}$$
   $$\vec{F}_B = I \alpha a^2 \hat{z} = \frac{\alpha^2 a^4 \lvert v \rvert}{R}\,\hat{z}$$

   Incluyendo la fuerza gravitacional $-mg\hat{z}$, la fuerza total sobre la espira es:
   $$\vec{F}_{\text{total}} = \left(\frac{\alpha^2 a^4 \lvert v \rvert}{R} - mg\right)\hat{z} \qquad \text{(0.1 pts)}$$

> **Nota:** En las expresiones de $\vec{F}_3$, $\vec{F}_4$, $\vec{F}_B$ y de la parte e), la solución oficial introduce inadvertidamente una longitud horizontal no definida $L$ en lugar del lado $a$ de la espira cuadrada (obteniendo $\frac{\alpha^2 a^3 \lvert v \rvert L}{R}$), y en la última línea de d) vuelve a etiquetar la fuerza total como $\vec{F}_B$ en lugar de $\vec{F}_{\text{total}}$. Dado que el enunciado define una espira **cuadrada** de lado $a$, se tiene $L = a$, de modo que lo correcto en función de los datos del problema es $\vec{F}_B = \frac{\alpha^2 a^4 \lvert v \rvert}{R}\,\hat{z}$ y $\vec{F}_{\text{total}} = \left(\frac{\alpha^2 a^4 \lvert v \rvert}{R} - mg\right)\hat{z}$.

$$\boxed{\vec{F}_{\text{total}} = \left(\frac{\alpha^2 a^4 \lvert v \rvert}{R} - mg\right)\hat{z}}$$

---

#### Parte e) Velocidad terminal de la espira

> **Nota:** En el PDF oficial de la pauta, este último inciso aparece etiquetado tipográficamente como `d)` por segunda vez en lugar de `e)`.

La velocidad terminal se alcanza cuando la espira deja de acelerar mientras cae, es decir, cuando la fuerza neta se anula ($\vec{F}_{\text{total}} = \vec{0}$) *(0.3 pts)*:
$$0 = \frac{\alpha^2 a^4 \lvert v_{\text{term}} \rvert}{R} - mg \qquad \text{(0.5 pts)}$$

Despejando la rapidez terminal (con la corrección $L = a$ señalada en el inciso anterior; la pauta oficial imprime $\frac{mgR}{\alpha^2 a^3 L}$):
$$\lvert v_{\text{term}} \rvert = \frac{mgR}{\alpha^2 a^4} \qquad \text{(0.2 pts)}$$

$$\boxed{\lvert v_{\text{term}} \rvert = \frac{mgR}{\alpha^2 a^4}, \qquad \vec{v}_{\text{term}} = -\frac{mgR}{\alpha^2 a^4}\,\hat{z}}$$

**Verificación (conservación de energía en régimen terminal):**
- A velocidad terminal constante, la tasa de pérdida de energía potencial gravitacional es $P_{\text{grav}} = mg \lvert v_{\text{term}} \rvert$.
- La potencia eléctrica disipada por efecto Joule en la resistencia es $P_{\text{Joule}} = I^2 R = \left(\frac{\alpha a^2 \lvert v_{\text{term}} \rvert}{R}\right)^2 R = \frac{\alpha^2 a^4 \lvert v_{\text{term}} \rvert^2}{R}$.
- Igualando $mg \lvert v_{\text{term}} \rvert = \frac{\alpha^2 a^4 \lvert v_{\text{term}} \rvert^2}{R}$ se recupera inmediatamente $\lvert v_{\text{term}} \rvert = \frac{mgR}{\alpha^2 a^4}$, confirmando el exponente $a^4$ y las unidades de velocidad ($\text{m/s}$).

---

## Problema 3

Dado el circuito RLC en la figura:

1. **(2 ptos.)** ¿Cuál es la impedancia entre los terminales de conexión?
2. **(2 ptos.)** Se aplica el voltaje alterno $U(t) = U_0 \cos(\omega t)$ a los terminales de conexión. Calcule la amplitud de oscilación de la corriente alterna $I(t)$ que entra al circuito.
3. **(2 ptos.)** ¿Cuál es la potencia que se disipa en el circuito durante un período de oscilación del voltaje alterno cuando la frecuencia angular del voltaje es $\omega = 1/(LC)$?

> **[Figura]:** Red pasiva con dos terminales abiertos de conexión en el lado izquierdo (superior e inferior). Entre ambos terminales se conectan dos ramas en paralelo: la rama vertical central contiene únicamente una resistencia $R$; la rama exterior derecha contiene una segunda resistencia $R$ (en el tramo horizontal superior) en serie con una inductancia $L$ y una capacitancia $C$ (en el tramo vertical derecho), retornando por el conductor inferior al terminal inferior.

### Solución

**Idea:** Se trabaja en representación fasorial (amplitudes complejas con dependencia temporal $e^{i\omega t}$), donde las impedancias de $R$, $L$ y $C$ son $R$, $i\omega L$ y $\frac{1}{i\omega C}$, respectivamente. La rama derecha constituye un circuito RLC serie cuya impedancia $Z_{\text{serie}}$ se asocia en paralelo con la resistencia $R$ central para obtener la impedancia equivalente $Z(\omega)$. A partir de la «ley de Ohm» compleja $\tilde{U}_0 = Z\tilde{I}_0$ se halla la amplitud $I_0 = \lvert \tilde{U}_0 / Z \rvert$. En resonancia ($\omega = \omega_{LC} = 1/\sqrt{LC}$), las reactancias inductiva y capacitiva se cancelan exactamente, reduciendo la red a dos resistencias iguales $R$ en paralelo.

---

#### Parte 1) Impedancia equivalente $Z$ entre los terminales

La resistencia $R$, la inductancia $L$ y la capacitancia $C$ en serie de la rama derecha tienen impedancia:
$$Z_{\text{serie}} = R + i\omega L + \frac{1}{i\omega C} = R + i\omega L \left[ 1 - \left(\frac{\omega_{LC}}{\omega}\right)^2 \right]$$
donde $\omega_{LC} = \frac{1}{\sqrt{LC}}$ es la frecuencia angular característica (de resonancia) del circuito $LC$.

Conectando esta rama en paralelo con la resistencia central $R$, la impedancia total $Z$ entre los terminales resulta:
$$Z = \left( \frac{1}{R} + \frac{1}{R + i\omega L \left[ 1 - \left(\frac{\omega_{LC}}{\omega}\right)^2 \right]} \right)^{-1} = R\,\frac{R + i\omega L \left[ 1 - \left(\frac{\omega_{LC}}{\omega}\right)^2 \right]}{2R + i\omega L \left[ 1 - \left(\frac{\omega_{LC}}{\omega}\right)^2 \right]} \qquad \text{(2 ptos.)}$$

$$\boxed{Z = R\,\frac{R + i\omega L \left[ 1 - \left(\dfrac{\omega_{LC}}{\omega}\right)^2 \right]}{2R + i\omega L \left[ 1 - \left(\dfrac{\omega_{LC}}{\omega}\right)^2 \right]}, \qquad \omega_{LC} = \frac{1}{\sqrt{LC}}}$$

---

#### Parte 2) Amplitud de oscilación $I_0$ de la corriente alterna

Representamos el voltaje y la corriente mediante sus amplitudes complejas $\tilde{U}_0$ e $\tilde{I}_0$:
$$U(t) = U_0 \cos(\omega t) = \Re\left(\underbrace{U_0}_{=\tilde{U}_0} e^{i\omega t}\right)$$
$$I(t) = I_0 \cos(\omega t + \varphi) = \Re\left(\underbrace{I_0 e^{i\varphi}}_{=\tilde{I}_0} e^{i\omega t}\right)$$

Aplicando la «ley de Ohm» para amplitudes complejas:
$$\tilde{U}_0 = Z\,\tilde{I}_0 \implies \tilde{I}_0 = \frac{\tilde{U}_0}{Z}$$

Tomando el módulo de $\tilde{I}_0$, la amplitud de oscilación de la corriente que entra al circuito es:
$$I_0 = \left\lvert \frac{U_0}{R}\,\frac{2R + i\omega L \left[ 1 - \left(\frac{\omega_{LC}}{\omega}\right)^2 \right]}{R + i\omega L \left[ 1 - \left(\frac{\omega_{LC}}{\omega}\right)^2 \right]} \right\rvert = \frac{U_0}{R}\sqrt{\frac{(2R)^2 + (\omega L)^2 \left[ 1 - \left(\frac{\omega_{LC}}{\omega}\right)^2 \right]^2}{R^2 + (\omega L)^2 \left[ 1 - \left(\frac{\omega_{LC}}{\omega}\right)^2 \right]^2}} \qquad \text{(2 ptos.)}$$

$$\boxed{I_0 = \frac{U_0}{R}\sqrt{\frac{(2R)^2 + (\omega L)^2 \left[ 1 - \left(\dfrac{\omega_{LC}}{\omega}\right)^2 \right]^2}{R^2 + (\omega L)^2 \left[ 1 - \left(\dfrac{\omega_{LC}}{\omega}\right)^2 \right]^2}}}$$

---

#### Parte 3) Potencia disipada en resonancia

Suponiendo la definición física correcta de la frecuencia angular de resonancia $\omega = \omega_{LC} = \frac{1}{\sqrt{LC}}$ (en lugar de la expresión dimensionalmente incorrecta $\omega = 1/(LC)$ impresa en el enunciado):

**Análisis físico directo:** En resonancia ($\omega = \omega_{LC}$), los voltajes (y reactancias) sobre la capacitancia y la inductancia se compensan exactamente ($i\omega L + \frac{1}{i\omega C} = 0$, sin desfase), por lo que la impedancia de la rama derecha se reduce puramente a $R$. El circuito completo equivale entonces a dos resistencias $R$ en paralelo ($Z = R/2$, fase $\varphi = 0$) y la amplitud de corriente es $I_0 = \frac{2U_0}{R}$.

Por lo tanto, la potencia media disipada durante un período de oscilación es:
$$\bar{P} = \frac{U_0 I_0}{2}\cos\varphi = \frac{U_0}{2}\left(\frac{2U_0}{R}\right)\cos(0) = \frac{U_0^2}{R} \qquad \text{(2 ptos.)}$$

*(Nota de rúbrica oficial: en caso de usar literalmente el valor impreso pero incorrecto $\omega = 1/(LC)$, se acepta el desarrollo que intenta calcular amplitud y fase de la corriente para obtener la potencia promediada.)*

> **Nota:** Se destacan dos observaciones sobre el enunciado de la parte 3: (i) como reconoce la propia pauta oficial, $\omega = 1/(LC)$ carece de raíz cuadrada y tiene unidades de $\text{s}^{-2}$ en lugar de $\text{rad/s}$, correspondiendo la condición de resonancia a $\omega_{LC} = 1/\sqrt{LC}$; y (ii) aunque la pregunta habla de «potencia que se disipa [...] durante un período de oscilación», la pauta evalúa la **potencia promedio** por período $\bar{P} = \frac{1}{T}\int_0^T P(t)\,dt = \frac{U_0^2}{R}$ (si se pidiera la energía total disipada en un período $T = 2\pi/\omega_{LC}$, esta sería $E_T = \bar{P}T = \frac{2\pi U_0^2\sqrt{LC}}{R}$).

$$\boxed{\bar{P} = \frac{U_0^2}{R}}$$

**Verificación:**
- **Límites de frecuencia en $I_0$:**
  - En $\omega \to 0$ (corriente continua) o $\omega \to \infty$, el término $\left[1 - (\omega_{LC}/\omega)^2\right]^2 \to \infty$, por lo que la rama RLC se comporta como circuito abierto y $I_0 \to \frac{U_0}{R}\sqrt{1} = \frac{U_0}{R}$ (toda la corriente pasa por la resistencia central $R$).
  - En $\omega = \omega_{LC}$, el término reactivo se anula y $I_0 = \frac{U_0}{R}\sqrt{\frac{4R^2}{R^2}} = \frac{2U_0}{R}$, coincidente con dos resistencias $R$ en paralelo.
- **Disipación por rama en resonancia:** Cada resistencia $R$ disipa una potencia promedio $\frac{U_0^2}{2R}$, por lo que la suma de ambas ramas da $2 \cdot \frac{U_0^2}{2R} = \frac{U_0^2}{R}$.

---

## Resumen de resultados

| Problema | Parte | Cantidad | Resultado |
| :--- | :--- | :--- | :--- |
| **Problema 1** | a) | Capacitancia total $C_T$ | $C_T = \dfrac{(\varepsilon_1 + \varepsilon_2)A}{d}$ |
| | b) | Densidad de carga libre $\sigma_1$ | $\sigma_1 = \dfrac{C_1}{C_T}\dfrac{Q}{A} = \dfrac{\varepsilon_1}{\varepsilon_1 + \varepsilon_2}\dfrac{Q}{A}$ |
| | c) | Densidad de carga ligada $\sigma_{b_1}$ | $\sigma_{b_1} = -\varepsilon_0(\varepsilon_{r_1} - 1)\dfrac{V_{ab}}{d} = -\varepsilon_0(\varepsilon_{r_1} - 1)\dfrac{Q}{d\,C_T}$ |
| **Problema 2** | a) | Flujo magnético $\Phi_B$ | $\Phi_B = a^2 B_0 - \dfrac{\alpha a^2 (2z + a)}{2}$ |
| | b) | FEM y corriente inducida | $\varepsilon = \alpha a^2 v = -\alpha a^2\lvert v \rvert, \quad I = \dfrac{\alpha a^2 \lvert v \rvert}{R}$ |
| | c) | Sentido de la corriente | Horario (visto desde $+\hat{x}$) |
| | d) | Fuerza total sobre la espira | $\vec{F}_{\text{total}} = \left(\dfrac{\alpha^2 a^4 \lvert v \rvert}{R} - mg\right)\hat{z}$ |
| | e) | Velocidad terminal | $\lvert v_{\text{term}} \rvert = \dfrac{mgR}{\alpha^2 a^4}$ |
| **Problema 3** | 1) | Impedancia equivalente $Z$ | $Z = R\,\dfrac{R + i\omega L\left[1 - (\omega_{LC}/\omega)^2\right]}{2R + i\omega L\left[1 - (\omega_{LC}/\omega)^2\right]}$ |
| | 2) | Amplitud de corriente $I_0$ | $I_0 = \dfrac{U_0}{R}\sqrt{\dfrac{(2R)^2 + (\omega L)^2\left[1 - (\omega_{LC}/\omega)^2\right]^2}{R^2 + (\omega L)^2\left[1 - (\omega_{LC}/\omega)^2\right]^2}}$ |
| | 3) | Potencia promedio en resonancia ($\omega = \omega_{LC}$) | $\bar{P} = \dfrac{U_0^2}{R}$ |
