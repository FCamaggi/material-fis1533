# Ayudantía 23 — Autoinductancia y energía magnética

> Clases relacionadas: [Clase 11 - Ley de Biot Savart](../../Clases/markdown/Clase%2011%20-%20Ley%20de%20Biot%20Savart.md), [Clase 12 - Ley de Ampere](../../Clases/markdown/Clase%2012%20-%20Ley%20de%20Ampere.md), [Clase 13 - Inducción Magnética](../../Clases/markdown/Clase%2013%20-%20Inducci%C3%B3n%20Magn%C3%A9tica.md), [Clase 14 - Inductancia](../../Clases/markdown/Clase%2014%20-%20Inductancia.md)

---

## Problema 1

Considere dos espiras de radios $a$ y $b$ ($a \gg b$) dispuestas de forma que sus centros se ubican en el eje $z$ separadas por una distancia $d$, como se muestra en la figura. Encuentre el coeficiente de inducción mutua del sistema.

> **[Figura]:** Dos espiras circulares coaxiales paralelas horizontales con centros sobre el eje vertical $z$. La espira inferior tiene radio grande $a$ y está centrada en el origen $z = 0$. La espira superior tiene radio pequeño $b$ ($b \ll a$) y está situada a una altura $z = d$.

### Solución

**Idea:** El coeficiente de inducción mutua $M$ entre dos circuitos cerrados relaciona el flujo magnético que atraviesa uno de ellos debido a una corriente que circula por el otro ($M = \Phi_{1 \to 2} / I_1$). Debido a que $a \gg b$, el campo magnético generado por la espira grande en la región que ocupa la espira pequeña es prácticamente homogéneo e igual a su valor en el eje axial a la distancia $d$.

#### 1. Campo magnético en el eje producido por la espira grande

Hacemos circular una corriente ficticia $I_1$ por la espira inferior de radio $a$ en sentido antihorario respecto al eje $z$.

Por la ley de Biot-Savart:
$$\vec{B}(\vec{r}) = \frac{\mu_0 I_1}{4\pi} \oint \frac{d\vec{l}' \times (\vec{r} - \vec{r}')}{|\vec{r} - \vec{r}'|^3}$$

En coordenadas cilíndricas:
- Posición de un elemento de la espira 1: $\vec{r}' = a\,\hat{r}'$.
- Elemento de longitud: $d\vec{l}' = a\, d\theta'\,\hat{\theta}'$.
- Posición en el eje sobre la espira 2: $\vec{r} = d\,\hat{z}$.
- Vector distancia relativa: $\vec{r} - \vec{r}' = d\,\hat{z} - a\,\hat{r}'$.
- Distancia: $|\vec{r} - \vec{r}'| = \sqrt{a^2 + d^2}$.

Calculamos el producto vectorial:
$$d\vec{l}' \times (\vec{r} - \vec{r}') = a\, d\theta'\,\hat{\theta}' \times (d\,\hat{z} - a\,\hat{r}')$$
Usando las identidades de productos cruz en cilíndricas ($\hat{\theta}' \times \hat{z} = \hat{r}'$ y $\hat{\theta}' \times \hat{r}' = -\hat{z}$):
$$d\vec{l}' \times (\vec{r} - \vec{r}') = a d\, d\theta'\,\hat{r}' + a^2\, d\theta'\,\hat{z}$$

Integrando a lo largo de la circunferencia ($\theta' \in [0, 2\pi]$):
$$\vec{B}(d\,\hat{z}) = \frac{\mu_0 I_1}{4\pi (a^2 + d^2)^{3/2}} \left[ ad \int_0^{2\pi} \hat{r}'\, d\theta' + a^2 \int_0^{2\pi} d\theta'\,\hat{z} \right]$$

Dado que el vector unitario radial satisface $\int_0^{2\pi} \hat{r}'\, d\theta' = \int_0^{2\pi} (\cos\theta'\,\hat{i} + \sin\theta'\,\hat{j})\, d\theta' = \vec{0}$, la componente radial neta se cancela por simetría azimutal. La integral en $\hat{z}$ entrega:
$$\int_0^{2\pi} a^2\, d\theta'\,\hat{z} = 2\pi a^2\,\hat{z}$$

Por lo tanto, el campo magnético en el eje a la altura $z = d$ es:
$$\vec{B}_1(d) = \frac{\mu_0 I_1 a^2}{2(a^2 + d^2)^{3/2}}\,\hat{z}$$

#### 2. Flujo magnético a través de la espira pequeña

Dado que el radio de la segunda espira es mucho menor que el de la primera ($b \ll a$), podemos considerar que en toda el área plana $S_2 = \pi b^2$ encerrada por la espira pequeña el campo magnético $\vec{B}_1$ es uniforme y aproximadamente igual al valor axial en $z = d$.

Tomando el vector normal unitario $\hat{n} = \hat{z}$:
$$\Phi_{1 \to 2} = \iint_{S_2} \vec{B}_1 \cdot d\vec{S} \approx \|\vec{B}_1(d)\| \cdot S_2 = \left(\frac{\mu_0 I_1 a^2}{2(a^2 + d^2)^{3/2}}\right) (\pi b^2)$$

$$\Phi_{1 \to 2} = \frac{\mu_0 \pi a^2 b^2 I_1}{2(a^2 + d^2)^{3/2}}$$

#### 3. Coeficiente de inductancia mutua

Por definición de inductancia mutua:
$$M = \frac{\Phi_{1 \to 2}}{I_1}$$

$$\boxed{M = \frac{\mu_0 \pi a^2 b^2}{2(a^2 + d^2)^{3/2}}}$$

**Verificación:**
- **Unidades:** $[\mu_0] = \text{H/m} = \text{T}\cdot\text{m/A}$. Por lo tanto, $[M] = (\text{H/m}) \cdot \text{m}^4 / \text{m}^3 = \text{H}$ (Henry), dimensionalmente correcto.
- **Simetría y reciprocidad:** Por el teorema de reciprocidad de Neumann, la inductancia mutua no depende de cuál espira transporta la corriente ($M_{12} = M_{21} = M$), lo cual se refleja en la simetría bilineal del producto $a^2 b^2$ en el numerador.
- **Límites:** Cuando $d \to \infty$, la interacción magnética se desvanece ($M \to 0$). Para espiras en el mismo plano ($d = 0$), $M = \frac{\mu_0 \pi b^2}{2a}$.

---

## Problema 2

Un cable coaxial está formado por dos superficies cilíndricas infinitamente largas, por las cuales circula la misma corriente en sentidos contrarios. Si las densidades superficiales de corriente que circulan por las superficies de radios $a$ y $b$ son, respectivamente:
$$\vec{K}_a = \frac{I}{2\pi a}\,\hat{z}, \qquad \vec{K}_b = -\frac{I}{2\pi b}\,\hat{z} \qquad (a < b)$$

1. Determine la energía por unidad de largo.  
2. Determine la autoinducción por unidad de largo del cable coaxial.

> **[Figura]:** Dos cilindros concéntricos coaxiales de longitud infinita alineados con el eje vertical $z$. La superficie cilíndrica interior tiene radio $a$ y transporta una densidad superficial de corriente $\vec{K}_a$ orientada hacia arriba ($+\hat{z}$). La superficie cilíndrica exterior tiene radio $b$ ($b > a$) y transporta una densidad superficial $\vec{K}_b$ orientada hacia abajo ($-\hat{z}$).

### Solución

**Idea:** La corriente total que viaja por la pared interna es $I$ en $+\hat{z}$, y por la externa es $-I$ en $-\hat{z}$. Aplicando la ley de Ampère por simetría cilíndrica, el campo magnético está confinado únicamente a la región intermedia $a < r < b$. Integrando la densidad de energía magnética $u_B = \frac{B^2}{2\mu_0}$ sobre el volumen entre cilindros obtenemos la energía por unidad de largo, y a partir de $U = \frac{1}{2} L I^2$ deducimos la autoinductancia por unidad de largo.

#### 1. Campo magnético en todo el espacio (Ley de Ampère)

Por la simetría cilíndrica del conductor coaxial, las líneas de campo magnético son circunferencias concéntricas centradas en el eje $z$:
$$\vec{B}(\vec{r}) = B(r)\,\hat{\theta}$$

Tomamos un lazo amperiano circular de radio $r$ concéntrico con el eje $z$. Por la ley de Ampère:
$$\oint \vec{B} \cdot d\vec{l} = B(r) (2\pi r) = \mu_0 I_{\text{enc}}$$

Analizamos las tres regiones del espacio:
- **Región interior ($r < a$):** No hay corriente encerrada:
  $$I_{\text{enc}} = 0 \implies \vec{B} = \vec{0}$$

- **Región intermedia ($a < r < b$):** La corriente encerrada es la corriente total del cilindro interior:
  $$I_{\text{enc}} = \int_0^{2\pi} \vec{K}_a \cdot (\hat{z}\, a\, d\theta) = \int_0^{2\pi} \left(\frac{I}{2\pi a}\right) a\, d\theta = I$$
  Por lo tanto:
  $$B(r) (2\pi r) = \mu_0 I \implies \vec{B}(r) = \frac{\mu_0 I}{2\pi r}\,\hat{\theta} \qquad (a < r < b)$$

- **Región exterior ($r > b$):** La corriente encerrada incluye ambas superficies cilíndricas:
  $$I_{\text{enc}} = I + \int_0^{2\pi} \vec{K}_b \cdot (\hat{z}\, b\, d\theta) = I + \left(-\frac{I}{2\pi b}\right) (2\pi b) = I - I = 0$$
  $$\vec{B} = \vec{0} \qquad (r > b)$$

---

#### Parte 1) Energía magnética por unidad de largo

La densidad volumétrica de energía magnética en el espacio es:
$$u_B(r) = \frac{B^2}{2\mu_0}$$

Para la región intermedia ($a < r < b$):
$$u_B(r) = \frac{1}{2\mu_0} \left(\frac{\mu_0 I}{2\pi r}\right)^2 = \frac{\mu_0^2 I^2}{8\pi^2 r^2 \mu_0} = \frac{\mu_0 I^2}{8\pi^2 r^2}$$

Consideramos un tramo de cable coaxial de longitud $l$. El elemento de volumen en coordenadas cilíndricas es $dV = r\, dr\, d\theta\, dz = 2\pi r l\, dr$.

La energía magnética total almacenada en el tramo de longitud $l$ es:
$$U = \int_V u_B\, dV = \int_0^l dz \int_0^{2\pi} d\theta \int_a^b dr\, r \left(\frac{\mu_0 I^2}{8\pi^2 r^2}\right)$$
$$U = 2\pi l \left(\frac{\mu_0 I^2}{8\pi^2}\right) \int_a^b \frac{dr}{r} = \frac{\mu_0 I^2 l}{4\pi} [\ln(r)]_a^b = \frac{\mu_0 I^2 l}{4\pi} \ln\left(\frac{b}{a}\right)$$

Dividiendo por la longitud $l$, la energía por unidad de largo es:
$$\boxed{\frac{U}{l} = \frac{\mu_0 I^2}{4\pi} \ln\left(\frac{b}{a}\right)}$$

---

#### Parte 2) Autoinducción por unidad de largo

Podemos calcular la autoinductancia $\mathcal{L}$ de dos maneras independientes:

**Método 1 (a partir de la energía magnética almacenada):**  
La energía almacenada en un inductor por el que circula una corriente $I$ es:
$$U = \frac{1}{2} \mathcal{L} I^2 \implies \mathcal{L} = \frac{2U}{I^2}$$

Sustituyendo la energía total del tramo de largo $l$:
$$\mathcal{L} = \frac{2}{I^2} \left[\frac{\mu_0 I^2 l}{4\pi} \ln\left(\frac{b}{a}\right)\right] = \frac{\mu_0 l}{2\pi} \ln\left(\frac{b}{a}\right)$$

Dividiendo por la longitud $l$:
$$\frac{\mathcal{L}}{l} = \frac{\mu_0}{2\pi} \ln\left(\frac{b}{a}\right)$$

> **Nota:** En la solución manuscrita oficial (página 4), al despejar la autoinductancia a partir de $\mathcal{L} = \frac{2U}{I^2}$, el ayudante escribió $\frac{\mu_0}{2} \ln(b/a)$ omitiendo por descuido el factor $\pi$ en el denominador. Lo correcto es $\frac{\mu_0}{2\pi} \ln(b/a)$, dado que $2 \cdot \frac{\mu_0}{4\pi} = \frac{\mu_0}{2\pi}$.

**Método 2 (a partir del flujo magnético):**  
Consideramos una superficie rectangular plana en la dirección radial comprendida entre $r = a$ y $r = b$, con longitud axial $l$. El flujo que atraviesa dicha superficie es:
$$\Phi = \int_0^l dz \int_a^b B(r)\, dr = l \int_a^b \frac{\mu_0 I}{2\pi r}\, dr = \frac{\mu_0 I l}{2\pi} \ln\left(\frac{b}{a}\right)$$
Por definición de autoinductancia:
$$\mathcal{L} = \frac{\Phi}{I} = \frac{\mu_0 l}{2\pi} \ln\left(\frac{b}{a}\right) \implies \frac{\mathcal{L}}{l} = \frac{\mu_0}{2\pi} \ln\left(\frac{b}{a}\right)$$
Ambos métodos coinciden con total exactitud.

$$\boxed{\frac{\mathcal{L}}{l} = \frac{\mu_0}{2\pi} \ln\left(\frac{b}{a}\right)}$$

**Verificación:**
- **Unidades:** $[\mu_0] = \text{H/m}$, luego $[\mathcal{L}/l] = \text{H/m}$, dimensionalmente consistente.
- **Límites:** Si $b \to a$, el espacio entre conductores desaparece y la autoinductancia se anula ($\ln(1) = 0$), tal como debe ser.

---

## Problema 3

Un cilindro de radio $R$ y largo $H \gg R$, posee una densidad de carga $\sigma_0$ con su eje coincidente con el eje $z$. En $t = 0$ el cilindro comienza a rotar lentamente con velocidad angular $\vec{\omega}(t) = \alpha t\,\hat{z}$, donde $\alpha$ es una constante.

Determine la energía eléctrica y magnética dentro del cilindro.

> **[Figura]:** Cilindro largo de radio $R$ y longitud $H \gg R$ orientado horizontalmente a lo largo del eje longitudinal $z$. La superficie del cilindro tiene una densidad superficial uniforme de carga $\sigma_0$. Una flecha curva indica la rotación en torno al eje $z$ con velocidad angular $\vec{\omega}(t) = \alpha t\,\hat{z}$.

### Solución

**Idea:** La rotación de la carga superficial $\sigma_0$ genera una densidad de corriente superficial azimutal $\vec{K}(t) = \sigma_0 \vec{v}$, comportándose electromagnéticamente como un solenoide ideal. Aplicando la ley de Ampère calculamos el campo magnético uniforme interno $\vec{B}(t)$, y a partir de este, su energía magnética. Debido a que la corriente se acelera linealmente en el tiempo, el campo magnético variable induce por ley de Faraday un campo eléctrico azimutal $\vec{E}_{\text{ind}}(r, t)$. Como la distribución electrostática hueca tiene campo electrostático interno nulo ($\vec{E}_{\text{stat}} = \vec{0}$), la energía eléctrica en el interior proviene íntegramente del campo eléctrico inducido.

#### 1. Densidad de corriente superficial inducida por la rotación

La velocidad lineal de un punto sobre la superficie exterior del cilindro ($r = R$) en rotación con velocidad angular $\vec{\omega}(t) = \alpha t\,\hat{z}$ es:
$$\vec{v} = \vec{\omega} \times \vec{r} = (\alpha t\,\hat{z}) \times (R\,\hat{r}) = \alpha R t\,\hat{\theta}$$

La densidad superficial de corriente en la cáscara cilíndrica es:
$$\vec{K}(t) = \sigma_0 \vec{v} = \sigma_0 \alpha R t\,\hat{\theta}$$

Esta corriente azimutal fluye sobre la superficie del cilindro de forma completamente análoga a las espiras de un solenoide de longitud $H \gg R$.

#### 2. Campo magnético y energía magnética en el interior

1. **Campo magnético (Ley de Ampère):**  
   Por la aproximación de cilindro muy largo ($H \gg R$), despreciamos los efectos de borde. El campo magnético fuera del cilindro es nulo ($\vec{B}_{\text{ext}} = \vec{0}$) y en el interior es puramente axial y uniforme:
   $$\vec{B}_{\text{int}} = B(t)\,\hat{z}$$

   Elegimos un lazo amperiano rectangular de lados $l$ y anchura radial arbitraria, con un lado dentro del cilindro ($r < R$) y el opuesto en el exterior ($r > R$):
   $$\oint \vec{B} \cdot d\vec{l} = B(t) l + 0 + 0 + 0 = B(t) l$$
   La corriente que atraviesa el lazo es la corriente superficial en la longitud $l$:
   $$I_{\text{enc}} = K(t) l = \sigma_0 \alpha R t\, l$$

   Por la ley de Ampère:
   $$B(t) l = \mu_0 I_{\text{enc}} = \mu_0 (\sigma_0 \alpha R t\, l) \implies B(t) = \mu_0 \sigma_0 \alpha R t$$

   Por lo tanto:
   $$\vec{B}(t) = \mu_0 \sigma_0 \alpha R t\,\hat{z} \qquad (r < R)$$

2. **Energía magnética dentro del cilindro:**  
   La densidad de energía magnética en el interior es:
   $$u_B(t) = \frac{B^2(t)}{2\mu_0} = \frac{(\mu_0 \sigma_0 \alpha R t)^2}{2\mu_0} = \frac{1}{2} \mu_0 \sigma_0^2 \alpha^2 R^2 t^2$$

   Como el campo es espacialmente uniforme dentro del cilindro, la integral sobre el volumen interior $V = \pi R^2 H$ es directamente el producto de la densidad por el volumen:
   $$U_m = \iiint_{V} u_B\, dV = u_B \cdot (\pi R^2 H) = \left(\frac{1}{2} \mu_0 \sigma_0^2 \alpha^2 R^2 t^2\right) (\pi R^2 H)$$

   $$U_m = \frac{1}{2} \mu_0 \sigma_0^2 \alpha^2 \pi R^4 H t^2$$

   > **Nota:** En la solución manuscrita oficial (página 6), al simplificar la densidad de energía magnética $u_B = \frac{B^2}{2\mu_0} = \frac{\mu_0^2 \sigma_0^2 \alpha^2 R^2 t^2}{2\mu_0} = \frac{\mu_0 \sigma_0^2 \alpha^2 R^2 t^2}{2}$, el factor $\mu_0$ del numerador se omitió involuntariamente al escribir la integral de volumen, resultando erróneamente en $U = \frac{\sigma_0^2 \alpha^2 R^4 t^2 \pi H}{2}$. Lo correcto es $U_m = \frac{1}{2} \mu_0 \sigma_0^2 \alpha^2 \pi R^4 H t^2$, lo cual preserva la consistencia dimensional (energía en Joules).

---

#### 3. Campo eléctrico inducido y energía eléctrica en el interior

1. **Campo electrostático interno:**  
   Por la ley de Gauss para electrostática, una cáscara cilíndrica de carga superficial uniforme sin carga interior no genera campo eléctrico en su interior:
   $$\vec{E}_{\text{stat}} = \vec{0} \qquad (r < R)$$

2. **Campo eléctrico inducido (Ley de Faraday):**  
   Dado que el campo magnético interno varía en el tiempo ($\partial\vec{B}/\partial t \neq \vec{0}$), se induce un campo eléctrico no conservativo. Tomamos una espira circular centrada en el eje $z$ de radio $r < R$:
   $$\oint \vec{E} \cdot d\vec{l} = -\frac{d\Phi_B}{dt}$$

   Por simetría azimutal, $\vec{E} = E(r)\,\hat{\theta}$, de modo que:
   $$\oint \vec{E} \cdot d\vec{l} = E(r) (2\pi r)$$

   El flujo magnético a través de la espira de radio $r$ es:
   $$\Phi_B(r, t) = \iint B(t)\, dA = B(t) (\pi r^2) = (\mu_0 \sigma_0 \alpha R t) (\pi r^2)$$

   Derivando respecto al tiempo:
   $$\frac{d\Phi_B}{dt} = \mu_0 \sigma_0 \alpha R \pi r^2$$

   Igualando según la ley de Faraday:
   $$E(r) (2\pi r) = -\mu_0 \sigma_0 \alpha R \pi r^2 \implies E(r) = -\frac{\mu_0 \sigma_0 \alpha R r}{2}$$

   Vectorialmente:
   $$\vec{E}(r) = -\frac{\mu_0 \sigma_0 \alpha R r}{2}\,\hat{\theta} \qquad (r < R)$$

3. **Energía eléctrica dentro del cilindro:**  
   La densidad de energía eléctrica está dada por:
   $$u_E(r) = \frac{1}{2} \varepsilon_0 \|\vec{E}(r)\|^2 = \frac{1}{2} \varepsilon_0 \left(\frac{\mu_0 \sigma_0 \alpha R r}{2}\right)^2 = \frac{\varepsilon_0 \mu_0^2 \sigma_0^2 \alpha^2 R^2 r^2}{8}$$

   Integrando sobre todo el volumen cilíndrico interior ($r \in [0, R]$, $\theta \in [0, 2\pi]$, $z \in [0, H]$):
   $$U_E = \int_0^H dz \int_0^{2\pi} d\theta \int_0^R dr\, r \cdot u_E(r)$$
   $$U_E = (H)(2\pi) \left(\frac{\varepsilon_0 \mu_0^2 \sigma_0^2 \alpha^2 R^2}{8}\right) \int_0^R r^3\, dr$$

   Calculando la integral radial:
   $$\int_0^R r^3\, dr = \frac{R^4}{4}$$

   Por lo tanto:
   $$U_E = 2\pi H \left(\frac{\varepsilon_0 \mu_0^2 \sigma_0^2 \alpha^2 R^2}{8}\right) \left(\frac{R^4}{4}\right) = \frac{\pi \varepsilon_0 \mu_0^2 \sigma_0^2 \alpha^2 H R^6}{16}$$

$$\boxed{U_m = \frac{1}{2} \mu_0 \sigma_0^2 \alpha^2 \pi R^4 H t^2}$$

$$\boxed{U_E = \frac{\pi \varepsilon_0 \mu_0^2 \sigma_0^2 \alpha^2 H R^6}{16}}$$

**Verificación:**
- **Cociente entre energías:**  
  Recordando que $c^2 = \frac{1}{\varepsilon_0 \mu_0}$, reescribimos la energía eléctrica como:
  $$U_E = \frac{\pi \mu_0 \sigma_0^2 \alpha^2 H R^6}{16 c^2}$$
  Comparando con la energía magnética en un instante $t$:
  $$\frac{U_E}{U_m} = \frac{\frac{\pi \mu_0 \sigma_0^2 \alpha^2 H R^6}{16 c^2}}{\frac{1}{2} \mu_0 \sigma_0^2 \alpha^2 \pi R^4 H t^2} = \frac{1}{8} \frac{R^2}{c^2 t^2} = \frac{1}{8} \left(\frac{v(R, t)}{c}\right)^2$$
  donde $v(R, t) = \alpha t R$ es la velocidad periférica del cilindro. Como la rotación es lenta ($v \ll c$), se cumple $U_E \ll U_m$, lo cual demuestra de forma impecable que el campo eléctrico inducido y su energía asociada representan la corrección relativista de orden $(v/c)^2$ predicha por la electrodinámica clásica.

---

## Resumen de resultados

| Problema | Magnitud requerida | Resultado analítico |
| :--- | :--- | :--- |
| **P1** | Inductancia mutua $M$ | $M = \dfrac{\mu_0 \pi a^2 b^2}{2(a^2 + d^2)^{3/2}}$ |
| **P2 (1)** | Energía magnética por unidad de largo $U/l$ | $\dfrac{U}{l} = \dfrac{\mu_0 I^2}{4\pi} \ln\left(\dfrac{b}{a}\right)$ |
| **P2 (2)** | Autoinductancia por unidad de largo $\mathcal{L}/l$ | $\dfrac{\mathcal{L}}{l} = \dfrac{\mu_0}{2\pi} \ln\left(\dfrac{b}{a}\right)$ |
| **P3** | Densidad superficial de corriente $\vec{K}(t)$ | $\vec{K}(t) = \sigma_0 \alpha R t\,\hat{\theta}$ |
| **P3** | Campo magnético interno $\vec{B}(t)$ | $\vec{B}(t) = \mu_0 \sigma_0 \alpha R t\,\hat{z}$ |
| **P3** | Energía magnética interna $U_m(t)$ | $U_m = \dfrac{1}{2} \mu_0 \sigma_0^2 \alpha^2 \pi R^4 H t^2$ |
| **P3** | Campo eléctrico inducido $\vec{E}(r)$ | $\vec{E}(r) = -\dfrac{\mu_0 \sigma_0 \alpha R r}{2}\,\hat{\theta}$ |
| **P3** | Energía eléctrica interna $U_E$ | $U_E = \dfrac{\pi \varepsilon_0 \mu_0^2 \sigma_0^2 \alpha^2 H R^6}{16}$ |
