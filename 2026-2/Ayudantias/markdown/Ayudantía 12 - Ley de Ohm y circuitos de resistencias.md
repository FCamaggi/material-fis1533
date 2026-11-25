# Ayudantía 12 — Ley de Ohm y circuitos de resistencias

> Clases relacionadas: [Clase 08 - Corriente electrica y resistencias](../../Clases/markdown/Clase%2008%20-%20Corriente%20electrica%20y%20resistencias.md), [Clase 09 - Potencia, circuitos de resistencias y circuito RC](../../Clases/markdown/Clase%2009%20-%20Potencia%2C%20circuitos%20de%20resistencias%20y%20circuito%20RC.md)

---

## Problema 1

Se tienen dos cascarones esféricos concéntricos conductores de radios $a$ y $b$ ($a < b$). Estos cascarones se mantienen cada uno a potenciales constantes. El espacio entre los cascarones se llena con un material Óhmico de conductividad $\sigma$, como se muestra en la figura. Suponiendo que entre los cascarones esféricos circula una corriente constante $I$, calcule:

a) La densidad de corriente eléctrica $J(r)$.  
b) El campo eléctrico en la región entre los cascarones.  
c) La diferencia de potencial en la región entre los cascarones.  
d) La resistencia entre los cascarones.

> **[Figura]:** Dos cascarones esféricos concéntricos en corte transversal. El cascarón interior tiene radio $a$ y el exterior tiene radio $b$ ($a < b$). La región anular comprendida entre ambos radios ($a \le r \le b$) se encuentra sombreada uniformemente, representando el material conductor óhmico de conductividad $\sigma$. La corriente $I$ fluye de manera estrictamente radial entre ambos cascarones.

### Solución

**Idea:** Debido a la simetría esférica del problema, la corriente constante $I$ se distribuye de manera isotrópica y puramente radial. La densidad de corriente $\vec{J}(r)$ se determina dividiendo la corriente total por el área esférica $4\pi r^2$. Mediante la forma microscópica de la ley de Ohm ($\vec{J} = \sigma \vec{E}$), se deduce el campo eléctrico $\vec{E}(r)$, cuya integral de línea proporciona la diferencia de potencial $\Delta V$ y la resistencia eléctrica del medio.

#### a) Densidad de corriente eléctrica $J(r)$

Consideremos una superficie esférica concéntrica de radio arbitrario $r$, tal que $a < r < b$. En régimen estacionario, la corriente total neta $I$ que atraviesa dicha superficie cerrada es constante y se orienta radialmente:
$$I = \iint_{S} \vec{J} \cdot d\vec{A} = \iint_{S} J(r)\,\hat{r} \cdot (r^2 \sin\theta\,d\theta\,d\phi\,\hat{r}) = J(r) \iint_{S} dA = J(r)(4\pi r^2)$$

Despejando la magnitud $J(r)$ y orientándola radialmente hacia afuera:
$$\vec{J}(r) = \frac{I}{4\pi r^2}\,\hat{r} \qquad (a < r < b)$$

$$\boxed{\vec{J}(r) = \frac{I}{4\pi r^2}\,\hat{r}}$$

---

#### b) Campo eléctrico en la región entre los cascarones

Un material óhmico obedece la ley de Ohm en su formulación microscópica:
$$\vec{J} = \sigma \vec{E}$$
donde $\sigma$ es la conductividad eléctrica del medio.

Despejando el campo eléctrico $\vec{E}$:
$$\vec{E} = \frac{\vec{J}}{\sigma} = \frac{1}{\sigma}\left(\frac{I}{4\pi r^2}\,\hat{r}\right) = \frac{I}{4\pi\sigma r^2}\,\hat{r}$$

$$\boxed{\vec{E}(r) = \frac{I}{4\pi\sigma r^2}\,\hat{r} \qquad (a < r < b)}$$

---

#### c) Diferencia de potencial en la región entre los cascarones

La diferencia de potencial eléctrico entre el cascarón exterior ($r = b$) y el cascarón interior ($r = a$) se calcula mediante la integral de línea del campo eléctrico a lo largo de una trayectoria radial ($d\vec{r} = dr\,\hat{r}$):
$$\Delta V = V(b) - V(a) = -\int_{a}^{b} \vec{E} \cdot d\vec{r} = -\int_{a}^{b} \frac{I}{4\pi\sigma r^2}\,dr$$

Extrayendo las constantes:
$$\Delta V = -\frac{I}{4\pi\sigma} \int_{a}^{b} \frac{dr}{r^2} = -\frac{I}{4\pi\sigma} \left[ -\frac{1}{r} \right]_{a}^{b} = \frac{I}{4\pi\sigma} \left( \frac{1}{b} - \frac{1}{a} \right) = -\frac{I}{4\pi\sigma}\left(\frac{1}{a} - \frac{1}{b}\right)$$

Reduciendo a común denominador:
$$\Delta V = V(b) - V(a) = -\frac{I(b - a)}{4\pi\sigma a b}$$

Si se define la caída de potencial en el sentido en que fluye la corriente ($V(a) - V(b)$):
$$V(a) - V(b) = \frac{I(b - a)}{4\pi\sigma a b}$$

$$\boxed{\Delta V = V(b) - V(a) = -\frac{I}{4\pi\sigma}\left(\frac{1}{a} - \frac{1}{b}\right) = -\frac{I(b - a)}{4\pi\sigma a b}}$$

---

#### d) Resistencia eléctrica entre los cascarones

La resistencia eléctrica $R$ del sistema se determina mediante la ley de Ohm macroscópica a partir de la magnitud de la diferencia de potencial:
$$R = \frac{|\Delta V|}{I} = \frac{\frac{I(b - a)}{4\pi\sigma a b}}{I} = \frac{b - a}{4\pi\sigma a b}$$

Alternativamente, dividiendo el espacio en cascarones esféricos diferenciales de radio $r$, espesor $dr$ y área transversal $A(r) = 4\pi r^2$, cada cascarón aporta una resistencia elemental $dR = \frac{dr}{\sigma A(r)} = \frac{dr}{4\pi\sigma r^2}$. Integrando en serie desde $r = a$ hasta $r = b$:
$$R = \int_{a}^{b} \frac{dr}{4\pi\sigma r^2} = \frac{1}{4\pi\sigma} \left( \frac{1}{a} - \frac{1}{b} \right) = \frac{b - a}{4\pi\sigma a b}$$

$$\boxed{R = \frac{b - a}{4\pi\sigma a b}}$$

**Verificación:**
- **Unidades:**
  $$[R] = \frac{[b - a]}{[\sigma][a][b]} = \frac{\text{m}}{(\Omega^{-1}\cdot\text{m}^{-1})\cdot \text{m}^2} = \frac{\text{m}}{\Omega^{-1}\cdot\text{m}} = \Omega$$
  La unidad resultante es el ohm ($\Omega$), dimensionalmente correcta.
- **Límites físicos:**
  - Si el espesor tiende a cero ($b \to a$), la resistencia se anula ($R \to 0$).
  - Si el radio exterior tiende a infinito ($b \to \infty$), se recupera la resistencia de contacto de una esfera aislada en un medio infinito: $R \to \frac{1}{4\pi\sigma a}$.

---

## Problema 2

Suponga que tiene una resistencia cilíndrica de largo $L$ y de radio $R$, dividida en dos regiones longitudinales con resistividad $\rho_1$ y $\rho_2$, como se muestra en la figura. Determine la resistencia vista entre los terminales A y B.

> **[Figura]:** Un cilindro macizo de longitud horizontal $L$ y sección transversal circular de radio $R$. Sus caras circulares planas corresponden a los contactos equipotenciales conectados a los terminales $A$ (izquierda) y $B$ (derecha). El cilindro está seccionado diametralmente a lo largo de su longitud en dos mitades semicilíndricas idénticas: la semicilíndrica superior posee resistividad uniforme $\rho_1$ y la semicilíndrica inferior posee resistividad uniforme $\rho_2$.

### Solución

**Idea:** Dado que las caras circulares extremas son superficies equipotenciales conductoras conectadas a los terminales $A$ y $B$, la diferencia de potencial aplicada $\Delta V = V_A - V_B$ es idéntica a lo largo de ambas mitades semicilíndricas. En consecuencia, ambas regiones funcionan como dos resistencias independientes conectadas en paralelo.

#### 1. Resistencia de cada sección longitudinal

Cada semicilindro tiene:
- Longitud: $L$.
- Área de la sección transversal semicircular:
  $$A_1 = A_2 = \frac{\pi R^2}{2}$$

La resistencia de un conductor cilíndrico de sección transversal uniforme $A$ y resistividad $\rho$ recorrida longitudinalmente por la corriente es $R = \frac{\rho L}{A}$. Por tanto:
- Para la mitad superior (resistividad $\rho_1$):
  $$R_1 = \frac{\rho_1 L}{A_1} = \frac{\rho_1 L}{\frac{\pi R^2}{2}} = \frac{2\rho_1 L}{\pi R^2}$$

- Para la mitad inferior (resistividad $\rho_2$):
  $$R_2 = \frac{\rho_2 L}{A_2} = \frac{\rho_2 L}{\frac{\pi R^2}{2}} = \frac{2\rho_2 L}{\pi R^2}$$

#### 2. Asociación en paralelo

Como ambas mitades comparten exactamente los mismos terminales equipotenciales $A$ y $B$, se encuentran asociadas en paralelo:
$$\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2}$$

Sustituyendo $R_1$ y $R_2$:
$$\frac{1}{R_{eq}} = \frac{\pi R^2}{2\rho_1 L} + \frac{\pi R^2}{2\rho_2 L} = \frac{\pi R^2}{2L}\left(\frac{1}{\rho_1} + \frac{1}{\rho_2}\right) = \frac{\pi R^2}{2L}\left(\frac{\rho_1 + \rho_2}{\rho_1 \rho_2}\right)$$

Invirtiendo la expresión:
$$R_{eq} = \frac{2L}{\pi R^2}\left(\frac{\rho_1 \rho_2}{\rho_1 + \rho_2}\right)$$

$$\boxed{R_{eq} = \frac{2L}{\pi R^2}\left(\frac{\rho_1 \rho_2}{\rho_1 + \rho_2}\right)}$$

**Verificación:**
- **Caso simétrico:** Si ambas mitades tienen la misma resistividad ($\rho_1 = \rho_2 = \rho$), el cilindro es homogéneo con área total $A_{\text{total}} = \pi R^2$. La fórmula arroja:
  $$R_{eq} = \frac{2L}{\pi R^2} \left(\frac{\rho^2}{2\rho}\right) = \frac{\rho L}{\pi R^2}$$
  que coincide de forma exacta con la fórmula clásica de un cilindro conductor completo.
- **Unidades:** $[\rho L / R^2] = (\Omega\cdot\text{m})\cdot\text{m}/\text{m}^2 = \Omega$, dimensionalmente consistente.

---

## Problema 3

Calcule la resistencia equivalente entre los terminales $a$ y $b$:

> **[Figura]:** Circuito eléctrico compuesto por seis resistencias entre dos terminales accesibles $a$ y $b$:
> - Desde el terminal de entrada $a$, un resistor de $9{,}0\,\Omega$ va en serie hasta un nodo central $c$.
> - Desde el nodo $c$, la corriente puede ramificarse:
>   - Hacia arriba: una rama contiene en serie un resistor de $3{,}0\,\Omega$ conectado a otro de $2{,}0\,\Omega$, llegando a un nodo intermedio $d$.
>   - En línea horizontal recta: un resistor de $6{,}0\,\Omega$ une directamente el nodo $c$ con el nodo $d$.
>   - Hacia la parte inferior: desde el nodo $c$, una rama oblicua contiene un resistor de $12{,}0\,\Omega$ y otra rama inferior contiene un resistor de $5{,}0\,\Omega$; ambas ramas van conectadas directamente al conductor inferior común que termina en $b$.
>   - Desde el nodo $d$, un resistor vertical de $7{,}0\,\Omega$ se conecta directamente al conductor inferior común que lleva a $b$.

### Solución

**Idea:** La red se resuelve mediante reducciones sucesivas de ramas en serie y paralelo, reconociendo adecuadamente los nodos equipotenciales del circuito:
1. Identificar la rama serie $3{,}0\,\Omega + 2{,}0\,\Omega$ conectada entre los nodos $c$ y $d$.
2. Asociar en paralelo dicha rama con la resistencia de $6{,}0\,\Omega$ entre $c$ y $d$.
3. Asociar en serie la resistencia equivalente resultante $R_{cd}$ con el resistor de $7{,}0\,\Omega$ hacia el nodo $b$.
4. Asociar en paralelo los dos resistores de $12{,}0\,\Omega$ y $5{,}0\,\Omega$ conectados directamente entre los nodos $c$ y $b$.
5. Combinar en paralelo las dos macro-ramas que unen $c$ con $b$.
6. Sumar en serie la resistencia de entrada de $9{,}0\,\Omega$ para obtener la resistencia equivalente total $R_{ab}$.

#### 1. Rama superior entre los nodos $c$ y $d$

Los resistores de $3{,}0\,\Omega$ y $2{,}0\,\Omega$ están recorridos por la misma corriente en serie:
$$R_{\text{serie 1}} = 3{,}0\,\Omega + 2{,}0\,\Omega = 5{,}0\,\Omega$$

Esta combinación está en paralelo con el resistor de $6{,}0\,\Omega$ conectado directamente entre los mismos nodos $c$ y $d$:
$$R_{cd} = \frac{R_{\text{serie 1}} \times 6{,}0\,\Omega}{R_{\text{serie 1}} + 6{,}0\,\Omega} = \frac{5{,}0 \times 6{,}0}{5{,}0 + 6{,}0} = \frac{30}{11}\,\Omega \approx 2{,}727\,\Omega$$

#### 2. Rama completa a través del nodo $d$ hacia el terminal $b$

Desde el nodo $d$ hacia el terminal inferior $b$, la corriente atraviesa el resistor de $7{,}0\,\Omega$. Al estar en serie con la sección previa $R_{cd}$:
$$R_{cdb} = R_{cd} + 7{,}0\,\Omega = \frac{30}{11}\,\Omega + 7\,\Omega = \frac{30 + 77}{11}\,\Omega = \frac{107}{11}\,\Omega \approx 9{,}727\,\Omega$$

#### 3. Rama inferior entre los nodos $c$ y $b$

Los resistores de $12{,}0\,\Omega$ y $5{,}0\,\Omega$ están ambos conectados en paralelo directamente entre el nodo $c$ y el conductor equipotencial del terminal $b$:
$$R_{12 \parallel 5} = \frac{12{,}0 \times 5{,}0}{12{,}0 + 5{,}0} = \frac{60}{17}\,\Omega \approx 3{,}529\,\Omega$$

#### 4. Resistencia equivalente entre los nodos $c$ y $b$

Entre el nodo $c$ y el terminal $b$ concurren en paralelo dos caminos independientes:
- La rama superior a través de $d$: $R_{cdb} = \frac{107}{11}\,\Omega$.
- La rama inferior directa: $R_{12 \parallel 5} = \frac{60}{17}\,\Omega$.

La conductancia equivalente entre $c$ y $b$ es la suma de conductancias:
$$\frac{1}{R_{cb}} = \frac{1}{R_{cdb}} + \frac{1}{R_{12 \parallel 5}} = \frac{11}{107} + \frac{17}{60} = \frac{11 \times 60 + 17 \times 107}{107 \times 60} = \frac{660 + 1819}{6420} = \frac{2479}{6420}\,\Omega^{-1}$$

Invirtiendo:
$$R_{cb} = \frac{6420}{2479}\,\Omega \approx 2{,}5898\,\Omega \approx 2{,}59\,\Omega$$

> **Nota:** En la pauta manuscrita oficial se escribió en este paso la igualdad $\frac{1}{R_{eq}} = \frac{11}{107} + \frac{17}{60} \approx 2{,}59\,\Omega$. Se trata de una omisión notacional menor en el miembro izquierdo, pues $2{,}59\,\Omega$ es el valor de $R_{cb} = \left(\frac{11}{107} + \frac{17}{60}\right)^{-1}$, valor que el ayudante utiliza de manera físicamente correcta en la suma final.

#### 5. Resistencia equivalente total entre $a$ y $b$

Finalmente, el resistor de entrada de $9{,}0\,\Omega$ está en serie con toda la subred entre $c$ y $b$:
$$R_{ab} = 9{,}0\,\Omega + R_{cb} = 9{,}0\,\Omega + \frac{6420}{2479}\,\Omega = \frac{22311 + 6420}{2479}\,\Omega = \frac{28731}{2479}\,\Omega \approx 11{,}5898\,\Omega \approx 11{,}59\,\Omega$$

$$\boxed{R_{ab} = \frac{28731}{2479}\,\Omega \approx 11{,}59\,\Omega}$$

**Verificación:**
- **Inspección de cotas:** La subred en paralelo entre $c$ y $b$ combina una rama de $\sim 9{,}73\,\Omega$ con una de $\sim 3{,}53\,\Omega$. La resistencia equivalente en paralelo siempre debe ser estrictamente menor que la más pequeña de las dos ramas ($R_{cb} < 3{,}53\,\Omega$). En efecto, $R_{cb} \approx 2{,}59\,\Omega < 3{,}53\,\Omega$.
- Al sumarle $9{,}0\,\Omega$ en serie, el resultado total debe ser superior a $9{,}0\,\Omega$ y menor a $9{,}0 + 3{,}53 = 12{,}53\,\Omega$, lo cual se cumple perfectamente con $11{,}59\,\Omega$.

---

## Resumen de resultados

| Problema | Inciso / Magnitud | Resultado final |
| :--- | :--- | :--- |
| **Problema 1** | **a)** Densidad de corriente $\vec{J}(r)$ | $\vec{J}(r) = \dfrac{I}{4\pi r^2}\,\hat{r} \quad (a < r < b)$ |
| | **b)** Campo eléctrico $\vec{E}(r)$ | $\vec{E}(r) = \dfrac{I}{4\pi\sigma r^2}\,\hat{r} \quad (a < r < b)$ |
| | **c)** Diferencia de potencial $\Delta V = V(b) - V(a)$ | $\Delta V = -\dfrac{I(b - a)}{4\pi\sigma a b}$ |
| | **d)** Resistencia eléctrica entre cascarones $R$ | $R = \dfrac{b - a}{4\pi\sigma a b}$ |
| **Problema 2** | Resistencia vista entre terminales $A$ y $B$ | $R_{eq} = \dfrac{2L}{\pi R^2}\left(\dfrac{\rho_1 \rho_2}{\rho_1 + \rho_2}\right)$ |
| **Problema 3** | Resistencia equivalente entre terminales $a$ y $b$ | $R_{ab} = \dfrac{28731}{2479}\,\Omega \approx 11{,}59\,\Omega$ |
