# Herramientas de cálculo vectorial y ley de Gauss en forma diferencial

*FIS1533 — Electricidad y Magnetismo.*

En la Clase 03 se enunció la ley de Gauss en forma **integral**, que relaciona el flujo a través de una superficie cerrada con la carga encerrada. En esta clase se introducen los operadores del cálculo vectorial (gradiente, divergencia y rotor) y los teoremas integrales (de la divergencia y de Stokes) que permiten escribir la ley de Gauss en forma **diferencial** (local), válida punto a punto: la primera ecuación de Maxwell.

---

## 1. Gradiente

### 1.1 Motivación: ¿cómo determinamos la pendiente?

> **[Figura]:** (1) Gráfico 3D de una superficie $z=F(x,y)$ con forma de paraboloide ("cuenco") sobre el dominio $-1\le x\le1$, $-1\le y\le1$: mínimo $z=0$ en el origen y $z\approx2$ en las esquinas, compatible con $F(x,y)=x^2+y^2$. (2) Corte de una superficie de este tipo en el plano $xz$: parábola simétrica con mínimo $z=10$ en $x=0$ que sube hasta $z\approx70$ en $x\approx\pm7{,}5$. (3) Corte en el plano $yz$: la misma parábola en función de $y$, con mínimo $z=10$ en $y=0$.

Para una función de una variable, la pendiente es la derivada $df/dx$. Para una función de varias variables $F(x,y,z)$, la pendiente depende de la dirección en que nos movemos. Cada corte (manteniendo fija una variable) da una curva cuya pendiente es la **derivada parcial**: $\partial F/\partial x$ en el corte $xz$, $\partial F/\partial y$ en el corte $yz$. Estas pendientes se agrupan en un vector: el gradiente.

### 1.2 Definición

El gradiente de una función escalar $F(x,y,z)$ es

$$\vec{\nabla}F=\frac{\partial F}{\partial x}\hat{i}+\frac{\partial F}{\partial y}\hat{j}+\frac{\partial F}{\partial z}\hat{k}$$

Se puede definir el operador vectorial **nabla**:

$$\vec{\nabla}=\frac{\partial}{\partial x}\hat{i}+\frac{\partial}{\partial y}\hat{j}+\frac{\partial}{\partial z}\hat{k}$$

**Propiedades:**
- $\vec\nabla F$ apunta en la dirección de **máximo crecimiento** de $F$, y su módulo es la pendiente máxima.
- La variación de $F$ al desplazarse $d\vec r$ es $dF=\vec\nabla F\cdot d\vec r$. La derivada direccional según el unitario $\hat u$ es $\vec\nabla F\cdot\hat u$.
- $\vec\nabla F$ es perpendicular a las superficies (o curvas) de nivel $F=\text{cte}$.

> **[Figura]:** Campo vectorial en el plano $xy$ ($-4\le x,y\le4$): flechas que apuntan radialmente hacia fuera desde el origen, con longitud que crece proporcionalmente a la distancia al origen (casi nulas cerca de $(0,0)$, largas en las esquinas). Corresponde al campo $\vec F=x\,\hat i+y\,\hat j$.

**Ejemplo ilustrativo (gradiente del paraboloide).** Para $F(x,y)=x^2+y^2$:
$$\vec\nabla F=2x\,\hat i+2y\,\hat j=2\,(x\,\hat i+y\,\hat j)$$
Es un campo radial hacia fuera, cuyo módulo $2\sqrt{x^2+y^2}$ crece con la distancia: exactamente el patrón de la figura (salvo un factor de escala). En el origen (mínimo del cuenco) el gradiente es nulo, y apunta "cuesta arriba" en todas partes. En el corte $y=0$, $\partial F/\partial x=2x$ es la pendiente de la parábola $z=x^2$.

*Conexión con el curso:* en la Clase 05 se verá que el campo electrostático es el gradiente (con signo menos) de un escalar, el potencial: $\vec E=-\vec\nabla V$.

---

## 2. Divergencia y rotacional

Aplicando el operador $\vec\nabla$ a un campo vectorial $\vec F=F_x\hat i+F_y\hat j+F_z\hat k$ se obtienen dos operaciones.

### 2.1 Divergencia (producto punto)

$$\vec{\nabla}\cdot\vec{F}=\frac{\partial F_x}{\partial x}+\frac{\partial F_y}{\partial y}+\frac{\partial F_z}{\partial z}$$

Es un **escalar** que indica el cambio de flujo en un volumen de control: es el flujo neto saliente por unidad de volumen en el límite de un volumen infinitesimal,
$$\vec\nabla\cdot\vec F=\lim_{\Delta V\to0}\frac{1}{\Delta V}\oint_{\partial(\Delta V)}\vec F\cdot d\vec A$$
- $\vec\nabla\cdot\vec F>0$: el punto actúa como **fuente** (las líneas nacen).
- $\vec\nabla\cdot\vec F<0$: **sumidero** (las líneas mueren).
- $\vec\nabla\cdot\vec F=0$: lo que entra sale.

*Ejemplo:* el campo de la figura, $\vec F=x\hat i+y\hat j$, tiene $\vec\nabla\cdot\vec F=1+1=2>0$: hay "fuentes" distribuidas uniformemente en todo el plano, por eso las flechas crecen al alejarse.

### 2.2 Rotacional (producto cruz)

$$\vec{\nabla}\times\vec{F}=\begin{vmatrix}\hat i&\hat j&\hat k\\ \partial_x&\partial_y&\partial_z\\ F_x&F_y&F_z\end{vmatrix}=\left(\frac{\partial F_z}{\partial y}-\frac{\partial F_y}{\partial z}\right)\hat{i}+\left(\frac{\partial F_x}{\partial z}-\frac{\partial F_z}{\partial x}\right)\hat{j}+\left(\frac{\partial F_y}{\partial x}-\frac{\partial F_x}{\partial y}\right)\hat{k}$$

Es un **vector** que muestra la tendencia de un campo vectorial a inducir rotación alrededor de un punto (piense en una pequeña rueda con aspas colocada en el campo). Es la circulación por unidad de área:
$$(\vec\nabla\times\vec F)\cdot\hat n=\lim_{\Delta A\to0}\frac{1}{\Delta A}\oint_{\partial(\Delta A)}\vec F\cdot d\vec\ell$$

*Ejemplos:* $\vec F=x\hat i+y\hat j$ tiene rotor nulo (es radial, no gira). En cambio $\vec G=-y\hat i+x\hat j$ (remolino) tiene $\vec\nabla\times\vec G=(1-(-1))\hat k=2\hat k$ y divergencia nula.

### 2.3 Identidades útiles

- $\vec\nabla\times(\vec\nabla F)=0$: el rotor de un gradiente es siempre cero.
- $\vec\nabla\cdot(\vec\nabla\times\vec F)=0$: la divergencia de un rotor es siempre cero.
- $\vec\nabla\cdot(\vec\nabla F)=\nabla^2F=\dfrac{\partial^2F}{\partial x^2}+\dfrac{\partial^2F}{\partial y^2}+\dfrac{\partial^2F}{\partial z^2}$ (laplaciano).

---

## 3. Teoremas integrales

### 3.1 Teorema de la divergencia (de Gauss)

Sea $\Omega$ una región del espacio con frontera cerrada $\partial\Omega$ (normal hacia fuera). Sea $\vec F$ un campo vectorial continuo y diferenciable en $\Omega$. Entonces,

$$\iiint_\Omega(\vec{\nabla}\cdot\vec{F})\,dV=\oiint_{\partial\Omega}\vec{F}\cdot d\vec{S}$$

*Interpretación:* la suma de todas las "fuentes" dentro del volumen es igual al flujo neto que sale por su frontera. Convierte una integral de superficie en una de volumen (y viceversa).

### 3.2 Teorema de Stokes (complemento)

Sea $S$ una superficie abierta con borde $C=\partial S$, orientado según la regla de la mano derecha respecto de la normal de $S$. Entonces

$$\iint_S(\vec\nabla\times\vec F)\cdot d\vec S=\oint_C\vec F\cdot d\vec\ell$$

*Interpretación:* la suma de las "rotaciones microscópicas" sobre la superficie es igual a la circulación del campo a lo largo del borde. Se usará con la ley de Ampère (Clase 12) y la ley de Faraday (Clase 13).

---

## 4. Coordenadas cilíndricas y esféricas (complemento)

Las distribuciones con simetría cilíndrica o esférica (Clase 03) se describen mejor en estas coordenadas.

### 4.1 Coordenadas cilíndricas $(r,\phi,z)$

$x=r\cos\phi$, $y=r\sin\phi$, $z=z$. Elemento de volumen: $dV=r\,dr\,d\phi\,dz$. Elemento de área del manto (radio $r$): $dA=r\,d\phi\,dz$.

$$\vec\nabla F=\frac{\partial F}{\partial r}\hat r+\frac1r\frac{\partial F}{\partial\phi}\hat\phi+\frac{\partial F}{\partial z}\hat z$$
$$\vec\nabla\cdot\vec F=\frac1r\frac{\partial(rF_r)}{\partial r}+\frac1r\frac{\partial F_\phi}{\partial\phi}+\frac{\partial F_z}{\partial z}$$
$$\vec\nabla\times\vec F=\left(\frac1r\frac{\partial F_z}{\partial\phi}-\frac{\partial F_\phi}{\partial z}\right)\hat r+\left(\frac{\partial F_r}{\partial z}-\frac{\partial F_z}{\partial r}\right)\hat\phi+\frac1r\left(\frac{\partial(rF_\phi)}{\partial r}-\frac{\partial F_r}{\partial\phi}\right)\hat z$$

### 4.2 Coordenadas esféricas $(r,\theta,\phi)$

$x=r\sin\theta\cos\phi$, $y=r\sin\theta\sin\phi$, $z=r\cos\theta$ ($\theta$: ángulo polar desde $+z$; $\phi$: azimutal). Elemento de volumen: $dV=r^2\sin\theta\,dr\,d\theta\,d\phi$. Elemento de área de una esfera de radio $r$: $dA=r^2\sin\theta\,d\theta\,d\phi$ (integrando, $4\pi r^2$).

$$\vec\nabla F=\frac{\partial F}{\partial r}\hat r+\frac1r\frac{\partial F}{\partial\theta}\hat\theta+\frac{1}{r\sin\theta}\frac{\partial F}{\partial\phi}\hat\phi$$
$$\vec\nabla\cdot\vec F=\frac{1}{r^2}\frac{\partial(r^2F_r)}{\partial r}+\frac{1}{r\sin\theta}\frac{\partial(\sin\theta\,F_\theta)}{\partial\theta}+\frac{1}{r\sin\theta}\frac{\partial F_\phi}{\partial\phi}$$
$$\vec\nabla\times\vec F=\frac{1}{r\sin\theta}\left[\frac{\partial(\sin\theta F_\phi)}{\partial\theta}-\frac{\partial F_\theta}{\partial\phi}\right]\hat r+\frac1r\left[\frac{1}{\sin\theta}\frac{\partial F_r}{\partial\phi}-\frac{\partial(rF_\phi)}{\partial r}\right]\hat\theta+\frac1r\left[\frac{\partial(rF_\theta)}{\partial r}-\frac{\partial F_r}{\partial\theta}\right]\hat\phi$$

Para un campo puramente radial que sólo depende de $r$, $\vec F=F_r(r)\hat r$, todo se reduce a:
- Esféricas: $\vec\nabla\cdot\vec F=\dfrac{1}{r^2}\dfrac{d(r^2F_r)}{dr}$, $\ \vec\nabla\times\vec F=0$.
- Cilíndricas: $\vec\nabla\cdot\vec F=\dfrac1r\dfrac{d(rF_r)}{dr}$, $\ \vec\nabla\times\vec F=0$.

---

## 5. Ley de Gauss en forma diferencial

Forma integral (Clase 03), escribiendo la carga encerrada como integral de la densidad:

$$\oiint\vec{E}\cdot d\vec{A}=\frac{q_{\text{enc}}}{\varepsilon_0}\quad\leftrightarrow\quad\oiint\vec{E}\cdot d\vec{A}=\frac{1}{\varepsilon_0}\iiint\rho\,dV$$

Al aplicar el teorema de la divergencia en el flujo:

$$\iiint(\vec{\nabla}\cdot\vec{E})\,dV=\frac{1}{\varepsilon_0}\iiint\rho\,dV\quad\Longrightarrow\quad\iiint\left(\vec\nabla\cdot\vec E-\frac{\rho}{\varepsilon_0}\right)dV=0$$

Como esto vale para **cualquier** volumen (por pequeño que sea y donde sea), el integrando debe anularse en cada punto:

$$\boxed{\vec{\nabla}\cdot\vec{E}=\frac{\rho}{\varepsilon_0}}$$

**Ley de Gauss en forma diferencial — Primera ecuación de Maxwell.**

*Interpretación:* las cargas positivas son fuentes de líneas de campo eléctrico y las negativas son sumideros. Donde no hay carga ($\rho=0$), la divergencia de $\vec E$ es nula, aunque $\vec E$ no lo sea. La forma diferencial permite el camino inverso al de la Clase 03: **conocido $\vec E$, se obtiene $\rho$ derivando**.

## 6. El campo electrostático es irrotacional: $\vec\nabla\times\vec E=0$

Para una carga puntual, $\vec E=\dfrac{kq}{r^2}\hat r$ es radial y sólo depende de $r$; por la sección 4.2 su rotor es nulo. Por superposición, el campo de **cualquier** distribución estática de cargas cumple

$$\boxed{\vec\nabla\times\vec E=0\quad\text{(electrostática)}}$$

Por el teorema de Stokes, esto equivale a que la circulación sea nula a lo largo de cualquier curva cerrada:
$$\oint_C\vec E\cdot d\vec\ell=0$$
Es decir, el trabajo que hace el campo electrostático sobre una carga que recorre una trayectoria cerrada es cero: **el campo electrostático es conservativo**. Como $\vec\nabla\times(\vec\nabla V)=0$, existe una función escalar $V$ tal que $\vec E=-\vec\nabla V$ (potencial eléctrico, Clase 05). Esta propiedad deja de cumplirse cuando hay campos magnéticos variables en el tiempo (ley de Faraday, Clase 13: $\vec\nabla\times\vec E=-\partial\vec B/\partial t$).

**Ecuaciones de la electrostática en forma diferencial:**
$$\vec\nabla\cdot\vec E=\frac{\rho}{\varepsilon_0},\qquad\vec\nabla\times\vec E=0$$

---

## 7. Ejemplos

### Ejemplo 1: Campo eléctrico de la atmósfera

En un día con buen tiempo, el campo eléctrico sobre la superficie de la Tierra queda descrito adecuadamente por la expresión empírica
$$\vec{E}=-\left(a\,e^{-\alpha z}+b\,e^{-\beta z}\right)\hat{k}$$
donde $a$, $b$, $\alpha$, $\beta>0$ son constantes, y $z$ denota la altura sobre la superficie de la Tierra.
a) Utilice la forma diferencial de la ley de Gauss para determinar la densidad de carga en función de la altura.
b) Calcule la carga total contenida en una columna vertical de sección transversal $A$ que va desde $z=0$ hasta $z=\infty$.

**Resolución**

*Idea:* conocido $\vec E$, la ley de Gauss diferencial $\vec\nabla\cdot\vec E=\rho/\varepsilon_0$ da $\rho$ por derivación (sección 5). Luego la carga total se obtiene integrando $\rho$ en el volumen; como control, se puede usar la ley de Gauss integral (Clase 03) sobre la columna.

**a)** El campo sólo tiene componente $z$ y sólo depende de $z$: $E_x=E_y=0$, $E_z=-(a e^{-\alpha z}+b e^{-\beta z})$.
$$\vec\nabla\cdot\vec E=\frac{\partial E_z}{\partial z}=-\left(-a\alpha\,e^{-\alpha z}-b\beta\,e^{-\beta z}\right)=a\alpha\,e^{-\alpha z}+b\beta\,e^{-\beta z}$$
Por la ley de Gauss diferencial, $\rho=\varepsilon_0\,\vec\nabla\cdot\vec E$:
$$\boxed{\rho(z)=\varepsilon_0\left(a\alpha\,e^{-\alpha z}+b\beta\,e^{-\beta z}\right)}$$

**b)** Elemento de volumen de la columna: $dV=A\,dz$.
$$Q=\int_0^\infty\rho(z)\,A\,dz=\varepsilon_0A\left[a\alpha\int_0^\infty e^{-\alpha z}dz+b\beta\int_0^\infty e^{-\beta z}dz\right]=\varepsilon_0A\left[a\alpha\cdot\frac1\alpha+b\beta\cdot\frac1\beta\right]$$
$$\boxed{Q=\varepsilon_0A\,(a+b)}$$

*Verificación (ley de Gauss integral):* se toma como superficie cerrada la columna, con tapa inferior en $z=0$ y tapa superior en $z\to\infty$.
- Paredes laterales: $\vec E\parallel\hat k$ es tangente a ellas → flujo nulo.
- Tapa superior: $E\to0$ cuando $z\to\infty$ → flujo nulo.
- Tapa inferior: normal exterior $-\hat k$, y $\vec E(0)=-(a+b)\hat k$: $\Phi=\vec E\cdot\vec A=(-(a+b)\hat k)\cdot(-A\hat k)=(a+b)A$.

Entonces $Q=\varepsilon_0\Phi=\varepsilon_0A(a+b)$, igual que en (b). ✔

*Interpretación:* $\rho>0$ en toda la atmósfera (decrece exponencialmente con la altura), y el campo apunta hacia abajo (de las cargas positivas del aire hacia la Tierra). Para que el campo sea nulo dentro de la Tierra (conductor, Clase 03), la superficie terrestre debe tener una carga superficial negativa $\sigma=-\varepsilon_0(a+b)$, que compensa exactamente la carga positiva de la columna: $\sigma A+Q=0$. Unidades: $[a]=[b]=$ N/C, $[\alpha]=[\beta]=$ m⁻¹ → $[\rho]=\frac{\text{C}^2}{\text{N·m}^2}\cdot\frac{\text{N}}{\text{C·m}}=$ C/m³. ✔

### Ejemplo 2 (complemento): Verificación de la ley diferencial en una esfera uniforme

Compruebe que el campo de la esfera maciza uniforme (Clase 03, Ejemplo 4) cumple $\vec\nabla\cdot\vec E=\rho/\varepsilon_0$ dentro y $\vec\nabla\cdot\vec E=0$ fuera, y que $\vec\nabla\times\vec E=0$.

**Resolución**

*Idea:* el campo es radial y sólo depende de $r$, así que se usa la divergencia en esféricas $\vec\nabla\cdot\vec E=\frac1{r^2}\frac{d}{dr}(r^2E_r)$ (sección 4.2).

- **Interior** ($r<a$): $E_r=\dfrac{\rho r}{3\varepsilon_0}$, $r^2E_r=\dfrac{\rho r^3}{3\varepsilon_0}$.
  $$\vec\nabla\cdot\vec E=\frac1{r^2}\cdot\frac{3\rho r^2}{3\varepsilon_0}=\frac{\rho}{\varepsilon_0}\ \checkmark$$
- **Exterior** ($r>a$): $E_r=\dfrac{kQ}{r^2}$, $r^2E_r=kQ$ constante ⇒ $\vec\nabla\cdot\vec E=0$, consistente con $\rho=0$ fuera. ✔
- **Rotor:** un campo $E_r(r)\hat r$ tiene rotor nulo (sección 4.2). ✔

$$\boxed{\vec\nabla\cdot\vec E=\begin{cases}\rho/\varepsilon_0,& r<a\\0,& r>a\end{cases},\qquad\vec\nabla\times\vec E=0}$$

*Interpretación:* lo mismo vale para la carga puntual: $\vec\nabla\cdot(kq\hat r/r^2)=0$ para todo $r\neq0$; toda la "fuente" está concentrada en el origen, donde está la carga. La forma diferencial sólo "ve" la carga local, mientras que la integral suma todas las fuentes encerradas.

### Ejemplo 3 (complemento): Densidad de carga a partir de un campo en coordenadas cartesianas

En cierta región el campo eléctrico es $\vec E=C\,(x\,\hat i+y\,\hat j)$, con $C$ constante. Determine $\rho$ y verifique si el campo puede ser electrostático.

**Resolución**

*Idea:* aplicar las definiciones de divergencia y rotor (sección 2) y la ley de Gauss diferencial.

1. $\vec\nabla\cdot\vec E=\dfrac{\partial(Cx)}{\partial x}+\dfrac{\partial(Cy)}{\partial y}+0=2C$ ⇒ $\rho=2C\varepsilon_0$ (uniforme).
2. $\vec\nabla\times\vec E=\left(\dfrac{\partial(Cy)}{\partial x}-\dfrac{\partial(Cx)}{\partial y}\right)\hat k=0$ ⇒ es compatible con la electrostática.

$$\boxed{\rho=2\varepsilon_0C,\qquad\vec\nabla\times\vec E=0}$$

*Verificación:* es el campo interior de un cilindro infinito uniforme (Clase 03, Ejemplo 6): $\vec E=\frac{\rho}{2\varepsilon_0}r\,\hat r=\frac{\rho}{2\varepsilon_0}(x\hat i+y\hat j)$, es decir, $C=\rho/2\varepsilon_0$ ⇒ $\rho=2\varepsilon_0C$. ✔ Este es además el campo de la figura del gradiente (sección 1).

---

## Resumen de fórmulas

| Concepto | Expresión |
|---|---|
| Operador nabla | $\vec\nabla=\hat i\,\partial_x+\hat j\,\partial_y+\hat k\,\partial_z$ |
| Gradiente | $\vec\nabla F=\partial_xF\,\hat i+\partial_yF\,\hat j+\partial_zF\,\hat k$; $dF=\vec\nabla F\cdot d\vec r$ |
| Divergencia | $\vec\nabla\cdot\vec F=\partial_xF_x+\partial_yF_y+\partial_zF_z$ |
| Rotor | $\vec\nabla\times\vec F=(\partial_yF_z-\partial_zF_y)\hat i+(\partial_zF_x-\partial_xF_z)\hat j+(\partial_xF_y-\partial_yF_x)\hat k$ |
| Identidades | $\vec\nabla\times\vec\nabla F=0$, $\ \vec\nabla\cdot(\vec\nabla\times\vec F)=0$ |
| Teorema de la divergencia | $\displaystyle\iiint_\Omega\vec\nabla\cdot\vec F\,dV=\oiint_{\partial\Omega}\vec F\cdot d\vec S$ |
| Teorema de Stokes | $\displaystyle\iint_S(\vec\nabla\times\vec F)\cdot d\vec S=\oint_{\partial S}\vec F\cdot d\vec\ell$ |
| Divergencia radial (esféricas / cilíndricas) | $\dfrac1{r^2}\dfrac{d(r^2F_r)}{dr}$ / $\dfrac1r\dfrac{d(rF_r)}{dr}$ |
| Elementos de volumen | cilíndricas $r\,dr\,d\phi\,dz$; esféricas $r^2\sin\theta\,dr\,d\theta\,d\phi$ |
| Ley de Gauss integral | $\displaystyle\oiint\vec E\cdot d\vec A=\frac{1}{\varepsilon_0}\iiint\rho\,dV$ |
| Ley de Gauss diferencial (1ª ec. de Maxwell) | $\vec\nabla\cdot\vec E=\dfrac{\rho}{\varepsilon_0}$ |
| Electrostática conservativa | $\vec\nabla\times\vec E=0\iff\oint\vec E\cdot d\vec\ell=0\iff\vec E=-\vec\nabla V$ |
| Atmósfera (Ejemplo 1) | $\rho=\varepsilon_0(a\alpha e^{-\alpha z}+b\beta e^{-\beta z})$, $\ Q=\varepsilon_0A(a+b)$ |
