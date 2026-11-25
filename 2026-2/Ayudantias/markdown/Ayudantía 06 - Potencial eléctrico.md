# Ayudantía 06 — Potencial eléctrico

> Clases relacionadas: [Clase 05 - Potencial electroestático](../../Clases/markdown/Clase%2005%20-%20Potencial%20electroest%C3%A1tico.md)

---

## Problema 1

Una densidad de carga lineal $\lambda$ está repartida de forma homogénea a lo largo de una semicircunferencia $BD$ centrada en $C$ y de radio $R$. Una carga puntual $q$ está ubicada en punto $A$ como se indica en la figura. ($CA = R$).

1. Calcule el potencial eléctrico en el punto $C$.  
2. Por argumentos de simetría, determine la dirección del campo eléctrico en $C$, $\vec{E}(C)$.  
3. Determine la relación entre $\lambda$ y $q$ tal que $\vec{E}(C) = 0$.

> **[Figura]:** Semicircunferencia en el semiplano superior con extremos sobre una línea horizontal en los puntos $B$ (extremo izquierdo) y $D$ (extremo derecho), con radio $R$ y centro en el punto $C$. La semicircunferencia porta una densidad lineal uniforme de carga $\lambda$. Directamente debajo del centro $C$, sobre la recta vertical perpendicular a la base y a una distancia $R$, se sitúa el punto $A$, donde se localiza una carga puntual $q$.

### Solución

**Idea:** Para el potencial en $C$, superponer el potencial escalar de una distribución continua $V = \frac{1}{4\pi\varepsilon_0}\int \frac{dq}{r}$ y el de una carga puntual. Para el campo eléctrico, emplear argumentos de paridad geométrica respecto al eje de simetría vertical para demostrar la anulación de la componente horizontal, y luego igualar vectorialmente el campo creado por la semicircunferencia y el de la carga puntual para lograr la cancelación neta en $C$.

#### 1. Potencial eléctrico en el punto $C$

Establecemos un sistema de coordenadas cartesiano con origen en el punto $C = (0, 0)$:
- El eje $X$ coincide con el segmento horizontal que une los extremos $B = (-R, 0)$ y $D = (R, 0)$.
- El eje $Y$ es perpendicular a la base, apuntando hacia arriba. La semicircunferencia se ubica en $y \ge 0$.
- La carga puntual en el punto $A$ tiene coordenadas $(0, -R)$.

Por el principio de superposición, tomando el potencial nulo en el infinito ($V(\infty) = 0$):
$$V(C) = V_\lambda(C) + V_q(C)$$

1. **Contribución de la semicircunferencia ($V_\lambda(C)$):**  
   Parametrizamos la semicircunferencia en coordenadas polares con radio constante $r' = R$ y ángulo $\theta \in [0, \pi]$:
   $$dq = \lambda\,dL = \lambda R\,d\theta$$
   Dado que todo elemento diferencial de la semicircunferencia dista exactamente $|\vec{r}_C - \vec{r}'| = R$ del centro $C$:
   $$V_\lambda(C) = \frac{1}{4\pi\varepsilon_0} \int_{\text{arco}} \frac{dq}{R} = \frac{1}{4\pi\varepsilon_0} \int_0^\pi \frac{\lambda R\,d\theta}{R} = \frac{\lambda}{4\pi\varepsilon_0} \int_0^\pi d\theta = \frac{\lambda \pi}{4\pi\varepsilon_0} = \frac{\lambda}{4\varepsilon_0}$$

2. **Contribución de la carga puntual en $A$ ($V_q(C)$):**  
   La distancia entre el punto $A$ y el centro $C$ es $CA = R$:
   $$V_q(C) = \frac{1}{4\pi\varepsilon_0}\frac{q}{R}$$

Sumando ambas contribuciones:
$$V(C) = \frac{\lambda}{4\varepsilon_0} + \frac{q}{4\pi\varepsilon_0 R}$$

$$\boxed{V(C) = \frac{1}{4\varepsilon_0}\left(\lambda + \frac{q}{\pi R}\right)}$$

---

#### 2. Dirección del campo eléctrico en $C$ por simetría

Analizamos la simetría del sistema respecto al eje vertical $Y$ (la recta que pasa por $A$ y $C$):
- **Semicircunferencia:** La distribución de carga $\lambda$ es simétrica respecto al eje $Y$. Para cada elemento de carga diferencial $dq$ ubicado en una posición angular $\theta \in [0, \pi/2]$, existe un elemento homólogo idéntico en $\pi - \theta \in [\pi/2, \pi]$. Los campos diferenciales producidos por este par tienen componentes horizontales en oposición:
  $$dE_x(\theta) = -dE_x(\pi - \theta)$$
  Por ende, la integral de la componente horizontal se anula idénticamente ($\int_0^\pi \cos\theta\,d\theta = 0$). Las componentes verticales apuntan ambas hacia abajo ($-\hat{y}$) si $\lambda > 0$, sumándose constructivamente.
- **Carga puntual en $A$:** La carga $q$ se encuentra sobre el propio eje $Y$, en $(0, -R)$. Su vector de posición relativo al punto $C$ es $\vec{r}_C - \vec{r}_A = R\,\hat{y}$. Por lo tanto, el campo que genera en $C$ es estrictamente vertical, a lo largo de la dirección $\hat{y}$.

Conclusión por simetría: La componente horizontal total del campo eléctrico en $C$ es nula ($E_x(C) = 0$), de modo que **el campo eléctrico $\vec{E}(C)$ apunta exclusivamente a lo largo del eje vertical (eje $Y$)**.

---

#### 3. Relación entre $\lambda$ y $q$ tal que $\vec{E}(C) = 0$

Calculamos explícitamente el campo de cada fuente en $C$:
- **Campo de la carga puntual:**
  $$\vec{E}_q(C) = \frac{1}{4\pi\varepsilon_0} \frac{q (\vec{r}_C - \vec{r}_A)}{|\vec{r}_C - \vec{r}_A|^3} = \frac{q (R\,\hat{y})}{4\pi\varepsilon_0 R^3} = \frac{q}{4\pi\varepsilon_0 R^2}\,\hat{y}$$

- **Campo de la semicircunferencia:**
  Un elemento de carga en posición $\vec{r}' = R(\cos\theta\,\hat{x} + \sin\theta\,\hat{y})$ ejerce en el origen $\vec{r} = 0$:
  $$d\vec{E}_\lambda = \frac{1}{4\pi\varepsilon_0} \frac{dq (0 - \vec{r}')}{R^3} = -\frac{\lambda R\,d\theta}{4\pi\varepsilon_0 R^2}(\cos\theta\,\hat{x} + \sin\theta\,\hat{y})$$
  Integrando entre $\theta = 0$ y $\theta = \pi$:
  $$\vec{E}_\lambda(C) = -\frac{\lambda}{4\pi\varepsilon_0 R} \left[ \left(\int_0^\pi \cos\theta\,d\theta\right)\hat{x} + \left(\int_0^\pi \sin\theta\,d\theta\right)\hat{y} \right]$$
  Dado que $\int_0^\pi \cos\theta\,d\theta = 0$ y $\int_0^\pi \sin\theta\,d\theta = [-\cos\theta]_0^\pi = 2$:
  $$\vec{E}_\lambda(C) = -\frac{\lambda}{4\pi\varepsilon_0 R}(2\,\hat{y}) = -\frac{\lambda}{2\pi\varepsilon_0 R}\,\hat{y}$$

El campo eléctrico total en $C$ es:
$$\vec{E}(C) = \vec{E}_\lambda(C) + \vec{E}_q(C) = \left(-\frac{\lambda}{2\pi\varepsilon_0 R} + \frac{q}{4\pi\varepsilon_0 R^2}\right)\hat{y}$$

Para que el campo eléctrico total sea nulo, $\vec{E}(C) = \vec{0}$:
$$-\frac{\lambda}{2\pi\varepsilon_0 R} + \frac{q}{4\pi\varepsilon_0 R^2} = 0 \implies \frac{q}{4\pi\varepsilon_0 R^2} = \frac{\lambda}{2\pi\varepsilon_0 R}$$

Multiplicando a ambos lados por $4\pi\varepsilon_0 R^2$:
$$q = 2 R \lambda \iff \lambda = \frac{q}{2R}$$

$$\boxed{q = 2R\lambda}$$

**Verificación:**
- **Unidades:** $[2R\lambda] = [\text{m}] \cdot [\text{C/m}] = [\text{C}]$, dimensionalmente coincide con una carga eléctrica.
- **Signos:** Si $\lambda > 0$, la semicircunferencia repele una carga positiva de prueba en $C$ hacia abajo ($-\hat{y}$). Para contrarrestarla, la carga puntual en $A$ (ubicada en $y = -R$) debe ser positiva ($q > 0$) para repeler la prueba hacia arriba ($+\hat{y}$). Por lo tanto, $q$ y $\lambda$ deben tener el mismo signo, lo que coincide con $q = 2R\lambda > 0$.

---

## Problema 2

Considere dos cascarones esféricos de radio $a$ y $b$ ($a < b$). El cascarón interior tiene una carga uniforme distribuida ($Q$), y el exterior lo mismo pero con ($-Q$). Encuentre la diferencia de potencial entre ambos objetos.

> **[Figura]:** Dos cascarones esféricos delgados concéntricos de radios $a$ y $b$ con $a < b$, centrados en el origen. El cascarón interior de radio $a$ posee una carga neta distribuida uniformemente $+Q$. El cascarón exterior de radio $b$ posee una carga neta distribuida uniformemente $-Q$.

### Solución

**Idea:** Emplear la ley de Gauss para hallar el campo eléctrico en la región comprendida entre ambos cascarones ($a \le r < b$), y luego calcular la diferencia de potencial mediante la integral de línea del campo eléctrico: $\Delta V = V(b) - V(a) = -\int_a^b \vec{E}\cdot d\vec{l}$.

#### 1. Campo eléctrico mediante la Ley de Gauss

Por la simetría esférica de la distribución de carga, el campo eléctrico es radial en todo el espacio: $\vec{E} = E(r)\,\hat{r}$.  
Tomando una superficie gaussiana esférica de radio $r$:
$$\oint_S \vec{E}\cdot d\vec{A} = E(r) \cdot (4\pi r^2) = \frac{Q_{\text{enc}}}{\varepsilon_0}$$

Analizamos las regiones del espacio:
- **Para $r < a$:** No hay carga encerrada ($Q_{\text{enc}} = 0$), por lo tanto $E(r) = 0$.
- **Para $a \le r < b$:** La superficie gaussiana encierra únicamente la carga $+Q$ del cascarón interior:
  $$Q_{\text{enc}} = +Q \implies E(r) \cdot 4\pi r^2 = \frac{Q}{\varepsilon_0} \implies \vec{E}(r) = \frac{Q}{4\pi\varepsilon_0 r^2}\,\hat{r}$$
- **Para $r > b$:** La superficie gaussiana encierra ambos cascarones:
  $$Q_{\text{enc}} = +Q + (-Q) = 0 \implies E(r) = 0$$

---

#### 2. Cálculo de la diferencia de potencial

La diferencia de potencial entre el cascarón exterior ($r = b$) y el cascarón interior ($r = a$) se calcula integrando a lo largo de una trayectoria radial con $d\vec{l} = dr\,\hat{r}$:
$$V(b) - V(a) = -\int_a^b \vec{E}\cdot d\vec{l} = -\int_a^b \frac{Q}{4\pi\varepsilon_0 r^2}\,dr$$

$$V(b) - V(a) = -\frac{Q}{4\pi\varepsilon_0} \left[ -\frac{1}{r} \right]_a^b = \frac{Q}{4\pi\varepsilon_0} \left( \frac{1}{b} - \frac{1}{a} \right)$$

Dado que $b > a$, se tiene $\frac{1}{b} < \frac{1}{a}$, por lo que $\left(\frac{1}{b} - \frac{1}{a}\right) < 0$.  
Si se expresa como la diferencia de potencial del cascarón interior respecto al exterior:
$$V(a) - V(b) = \frac{Q}{4\pi\varepsilon_0} \left( \frac{1}{a} - \frac{1}{b} \right)$$

$$\boxed{V(b) - V(a) = \frac{Q}{4\pi\varepsilon_0}\left(\frac{1}{b} - \frac{1}{a}\right) = -\frac{Q}{4\pi\varepsilon_0}\left(\frac{1}{a} - \frac{1}{b}\right)}$$

$$\boxed{\Delta V_{a \to b} = V(a) - V(b) = \frac{Q}{4\pi\varepsilon_0}\left(\frac{1}{a} - \frac{1}{b}\right)}$$

**Verificación:**
- **Unidades:** $[Q/(4\pi\varepsilon_0 r)] = \text{C} / [(\text{C}^2/(\text{N}\cdot\text{m}^2)) \cdot \text{m}] = \text{N}\cdot\text{m}/\text{C} = \text{J}/\text{C} = \text{V}$, unidad de potencial.
- **Signo:** Como el cascarón interior está cargado positivamente ($+Q$) y el exterior negativamente ($-Q$), las líneas de campo eléctrico apuntan hacia afuera (de $a$ hacia $b$). Dado que el potencial disminuye a lo largo de las líneas de campo, se debe tener $V(a) > V(b)$, lo que hace que $V(a) - V(b) > 0$, plenamente consistente.

---

## Problema 3

Un alambre, cuya densidad lineal de carga ($\lambda$), se extiende en el eje $z$ desde $z = -d$ hasta $z = d$.

1. Calcule el potencial en un punto $z > d$ sobre el eje del alambre (eje $z$).  
2. ¿Cuál es el cambio de energía potencial de un electrón si se mueve de $z = 4d$ hacia $z = 3d$?  
3. Si el electrón parte del reposo desde $z = 4d$, ¿cuál sería su velocidad en $z = 3d$?

> **[Figura]:** Segmento de recta sobre el eje vertical $z$ de longitud total $2d$, con centro en el origen $O$, que se extiende desde $z = -d$ hasta $z = d$ portando una densidad lineal de carga uniforme $\lambda$. Sobre el mismo eje vertical, en una cota superior $z > d$, se destaca un punto de observación a lo largo del eje del alambre.

### Solución

**Idea:** Para la parte 1, integrar el potencial electrostático de una distribución lineal finita a lo largo de su eje de simetría $z$. Para la parte 2, calcular la variación de energía potencial $\Delta U = q\,\Delta V$ para la carga del electrón ($q = -e$). Para la parte 3, aplicar el teorema de conservación de la energía mecánica total $K_i + U_i = K_f + U_f$.

#### 1. Potencial en un punto $z > d$ sobre el eje

El potencial electrostático debido a una distribución lineal de carga se expresa como:
$$V(\vec{r}) = \frac{1}{4\pi\varepsilon_0}\int \frac{dq}{|\vec{r} - \vec{r}'|}$$

Para un punto sobre el eje $z$ con $z > d$:
- Posición del punto de observación: $\vec{r} = z\,\hat{z}$.
- Posición del elemento diferencial de carga: $\vec{r}' = z'\,\hat{z}$ con $z' \in [-d, d]$.
- Elemento de carga: $dq = \lambda\,dz'$.
- Distancia entre la fuente y el punto de observación: $|\vec{r} - \vec{r}'| = z - z'$ (dado que $z > d \ge z'$, la diferencia $z - z'$ es estrictamente positiva).

Sustituyendo en la integral:
$$V(z) = \frac{\lambda}{4\pi\varepsilon_0}\int_{-d}^d \frac{dz'}{z - z'}$$

Realizando el cambio de variable $u = z - z'$, con $du = -dz'$:
$$V(z) = \frac{\lambda}{4\pi\varepsilon_0} \left[ -\ln(z - z') \right]_{-d}^d = -\frac{\lambda}{4\pi\varepsilon_0} \Big( \ln(z - d) - \ln(z + d) \Big)$$

Aplicando propiedades de logaritmos:
$$\boxed{V(z) = \frac{\lambda}{4\pi\varepsilon_0}\ln\left(\frac{z + d}{z - d}\right)}$$

---

#### 2. Cambio de energía potencial del electrón de $z = 4d$ a $z = 3d$

La carga eléctrica de un electrón es $q = -e$ (con $e \approx 1{,}602 \times 10^{-19}\text{ C}$).  
El cambio de energía potencial al pasar de una posición inicial $z_i = 4d$ a una posición final $z_f = 3d$ es:
$$\Delta U = U_f - U_i = q \big( V(z_f) - V(z_i) \big) = -e \big( V(3d) - V(4d) \big)$$

Evaluamos el potencial electrostático en ambos puntos:
- En $z = 3d$:
  $$V(3d) = \frac{\lambda}{4\pi\varepsilon_0}\ln\left(\frac{3d + d}{3d - d}\right) = \frac{\lambda}{4\pi\varepsilon_0}\ln\left(\frac{4d}{2d}\right) = \frac{\lambda}{4\pi\varepsilon_0}\ln(2)$$
- En $z = 4d$:
  $$V(4d) = \frac{\lambda}{4\pi\varepsilon_0}\ln\left(\frac{4d + d}{4d - d}\right) = \frac{\lambda}{4\pi\varepsilon_0}\ln\left(\frac{5d}{3d}\right) = \frac{\lambda}{4\pi\varepsilon_0}\ln\left(\frac{5}{3}\right)$$

La diferencia de potencial $\Delta V = V(3d) - V(4d)$ resulta:
$$\Delta V = \frac{\lambda}{4\pi\varepsilon_0} \left( \ln(2) - \ln\left(\frac{5}{3}\right) \right) = \frac{\lambda}{4\pi\varepsilon_0} \ln\left(\frac{2}{5/3}\right) = \frac{\lambda}{4\pi\varepsilon_0}\ln\left(\frac{6}{5}\right)$$

Por consiguiente, el cambio de energía potencial es:
$$\Delta U = -e \cdot \frac{\lambda}{4\pi\varepsilon_0}\ln\left(\frac{6}{5}\right)$$

$$\boxed{\Delta U = -\frac{e\lambda}{4\pi\varepsilon_0}\ln\left(\frac{6}{5}\right)}$$

> **Nota:** La solución oficial manuscrita utiliza la notación $e^-$ para representar la entidad del electrón y escribe formalmente $\Delta U = e^-\left(k\lambda\ln(6/5)\right)$. Al aplicar conservación de energía en la parte siguiente, escribe explícitamente $-\Delta U = -e^- k\lambda\ln(6/5) = \frac{1}{2}m_e v_f^2$, reconociendo que al ser la carga del electrón negativa ($q = -e$), el producto resulta estrictamente positivo y la energía potencial del electrón disminuye al aproximarse a una varilla con carga positiva ($\lambda > 0$).

---

#### 3. Velocidad del electrón en $z = 3d$ partiendo del reposo en $z = 4d$

Dado que el campo electrostático es conservativo, la energía mecánica se conserva:
$$K_i + U_i = K_f + U_f$$

Como el electrón parte del reposo en $z = 4d$, $K_i = 0$:
$$0 + U_i = \frac{1}{2}m_e v_f^2 + U_f \implies \frac{1}{2}m_e v_f^2 = U_i - U_f = -\Delta U$$

Sustituyendo el valor de $-\Delta U$:
$$\frac{1}{2}m_e v_f^2 = \frac{e\lambda}{4\pi\varepsilon_0}\ln\left(\frac{6}{5}\right)$$

Despejando la velocidad final $v_f$:
$$v_f^2 = \frac{2 e \lambda}{4\pi\varepsilon_0 m_e}\ln\left(\frac{6}{5}\right) = \frac{e \lambda}{2\pi\varepsilon_0 m_e}\ln\left(\frac{6}{5}\right)$$

$$\boxed{v_f = \sqrt{\frac{e\lambda}{2\pi\varepsilon_0 m_e}\ln\left(\frac{6}{5}\right)}}$$

**Verificación:**
- **Unidades:**
  $$\left[\frac{e\lambda}{\varepsilon_0 m_e}\right] = \frac{\text{C}\cdot(\text{C/m})}{(\text{C}^2/(\text{N}\cdot\text{m}^2))\cdot\text{kg}} = \frac{\text{N}\cdot\text{m}}{\text{kg}} = \frac{\text{J}}{\text{kg}} = \frac{\text{m}^2/\text{s}^2}{1} = \text{m}^2/\text{s}^2$$
  Al aplicar la raíz cuadrada, se obtiene $\text{m/s}$, unidad correcta de rapidez.
- **Física:** Con $\lambda > 0$, la varilla positiva atrae al electrón negativo, por lo que el electrón se acelera espontáneamente hacia la varilla ($z = 4d \to z = 3d$). La energía potencial electrostática disminuye ($\Delta U < 0$) y se transforma enteramente en energía cinética ($K_f > 0$).

---

## Problema 4

Considere un plano infinito con densidad superficial uniforme positiva $\sigma$, en el cual tiene una perforación circular de radio $R$, centrado en el origen del sistema. Se define un sistema de coordenadas cartesianas con origen en el centro del orificio, tal que la distribución de carga se encuentra en el plano $YZ$. Calcule el trabajo que debe realizar un agente externo para llevar un electrón desde el centro del disco hasta un punto sobre el eje $X$ ubicado a una distancia $D$ del origen.

> **[Figura]:** Plano infinito en el plano coordenado $yz$ con una perforación circular vacía de radio $R$ concéntrica con el origen $(0,0,0)$. El plano porta una densidad superficial constante $\sigma > 0$. El eje $x$ es perpendicular al plano $yz$ y atraviesa el centro del orificio. Se muestra la trayectoria de un electrón $e^-$ que se traslada sobre el eje $x$ desde el origen $x = 0$ hasta una posición $x = D$.

### Solución

**Idea:** Por el principio de superposición, el plano perforado equivale a un plano infinito completo con densidad $\sigma$ menos un disco de radio $R$ con densidad $\sigma$: $\vec{E}_T(x) = \vec{E}_{\text{plano}}(x) - \vec{E}_{\text{disco}}(x)$. A partir de este campo eléctrico a lo largo del eje $X$, se calcula la diferencia de potencial electrostático $\Delta V = V(D) - V(0) = -\int_0^D E_T(x)\,dx$ y finalmente el trabajo del agente externo cuasiestático: $W_{\text{ext}} = \Delta U = q\,\Delta V = -e [V(D) - V(0)]$.

#### 1. Campo eléctrico del plano perforado sobre el eje $X$

Para $x > 0$:
1. **Plano infinito continuo:**
   $$E_{\text{plano}}(x) = \frac{\sigma}{2\varepsilon_0}\,\hat{x}$$
2. **Disco circular de radio $R$ con densidad uniforme $\sigma$ sobre su eje de simetría:**  
   Integrando la contribución de anillos de radio $r' \in [0, R]$:
   $$E_{\text{disco}}(x) = \frac{\sigma}{2\varepsilon_0}\left(1 - \frac{x}{\sqrt{x^2 + R^2}}\right)\hat{x}$$

Restando la contribución del orificio circular:
$$\vec{E}_T(x) = \vec{E}_{\text{plano}}(x) - \vec{E}_{\text{disco}}(x) = \left[ \frac{\sigma}{2\varepsilon_0} - \frac{\sigma}{2\varepsilon_0}\left(1 - \frac{x}{\sqrt{x^2 + R^2}}\right) \right]\hat{x}$$

$$\vec{E}_T(x) = \frac{\sigma}{2\varepsilon_0}\frac{x}{\sqrt{x^2 + R^2}}\,\hat{x}$$

*(Método alternativo directo: Integrar anillos de radio $r'$ desde el borde del orificio $r' = R$ hasta el infinito $r' \to \infty$)*:
$$E_T(x) = \frac{1}{4\pi\varepsilon_0} \int_R^\infty \frac{x\,(\sigma 2\pi r'\,dr')}{(x^2 + {r'}^2)^{3/2}} = \frac{\sigma x}{2\varepsilon_0} \left[ -\frac{1}{\sqrt{x^2 + {r'}^2}} \right]_R^\infty = \frac{\sigma}{2\varepsilon_0}\frac{x}{\sqrt{x^2 + R^2}}$$
Ambos métodos coinciden con total exactitud.

---

#### 2. Diferencia de potencial electrostático entre $x = 0$ y $x = D$

La diferencia de potencial se obtiene integrando el campo eléctrico a lo largo del eje $X$:
$$V(D) - V(0) = -\int_0^D \vec{E}_T(x)\cdot d\vec{x} = -\int_0^D \frac{\sigma}{2\varepsilon_0}\frac{x}{\sqrt{x^2 + R^2}}\,dx$$

Utilizando la sustitución inmediata $u = x^2 + R^2$, con $du = 2x\,dx$:
$$\int \frac{x}{\sqrt{x^2 + R^2}}\,dx = \sqrt{x^2 + R^2}$$

Evaluando entre los límites $0$ y $D$:
$$V(D) - V(0) = -\frac{\sigma}{2\varepsilon_0} \left[ \sqrt{x^2 + R^2} \right]_0^D = -\frac{\sigma}{2\varepsilon_0} \left( \sqrt{D^2 + R^2} - \sqrt{0^2 + R^2} \right)$$

$$V(D) - V(0) = -\frac{\sigma}{2\varepsilon_0}\left(\sqrt{D^2 + R^2} - R\right)$$

---

#### 3. Trabajo realizado por el agente externo

El trabajo realizado por una fuerza externa para trasladar una carga $q$ cuasiestáticamente (sin variación de energía cinética) es igual al cambio en su energía potencial:
$$W_{\text{ext}} = \Delta U = q \Delta V = q \big( V(D) - V(0) \big)$$

Para un electrón, $q = -e$:
$$W_{\text{ext}} = (-e) \left[ -\frac{\sigma}{2\varepsilon_0}\left(\sqrt{D^2 + R^2} - R\right) \right]$$

$$\boxed{W_{\text{ext}} = \frac{e\sigma}{2\varepsilon_0}\left(\sqrt{D^2 + R^2} - R\right)}$$

**Verificación:**
- **Signo del trabajo:** Dado que $D > 0$, tenemos $\sqrt{D^2 + R^2} > R$, por lo que la cantidad entre paréntesis es estrictamente positiva. Siendo $e > 0$ y $\sigma > 0$, el trabajo externo es positivo ($W_{\text{ext}} > 0$).  
  Físicamente esto es irreprochable: el plano posee carga positiva $\sigma > 0$ y ejerce una fuerza de atracción electrostática dirigida hacia el plano sobre el electrón (carga negativa). Para desplazarlo alejándose del plano desde $x = 0$ hasta $x = D$, el agente externo debe aplicar una fuerza paralela al desplazamiento, realizando trabajo mecánico positivo sobre el sistema.
- **Límite $D \to 0$:** Si no hay desplazamiento ($D = 0$), $W_{\text{ext}} = 0$.
- **Límite $R \to \infty$:** Si el orificio es infinitamente grande, la carga del plano se aleja al infinito y el trabajo requerido para mover el electrón se reduce a cero, ya que $\sqrt{D^2 + R^2} - R = R\left(\sqrt{1 + D^2/R^2} - 1\right) \approx \frac{D^2}{2R} \to 0$.

---

## Resumen de resultados

| Problema | Parte | Parámetro / Condición | Resultado |
| :--- | :--- | :--- | :--- |
| **Problema 1** | 1. Potencial en el centro $C$ | $V(C) = V_\lambda(C) + V_q(C)$ | $V(C) = \dfrac{1}{4\varepsilon_0}\left(\lambda + \dfrac{q}{\pi R}\right)$ |
| | 2. Dirección de $\vec{E}(C)$ | Simetría respecto al eje vertical | Puramente vertical (eje $Y$) |
| | 3. Condición para $\vec{E}(C) = \vec{0}$ | Cancelación de campos | $q = 2R\lambda \iff \lambda = \dfrac{q}{2R}$ |
| **Problema 2** | Diferencia de potencial | Entre cascarón interior $a$ y exterior $b$ | $V(b) - V(a) = \dfrac{Q}{4\pi\varepsilon_0}\left(\dfrac{1}{b} - \dfrac{1}{a}\right)$ <br> $V(a) - V(b) = \dfrac{Q}{4\pi\varepsilon_0}\left(\dfrac{1}{a} - \dfrac{1}{b}\right)$ |
| **Problema 3** | 1. Potencial en el eje | $z > d$ | $V(z) = \dfrac{\lambda}{4\pi\varepsilon_0}\ln\left(\dfrac{z + d}{z - d}\right)$ |
| | 2. Variación de energía potencial | De $z = 4d$ a $z = 3d$ ($q = -e$) | $\Delta U = -\dfrac{e\lambda}{4\pi\varepsilon_0}\ln\left(\dfrac{6}{5}\right)$ |
| | 3. Velocidad del electrón | En $z = 3d$ (desde el reposo en $4d$) | $v_f = \sqrt{\dfrac{e\lambda}{2\pi\varepsilon_0 m_e}\ln\left(\dfrac{6}{5}\right)}$ |
| **Problema 4** | Trabajo agente externo | De $x = 0$ a $x = D$ sobre el eje $X$ | $W_{\text{ext}} = \dfrac{e\sigma}{2\varepsilon_0}\left(\sqrt{D^2 + R^2} - R\right) > 0$ |
