# Pauta Examen — Electromagnetismo FIS1533

> **Curso:** FIS1533 (Primer semestre 2026) · **Fecha:** 2 de julio de 2026 · **Evaluación:** Examen (Forma 1)

---

## Indicaciones Problema 1

Cada estudiante deberá resolver **solo uno** de los dos problemas que se presentan a continuación (1A o 1B), de acuerdo con el siguiente criterio:
- Quienes **no hayan rendido la I1** deberán resolver el **Problema 1A**.
- Quienes **no hayan rendido la I2** deberán resolver el **Problema 1B**.
- Quienes **hayan rendido ambas interrogaciones (I1 e I2)** podrán **elegir libremente** cuál de los dos problemas resolver.

> **Importante:** Se corregirá únicamente uno de los dos problemas. Si se resuelven ambos, se debe indicar/subir el escáner del problema que se desea corregir. Quienes resuelvan un problema distinto al que les corresponde serán calificados con 0 puntos en esta pregunta.

---

## Problema 1A

Ocho cargas puntuales se ubican en los vértices de un cubo de arista $a$. Si el sistema de referencia mostrado en la figura está situado en el centro del cubo:

a) **(1 pto.)** Determine la fuerza eléctrica sobre una carga $q$ situada en el centro del cubo en el caso en que todas las cargas de los vértices son iguales.

Considere ahora que la arista del cubo es $a = 400\,\mu\text{m} = 400 \times 10^{-6}\,\text{m}$ y la constante de Coulomb puede aproximarse como:
$$K \approx 9 \times 10^9\,\text{N}\cdot\text{m}^2/\text{C}^2$$

b) **(1 pto.)** Determine el trabajo necesario para traer una carga $q = 1\,\mu\text{C}$ desde el infinito hasta el centro del cubo cuando todas las cargas de los vértices son $Q_i = \sqrt{3}\,\mu\text{C}$ con $i = 1, \dots, 8$.

c) **(2 pts.)** Si la carga $Q_8$ ahora es tal que $Q_8 = 0$, determine el vector campo eléctrico en el centro del cubo debido sólo a las cargas ubicadas en los vértices del cubo.

d) **(2 pts.)** Para la configuración original de cargas [inciso a)], considere tres superficies cerradas:
- **Superficie $S_1$:** una esfera centrada en el centro del cubo con radio tal que $R > \sqrt{3}a/2$.
- **Superficie $S_2$:** un cubo más grande que el original (arista mayor a $a$), también centrado en el mismo punto, que encierra las 8 cargas.
- **Superficie $S_3$:** un cilindro centrado en el eje vertical del cubo, cuya base está en el plano $x$–$y$ y su radio basal es tal que $R > \sqrt{3}a/2$.

Para cada caso:
- **i)** Determine el flujo eléctrico neto a través de la superficie.
- **ii)** ¿Es posible que el flujo eléctrico neto a través de una superficie cerrada sea cero aun cuando el campo eléctrico no sea nulo en la superficie? Explique.

> **[Figura]:** Cubo de arista $a$ con el origen $O$ del sistema de referencia ubicado exactamente en su centro geométrico. Desde $O$ parten los vectores unitarios $\hat{\imath}$ (hacia adelante-izquierda, saliendo hacia la cara frontal), $\hat{\jmath}$ (hacia la derecha) y $\hat{k}$ (verticalmente hacia arriba). En la cara inferior ($z = -a/2$) los vértices se rotulan en sentido antihorario visto desde arriba: $Q_1$ (atrás-izquierda, $(-a/2, -a/2, -a/2)$), $Q_2$ (adelante-izquierda, $(+a/2, -a/2, -a/2)$), $Q_3$ (adelante-derecha, $(+a/2, +a/2, -a/2)$) y $Q_4$ (atrás-derecha, $(-a/2, +a/2, -a/2)$). En la cara superior ($z = +a/2$) los vértices están directamente sobre los inferiores: $Q_5$ sobre $Q_1$, $Q_6$ sobre $Q_2$, $Q_7$ sobre $Q_3$, y $Q_8$ sobre $Q_4$ (en $(-a/2, +a/2, +a/2)$).

---

### Solución Problema 1A

**Idea:** Usar la simetría de inversión del cubo para las partes a) y c), la superposición escalar del potencial eléctrico en b), y la ley de Gauss $\Phi_E = \oint \vec{E}\cdot d\vec{A} = Q_{\text{enc}}/\varepsilon_0$ en d), distinguiendo si se incluye o no la carga central $q_0$ mencionada en a).

#### Parte a) Fuerza en el centro (1.0 pto.)

Por simetría, las fuerzas ejercidas por cargas en vértices diametralmente opuestos respecto del centro se cancelan par a par. Por lo tanto:
$$\boxed{\vec{F} = 0} \qquad \text{(1.0 pts.)}$$

---

#### Parte b) Trabajo para traer la carga al centro (1.0 pto.)

El trabajo es $W = q V_{\text{centro}}$, donde el potencial es la suma escalar de las 8 contribuciones:
$$V = \sum_{i=1}^{8} K\frac{Q}{r} = 8K\frac{Q}{r} \qquad \text{(0.25 pts.)}$$
con la distancia desde el centro a cada vértice igual a la semidiagonal del cubo:
$$r = \frac{\sqrt{3}}{2}\,a \qquad \text{(0.25 pts.)}$$

Entonces, sustituyendo $Q = \sqrt{3}\,\mu\text{C}$:
$$V = 8K\frac{\sqrt{3}\,\mu\text{C}}{\dfrac{\sqrt{3}a}{2}} = 8K\frac{2}{a}\,\mu\text{C} = \frac{16K}{a}\,\mu\text{C} \qquad \text{(0.25 pts.)}$$

Por tanto, con $q = 1\,\mu\text{C} = 10^{-6}\,\text{C}$ (y representando el factor $\mu\text{C}$ el valor $Q/\sqrt{3} = 10^{-6}\,\text{C}$):
$$W = qV = \frac{16Kq}{a}\,\mu\text{C}$$
Sustituyendo $K = 9\times 10^9\,\text{N}\cdot\text{m}^2/\text{C}^2$, $a = 400\,\mu\text{m} = 400\times 10^{-6}\,\text{m}$ y $Q = \sqrt{3}\,\mu\text{C}$:
$$W = \frac{16 \times (9\times 10^9) \times 10^{-6} \times 10^{-6}}{400\times 10^{-6}} = 360\,\text{J}$$
$$\boxed{W \approx 360\,\text{J}} \qquad \text{(0.25 pts.)}$$

---

#### Parte c) Campo eléctrico con una carga faltante (2.0 pts.)

El campo total en el centro con las 8 cargas iguales es cero. Al hacer $Q_8 = 0$, el campo resultante de las 7 cargas restantes es:
$$\vec{E} = -\vec{E}_{\text{faltante}} = -\vec{E}_8 \qquad \text{(0.25 pts.)}$$

El campo producido por $Q_8$ en el origen es:
$$\vec{E}_{\text{faltante}} = K\frac{Q}{r^2}\,\hat{r}_8 \qquad \text{(0.25 pts.)}$$
con:
$$r = \frac{\sqrt{3}a}{2} \qquad \text{(0.25 pts.)}$$
y el vector unitario dirigido desde $Q_8$ en $\frac{a}{2}(-\hat{\imath} + \hat{\jmath} + \hat{k})$ hacia el origen:
$$\hat{r}_8 = -\left(\frac{1}{\sqrt{3}}(-\hat{\imath} + \hat{\jmath} + \hat{k})\right) \qquad \text{(0.5 pts.)}$$

Nótese que $r^2 = \dfrac{3}{4}a^2$. Por tanto:
$$\vec{E}_{\text{faltante}} = -K\frac{Q}{\frac{3}{4}a^2}\left(\frac{1}{\sqrt{3}}(-\hat{\imath} + \hat{\jmath} + \hat{k})\right) = -\frac{4KQ}{3a^2\sqrt{3}}(-\hat{\imath} + \hat{\jmath} + \hat{k})$$

Es decir que:
$$\vec{E} = -\vec{E}_{\text{faltante}} = \frac{4KQ}{3a^2\sqrt{3}}(-\hat{\imath} + \hat{\jmath} + \hat{k}) \qquad \text{(0.25 pts.)}$$

Sustituyendo el valor de la carga $Q = \sqrt{3}\,\mu\text{C} = \sqrt{3}\times 10^{-6}\,\text{C}$:
$$\vec{E} = \frac{4K}{3a^2}\times 10^{-6}(-\hat{\imath} + \hat{\jmath} + \hat{k})$$

Con $K = 9\times 10^9\,\text{N}\cdot\text{m}^2/\text{C}^2$ y $a = 400\,\mu\text{m}$:
$$\vec{E} = \frac{3}{(200)^2}\times 10^{15}(-\hat{\imath} + \hat{\jmath} + \hat{k})\,\text{N/C} = 75\times 10^9(-\hat{\imath} + \hat{\jmath} + \hat{k})\,\text{N/C}$$
$$\boxed{\vec{E} = 75 \times 10^9(-\hat{\imath} + \hat{\jmath} + \hat{k})\,\text{N/C}} \qquad \text{(0.5 pts.)}$$

---

#### Parte d) Análisis de flujo eléctrico (2.0 pts.)

Se presentan dos desarrollos en la pauta oficial dependiendo de si el estudiante consideró en la configuración original la carga central $q_0$ del inciso a) (con cada vértice de carga $Q$).

##### Caso 1: No considera carga central

- **i)** Para determinar el flujo eléctrico neto, se aplica la ley de Gauss:
  $$\Phi_E = \oint \vec{E}\cdot d\vec{A} = \frac{Q_{\text{enc}}}{\varepsilon_0} \qquad \text{(0.25 pts.)}$$
  El flujo a través de cada superficie cerrada queda determinado únicamente por la carga neta encerrada, independientemente de la forma geométrica de la superficie:
  - Para $S_1$ (esfera de radio $R > \sqrt{3}a/2$) y $S_2$ (cubo mayor que encierra las 8 cargas), se encierran todas las cargas de los vértices:
    $$Q_{\text{enc}} = \sum_{i=1}^{8} Q_i = 8Q \implies \boxed{\Phi_{S_1} = \Phi_{S_2} = \frac{8Q}{\varepsilon_0}} \qquad \text{(0.25 pts.)}$$
    Ambas superficies entregan el mismo flujo (0.25 pts.).
  - Para $S_3$ (cilindro con base en el plano $x$–$y$, centrado en el eje $z$ y radio $R > \sqrt{3}a/2$ en el semiespacio $z \ge 0$), se encierran sólo las 4 cargas superiores ($Q_5, Q_6, Q_7, Q_8$):
    $$Q_{\text{enc}} = \sum_{i=5}^{8} Q_i = 4Q \implies \boxed{\Phi_{S_3} = \frac{4Q}{\varepsilon_0}} \qquad \text{(0.25 pts.)}$$
    donde $Q_{\text{enc}}$ corresponde únicamente a las cargas contenidas dentro del cilindro.

- **ii)** **Sí es posible** que $\Phi_E = 0$ aun cuando $\vec{E} \neq 0$ sobre la superficie (0.5 pts.). Esto ocurre cuando la carga neta encerrada es cero ($Q_{\text{enc}} = 0$), por ejemplo, cuando la cantidad de líneas de campo (flujo) que entran a la superficie es igual a la cantidad que salen de ella (como en una superficie que encierra un dipolo eléctrico o que no encierra ninguna carga) (0.5 pts.).

##### Caso 2: Sí considera carga central ($q_0$)

- **i)** Aplicando la ley de Gauss $\Phi_E = \oint \vec{E}\cdot d\vec{A} = Q_{\text{enc}}/\varepsilon_0$ (0.25 pts.):
  - Para $S_1$ y $S_2$ se encierran las 8 cargas de los vértices más la carga central $q_0$:
    $$Q_{\text{enc}} = \sum_{i=1}^{8} Q_i + q_0 = 8Q + q_0 \implies \boxed{\Phi_{S_1} = \Phi_{S_2} = \frac{8Q + q_0}{\varepsilon_0}} \qquad \text{(0.25 pts.)}$$
    Ambas superficies entregan el mismo flujo (0.25 pts.).
  - Para $S_3$ se encierran las 4 cargas superiores y, según lo indicado por el estudiante respecto de si $q_0$ en el plano $x$–$y$ queda justo bajo o justo sobre la base del cilindro:
    - Sin incluir $q_0$:
      $$Q_{\text{enc}} = \sum_{i=5}^{8} Q_i = 4Q \implies \boxed{\Phi_{S_3,\,\text{sin } q_0} = \frac{4Q}{\varepsilon_0}} \qquad \text{(0.25 pts.)}$$
    - O bien incluyendo $q_0$:
      $$Q_{\text{enc}} = \sum_{i=5}^{8} Q_i + q_0 = 4Q + q_0 \implies \boxed{\Phi_{S_3,\,\text{con } q_0} = \frac{4Q + q_0}{\varepsilon_0}} \qquad \text{(0.25 pts.)}$$

- **ii)** **Sí es posible** que $\Phi_E = 0$ aun cuando $\vec{E} \neq 0$ (0.5 pts.): ocurre si $Q_{\text{enc}} = 0$, es decir, cuando entra y sale igual flujo neto de la superficie (como en el caso de un dipolo eléctrico) (0.5 pts.).

---

## Problema 1B

Considere el circuito mostrado en la figura alimentado por una fuente $\mathcal{E}$. Las resistencias son tales que $R_1 = R_2 = R_4 = R_6 = R$, $R_3 = 2R = R_5$ y la capacitancia es $C$ conocidos.

a) **(2 pts.)** Después de un largo tiempo en que el interruptor está cerrado, determine la corriente que circula por la batería y por cada una de las resistencias del circuito.

b) **(1 pto.)** Determine la diferencia de potencial del capacitor cuando se encuentra completamente cargado.

c) **(1 pto.)** Determine la energía almacenada en el capacitor en el régimen estacionario. ¿Cómo cambia la energía almacenada en el capacitor si entre las placas de éste hay un material dieléctrico de constante dieléctrica $\kappa$?

d) **(2 pts.)** Si la batería se desconecta en $t = 0$ (el interruptor se abre), determinar las ecuaciones para $q(t)$ y $\Delta V_C(t)$ en el capacitor durante la descarga. Asuma conocida la carga inicial del capacitor $q(t = 0)$.

> **[Figura]:** Circuito formado por una fuente de voltaje continua $\mathcal{E}$ (borne positivo arriba, negativo abajo) conectada en serie con un interruptor (dibujado abierto en la rama vertical superior izquierda) y la resistencia $R_6$ (en la rama horizontal inferior izquierda), alimentando los nodos superior ($a$) e inferior ($d$) de un puente en rombo:
> - **Rama izquierda del puente ($a \to b \to d$):** resistencia $R_1$ entre $a$ y el nodo izquierdo $b$; resistencia $R_2$ entre $b$ y $d$.
> - **Rama derecha del puente ($a \to c \to d$):** resistencia $R_3$ entre $a$ y el nodo derecho $c$; resistencia $R_4$ entre $c$ y $d$.
> - **Rama central horizontal ($b$–$c$):** une los nodos $b$ y $c$, y contiene el condensador $C$ (al lado izquierdo, junto a $b$) en serie con la resistencia $R_5$ (al lado derecho, junto a $c$).

---

### Solución Problema 1B

**Idea:** En régimen estacionario con el interruptor cerrado, el capacitor actúa como rama abierta ($I_5 = 0$), reduciendo el circuito a un puente paralelo en serie con $R_6$. Con la diferencia de potencial $\Delta V_{cb}$ sobre el condensador se calcula la energía almacenada $U = \frac{1}{2}C(\Delta V_{cb})^2$ y su variación al introducir un dieléctrico a voltaje constante. Al abrir el interruptor en $t = 0$, la descarga ocurre por la resistencia equivalente vista desde el condensador en el circuito $RC$.

#### Parte a) Corrientes en régimen estacionario (2.0 pts.)

Después de un largo tiempo, el capacitor se encuentra completamente cargado y se comporta como un circuito abierto (no circula corriente por la rama central $b$–$c$), por lo que:
$$I_5 = 0 \qquad \text{(0.3 pts.)}$$

Las resistencias $R_1$ y $R_2$ quedan en serie, al igual que $R_3$ y $R_4$:
$$R_{\text{izq}} = R_1 + R_2 = 2R \qquad \text{(0.2 pts.)}$$
$$R_{\text{der}} = R_3 + R_4 = 3R \qquad \text{(0.2 pts.)}$$

La resistencia equivalente del puente ($R_{\text{izq}}$ y $R_{\text{der}}$ en paralelo) es:
$$R_p = \left(\frac{1}{R_1 + R_2} + \frac{1}{R_3 + R_4}\right)^{-1} = \frac{(R_1 + R_2)(R_3 + R_4)}{R_1 + R_2 + R_3 + R_4} = \frac{6R}{5} \qquad \text{(0.2 pts.)}$$

Como $R_p$ está en serie con $R_6$ (0.2 pts.), la corriente que pasa por la batería y por $R_6$ es:
$$I(\infty) = \frac{\mathcal{E}}{R_6 + R_p} = \frac{5\mathcal{E}}{11R} \qquad \text{(0.3 pts.)}$$

Dividiendo la corriente entre la rama izquierda ($R_1, R_2$) y la rama derecha ($R_3, R_4$):
$$I_{\text{izq}} = \frac{\Delta V_{ad}}{R_{\text{izq}}} = \frac{I(\infty) R_p}{R_{\text{izq}}} = \frac{\mathcal{E} R_p}{(R_6 + R_p)(R_1 + R_2)} = \frac{3\mathcal{E}}{11R} \qquad \text{(0.3 pts.)}$$
$$I_{\text{der}} = \frac{\Delta V_{ad}}{R_{\text{der}}} = \frac{I(\infty) R_p}{R_{\text{der}}} = \frac{\mathcal{E} R_p}{(R_6 + R_p)(R_3 + R_4)} = \frac{2\mathcal{E}}{11R} \qquad \text{(0.3 pts.)}$$

$$\boxed{I_{\text{bat}} = I_6 = \frac{5\mathcal{E}}{11R}, \qquad I_1 = I_2 = \frac{3\mathcal{E}}{11R}, \qquad I_3 = I_4 = \frac{2\mathcal{E}}{11R}, \qquad I_5 = 0}$$

---

#### Parte b) Diferencia de potencial en el capacitor cargado (1.0 pto.)

Consideramos que la diferencia de potencial en el capacitor es $\Delta V_{cb} = V_b - V_c$, ya que al no pasar corriente por la rama central, la resistencia $R_5$ no influye (0.25 pts.). Luego:
$$V_b = V_a - I_{\text{izq}} R_1 \qquad \text{(0.25 pts.)}$$
$$V_c = V_a - I_{\text{der}} R_3 \qquad \text{(0.25 pts.)}$$
$$\Delta V_{cb} = V_b - V_c = -I_{\text{izq}} R_1 + I_{\text{der}} R_3 = -\frac{3\mathcal{E}}{11} + \frac{4\mathcal{E}}{11} = \frac{\mathcal{E}}{11}$$
$$\boxed{\Delta V_{cb} = \frac{\mathcal{E}}{11}} \qquad \text{(0.25 pts.)}$$

---

#### Parte c) Energía almacenada y efecto de un dieléctrico (1.0 pto.)

La energía almacenada en el capacitor en régimen estacionario está dada por su carga máxima o por la diferencia de potencial calculada en b) (0.3 pts.):
$$U = \frac{Q_{\max}^2}{2C}$$
O bien, considerando $\Delta V_{cb} = Q_{\max}/C$ *(en la pauta oficial se lee por error tipográfico «consideranco $\Delta V_{cd}$»)*:
$$U = \frac{C(\Delta V_{cb})^2}{2} = \frac{C\left(\mathcal{E}/11\right)^2}{2} = \frac{C\mathcal{E}^2}{242}$$
$$\boxed{U = \frac{C\mathcal{E}^2}{242}} \qquad \text{(0.5 pts.)}$$

Si se introduce un dieléctrico de constante dieléctrica $\kappa$, la capacitancia aumenta a $C' = \kappa C$. Como el capacitor permanece conectado al circuito, la diferencia de potencial entre sus placas se mantiene constante ($\Delta V_{cb}$ fijo, pues no circula corriente en estado estacionario), por lo que la energía almacenada pasa a ser:
$$\boxed{U' = \frac{C'(\Delta V_{cb})^2}{2} = \kappa U} \quad (\text{aumenta en un factor }\kappa\text{ respecto a la original}) \qquad \text{(0.2 pts.)}$$

---

#### Parte d) Descarga del capacitor al abrir el interruptor en $t = 0$ (2.0 pts.)

Cuando se abre el interruptor, no pasa corriente por la resistencia $R_6$ (0.2 pts.). Además, las resistencias $R_1$ y $R_3$ quedan en serie, al igual que $R_2$ y $R_4$ (0.2 pts.):
$$R_{\text{sup}} = R_1 + R_3 = 3R \qquad \text{(0.2 pts.)}$$
$$R_{\text{inf}} = R_2 + R_4 = 2R \qquad \text{(0.2 pts.)}$$

Ambas quedan en paralelo entre sí y frente a la rama central:
$$R_{\text{eq1}} = \frac{R_{\text{sup}} R_{\text{inf}}}{R_{\text{sup}} + R_{\text{inf}}} = \frac{6R}{5} \qquad \text{(0.2 pts.)}$$

Y esta última queda en serie con $R_5 = 2R$:
$$R_{\text{eq}} = R_{\text{eq1}} + R_5 = \frac{16R}{5} \qquad \text{(0.2 pts.)}$$

Aplicando la ley de mallas de Kirchhoff en el circuito de descarga se obtiene la ecuación diferencial:
$$I R_{\text{eq}} + \frac{q}{C} = 0 \implies \frac{dq}{dt} + \frac{q}{R_{\text{eq}} C} = 0 \qquad \text{(0.4 pts.)}$$

Definiendo $\tau = R_{\text{eq}} C = \dfrac{16RC}{5}$ y resolviendo por separación de variables con $q(0) = q_i$:
$$\int_{q_i}^{q} \frac{dq'}{q'} = -\int_0^t \frac{dt'}{\tau} \implies \ln\left(\frac{q}{q_i}\right) = -\frac{t}{\tau}$$
$$\boxed{q(t) = q_i\,e^{-t/\tau} = q_i\,e^{-5t/(16RC)}} \qquad \text{(0.2 pts.)}$$

Considerando $\Delta V_C = q/C$, la diferencia de potencial es:
$$\boxed{\Delta V_C(t) = \frac{q_i}{C}\,e^{-t/\tau} = \frac{q_i}{C}\,e^{-5t/(16RC)}} \qquad \text{(0.2 pts.)}$$

---

## Problema 2

Una espira cuadrada de resistencia $R$ y arista $a$ se mueve con velocidad constante $\vec{v}$ hacia una zona de campo magnético constante $\vec{B}$ entrante, como se visualiza en la figura.

a) **(5 pts.)** Determine la fem inducida en la espira, la corriente inducida, y el sentido de la corriente inducida en las siguientes tres etapas:
- **I)** Antes de que la espira entre en la región donde hay un campo magnético $\vec{B}$.
- **II)** Cuando está parcialmente inmersa en el campo $\vec{B}$.
- **III)** Cuando avanza completamente inmersa en el campo $\vec{B}$.

b) **(1 pto.)** Utilizando la Ley de Lenz, indique el sentido en que debe aplicarse una fuerza externa para mantener la rapidez constante de la espira mientras ingresa a la región con campo magnético.

Asumir que la corriente transporta cargas positivas.

> **[Figura]:** Vista frontal en el plano de la página. A la izquierda se encuentra una espira conductora cuadrada de lado $a$ que se traslada horizontalmente hacia la derecha con velocidad constante $\vec{v}$. A la derecha de una línea recta vertical fronteriza se extiende una región con campo magnético uniforme $\vec{B}$ apuntando perpendicularmente hacia adentro de la página (representado por una matriz de cruces $\times$). En el instante ilustrado, la espira está ingresando parcialmente a la zona con campo magnético.

---

### Solución

**Idea:** Calcular el flujo magnético $\Phi_B = \int \vec{B}\cdot d\vec{A}$ que atraviesa la espira en cada etapa y aplicar la ley de inducción de Faraday, $\varepsilon = -d\Phi_B/dt$, junto con la ley de Ohm $I = |\varepsilon|/R$. Utilizar la ley de Lenz para determinar el sentido de la corriente inducida y la fuerza magnética que se opone al movimiento.

#### Parte a) Fem inducida, corriente y sentido en las tres etapas (5.0 pts.)

- **a I) Antes de que la espira entre en la región de campo magnético (1.0 pto.):**  
  Cuando la espira está completamente fuera de la región con campo magnético, $\vec{B} = 0$ en todo su interior, por lo que el flujo magnético a través de ella es nulo ($\Phi_B = 0$) y no varía en el tiempo. Por lo tanto, no habrá fem ni corriente inducida:
  $$\boxed{\varepsilon = 0, \qquad I = 0} \qquad \text{(1.0 pto.)}$$

- **a II) Cuando está parcialmente inmersa en el campo $\vec{B}$ (3.0 pts.):**  
  Considerando que el vector área $d\vec{A}$ apunta en la misma dirección que el campo magnético (entrante a la página), y sea $x$ la distancia que la espira ha penetrado dentro de la región con campo magnético ($0 < x < a$), el área inmersa es $A_{\text{inm}} = ax$ y el flujo magnético es:
  $$\Phi_B = B A_{\text{inm}} = Bax \qquad \text{(0.5 pts.)}$$
  La variación temporal del flujo magnético, siendo $\dfrac{dx}{dt} = v$ la rapidez de la espira, es:
  $$\frac{d\Phi_B}{dt} = Ba\frac{dx}{dt} = Bav \qquad \text{(1.0 pts.)}$$
  Por la ley de Faraday ($\varepsilon = -d\Phi_B/dt$), la fem inducida es:
  $$\boxed{\varepsilon = -Bav} \qquad \text{(0.5 pts.)}$$
  La magnitud de la corriente inducida en la espira de resistencia $R$ es:
  $$\boxed{I = \frac{|\varepsilon|}{R} = \frac{Bav}{R}} \qquad \text{(0.5 pts.)}$$
  Como el flujo magnético entrante está aumentando, por la ley de Lenz la corriente inducida genera un flujo saliente que se opone al aumento, de modo que **la corriente circulará en sentido antihorario** (0.5 pts.).

- **a III) Cuando avanza completamente inmersa en el campo $\vec{B}$ (1.0 pto.):**  
  Cuando toda la espira se encuentra dentro de la región de campo magnético uniforme, el flujo magnético alcanza su valor máximo $\Phi_B = Ba^2$, pero éste permanece constante en el tiempo ($\frac{d\Phi_B}{dt} = 0$), por lo que no habrá fem ni corriente inducida:
  $$\boxed{\varepsilon = 0, \qquad I = 0} \qquad \text{(1.0 pto.)}$$

---

#### Parte b) Sentido de la fuerza externa al ingresar (1.0 pto.)

Al entrar la espira en la región con campo magnético entrante, el flujo hacia adentro aumenta, por lo que la corriente inducida (en sentido antihorario) genera un campo magnético saliente para oponerse a dicha variación (0.5 pts.).

Sobre el segmento vertical derecho de la espira (inmerso en $\vec{B}$ entrante, con corriente antihoraria hacia arriba), la fuerza magnética $\vec{F}_m = I\vec{L}\times\vec{B}$ apunta hacia la **izquierda** (oponiéndose al movimiento, lo cual también se deduce directamente de la ley de Lenz). Por lo tanto, para mantener la velocidad $\vec{v}$ constante ($\sum \vec{F} = 0$), **la fuerza externa debe aplicarse hacia la derecha** (0.5 pts.).

$$\boxed{\vec{F}_{\text{ext}} \text{ hacia la derecha (en la dirección de } \vec{v}\text{)}}$$

**Verificación:**
- **Balance energético en a II) y b):** La potencia suministrada por la fuerza externa es $P_{\text{ext}} = F_{\text{ext}} v = (IaB)v = \left(\frac{Bav}{R}\right)aBv = \frac{B^2 a^2 v^2}{R}$, que iguala exactamente a la potencia disipada por efecto Joule en la resistencia, $P_R = I^2 R = \frac{B^2 a^2 v^2}{R}$.
- **Unidades:** $[Bav] = \text{T}\cdot\text{m}\cdot(\text{m/s}) = \text{V}$, $[Bav/R] = \text{V}/\Omega = \text{A}$.

---

## Problema 3

Considere un circuito formado por dos mallas que comparten una inductancia ideal $L$, como se muestra en la figura. Cada una de las mallas contiene un interruptor: $S_1$ para la malla izquierda y $S_2$ para la derecha. El condensador $C$ inicialmente se encuentra descargado.

- **Etapa I:** Inicialmente ambos interruptores están abiertos. En $t = 0$ se cierra $S_1$, permaneciendo $S_2$ abierto. Por tanto se forma un circuito $RL$ conectado a una FEM.
  - **a) (2 pts.)** Determine la diferencia de potencial $v_L$ sobre la inductancia (entre los puntos $c$ y $d$ de la figura), en ese instante. Justifique físicamente su respuesta.

- **Etapa II:** Después de un tiempo muy largo ($t \to \infty$) el circuito (con $S_1$ cerrado y $S_2$ abierto) alcanza un régimen permanente.
  - **b) (2 pts.)** Determine la corriente $i_L$ que circula por el cable entre los puntos $c$ y $d$ en este régimen. Justifique su respuesta.

- **Etapa III:** Suponga que el circuito, con $S_1$ cerrado y $S_2$ abierto, se encuentra en régimen permanente. En un instante dado, denotado como $t = 0$ (diferente al de la etapa I), $S_1$ se abre simultáneamente con el cierre de $S_2$.
  - **c) (1 pto.)** Determine la corriente que circula por el cable que contiene el condensador, $i_C(t)$, y la diferencia de potencial $v_C(t)$ sobre éste (entre los puntos $e$ y $f$ de la figura), para $t > 0$.
  - **d) (1 pto.)** Explique por qué el sistema no alcanza un régimen permanente cuando $t \to \infty$.

> **[Figura]:** Circuito rectangular de dos mallas adyacentes que comparten la rama vertical central entre los nodos $c$ (arriba) y $d$ (abajo), donde se encuentra la inductancia ideal $L$ con una flecha de corriente $i_L$ apuntando hacia **abajo** (de $c$ hacia $d$):
> - **Malla izquierda ($a$–$c$–$d$–$b$–$a$):** en el lado izquierdo ($a$–$b$) está la fuente de fem $\mathcal{E}$ con su borne positivo ($+$) arriba conectado a $a$ y su borne negativo abajo conectado a $b$. En la rama superior ($a$–$c$) circula la corriente $i_R$ hacia la derecha y está ubicado el interruptor $S_1$. En la rama inferior ($b$–$d$) está conectada la resistencia $R$.
> - **Malla derecha ($c$–$e$–$f$–$d$–$c$):** en la rama superior ($c$–$e$) está ubicado el interruptor $S_2$; la rama inferior ($d$–$f$) es un conductor ideal; en el lado derecho ($e$–$f$) se encuentra el condensador $C$ con una flecha de corriente $i_C$ apuntando hacia **arriba** (de $f$ hacia $e$).

---

### Solución

**Idea:** Usar la propiedad de continuidad de la corriente en un inductor ($v_L = L\,di_L/dt$): en $t = 0^+$ al cerrar $S_1$ la corriente no puede saltar y $L$ actúa como circuito abierto; en $t \to \infty$ ($di_L/dt = 0$) el inductor actúa como cortocircuito ideal. Al conmutar a la Etapa III ($S_1$ abierto, $S_2$ cerrado), la malla derecha forma un oscilador $LC$ ideal sin disipación con corriente inicial $i_L(0) = \mathcal{E}/R$ y voltaje inicial $v_C(0) = 0$.

#### Etapa I — Parte a) Diferencia de potencial $v_L(0^+)$ (2.0 pts.)

##### Solución de a)

Al cerrar el interruptor $S_1$, mientras $S_2$ permanece abierto, se forma un circuito $RL$ en serie conectado a la FEM $\mathcal{E}$.

- La corriente a través de una inductancia no puede cambiar de manera instantánea, ya que el potencial en sus terminales satisface la relación:
  $$v_L = L\frac{di_L}{dt}$$
  donde $i_L$ es la corriente que circula por la inductancia. *(0.4 pts.)*
- Como antes del cierre del interruptor la corriente era nula, se tiene la condición inicial $i_L(0^-) = 0$, y por continuidad de la corriente en una inductancia:
  $$i_L(0^+) = 0 \qquad \text{(0.4 pts.)}$$
- En consecuencia, inmediatamente después de cerrar el interruptor la corriente que circula por la resistencia también es nula:
  $$i_R(0^+) = 0 \qquad \text{(0.4 pts.)}$$
- La caída de potencial sobre la resistencia es:
  $$v_R(0^+) = R\,i_R(0^+) = 0 \qquad \text{(0.4 pts.)}$$
- Aplicando la ley de voltajes de Kirchhoff a la malla *(la pauta oficial omite tipográficamente la letra $v$ en ${}_L(0^+)$)*:
  $$\mathcal{E} = v_L(0^+) + v_R(0^+) = v_L(0^+)$$
  es decir, toda la diferencia de potencial de la fuente aparece inicialmente sobre la inductancia:
  $$\boxed{v_L(0^+) = \mathcal{E}} \qquad \text{(0.4 pts.)}$$

##### Solución alternativa de a)

Al cerrar el interruptor $S_1$, mientras $S_2$ permanece abierto, se forma un circuito $RL$ en serie conectado a la FEM $\mathcal{E}$.

> **[Figura equivalente en $t = 0$]:** Circuito de una sola malla con la fuente $\mathcal{E}$ (borne $+$ arriba), la resistencia $R$ en la rama inferior, y el inductor reemplazado por un **circuito abierto** en el lado derecho con polaridad $+$ arriba, $-$ abajo y diferencia de potencial $v_L$, indicando $i_R = 0$ en la rama superior.

- En el tiempo $t = 0$ la inductancia se comporta como un circuito abierto (ver circuito equivalente). *(0.4 pts.)*
- Esto ocurre porque la inductancia tiene un comportamiento inercial, es decir, la corriente no puede cambiar instantáneamente. *(0.4 pts.)*
- Del circuito equivalente vemos que $i_R = 0$. *(0.4 pts.)*
- Por tanto, $v_R = 0$. *(0.4 pts.)*
- Esto implica que $\boxed{v_L = \mathcal{E}}$. *(0.4 pts.)*

---

#### Etapa II — Parte b) Corriente $i_L$ en régimen permanente (2.0 pts.)

##### Solución de b)

Después de un tiempo suficientemente largo, el circuito alcanza el régimen permanente. Por tanto, la corriente eléctrica se estabiliza en un valor constante, lo que implica:
$$\frac{di_L}{dt} = 0 \qquad \text{(1.0 pts.)}$$

Por tanto:
$$v_L = L\frac{di_L}{dt} = 0 \qquad \text{(0.5 pts.)}$$

Entonces la inductancia se comporta como un cortocircuito ideal. Aplicando la ley de Kirchhoff a la malla izquierda:
$$\mathcal{E} - R i_L = 0$$
Por lo tanto:
$$\boxed{i_L = \frac{\mathcal{E}}{R}} \qquad \text{(0.5 pts.)}$$

##### Solución alternativa de b)

En un circuito de corriente continua, para $t \to \infty$, la inductancia se comporta como un cortocircuito.

> **[Figura equivalente en $t \to \infty$]:** Circuito de una sola malla con la fuente $\mathcal{E}$ (borne $+$ arriba), la resistencia $R$ en la rama inferior y un cable recto ideal (cortocircuito) en el lado derecho en lugar de $L$, indicando $v_L = 0$ entre sus extremos y corriente $i_R$ circulando hacia la derecha en la rama superior.

- Para $t \to \infty$, la inductancia se comporta como un cortocircuito (ver circuito equivalente). *(0.5 pts.)*
- Del circuito equivalente concluimos que:
  $$\boxed{i_R = i_L = \frac{\mathcal{E}}{R}} \qquad \text{(0.5 pts.)}$$
- El comportamiento de cortocircuito de la inductancia se debe a que la corriente eléctrica se encuentra en estado estacionario, lo que implica que la diferencia de potencial es $v_L = 0$. *(1.0 pts.)*

---

#### Etapa III — Parte c) Corriente $i_C(t)$ y voltaje $v_C(t)$ para $t > 0$ (1.0 pto.)

Inicialmente el circuito se encuentra en régimen permanente. En el nuevo instante $t = 0$, simultáneamente se abre $S_1$ y se cierra $S_2$. Entonces la fuente y la resistencia quedan desconectadas y permanece un circuito ideal formado únicamente por la inductancia $L$ y el condensador $C$.

> **[Figura del circuito LC]:** Malla única rectangular con la inductancia $L$ en la rama izquierda (corriente inicial $i_L(0)$ apuntando hacia abajo) y el condensador $C$ en la rama derecha (corriente $i_C(t)$ apuntando hacia arriba). El sentido de circulación continuo es antihorario, por lo que $i_C(t) = i_L(t)$.

Las condiciones iniciales son:
$$i_L(0) = \frac{\mathcal{E}}{R} \quad \text{(0.1 pts.)}, \qquad v_C(0) = 0 \quad \text{(0.1 pts.)}$$
La última condición se cumple porque el condensador permanecía aislado antes de cerrarse $S_2$ y además se encontraba descargado.

Nótese que $i_C(t) = i_L(t)$ (y por tanto $i_C(0) = i_L(0)$). Aplicando las reglas de Kirchhoff alrededor de la malla (con la convención de voltaje sobre el condensador positivo en la placa inferior $f$ por donde entra $i_C$, de modo que $v_C = V_f - V_e$, $i_C = C\frac{dv_C}{dt}$ y $v_L = V_c - V_d = L\frac{di_L}{dt}$):
$$v_L + v_C = 0 \qquad \text{(0.1 pts.)}$$

Como $v_L = L\dfrac{di_L}{dt}$, $i_C = C\dfrac{dv_C}{dt}$ y $i_C = i_L$, derivando respecto al tiempo la ecuación de malla se obtiene:
$$L\frac{d^2 i_L}{dt^2} + \frac{1}{C}i_C = 0 \implies \frac{d^2 i_L}{dt^2} + \frac{1}{LC}i_L = 0 \qquad \text{(0.1 pts.)}$$

Por comparación con la ecuación del oscilador armónico simple, la solución general para la corriente es *(la pauta oficial usa indistintamente $\omega_0$ y $\omega$ para la frecuencia natural)*:
$$i_L(t) = A\cos(\omega t) + B\sin(\omega t) \qquad \text{(0.1 pts.)}$$
con frecuencia angular natural:
$$\omega = \frac{1}{\sqrt{LC}} \qquad \text{(0.1 pts.)}$$

Usando las condiciones iniciales:
- $i_L(0) = \dfrac{\mathcal{E}}{R} \implies A = \dfrac{\mathcal{E}}{R}$ *(0.1 pts.)*
- $v_C(0) = 0 \implies v_L(0) = -v_C(0) = 0 \implies \dfrac{di_L}{dt}(0) = 0 \implies B\omega = 0 \implies B = 0$ *(0.1 pts.)*

Por tanto:
$$\boxed{i_L(t) = i_C(t) = \frac{\mathcal{E}}{R}\cos(\omega t)} \qquad \left(\text{con }\omega = \frac{1}{\sqrt{LC}}\right) \qquad \text{(0.1 pts.)}$$

El voltaje sobre el condensador se obtiene integrando $i_C = C\dfrac{dv_C}{dt}$ desde $t = 0$ con $v_C(0) = 0$:
$$v_C(t) = \frac{1}{C}\int_0^t i_C(t')\,dt' = \frac{\mathcal{E}}{RC}\int_0^t \cos(\omega t')\,dt' = \frac{\mathcal{E}}{RC\omega}\sin(\omega t) = \frac{\mathcal{E}}{R}\frac{\sqrt{LC}}{C}\sin(\omega t)$$
$$\boxed{v_C(t) = \frac{\mathcal{E}}{R}\sqrt{\frac{L}{C}}\sin(\omega t)} \qquad \text{(0.1 pts.)}$$

---

#### Etapa III — Parte d) Ausencia de régimen permanente cuando $t \to \infty$ (1.0 pto.)

##### Solución de d)

La energía en la inductancia no se almacena de manera permanente, sino temporalmente en su campo magnético, el cual existe únicamente mientras circula corriente eléctrica. Como consecuencia, la energía se transfiere periódicamente entre el campo magnético de la inductancia y el campo eléctrico del condensador, oscilando indefinidamente sin alcanzar un régimen estacionario. *(1.0 pts.)*

##### Solución alternativa de d)

En un circuito $LC$ ideal no existe ninguna resistencia que disipe energía, por tanto, la energía total permanece constante. Esto significa que el sistema oscila permanentemente y no alcanza un mínimo de estabilidad o estado estacionario. *(1.0 pts.)*

**Verificación (Problema 3):**
- **Conservación de energía en Etapa III:** En todo instante $t > 0$, la energía total es:
  $$E_{\text{tot}}(t) = \frac{1}{2}L\,i_L^2(t) + \frac{1}{2}C\,v_C^2(t) = \frac{1}{2}L\frac{\mathcal{E}^2}{R^2}\cos^2(\omega t) + \frac{1}{2}C\frac{\mathcal{E}^2}{R^2}\frac{L}{C}\sin^2(\omega t) = \frac{1}{2}L\left(\frac{\mathcal{E}}{R}\right)^2 = \text{cte.}$$
- **Unidades de $v_C(t)$:** La impedancia característica $\sqrt{L/C}$ tiene unidades de $\sqrt{\text{H}/\text{F}} = \Omega$, por lo que $\frac{\mathcal{E}}{R}\sqrt{\frac{L}{C}}$ tiene unidades de $(\text{V}/\Omega)\cdot\Omega = \text{V}$, consistente.

---

## Resumen de resultados

| Problema | Parte | Magnitud / Caso | Resultado |
| :--- | :--- | :--- | :--- |
| **Problema 1A** | a) | Fuerza en el centro ($Q_i$ iguales) | $\vec{F} = 0$ |
| | b) | Trabajo ($q = 1\,\mu\text{C}$, $Q_i = \sqrt{3}\,\mu\text{C}$) | $W \approx 360\,\text{J}$ |
| | c) | Campo eléctrico en el centro ($Q_8 = 0$) | $\vec{E} = \dfrac{4KQ}{3a^2\sqrt{3}}(-\hat{\imath}+\hat{\jmath}+\hat{k}) = 75\times 10^9(-\hat{\imath}+\hat{\jmath}+\hat{k})\,\text{N/C}$ |
| | d) i | Flujo en $S_1, S_2$ (sin / con $q_0$) | $\Phi = \dfrac{8Q}{\varepsilon_0}$ $\;\Big/\;$ $\Phi = \dfrac{8Q + q_0}{\varepsilon_0}$ |
| | d) i | Flujo en $S_3$ (sin / con $q_0$) | $\Phi = \dfrac{4Q}{\varepsilon_0}$ $\;\Big/\;$ $\Phi = \dfrac{4Q}{\varepsilon_0}$ o $\dfrac{4Q + q_0}{\varepsilon_0}$ |
| | d) ii | $\Phi_E = 0$ con $\vec{E} \neq 0$ | Sí es posible si $Q_{\text{enc}} = 0$ (flujo entrante = flujo saliente) |
| **Problema 1B** | a) | Corrientes estacionarias | $I_{\text{bat}} = I_6 = \dfrac{5\mathcal{E}}{11R}$, $\;I_1 = I_2 = \dfrac{3\mathcal{E}}{11R}$, $\;I_3 = I_4 = \dfrac{2\mathcal{E}}{11R}$, $\;I_5 = 0$ |
| | b) | Voltaje del capacitor cargado | $\Delta V_{cb} = \dfrac{\mathcal{E}}{11}$ |
| | c) | Energía almacenada (vacío / dieléctrico $\kappa$) | $U = \dfrac{C\mathcal{E}^2}{242}$; con dieléctrico $U' = \kappa U$ (aumenta) |
| | d) | Descarga del capacitor ($t > 0$) | $q(t) = q_i\,e^{-5t/(16RC)}$, $\;\Delta V_C(t) = \dfrac{q_i}{C}\,e^{-5t/(16RC)}$ |
| **Problema 2** | a) I | Antes de entrar en $\vec{B}$ | $\varepsilon = 0$, $\;I = 0$ |
| | a) II | Parcialmente inmersa en $\vec{B}$ | $\varepsilon = -Bav$, $\;I = \dfrac{Bav}{R}$, sentido antihorario |
| | a) III | Completamente inmersa en $\vec{B}$ | $\varepsilon = 0$, $\;I = 0$ |
| | b) | Sentido de la fuerza externa al ingresar | Hacia la derecha (en el sentido de $\vec{v}$) |
| **Problema 3** | a) | Voltaje en $L$ justo al cerrar $S_1$ ($t = 0^+$) | $v_L(0^+) = \mathcal{E}$ |
| | b) | Corriente en $L$ en régimen permanente | $i_L = \dfrac{\mathcal{E}}{R}$ |
| | c) | Corriente y voltaje en $C$ en Etapa III ($\omega = 1/\sqrt{LC}$) | $i_C(t) = \dfrac{\mathcal{E}}{R}\cos(\omega t)$, $\;v_C(t) = \dfrac{\mathcal{E}}{R}\sqrt{\dfrac{L}{C}}\sin(\omega t)$ |
| | d) | Por qué no alcanza régimen permanente | Circuito $LC$ ideal sin disipación; la energía oscila indefinidamente entre $L$ y $C$ |
