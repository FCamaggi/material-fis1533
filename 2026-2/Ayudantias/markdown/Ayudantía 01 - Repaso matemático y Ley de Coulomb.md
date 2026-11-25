# Ayudantía 01 — Repaso matemático y Ley de Coulomb

> Clases relacionadas: [Clase 02 - Carga eléctrica, ley de Coulomb, Campo eléctrico](../../Clases/markdown/Clase%2002%20-%20Carga%20el%C3%A9ctrica%2C%20ley%20de%20Coulomb%2C%20Campo%20el%C3%A9ctrico.md), [Clase 04 - Calculo y Gauss diferencial](../../Clases/markdown/Clase%2004%20-%20Calculo%20y%20Gauss%20diferencial.md)

---

## Repaso Matemático

### Ejercicio 1

Calcule la divergencia y rotacional de los siguientes campos vectoriales:

a) $\vec{F} = x\,\hat{i} + y\,\hat{j}$  
b) $\vec{F} = -y\,\hat{i} + x\,\hat{j}$

#### Solución (propuesta, no oficial)

**Idea:** La divergencia mide la tasa neta de flujo saliente por unidad de volumen ($\nabla \cdot \vec{F}$), mientras que el rotacional mide la tendencia a inducir rotación o circulación alrededor de un punto ($\nabla \times \vec{F}$). En dos dimensiones cartesianas $(x, y)$, considerando componente $z$ nula:

$$\nabla \cdot \vec{F} = \frac{\partial F_x}{\partial x} + \frac{\partial F_y}{\partial y}$$

$$\nabla \times \vec{F} = \left( \frac{\partial F_y}{\partial x} - \frac{\partial F_x}{\partial y} \right) \hat{k}$$

---

#### Parte a) Campo $\vec{F} = x\,\hat{i} + y\,\hat{j}$

1. **Divergencia:**
   $$\nabla \cdot \vec{F} = \frac{\partial}{\partial x}(x) + \frac{\partial}{\partial y}(y) = 1 + 1 = 2$$

2. **Rotacional:**
   $$\nabla \times \vec{F} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ x & y & 0 \end{vmatrix} = \hat{k} \left( \frac{\partial y}{\partial x} - \frac{\partial x}{\partial y} \right) = \hat{k}(0 - 0) = \vec{0}$$

$$\boxed{\nabla \cdot \vec{F} = 2, \qquad \nabla \times \vec{F} = \vec{0}}$$

**Verificación:** El campo apunta radialmente hacia afuera desde el origen con magnitud proporcional a la distancia; es puramente divergente (fuente uniforme) y no tiene componente de giro angular, por lo que su rotacional es idénticamente nulo.

---

#### Parte b) Campo $\vec{F} = -y\,\hat{i} + x\,\hat{j}$

1. **Divergencia:**
   $$\nabla \cdot \vec{F} = \frac{\partial}{\partial x}(-y) + \frac{\partial}{\partial y}(x) = 0 + 0 = 0$$

2. **Rotacional:**
   $$\nabla \times \vec{F} = \hat{k} \left( \frac{\partial}{\partial x}(x) - \frac{\partial}{\partial y}(-y) \right) = \hat{k}(1 - (-1)) = 2\,\hat{k}$$

$$\boxed{\nabla \cdot \vec{F} = 0, \qquad \nabla \times \vec{F} = 2\,\hat{k}}$$

**Verificación:** Las líneas de campo forman circunferencias concéntricas en sentido antihorario. No hay flujo neto saliente de ninguna región cerrada ($\nabla \cdot \vec{F} = 0$), pero existe una vorticidad constante no nula en dirección perpendicular al plano ($+\hat{k}$).

---

### Ejercicio 2

Demuestre que el rotacional del gradiente es siempre cero. Indique qué supuesto se debe hacer para completar lo pedido.

#### Solución (propuesta, no oficial)

**Idea:** Aplicar la definición del operador rotacional sobre el campo vectorial gradiente $\nabla f$ en coordenadas cartesianas y utilizar la igualdad de derivadas cruzadas mixtas.

Sea un campo escalar $f(x, y, z)$. Su gradiente es:

$$\nabla f = \frac{\partial f}{\partial x}\,\hat{i} + \frac{\partial f}{\partial y}\,\hat{j} + \frac{\partial f}{\partial z}\,\hat{k}$$

El rotacional de este campo es:

$$\nabla \times (\nabla f) = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ \frac{\partial f}{\partial x} & \frac{\partial f}{\partial y} & \frac{\partial f}{\partial z} \end{vmatrix}$$

Desarrollando por componentes:

$$\nabla \times (\nabla f) = \left[ \frac{\partial}{\partial y}\left(\frac{\partial f}{\partial z}\right) - \frac{\partial}{\partial z}\left(\frac{\partial f}{\partial y}\right) \right]\hat{i} + \left[ \frac{\partial}{\partial z}\left(\frac{\partial f}{\partial x}\right) - \frac{\partial}{\partial x}\left(\frac{\partial f}{\partial z}\right) \right]\hat{j} + \left[ \frac{\partial}{\partial x}\left(\frac{\partial f}{\partial y}\right) - \frac{\partial}{\partial y}\left(\frac{\partial f}{\partial x}\right) \right]\hat{k}$$

$$\nabla \times (\nabla f) = \left( \frac{\partial^2 f}{\partial y \partial z} - \frac{\partial^2 f}{\partial z \partial y} \right)\hat{i} + \left( \frac{\partial^2 f}{\partial z \partial x} - \frac{\partial^2 f}{\partial x \partial z} \right)\hat{j} + \left( \frac{\partial^2 f}{\partial x \partial y} - \frac{\partial^2 f}{\partial y \partial x} \right)\hat{k}$$

Para que cada paréntesis se anule idénticamente:

$$\frac{\partial^2 f}{\partial x_i \partial x_j} = \frac{\partial^2 f}{\partial x_j \partial x_i}$$

Por el **teorema de Clairaut** (o **teorema de Schwarz**), la igualdad de derivadas parciales mixtas se cumple si y solo si las segundas derivadas parciales de la función $f$ son continuas en la región considerada (es decir, $f \in C^2$).

$$\boxed{\nabla \times (\nabla f) = \vec{0} \quad \text{bajo el supuesto de que } f \in C^2 \text{ (segundas derivadas continuas)}}$$

**Verificación:** En electrostática, el campo eléctrico se define a partir del potencial electrostático como $\vec{E} = -\nabla V$. Como consecuencia directa de esta identidad, $\nabla \times \vec{E} = -\nabla \times (\nabla V) = \vec{0}$, lo que garantiza que el campo electrostático es conservativo.

---

### Ejercicio 3

Señale la relación existente entre una integral de línea de campo vectorial y otra de campo escalar.

#### Solución (propuesta, no oficial)

**Idea:** La integral de línea de un campo vectorial calcula el trabajo o circulación a lo largo de una trayectoria orientada, mientras que la de un campo escalar integra respecto al diferencial de longitud de arco $ds = |d\vec{r}|$. Ambas se relacionan a través de la proyección del campo vectorial sobre el vector unitario tangente a la curva.

Sea una curva orientada $C$ parametrizada por $\vec{r}(t)$ para $t \in [t_0, t_1]$.
- El diferencial de desplazamiento vectorial es $d\vec{r} = \vec{r}'(t)\,dt$.
- El diferencial de longitud de arco escalar es $ds = \|d\vec{r}\| = \|\vec{r}'(t)\|\,dt$.
- El vector tangente unitario a la curva en cada punto es:
  $$\hat{T} = \frac{d\vec{r}}{ds} = \frac{\vec{r}'(t)}{\|\vec{r}'(t)\|}$$

Por lo tanto, $d\vec{r} = \hat{T}\,ds$.

Al evaluar la integral de línea del campo vectorial $\vec{F}$:

$$\int_C \vec{F} \cdot d\vec{r} = \int_C \vec{F} \cdot (\hat{T}\,ds) = \int_C (\vec{F} \cdot \hat{T})\,ds$$

Definiendo la componente tangencial escalar del campo como $\phi(\vec{r}) \equiv \vec{F}(\vec{r}) \cdot \hat{T}(\vec{r})$:

$$\boxed{\int_C \vec{F} \cdot d\vec{r} = \int_C \phi\,ds, \qquad \text{donde } \phi = \vec{F} \cdot \hat{T}}$$

La integral de línea del campo vectorial $\vec{F}$ a lo largo de una trayectoria orientada $C$ es exactamente igual a la integral de línea escalar de la componente tangencial de dicho campo ($\vec{F} \cdot \hat{T}$) a lo largo de la misma curva.

---

### Ejercicio 4

Calcule la integral de línea cerrada de la función $\vec{F} = y^2\,\hat{i} + 2x(y+1)\,\hat{j}$ según ambas trayectorias de la imagen:

> **[Figura]:** Plano cartesiano $xy$. Punto $a$ en $(1, 1)$ y punto $b$ en $(2, 2)$. La trayectoria (1) conecta $a$ con $b$ en dos etapas ortogonales: primero un segmento horizontal (i) desde $(1, 1)$ hasta $(2, 1)$, y luego un segmento vertical (ii) desde $(2, 1)$ hasta $(2, 2)$. La trayectoria (2) conecta $a$ con $b$ directamente a lo largo de la diagonal en línea recta $y = x$. La curva cerrada se forma yendo de $a$ a $b$ por la trayectoria (1) y retornando de $b$ a $a$ por la trayectoria (2).

#### Solución (propuesta, no oficial)

**Idea:** Evaluar $\int_a^b \vec{F}\cdot d\vec{r}$ a lo largo de la trayectoria (1) y a lo largo de la trayectoria (2). La integral de línea cerrada $\oint_C \vec{F}\cdot d\vec{r}$ a lo largo del circuito cerrado formado por la trayectoria (1) seguida del retorno por la trayectoria (2) en sentido horario (o antihorario) corresponde a la diferencia entre ambas integrales de línea, la cual se puede verificar mediante el teorema de Green.

El diferencial de desplazamiento es $d\vec{r} = dx\,\hat{i} + dy\,\hat{j}$, por lo que:

$$\vec{F} \cdot d\vec{r} = y^2\,dx + 2x(y+1)\,dy$$

---

#### 1. Integral a lo largo de la trayectoria (1)

La trayectoria (1) se divide en dos tramos:

- **Tramo (i) horizontal:** de $(1, 1)$ a $(2, 1)$.  
  Aquí $y = 1 \implies dy = 0$, mientras que $x$ varía de $1$ a $2$:
  $$I_{(i)} = \int_{x=1}^2 (1)^2\,dx = [x]_1^2 = 2 - 1 = 1$$

- **Tramo (ii) vertical:** de $(2, 1)$ a $(2, 2)$.  
  Aquí $x = 2 \implies dx = 0$, mientras que $y$ varía de $1$ a $2$:
  $$I_{(ii)} = \int_{y=1}^2 2(2)(y+1)\,dy = 4 \int_1^2 (y+1)\,dy = 4 \left[ \frac{y^2}{2} + y \right]_1^2 = 4 \left( (2 + 2) - \left(\frac{1}{2} + 1\right) \right) = 4(4 - 1{,}5) = 10$$

Sumando ambos tramos:
$$I_1 = I_{(i)} + I_{(ii)} = 1 + 10 = 11$$

---

#### 2. Integral a lo largo de la trayectoria (2)

La trayectoria (2) va en línea recta desde $(1, 1)$ hasta $(2, 2)$:
$$y = x \implies dy = dx, \qquad x \in [1, 2]$$

Sustituyendo $y = x$ y $dy = dx$:
$$\vec{F} \cdot d\vec{r} = x^2\,dx + 2x(x+1)\,dx = (x^2 + 2x^2 + 2x)\,dx = (3x^2 + 2x)\,dx$$

Integrando respecto a $x$ de $1$ a $2$:
$$I_2 = \int_1^2 (3x^2 + 2x)\,dx = \left[ x^3 + x^2 \right]_1^2 = (2^3 + 2^2) - (1^3 + 1^2) = (8 + 4) - (1 + 1) = 12 - 2 = 10$$

---

#### 3. Integral de línea cerrada

El circuito cerrado formado recorriendo la trayectoria (1) desde $a$ hacia $b$ y regresando por la trayectoria (2) desde $b$ hacia $a$ (circuito en sentido horario):

$$\oint_{C_{\text{horario}}} \vec{F} \cdot d\vec{r} = I_1 - I_2 = 11 - 10 = 1$$

Si se orienta en sentido antihorario estándar (de $a$ a $b$ por la trayectoria (2) y retorno por la (1)):

$$\oint_{C_{\text{antihorario}}} \vec{F} \cdot d\vec{r} = I_2 - I_1 = 10 - 11 = -1$$

$$\boxed{I_1 = 11, \qquad I_2 = 10, \qquad \oint_C \vec{F}\cdot d\vec{r} = \pm 1}$$

**Verificación por teorema de Green:**
Para el lazo en sentido horario $C_{\text{horario}} = -\partial R$:
$$\oint_C (P\,dx + Q\,dy) = -\iint_R \left( \frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y} \right) dA$$
Con $P = y^2$ y $Q = 2x(y+1)$:
$$\frac{\partial Q}{\partial x} = 2(y+1) = 2y + 2, \qquad \frac{\partial P}{\partial y} = 2y$$
$$\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y} = (2y + 2) - 2y = 2$$
La región triangular $R$ tiene base $\Delta x = 1$ y altura $\Delta y = 1$, por lo que su área es $A = \frac{1 \times 1}{2} = \frac{1}{2}$.
En sentido antihorario:
$$\oint_{C_{\text{antihorario}}} \vec{F}\cdot d\vec{r} = \iint_R 2\,dA = 2 \times \frac{1}{2} = 1 \quad (\text{o } -1 \text{ en sentido horario})$$
El resultado analítico coincide exactamente.

---

### Ejercicio 5

Compruebe el teorema fundamental para los gradientes calculando la integral de línea de $\nabla T$ con $T = xy^2$ según las siguientes trayectorias entre $a$ y $b$:

> **[Figura]:** Plano cartesiano $xy$. Punto $a$ en el origen $(0, 0)$ y punto $b$ en $(2, 1)$. La trayectoria escalonada conecta $a$ y $b$ mediante: tramo horizontal (i) sobre el eje $x$ desde $(0, 0)$ hasta $(2, 0)$, y tramo vertical (ii) desde $(2, 0)$ hasta $(2, 1)$. La trayectoria directa (iii) es el segmento recto que une $(0, 0)$ directamente con $(2, 1)$ mediante la recta $x = 2y$.

¿El resultado es el mismo independientemente del camino?

#### Solución (propuesta, no oficial)

**Idea:** El teorema fundamental del cálculo para gradientes establece que para cualquier campo escalar diferenciable $T$, la integral de línea de su gradiente entre dos puntos depende únicamente de los valores de $T$ en los extremos:

$$\int_a^b \nabla T \cdot d\vec{r} = T(b) - T(a)$$

Calculamos primero el gradiente de $T = xy^2$:

$$\nabla T = \frac{\partial T}{\partial x}\,\hat{i} + \frac{\partial T}{\partial y}\,\hat{j} = y^2\,\hat{i} + 2xy\,\hat{j}$$

El diferencial de desplazamiento es $d\vec{r} = dx\,\hat{i} + dy\,\hat{j}$, por lo que:

$$\nabla T \cdot d\vec{r} = y^2\,dx + 2xy\,dy$$

Los extremos son $a = (0, 0)$ y $b = (2, 1)$. El valor teórico esperado según el teorema fundamental es:

$$T(b) - T(a) = T(2, 1) - T(0, 0) = (2)(1)^2 - (0)(0)^2 = 2 - 0 = 2$$

---

#### 1. Cálculo a lo largo de la trayectoria por tramos (i) + (ii)

- **Tramo (i):** desde $(0, 0)$ hasta $(2, 0)$ sobre el eje $x$.  
  $y = 0 \implies dy = 0$, $x \in [0, 2]$:
  $$I_{(i)} = \int_0^2 (0)^2\,dx = 0$$

- **Tramo (ii):** desde $(2, 0)$ hasta $(2, 1)$ verticalmente.  
  $x = 2 \implies dx = 0$, $y \in [0, 1]$:
  $$I_{(ii)} = \int_0^1 2(2)y\,dy = 4 \int_0^1 y\,dy = 4 \left[ \frac{y^2}{2} \right]_0^1 = 4\left(\frac{1}{2}\right) = 2$$

Sumando ambos tramos:
$$I_{(i)+(ii)} = 0 + 2 = 2$$

---

#### 2. Cálculo a lo largo de la trayectoria recta (iii)

La recta que une $(0, 0)$ con $(2, 1)$ tiene ecuación:
$$x = 2y \implies dx = 2\,dy, \qquad y \in [0, 1]$$

Sustituyendo $x$ y $dx$:
$$\nabla T \cdot d\vec{r} = y^2 (2\,dy) + 2(2y)y\,dy = 2y^2\,dy + 4y^2\,dy = 6y^2\,dy$$

Integrando respecto a $y$ de $0$ a $1$:
$$I_{(iii)} = \int_0^1 6y^2\,dy = \left[ 2y^3 \right]_0^1 = 2(1)^3 - 0 = 2$$

---

#### 3. Conclusión

$$\boxed{\int_a^b \nabla T \cdot d\vec{r} = 2 \quad \text{en ambas trayectorias}}$$

**¿El resultado es el mismo independientemente del camino?**  
**Sí**, el resultado es idéntico en cualquier trayectoria que una los puntos $a$ y $b$. Esto se debe a que $\nabla T$ es un campo conservativo ($\nabla \times (\nabla T) = \vec{0}$), lo que asegura que la integral de línea sea completamente independiente del camino y quede determinada únicamente por la diferencia de potencial $T(b) - T(a) = 2$.

---

## Problema 1

Dos pequeñas esferas de igual masa $m$ y carga $q > 0$, cuelgan por 2 hilos sin masa, sin carga y de largo $l$. Cada esfera forma un ángulo $\theta$ con el eje vertical, como se muestra en la figura. Calcule el valor de la carga $q$ para el equilibrio estático del problema.

> **[Figura]:** Dos hilos de longitud $l$ parten de un mismo punto en un techo horizontal. Cada hilo sostiene una pequeña esfera de masa $m$ y carga positiva $q > 0$. Cada hilo se desvía un ángulo $\theta$ respecto a la vertical punteada central. La distancia horizontal total entre los centros de las dos esferas es $r$. En el diagrama de cuerpo libre (DCL) de la esfera derecha actúan tres fuerzas: la tensión $\vec{T}$ dirigida a lo largo del hilo hacia el punto de suspensión (formando un ángulo $\theta$ con la vertical), la fuerza electrostática de repulsión $\vec{F}_e$ en dirección horizontal hacia la derecha ($+\hat{i}$), y el peso $\vec{F}_p = m\vec{g}$ hacia abajo ($-\hat{j}$).

### Solución

**Idea:** Plantear la condición de equilibrio estático ($\sum \vec{F} = \vec{0}$) para una de las esferas mediante un diagrama de cuerpo libre (DCL), descomponiendo la tensión en sus componentes horizontal y vertical, y relacionando la fuerza electrostática de repulsión de Coulomb con la separación geométrica $r = 2l\sin\theta$.

#### 1. Geometría del sistema

Por simetría, la recta vertical que pasa por el punto de suspensión divide el sistema en dos triángulos rectángulos congruentes. Para cada esfera:
- El cateto opuesto al ángulo vertical $\theta$ es la mitad de la separación: $\frac{r}{2} = l\sin\theta$.
- Por lo tanto, la distancia de separación entre ambas cargas es:
  $$r = 2l\sin\theta$$

#### 2. Diagrama de cuerpo libre y equilibrio estático

Analizamos la esfera ubicada a la derecha:
- Fuerzas presentes:
  - Tensión del hilo: $\vec{T} = -T\sin\theta\,\hat{i} + T\cos\theta\,\hat{j}$
  - Fuerza gravitatoria (peso): $\vec{F}_p = -mg\,\hat{j}$
  - Fuerza electrostática de Coulomb (repulsiva): $\vec{F}_e = F_e\,\hat{i}$

Para equilibrio estático:
$$\sum \vec{F} = \begin{pmatrix} -T\sin\theta + F_e \\ T\cos\theta - mg \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}$$

1. **Equilibrio vertical ($\hat{j}$):**
   $$T\cos\theta - mg = 0 \implies T = \frac{mg}{\cos\theta}$$

2. **Equilibrio horizontal ($\hat{i}$):**
   $$-T\sin\theta + F_e = 0 \implies F_e = T\sin\theta$$

Sustituyendo la tensión $T$:
$$F_e = \left(\frac{mg}{\cos\theta}\right)\sin\theta = mg\tan\theta$$

#### 3. Determinación de la carga $q$

Por la ley de Coulomb ($k = \frac{1}{4\pi\varepsilon_0}$):
$$F_e = \frac{1}{4\pi\varepsilon_0}\frac{q^2}{r^2}$$

Igualando las dos expresiones para $F_e$:
$$\frac{1}{4\pi\varepsilon_0}\frac{q^2}{r^2} = mg\tan\theta$$

Despejando $q^2$:
$$q^2 = 4\pi\varepsilon_0\,r^2\,mg\tan\theta$$

Extrayendo raíz cuadrada (dado que el enunciado especifica $q > 0$):
$$q = \sqrt{4\pi\varepsilon_0\,r^2\,mg\tan\theta} = 2r\sqrt{\pi\varepsilon_0\,mg\tan\theta}$$

Sustituyendo la expresión geométrica $r = 2l\sin\theta$:
$$q = 2(2l\sin\theta)\sqrt{\pi\varepsilon_0\,mg\tan\theta} = 4l\sin\theta\sqrt{\pi\varepsilon_0\,mg\tan\theta}$$

$$\boxed{q = 4l\sin\theta\sqrt{\pi\varepsilon_0\,mg\tan\theta}}$$

**Verificación:**
- **Unidades:**
  $$\left[ \text{m} \cdot \sqrt{\left(\frac{\text{C}^2}{\text{N}\cdot\text{m}^2}\right)(\text{kg})\left(\frac{\text{m}}{\text{s}^2}\right)} \right] = \left[ \text{m} \cdot \sqrt{\frac{\text{C}^2}{\text{N}\cdot\text{m}^2}\cdot\text{N}} \right] = \left[ \text{m} \cdot \frac{\text{C}}{\text{m}} \right] = [\text{C}]$$
  La expresión es dimensionalmente homogénea.
- **Límite $\theta \to 0$:** Si $\theta \to 0$, $q \to 0$; sin carga no hay fuerza eléctrica repulsiva y las esferas cuelgan verticalmente juntas.
- **Límite $\theta \to \pi/2$:** A medida que $\theta \to 90^\circ$, $\tan\theta \to \infty$, requiriendo una carga infinitamente grande para mantener las cuerdas perfectamente horizontales frente a la gravedad.

---

## Problema 2

En los vértices de un triángulo equilátero de lado $L$ se han situado tres cargas negativas $-e$. Si en el centro de gravedad del triángulo se sitúa una carga de magnitud $Q$, determine el valor que debe poseer esa carga para mantener el sistema en equilibrio.

> **[Figura]:** Triángulo equilátero de lado $L$. En cada uno de sus tres vértices hay una carga negativa $-e$. En el baricentro (centro de gravedad) se ubica una carga $Q$. Sobre la carga del vértice superior actúan: dos fuerzas repulsivas $\vec{F}_1$ y $\vec{F}_2$ debidas a las otras dos cargas negativas en los vértices inferiores, dirigidas hacia arriba formando un ángulo de $30^\circ$ con la vertical ($60^\circ$ con la horizontal), y una fuerza $\vec{F}_3$ debida a la carga central $Q$. Para el equilibrio, la fuerza $\vec{F}_3$ debe ser atractiva, dirigida verticalmente hacia abajo ($-\hat{j}$), lo que requiere $Q > 0$.

### Solución

**Idea:** Por simetría trigonométrica de un triángulo equilátero, la fuerza sobre la carga central $Q$ es nula independientemente del valor de $Q$. Para que todo el sistema esté en equilibrio mecánico, la fuerza neta sobre cualquiera de las tres cargas en los vértices debe ser cero. Aplicamos la ley de Coulomb sobre la carga del vértice superior y proyectamos en los ejes cartesiano horizontal ($X$) y vertical ($Y$).

#### 1. Geometría del triángulo equilátero

Sea un triángulo equilátero de lado $L$:
- La altura total del triángulo equilátero es:
  $$h = \sqrt{L^2 - \left(\frac{L}{2}\right)^2} = \frac{L\sqrt{3}}{2}$$
- El baricentro (centro de gravedad) divide la altura en razón $2:1$, ubicándose a una distancia $r$ desde cada vértice:
  $$r = \frac{2}{3}h = \frac{2}{3}\left(\frac{L\sqrt{3}}{2}\right) = \frac{L\sqrt{3}}{3} = \frac{L}{\sqrt{3}}$$
- El cuadrado de esta distancia es:
  $$r^2 = \frac{L^2}{3}$$

#### 2. Fuerzas sobre la carga del vértice superior

Ubicamos el origen de coordenadas en el vértice superior:
- El eje $Y$ apunta hacia arriba ($+\hat{j}$); por ende, el centro del triángulo está en dirección $-\hat{j}$.
- Los dos vértices inferiores se encuentran a los lados izquierdo y derecho, formando un ángulo interior de $60^\circ$ en el vértice superior. La vertical es la bisectriz de este ángulo, por lo que cada lado forma un ángulo de $30^\circ$ con el eje vertical (o $60^\circ$ respecto al eje horizontal).

Las fuerzas que actúan sobre la carga $-e$ del vértice superior son:
1. **Fuerza repulsiva $\vec{F}_1$ debida al vértice inferior izquierdo:**
   $$\vec{F}_1 = \frac{e^2}{4\pi\varepsilon_0 L^2} \left( -\cos(60^\circ)\,\hat{i} + \sin(60^\circ)\,\hat{j} \right)$$
2. **Fuerza repulsiva $\vec{F}_2$ debida al vértice inferior derecho:**
   $$\vec{F}_2 = \frac{e^2}{4\pi\varepsilon_0 L^2} \left( \cos(60^\circ)\,\hat{i} + \sin(60^\circ)\,\hat{j} \right)$$
3. **Fuerza $\vec{F}_3$ debida a la carga central $Q$:**
   Para compensar la fuerza resultante hacia arriba debida a la repulsión mutua de las cargas negativas, la carga $Q$ debe atraer a la carga $-e$, es decir, debe apuntar hacia el centro ($-\hat{j}$). Siendo $-e < 0$, esto exige que **$Q > 0$**:
   $$\vec{F}_3 = -\frac{e Q}{4\pi\varepsilon_0 r^2}\,\hat{j}$$

Sustituyendo $r^2 = \frac{L^2}{3}$:
$$\vec{F}_3 = -\frac{3 e Q}{4\pi\varepsilon_0 L^2}\,\hat{j}$$

#### 3. Condición de equilibrio

1. **Eje $X$:**
   $$\sum F_x = F_{1x} + F_{2x} = \frac{e^2}{4\pi\varepsilon_0 L^2}(-\cos(60^\circ) + \cos(60^\circ)) = 0$$
   Se anulan exactamente por simetría bilateral.

2. **Eje $Y$:**
   $$\sum F_y = 2 \left( \frac{e^2}{4\pi\varepsilon_0 L^2} \sin(60^\circ) \right) - \frac{3 e Q}{4\pi\varepsilon_0 L^2} = 0$$

Multiplicando toda la ecuación por $\frac{4\pi\varepsilon_0 L^2}{e}$:
$$2 e \sin(60^\circ) - 3Q = 0$$

Recordando que $\sin(60^\circ) = \frac{\sqrt{3}}{2}$:
$$2 e \left(\frac{\sqrt{3}}{2}\right) - 3Q = 0 \implies e\sqrt{3} - 3Q = 0$$

Despejando $Q$:
$$Q = \frac{e\sqrt{3}}{3} = \frac{e}{\sqrt{3}}$$

$$\boxed{Q = +\frac{e}{\sqrt{3}} = +\frac{e\sqrt{3}}{3}}$$

**Verificación:**
- **Signo:** Las cargas de los vértices se repelen con una fuerza neta radial hacia afuera de magnitud $\sqrt{3}\frac{e^2}{4\pi\varepsilon_0 L^2}$. La carga central debe ser positiva ($Q > 0$) para tirar hacia el centro con exactamente la misma magnitud.
- **Equilibrio de las demás cargas:** Por rotación de $120^\circ$ y $240^\circ$, la misma condición se satisface simultáneamente en los tres vértices. La carga central siente tres fuerzas de igual magnitud espaciadas a $120^\circ$, cuya suma vectorial es idénticamente cero. Todo el sistema está en equilibrio.

---

## Problema 3

Encuentre la magnitud y dirección del campo eléctrico en el punto $P$, que se encuentra a una distancia $z$ sobre el punto medio de dos cargas puntuales con valor $+q$, ubicadas a una distancia $d$ la una de la otra.

> **[Figura]:** Eje horizontal que une dos cargas idénticas $+q$, separadas por una distancia total $d$. El origen de coordenadas se sitúa en el punto medio entre ambas cargas, de modo que las posiciones de las cargas son $(-d/2, 0)$ y $(+d/2, 0)$. El punto $P$ se ubica sobre el eje perpendicular vertical a una altura $z$, en las coordenadas $(0, z)$. Los vectores de campo eléctrico $\vec{E}_1$ y $\vec{E}_2$ debidos a cada carga apuntan saliendo desde cada carga positiva en dirección a $P$, formando un ángulo $\phi$ con la horizontal. Las componentes horizontales se cancelan mutuamente, mientras que las componentes verticales se suman apuntando verticalmente hacia arriba ($+\hat{j}$ o $+\hat{z}$).

### Solución

**Idea:** Aplicar el principio de superposición para campos electrostáticos: $\vec{E}_{\text{total}} = \vec{E}_1 + \vec{E}_2$. Por simetría geométrica respecto al eje perpendicular medio, las componentes horizontales del campo generadas por cargas iguales se anulan entre sí, sumándose únicamente las componentes verticales.

#### 1. Geometría y distancias

Ubicamos el sistema en el plano cartesiano con:
- Carga 1 en $\vec{r}_1 = \left(-\frac{d}{2},\, 0\right)$
- Carga 2 en $\vec{r}_2 = \left(+\frac{d}{2},\, 0\right)$
- Punto de observación $P$ en $\vec{r} = (0,\, z)$

La distancia $r$ desde cualquiera de las cargas al punto $P$ es:
$$r = \sqrt{\left(\frac{d}{2}\right)^2 + z^2} = \sqrt{\frac{d^2}{4} + z^2}$$

El seno del ángulo $\phi$ que forma la línea de unión con el eje horizontal es:
$$\sin\phi = \frac{z}{r} = \frac{z}{\sqrt{\frac{d^2}{4} + z^2}}$$

El coseno del ángulo es:
$$\cos\phi = \frac{d/2}{r} = \frac{d}{2\sqrt{\frac{d^2}{4} + z^2}}$$

#### 2. Campos individuales

Por la ley de Coulomb para el campo eléctrico ($k = \frac{1}{4\pi\varepsilon_0}$):
$$\|\vec{E}_1\| = \|\vec{E}_2\| = \frac{1}{4\pi\varepsilon_0}\frac{q}{r^2} = \frac{q}{4\pi\varepsilon_0 \left(\frac{d^2}{4} + z^2\right)}$$

Descomponiendo vectorialmente:
$$\vec{E}_1 = \|\vec{E}_1\|\cos\phi\,\hat{i} + \|\vec{E}_1\|\sin\phi\,\hat{j}$$
$$\vec{E}_2 = -\|\vec{E}_2\|\cos\phi\,\hat{i} + \|\vec{E}_2\|\sin\phi\,\hat{j}$$

#### 3. Superposición y campo total

Sumando vectorialmente ambos campos:
$$\vec{E}_{\text{total}} = \vec{E}_1 + \vec{E}_2 = 2\,\|\vec{E}_1\|\sin\phi\,\hat{j}$$

Sustituyendo $\|\vec{E}_1\|$ y $\sin\phi$:
$$\vec{E}_{\text{total}} = 2 \left( \frac{q}{4\pi\varepsilon_0 \left(\frac{d^2}{4} + z^2\right)} \right) \left( \frac{z}{\sqrt{\frac{d^2}{4} + z^2}} \right)\hat{j}$$

Simplificando los factores numéricos:
$$\vec{E}_{\text{total}} = \frac{q z}{2\pi\varepsilon_0 \left(\frac{d^2}{4} + z^2\right)^{3/2}}\,\hat{j}$$

$$\boxed{\vec{E}(0, z) = \frac{q z}{2\pi\varepsilon_0 \left(\frac{d^2}{4} + z^2\right)^{3/2}}\,\hat{j}}$$

**Verificación:**
- **Límite $z = 0$ (punto medio entre las cargas):** $\vec{E}(0, 0) = \vec{0}$, coherente con el hecho de que en el punto medio exacto dos cargas idénticas se repelen con campos opuestos que se anulan.
- **Límite $z \gg d$ (distancias muy lejanas):**
  $$\left(\frac{d^2}{4} + z^2\right)^{3/2} \approx z^3 \implies \vec{E} \approx \frac{q z}{2\pi\varepsilon_0 z^3}\,\hat{j} = \frac{2q}{4\pi\varepsilon_0 z^2}\,\hat{j}$$
  El sistema se comporta a grandes distancias como una única carga puntual de valor total $Q_{\text{total}} = 2q$.
- **Unidades:**
  $$\left[ \frac{\text{C}\cdot\text{m}}{\left(\frac{\text{C}^2}{\text{N}\cdot\text{m}^2}\right)\text{m}^3} \right] = \left[ \frac{\text{C}\cdot\text{m}\cdot\text{N}\cdot\text{m}^2}{\text{C}^2\cdot\text{m}^3} \right] = [\text{N/C}]$$
  Dimensionalmente correcto.

---

## Resumen de resultados

| Problema / Ejercicio | Parámetro / Pregunta | Resultado Final |
| :--- | :--- | :--- |
| **Repaso Mat. 1a** | Divergencia y rotacional de $\vec{F} = x\hat{i} + y\hat{j}$ | $\nabla \cdot \vec{F} = 2, \quad \nabla \times \vec{F} = \vec{0}$ |
| **Repaso Mat. 1b** | Divergencia y rotacional de $\vec{F} = -y\hat{i} + x\hat{j}$ | $\nabla \cdot \vec{F} = 0, \quad \nabla \times \vec{F} = 2\hat{k}$ |
| **Repaso Mat. 2** | Identidad y supuesto para $\nabla \times (\nabla f) = \vec{0}$ | $\nabla \times (\nabla f) = \vec{0}$, requiere $f \in C^2$ (teorema de Clairaut/Schwarz) |
| **Repaso Mat. 3** | Relación integral vectorial vs escalar | $\int_C \vec{F}\cdot d\vec{r} = \int_C (\vec{F}\cdot\hat{T})\,ds$ |
| **Repaso Mat. 4** | Integrales de línea y circulación de $\vec{F} = y^2\hat{i} + 2x(y+1)\hat{j}$ | $I_1 = 11, \quad I_2 = 10, \quad \oint_C \vec{F}\cdot d\vec{r} = \pm 1$ |
| **Repaso Mat. 5** | Teorema fundamental del gradiente con $T = xy^2$ | $I = 2$ en ambos caminos; independiente de la trayectoria |
| **Problema 1** | Carga $q$ para equilibrio de esferas suspendidas | $q = 4l\sin\theta\sqrt{\pi\varepsilon_0 mg\tan\theta}$ |
| **Problema 2** | Carga central $Q$ en triángulo equilátero | $Q = +\frac{e\sqrt{3}}{3} = +\frac{e}{\sqrt{3}}$ |
| **Problema 3** | Campo eléctrico en $P(0, z)$ de dos cargas $+q$ | $\vec{E} = \frac{q z}{2\pi\varepsilon_0 \left(\frac{d^2}{4} + z^2\right)^{3/2}}\,\hat{j}$ |
