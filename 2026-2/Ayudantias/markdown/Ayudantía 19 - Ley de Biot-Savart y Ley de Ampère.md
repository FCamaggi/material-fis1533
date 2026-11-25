# Ayudantía 19 — Ley de Biot-Savart y Ley de Ampère

> Clases relacionadas: [Clase 11 - Ley de Biot Savart](../../Clases/markdown/Clase%2011%20-%20Ley%20de%20Biot%20Savart.md), [Clase 12 - Ley de Ampere](../../Clases/markdown/Clase%2012%20-%20Ley%20de%20Ampere.md)

---

## Problema 1

Considere la espira de corriente formada por segmentos radiales y arcos de circunferencias como se describe en la figura. Obtenga el campo magnético $\vec{B}$ medido en $P$.

> **[Figura]:** Circuito cerrado coplanar en el plano horizontal $XY$ alimentado por cables exteriores, que delimita un sector circular de ángulo de apertura $\phi$ con vértice común en el punto $P$ (origen de coordenadas $(0,0)$):
> - **Líneas de alimentación (tramos 1 y 5):** Dos conductores rectilíneos horizontales coincidentes a lo largo del semieje $X$ positivo. El tramo 1 ingresa corriente $I$ hacia la izquierda ($\leftarrow I$) hasta $x = b$, mientras que el tramo 5 retorna corriente $I$ hacia la derecha desde $x = a$ hacia la fuente.
> - **Tramo 2 (arco exterior):** Arco de circunferencia de radio $b$ subtendido por el ángulo $\phi$ (desde $\theta = 0$ hasta $\theta = \phi$), recorrido en sentido antihorario con corriente $I$.
> - **Tramo 3 (segmento radial inclinado):** Alambre recto sobre el rayo $\theta = \phi$, que conecta el arco exterior de radio $b$ con el arco interior de radio $a$, con la corriente $I$ dirigida radialmente hacia el origen $P$.
> - **Tramo 4 (arco interior):** Arco de circunferencia de radio $a$ subtendido por el ángulo $\phi$ (desde $\theta = \phi$ hasta $\theta = 0$), recorrido en sentido horario con corriente $I$.
> El punto de medición $P$ es el centro de curvatura de ambos arcos circulares.

### Solución

**Idea:** Aplicar el principio de superposición junto con la ley de Biot-Savart:
$$d\vec{B} = \frac{\mu_0 I}{4\pi} \frac{d\vec{\ell} \times (\vec{r} - \vec{r}')}{|\vec{r} - \vec{r}'|^3}$$
Fijando el origen de coordenadas en el punto $P$ ($\vec{r} = \vec{0}$), el vector hacia la fuente es $\vec{r}'$, de modo que $\vec{r} - \vec{r}' = -\vec{r}'$. Para cualquier tramo rectilíneo que apunte a lo largo de una recta que pasa por el punto $P$, el elemento diferencial $d\vec{\ell}$ es estrictamente colineal con el vector de posición radial $\vec{r}'$, haciendo que el producto vectorial $d\vec{\ell} \times (-\vec{r}')$ sea idénticamente nulo. Por ende, solo los arcos de circunferencia contribuyen al campo magnético en $P$.

#### 1. Segmentos rectilíneos radiales (tramos 1, 3 y 5)

1. **Líneas de alimentación horizontales (tramos 1 y 5):**  
   Ubicadas sobre el eje polar horizontal ($y = 0$, $x > 0$).  
   Tienen $\vec{r}' = x\,\hat{i}$ y diferencial de longitud $d\vec{\ell} = dx\,\hat{i}$.  
   El producto vectorial es:
   $$d\vec{\ell} \times (\vec{r} - \vec{r}') = (dx\,\hat{i}) \times (-x\,\hat{i}) = \vec{0}$$
   Ambos tramos aportan campo magnético nulo en el punto $P$:
   $$\vec{B}_1 = \vec{B}_5 = \vec{0}$$

2. **Segmento radial inclinado (tramo 3):**  
   Se encuentra a lo largo del rayo a ángulo constante $\theta = \phi$.  
   La posición es $\vec{r}' = r\,\hat{r}(\phi)$ con $r \in [a, b]$.  
   El elemento de longitud apunta hacia el centro: $d\vec{\ell} = dr\,(-\hat{r}) = -dr\,\hat{r}$.  
   Como $d\vec{\ell}$ es estrictamente paralelo a $\vec{r}'$:
   $$d\vec{\ell} \times (\vec{r} - \vec{r}') = (-dr\,\hat{r}) \times (-r\,\hat{r}) = \vec{0} \implies \vec{B}_3 = \vec{0}$$

---

#### 2. Arco exterior de radio $b$ (tramo 2)

El arco se encuentra a distancia radial constante $r' = b$, con $\theta \in [0, \phi]$.
- Vector posición: $\vec{r}' = b\,\hat{r}$.
- Vector relativo al punto $P$: $\vec{r} - \vec{r}' = -b\,\hat{r}$.
- Distancia: $|\vec{r} - \vec{r}'| = b$.
- Elemento de longitud en sentido antihorario: $d\vec{\ell} = b\,d\theta\,\hat{\theta}$.

Calculamos el producto vectorial en coordenadas polares en el plano $XY$:
$$d\vec{\ell} \times (\vec{r} - \vec{r}') = (b\,d\theta\,\hat{\theta}) \times (-b\,\hat{r}) = -b^2 d\theta\,(\hat{\theta} \times \hat{r})$$

Sabiendo que en la base cilíndrica $\hat{r} \times \hat{\theta} = \hat{k}$, se tiene $\hat{\theta} \times \hat{r} = -\hat{k}$:
$$d\vec{\ell} \times (\vec{r} - \vec{r}') = -b^2 d\theta\,(-\hat{k}) = b^2 d\theta\,\hat{k}$$

Integrando sobre el ángulo $\theta$ desde $0$ hasta $\phi$:
$$\vec{B}_2 = \frac{\mu_0 I}{4\pi} \int_0^\phi \frac{b^2 d\theta}{b^3}\,\hat{k} = \frac{\mu_0 I}{4\pi b} \left[ \int_0^\phi d\theta \right] \hat{k}$$

$$\vec{B}_2 = \frac{\mu_0 I \phi}{4\pi b}\,\hat{k}$$

El campo del arco exterior apunta saliendo de la hoja ($+\hat{k}$), coherente con el giro antihorario de la corriente.

---

#### 3. Arco interior de radio $a$ (tramo 4)

El arco se encuentra a radio constante $r' = a$. La corriente circula en sentido horario, desde $\theta = \phi$ hasta $\theta = 0$:
- Vector relativo: $\vec{r} - \vec{r}' = -a\,\hat{r}$.
- Elemento de longitud en sentido horario: $d\vec{\ell} = a\,d\theta\,(-\hat{\theta}) = -a\,d\theta\,\hat{\theta}$.

El producto vectorial entrega:
$$d\vec{\ell} \times (\vec{r} - \vec{r}') = (-a\,d\theta\,\hat{\theta}) \times (-a\,\hat{r}) = a^2 d\theta\,(\hat{\theta} \times \hat{r}) = -a^2 d\theta\,\hat{k}$$

Integrando para el arco de apertura $\phi$:
$$\vec{B}_4 = \frac{\mu_0 I}{4\pi} \int_0^\phi \frac{-a^2 d\theta}{a^3}\,\hat{k} = -\frac{\mu_0 I \phi}{4\pi a}\,\hat{k}$$

El campo del arco interior apunta entrando a la hoja ($-\hat{k}$), coherente con el giro horario de la corriente.

---

#### 4. Campo magnético total en el punto $P$

Sumando vectorialmente las contribuciones de todos los tramos:

$$\vec{B}_T = \vec{B}_1 + \vec{B}_2 + \vec{B}_3 + \vec{B}_4 + \vec{B}_5 = \vec{B}_2 + \vec{B}_4$$

$$\vec{B}_T = \left( \frac{\mu_0 I \phi}{4\pi b} - \frac{\mu_0 I \phi}{4\pi a} \right) \hat{k}$$

$$\boxed{\vec{B}_P = \frac{\mu_0 I \phi}{4\pi} \left( \frac{1}{b} - \frac{1}{a} \right) \hat{k} = -\frac{\mu_0 I \phi (b - a)}{4\pi a b}\,\hat{k}}$$

Como $b > a$, se cumple $\frac{1}{a} > \frac{1}{b}$, por lo que la cantidad en el paréntesis es negativa:
$$|\vec{B}_P| = \frac{\mu_0 I \phi (b - a)}{4\pi a b}$$
y el vector apunta **entrando al plano de la hoja** ($-\hat{k}$).

**Verificación:**
- **Unidades:** $[\mu_0 I / a] = \text{T}$, y el ángulo $\phi$ en radianes es adimensional. Dimensionalmente correcto.
- **Caso límite $\phi \to 2\pi$ y $b \to \infty$:** Si no hay arco exterior ($b \to \infty$) y el arco interior se convierte en una espira circular completa horaria ($\phi = 2\pi$), $\vec{B}_P \to -\frac{\mu_0 I (2\pi)}{4\pi a}\hat{k} = -\frac{\mu_0 I}{2a}\hat{k}$, recuperando el resultado estándar para el centro de una espira circular de radio $a$.
- **Caso límite $a \to b$:** Si los radios coinciden ($b \to a$), la espira encierra área nula y las corrientes opuestas se cancelan, entregando $\vec{B}_P = \vec{0}$.

---

## Problema 2

Tres alambres infinitos están ubicados mutuamente paralelos orientados perpendicularmente al plano de la hoja y ubicados en los vértices de un cuadrado de lado $d$. Uno de ellos lleva corriente $2I$ que entra al plano, mientras que los otros llevan corriente $I$ que emerge del plano de la hoja. Calcule el vector campo magnético en los puntos $P_1$ y $P_2$.

> **[Figura]:** Un cuadrado de lado $d$ dispuesto en el plano de la hoja:
> - **Vértice superior izquierdo $(0, d)$:** Alambre rectilíneo infinito con corriente $2I$ entrando al plano ($\otimes$).
> - **Vértice superior derecho $(d, d)$:** Alambre rectilíneo infinito con corriente $I$ saliendo del plano ($\odot$).
> - **Vértice inferior izquierdo $(0, 0)$:** Alambre rectilíneo infinito con corriente $I$ saliendo del plano ($\odot$).
> - **Vértice inferior derecho $(d, 0)$:** Vértice desocupado (sin alambre), donde se sitúa el punto de observación $P_2$.
> - **Centro del cuadrado $(d/2, d/2)$:** Punto de intersección de las diagonales, rotulado como $P_1$.

### Solución

**Idea:** La ley de Ampère determina que a una distancia radial $r$ de un alambre infinito que transporta corriente estacionaria $I_c$, el campo magnético es puramente tangencial:
$$\vec{B} = \frac{\mu_0 I_c}{2\pi r}\,\hat{\theta}$$
donde el sentido de $\hat{\theta}$ se establece por la regla de la mano derecha:
- Si la corriente sale de la hoja ($+\hat{z}$), las líneas de campo circulan en sentido antihorario.
- Si la corriente entra a la hoja ($-\hat{z}$), las líneas de campo circulan en sentido horario.

Utilizamos el principio de superposición para sumar vectorialmente el campo magnético de los tres alambres en cada punto de observación.

Establecemos un sistema coordenado cartesiano bidimensional con origen en el vértice inferior izquierdo $(0,0)$:
- Alambre 1 (superior izquierdo): posición $\vec{r}_1 = (0, d)$, corriente $I_{(1)} = 2I$ entrando ($-\hat{z}$).
- Alambre 2 (inferior izquierdo): posición $\vec{r}_2 = (0, 0)$, corriente $I_{(2)} = I$ saliendo ($+\hat{z}$).
- Alambre 3 (superior derecho): posición $\vec{r}_3 = (d, d)$, corriente $I_{(3)} = I$ saliendo ($+\hat{z}$).

---

#### 1. Cálculo del campo magnético en el punto $P_1$ (centro del cuadrado)

El punto $P_1$ está ubicado en $\vec{r}_{P_1} = \left(\frac{d}{2}, \frac{d}{2}\right)$.  
La distancia desde cualquiera de los cuatro vértices del cuadrado al centro $P_1$ es:

$$r = \sqrt{\left(\frac{d}{2}\right)^2 + \left(\frac{d}{2}\right)^2} = \sqrt{\frac{d^2}{2}} = \frac{d}{\sqrt{2}}$$

1. **Contribuciones de los alambres con corriente $I$ (alambres 2 y 3):**  
   - Los alambres 2 en $(0,0)$ y 3 en $(d,d)$ están situados en extremos diagonalmente opuestos respecto a $P_1$.
   - Ambos transportan la misma corriente $I$ en el mismo sentido ($+\hat{z}$, saliendo de la hoja).
   - Por simetría de inversión central respecto al punto medio $P_1$, las líneas tangenciales de campo magnético producidas por el alambre 2 y por el alambre 3 tienen idéntica magnitud y sentidos exactamente opuestos en el punto central:
     $$\vec{B}_2(P_1) + \vec{B}_3(P_1) = \vec{0}$$
     *Demostración explícita:*  
     Vector unitario desde el alambre 2 hacia $P_1$: $\hat{u}_2 = \frac{\hat{i} + \hat{j}}{\sqrt{2}}$.  
     Campo: $\vec{B}_2 = \frac{\mu_0 I}{2\pi (d/\sqrt{2})}(\hat{z} \times \hat{u}_2) = \frac{\mu_0 I}{\pi \sqrt{2}d}\left(\frac{-\hat{i} + \hat{j}}{\sqrt{2}}\right) = \frac{\mu_0 I}{2\pi d}(-\hat{i} + \hat{j})$.  
     Vector unitario desde el alambre 3 hacia $P_1$: $\hat{u}_3 = \frac{-\hat{i} - \hat{j}}{\sqrt{2}} = -\hat{u}_2$.  
     Campo: $\vec{B}_3 = \frac{\mu_0 I}{2\pi (d/\sqrt{2})}(\hat{z} \times \hat{u}_3) = -\vec{B}_2$.  
     Por tanto, se anulan rigurosamente entre sí.

2. **Contribución del alambre 1 (corriente $2I$ entrando al plano en $(0,d)$):**  
   Vector posición desde el alambre 1 hacia $P_1$:
   $$\vec{r}_{P_1} - \vec{r}_1 = \left(\frac{d}{2} - 0\right)\hat{i} + \left(\frac{d}{2} - d\right)\hat{j} = \frac{d}{2}\hat{i} - \frac{d}{2}\hat{j}$$
   El vector unitario radial desde la fuente es:
   $$\hat{u}_1 = \frac{\hat{i} - \hat{j}}{\sqrt{2}}$$
   Dado que la corriente entra a la hoja, el vector corriente apunta en $-\hat{z}$. La dirección del campo magnético es:
   $$(-\hat{z}) \times \hat{u}_1 = (-\hat{z}) \times \left(\frac{\hat{i} - \hat{j}}{\sqrt{2}}\right) = \frac{-(\hat{z} \times \hat{i}) + (\hat{z} \times \hat{j})}{\sqrt{2}} = \frac{-\hat{j} - \hat{i}}{\sqrt{2}} = -\frac{\hat{i} + \hat{j}}{\sqrt{2}}$$
   La magnitud del campo producido por la corriente $2I$ a distancia $r = \frac{d}{\sqrt{2}}$ es:
   $$B_1 = \frac{\mu_0 (2I)}{2\pi r} = \frac{\mu_0 I}{\pi \left(\frac{d}{\sqrt{2}}\right)} = \frac{\sqrt{2}\mu_0 I}{\pi d}$$
   Multiplicando la magnitud por el vector unitario de dirección:
   $$\vec{B}_T(P_1) = \vec{B}_1 = \left( \frac{\sqrt{2}\mu_0 I}{\pi d} \right) \left( -\frac{\hat{i} + \hat{j}}{\sqrt{2}} \right)$$

$$\boxed{\vec{B}(P_1) = -\frac{\mu_0 I}{\pi d}(\hat{i} + \hat{j})}$$

Magnitud:
$$|\vec{B}(P_1)| = \frac{\sqrt{2}\mu_0 I}{\pi d}$$

---

#### 2. Cálculo del campo magnético en el punto $P_2$ (vértice inferior derecho)

El punto $P_2$ está ubicado en $\vec{r}_{P_2} = (d, 0)$.

1. **Campo debido al alambre 2 (en $(0,0)$, corriente $I$ saliendo, $+\hat{z}$):**  
   - Distancia: $r_2 = d$.  
   - Vector de posición de la fuente al punto: $\vec{r}_{P_2} - \vec{r}_2 = d\,\hat{i} \implies \hat{u}_2 = \hat{i}$.  
   - Dirección: $\hat{z} \times \hat{i} = \hat{j}$.  
   $$\vec{B}_2(P_2) = \frac{\mu_0 I}{2\pi d}\,\hat{j}$$

2. **Campo debido al alambre 3 (en $(d,d)$, corriente $I$ saliendo, $+\hat{z}$):**  
   - Distancia: $r_3 = d$.  
   - Vector de posición de la fuente al punto: $\vec{r}_{P_2} - \vec{r}_3 = -d\,\hat{j} \implies \hat{u}_3 = -\hat{j}$.  
   - Dirección: $\hat{z} \times (-\hat{j}) = -(-\hat{i}) = \hat{i}$.  
   $$\vec{B}_3(P_2) = \frac{\mu_0 I}{2\pi d}\,\hat{i}$$

   La suma de los campos de los alambres 2 y 3 en $P_2$ es:
   $$\vec{B}_2 + \vec{B}_3 = \frac{\mu_0 I}{2\pi d}(\hat{i} + \hat{j})$$

3. **Campo debido al alambre 1 (en $(0,d)$, corriente $2I$ entrando, $-\hat{z}$):**  
   - Distancia diagonal: $r_1 = \sqrt{d^2 + d^2} = \sqrt{2}d$.  
   - Vector de posición de la fuente al punto: $\vec{r}_{P_2} - \vec{r}_1 = d\,\hat{i} - d\,\hat{j}$.  
   - Vector unitario: $\hat{u}_1 = \frac{\hat{i} - \hat{j}}{\sqrt{2}}$.  
   - Dirección: $(-\hat{z}) \times \hat{u}_1 = -\frac{\hat{i} + \hat{j}}{\sqrt{2}}$.  
   - Magnitud del campo:
     $$B_1 = \frac{\mu_0 (2I)}{2\pi r_1} = \frac{\mu_0 I}{\pi (\sqrt{2}d)} = \frac{\mu_0 I}{\sqrt{2}\pi d}$$
   - Vector campo magnético $\vec{B}_1$:
     $$\vec{B}_1(P_2) = \left(\frac{\mu_0 I}{\sqrt{2}\pi d}\right) \left(-\frac{\hat{i} + \hat{j}}{\sqrt{2}}\right) = -\frac{\mu_0 I}{2\pi d}(\hat{i} + \hat{j})$$

4. **Suma vectorial total en $P_2$:**
   $$\vec{B}_T(P_2) = \vec{B}_1(P_2) + \vec{B}_2(P_2) + \vec{B}_3(P_2)$$
   $$\vec{B}_T(P_2) = -\frac{\mu_0 I}{2\pi d}(\hat{i} + \hat{j}) + \frac{\mu_0 I}{2\pi d}(\hat{i} + \hat{j})$$

$$\boxed{\vec{B}(P_2) = \vec{0}}$$

El campo magnético en el vértice desocupado $P_2$ es idénticamente nulo.

**Verificación:**
- **Unidades:** En $P_1$, $[\mu_0 I / d] = \frac{(\text{T}\cdot\text{m/A})\cdot\text{A}}{\text{m}} = \text{T}$, consistente.
- **Cancelación exacta en $P_2$:** Los dos alambres adyacentes de corriente $I$ generan campos ortogonales de igual magnitud $\frac{\mu_0 I}{2\pi d}$, cuya resultante apunta a $45^\circ$ en dirección $\frac{\hat{i}+\hat{j}}{\sqrt{2}}$ con magnitud $\sqrt{2}\frac{\mu_0 I}{2\pi d} = \frac{\mu_0 I}{\sqrt{2}\pi d}$. El alambre opuesto de corriente $2I$ está a distancia diagonal $\sqrt{2}d$, por lo que su campo tiene magnitud $\frac{\mu_0 (2I)}{2\pi\sqrt{2}d} = \frac{\mu_0 I}{\sqrt{2}\pi d}$ y apunta exactamente en la dirección opuesta $-\frac{\hat{i}+\hat{j}}{\sqrt{2}}$. La anulación es perfecta.

---

## Problema 3

Dentro de una tubería metálica cilíndrica de radio $a$ circula un fluido viscoso con una cierta densidad de carga. En los puntos al interior de la tubería se ha determinado que el campo magnético vale
$$\vec{B} = \frac{\mu_0 J_0 r}{2}\left(1 - \frac{r^2}{2a^2}\right)\hat{\theta}$$
donde $J_0$ es una constante y $r$ es la distancia del eje del cilindro. Determine:

a) El vector densidad de corriente y la intensidad de corriente eléctrica dentro de la tubería.  
b) El campo magnético fuera de la tubería.  
c) El valor de la densidad superficial de corriente $\vec{K}$ que debe circular por el borde de la tubería para que el campo magnético en el exterior sea nulo (suponga que $\vec{K}$ se distribuye uniformemente por la superficie).

> **[Figura]:** Un cilindro infinitamente largo de radio $a$ representativo de la tubería metálica, orientado verticalmente con su eje coincidente con el eje $Z$. Un fluido cargado circula longitudinalmente a través de la sección transversal con densidad volumétrica de corriente $\vec{J} = J_z(r)\,\hat{z}$ dirigida hacia arriba. Las líneas de campo magnético en el interior son circunferencias concéntricas orientadas en la dirección azimutal $\hat{\theta}$.

### Solución

**Idea:** La relación local entre el campo magnético y la densidad de corriente está gobernada por la ley de Ampère en su forma diferencial, $\nabla \times \vec{B} = \mu_0 \vec{J}$. Al integrar la densidad de corriente sobre la sección transversal del cilindro obtenemos la corriente neta interior. Fuera de la tubería, la simetría cilíndrica permite usar la ley de Ampère en su forma integral para relacionar el campo exterior con la corriente total encerrada. Finalmente, una corriente superficial en $r = a$ agrega una discontinuidad en la componente tangencial del campo, permitiendo anular el campo exterior al imponer corriente neta encerrada nula.

---

#### a) Vector densidad de corriente $\vec{J}$ e intensidad total de corriente $I$

1. **Densidad de corriente $\vec{J}$:**  
   En coordenadas cilíndricas $(r, \theta, z)$, el rotacional de un campo magnético que posee únicamente componente azimutal dependiente solo del radio, $\vec{B} = B_\theta(r)\,\hat{\theta}$, se reduce a:
   $$\nabla \times \vec{B} = \frac{1}{r}\frac{\partial(r B_\theta)}{\partial r}\,\hat{z}$$
   Por la forma diferencial de la ley de Ampère:
   $$\nabla \times \vec{B} = \mu_0 \vec{J} \implies \vec{J} = \frac{1}{\mu_0 r}\frac{\partial(r B_\theta)}{\partial r}\,\hat{z}$$
   Reemplazando la expresión dada de $B_\theta(r)$:
   $$r B_\theta(r) = r \left[ \frac{\mu_0 J_0 r}{2}\left(1 - \frac{r^2}{2a^2}\right) \right] = \frac{\mu_0 J_0}{2}\left(r^2 - \frac{r^4}{2a^2}\right)$$
   Derivando respecto a $r$:
   $$\frac{\partial(r B_\theta)}{\partial r} = \frac{\mu_0 J_0}{2}\left(2r - \frac{4r^3}{2a^2}\right) = \frac{\mu_0 J_0}{2}\left(2r - \frac{2r^3}{a^2}\right) = \mu_0 J_0 r\left(1 - \frac{r^2}{a^2}\right)$$
   Dividiendo por $\mu_0 r$:
   $$\vec{J}(r) = \frac{\mu_0 J_0 r\left(1 - \frac{r^2}{a^2}\right)}{\mu_0 r}\,\hat{z} = J_0\left(1 - \frac{r^2}{a^2}\right)\hat{z}$$

$$\boxed{\vec{J}(r) = J_0\left(1 - \frac{r^2}{a^2}\right)\hat{z} \quad (r \le a)}$$

2. **Intensidad de corriente eléctrica total $I$:**  
   La corriente total que fluye a través de la sección transversal de la tubería se calcula integrando el flujo de $\vec{J}$ en el disco de radio $a$:
   $$I = \iint_{\text{sección}} \vec{J} \cdot d\vec{a} = \int_0^{2\pi} d\theta \int_0^a J_0\left(1 - \frac{r^2}{a^2}\right) r\,dr$$
   $$I = 2\pi J_0 \int_0^a \left(r - \frac{r^3}{a^2}\right) dr = 2\pi J_0 \left[ \frac{r^2}{2} - \frac{r^4}{4a^2} \right]_0^a$$
   $$I = 2\pi J_0 \left( \frac{a^2}{2} - \frac{a^4}{4a^2} \right) = 2\pi J_0 \left( \frac{a^2}{2} - \frac{a^2}{4} \right) = 2\pi J_0 \left(\frac{a^2}{4}\right)$$

$$\boxed{I = \frac{\pi J_0 a^2}{2}}$$

---

#### b) Campo magnético fuera de la tubería ($r > a$)

Por la simetría cilíndrica del sistema, las líneas de campo en el exterior son circunferencias concéntricas centradas en el eje $Z$: $\vec{B} = B(r)\,\hat{\theta}$.

Considerando un lazo amperiano circular de radio $r > a$ en el plano perpendicular al eje:
$$\oint_C \vec{B} \cdot d\vec{\ell} = \mu_0 I_{\text{enc}}$$

El lado izquierdo entrega la circulación del campo a lo largo del perímetro:
$$\oint_C \vec{B} \cdot d\vec{\ell} = B(r) \int_0^{2\pi} r\,d\theta = 2\pi r B(r)$$

Dado que la curva amperiana encierra toda la sección transversal de la tubería, la corriente encerrada es la corriente total del fluido viscoso:
$$I_{\text{enc}} = I = \frac{\pi J_0 a^2}{2}$$

Igualando:
$$2\pi r B(r) = \mu_0 \left(\frac{\pi J_0 a^2}{2}\right) \implies B(r) = \frac{\mu_0 J_0 a^2}{4r}$$

Vectorialmente:

$$\boxed{\vec{B}(r) = \frac{\mu_0 J_0 a^2}{4r}\,\hat{\theta} \quad (r > a)}$$

Equivalentemente, en términos de la corriente total $I$: $\vec{B}(r) = \frac{\mu_0 I}{2\pi r}\,\hat{\theta}$.

---

#### c) Densidad superficial de corriente $\vec{K}$ para anular el campo exterior

Para que el campo magnético en el exterior sea nulo ($\vec{B}(r) = \vec{0}$ para todo $r > a$), la ley de Ampère sobre cualquier lazo amperiano de radio $r > a$ exige que la corriente total neta encerrada sea cero:

$$I_{\text{enc}} = 0$$

La corriente neta encerrada se compone de la corriente volumétrica del fluido viscoso $I$ más la corriente superficial conducida por el borde de la tubería en $r = a$:

$$I_{\text{enc}} = I + I_{\text{sup}} = 0 \implies I_{\text{sup}} = -I = -\frac{\pi J_0 a^2}{2}$$

Como la densidad superficial de corriente $\vec{K} = K_z\,\hat{z}$ se distribuye uniformemente en el perímetro $2\pi a$ de la tubería cilíndrica:

$$I_{\text{sup}} = K_z (2\pi a)$$

Despejando la componente longitudinal $K_z$:

$$K_z = \frac{I_{\text{sup}}}{2\pi a} = \frac{-\frac{\pi J_0 a^2}{2}}{2\pi a} = -\frac{J_0 a}{4}$$

Vectorialmente:

$$\boxed{\vec{K} = -\frac{J_0 a}{4}\,\hat{z}}$$

**Verificación:**
- **Continuidad del campo sin corriente superficial:**  
  En $r = a$, el campo interior es $\vec{B}_{\text{int}}(a) = \frac{\mu_0 J_0 a}{2}\left(1 - \frac{1}{2}\right)\hat{\theta} = \frac{\mu_0 J_0 a}{4}\hat{\theta}$.  
  El campo exterior es $\vec{B}_{\text{ext}}(a) = \frac{\mu_0 J_0 a^2}{4a}\hat{\theta} = \frac{\mu_0 J_0 a}{4}\hat{\theta}$.  
  Ambos coinciden exactamente, verificando que $\vec{B}$ es continuo en la frontera cuando no hay corrientes superficiales singulares.
- **Condición de salto con corriente superficial $\vec{K}$:**  
  La condición de contorno general del electromagnetismo establece:
  $$\hat{n}_{1\to 2} \times (\vec{B}_2 - \vec{B}_1) = \mu_0 \vec{K}$$
  Tomando región 1 como el interior ($r \to a^-$) y región 2 como el exterior ($r \to a^+$), con normal hacia el exterior $\hat{n} = \hat{r}$:
  $$\hat{r} \times \left(\vec{0} - \frac{\mu_0 J_0 a}{4}\hat{\theta}\right) = -\frac{\mu_0 J_0 a}{4}(\hat{r} \times \hat{\theta}) = -\frac{\mu_0 J_0 a}{4}\hat{z}$$
  Igualando a $\mu_0 \vec{K}$, se obtiene de inmediato $\vec{K} = -\frac{J_0 a}{4}\hat{z}$, verificando de forma cruzada el resultado.
- **Unidades:** $[J_0] = \text{A/m}^2 \implies [K] = [J_0][a] = (\text{A/m}^2)\cdot\text{m} = \text{A/m}$, unidades estándar de densidad superficial de corriente.

---

## Resumen de resultados

| Problema / Inciso | Expresión / Resultado | Comentarios |
| :--- | :--- | :--- |
| **P1** Campo en el vértice $P$ | $\vec{B}_P = \frac{\mu_0 I \phi}{4\pi}\left(\frac{1}{b} - \frac{1}{a}\right)\hat{k} = -\frac{\mu_0 I \phi(b-a)}{4\pi a b}\hat{k}$ | Solo contribuyen los arcos circulares; segmentos radiales tienen $d\vec{\ell} \parallel \vec{r}'$ y aportan cero. |
| **P2** Campo en el centro $P_1$ | $\vec{B}(P_1) = -\frac{\mu_0 I}{\pi d}(\hat{i} + \hat{j})$ | Las corrientes simétricas $I$ se cancelan; solo contribuye la corriente $2I$ entrando. |
| **P2** Campo en el vértice $P_2$ | $\vec{B}(P_2) = \vec{0}$ | Cancelación exacta entre el alambre de $2I$ ($\sqrt{2}d$) y los dos de $I$ ($d$). |
| **P3 a)** Densidad volumétrica de corriente | $\vec{J}(r) = J_0\left(1 - \frac{r^2}{a^2}\right)\hat{z} \quad (r \le a)$ | Obtenida mediante rotacional en cilíndricas $(\nabla \times \vec{B})_z = \mu_0 J_z$. |
| **P3 a)** Intensidad de corriente total | $I = \frac{\pi J_0 a^2}{2}$ | Flujo de $\vec{J}$ integrado en la sección de radio $a$. |
| **P3 b)** Campo magnético exterior ($r > a$) | $\vec{B}(r) = \frac{\mu_0 J_0 a^2}{4r}\,\hat{\theta} = \frac{\mu_0 I}{2\pi r}\,\hat{\theta}$ | Ley de Ampère integral en lazo circular exterior de radio $r$. |
| **P3 c)** Densidad superficial en la tubería | $\vec{K} = -\frac{J_0 a}{4}\,\hat{z}$ | Anula la corriente total neta encerrada ($I_{\text{enc}} = 0$). |
