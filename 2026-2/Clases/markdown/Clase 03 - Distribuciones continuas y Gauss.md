# Distribuciones continuas de carga y ley de Gauss

*FIS1533 — Electricidad y Magnetismo. Prof. Marcelo Cisternas.*

En esta clase se generaliza el cálculo del campo eléctrico (Clase 02: ley de Coulomb y superposición) a distribuciones continuas de carga, se introduce el concepto de **flujo eléctrico** y se enuncia la **ley de Gauss** en forma integral, con sus aplicaciones a distribuciones simétricas y a conductores en equilibrio electrostático.

---

## 1. Principio de superposición (repaso)

El principio de superposición es válido para determinar el campo eléctrico de una distribución de cargas más compleja: el campo eléctrico total en un punto es la **suma vectorial** de los campos individuales producidos por cada carga en ese punto:

$$\vec{E}=k \sum_{i} \frac{q_{i}}{r_{i}^{2}}\,\hat{r}_{i}, \qquad k=\frac{1}{4\pi\varepsilon_0}\approx 8{,}99\times10^{9}\ \text{N·m}^2/\text{C}^2$$

donde $r_i$ es la distancia desde la $i$-ésima carga $q_i$ hasta el punto donde se evalúa el campo y $\hat{r}_i$ es el vector unitario que apunta **desde la carga $q_i$ hacia el punto**.

---

## 2. Distribuciones continuas de carga

Una distribución continua es la generalización de una distribución discreta: el sistema de cargas muy próximas entre sí se modela como una carga distribuida de forma continua en una línea, una superficie o un volumen. Se caracteriza por una **densidad de carga** $\rho(x,y,z)$, con dimensiones de [carga/volumen].

> **[Figura]:** Una región del espacio de forma irregular con densidad $\rho(\vec r\,')=\rho(x',y',z')$. Dentro de ella se marca un elemento de volumen $dx'\,dy'\,dz'=d^3r'$. Desde el **origen** salen dos vectores: $\vec r\,'$, que apunta al elemento de carga, y $\vec r$, que apunta al **punto de observación**. El vector $\vec r-\vec r\,'$ va desde el elemento de carga hasta el punto de observación.

### 2.1 Procedimiento de cálculo

1. Se divide la distribución en pequeños elementos, cada uno con carga $\Delta q$.
2. Cada elemento se trata como carga puntual: su campo en $P$ es
   $$\Delta\vec E = k\,\frac{\Delta q}{r^2}\,\hat r$$
   donde $r$ es la distancia del elemento a $P$ y $\hat r$ el unitario dirigido desde el elemento hacia $P$.
3. Se suman todas las contribuciones (superposición) y se toma el límite $\Delta q\to 0$:
   $$\vec{E} = k\lim_{\Delta q_i\to 0}\sum_i \frac{\Delta q_i}{r_i^2}\,\hat r_i = k\int \frac{dq}{r^2}\,\hat r$$

La integral es **vectorial**: en la práctica se descompone $d\vec E$ en componentes y se integra cada una por separado (aprovechando la simetría para anular componentes).

En notación vectorial general, con origen arbitrario:

$$\vec{E}(\vec{r})=k\int \frac{\rho(\vec{r}\,')\,d^{3}r'}{\left| \vec{r}-\vec{r}\,' \right|^{3}}\,(\vec{r}-\vec{r}\,')$$

Habitualmente se elige el origen en el punto de observación; $\rho(\vec r)$ es una constante o una función analítica en el volumen de interés. Con $R$ la distancia del elemento al punto de observación:

$$\vec{E}=k\int \frac{dq}{R^{2}}\,\hat{R}=k\rho \int \frac{dV}{R^{2}}\,\hat{R}\quad(\rho\ \text{constante})$$

### 2.2 Densidades de carga

| Distribución | Densidad (no uniforme) | Uniforme | Unidad | Elemento de carga |
|---|---|---|---|---|
| Volumen $V$ | $\rho=\dfrac{dQ}{dV}$ | $\rho=\dfrac{Q}{V}$ | C/m³ | $dq=\rho\,dV$ |
| Superficie de área $A$ | $\sigma=\dfrac{dQ}{dA}$ | $\sigma=\dfrac{Q}{A}$ | C/m² | $dq=\sigma\,dA$ |
| Línea de longitud $L$ | $\lambda=\dfrac{dQ}{dL}$ | $\lambda=\dfrac{Q}{L}$ | C/m | $dq=\lambda\,d\ell$ |

---

## 3. Ejemplos de campo de distribuciones continuas

### Ejemplo 1: Campo de una línea finita cargada (punto en el eje)

Una línea de largo $L$ tiene una densidad de carga $\lambda$ y carga total $Q$. Determine el campo eléctrico en el punto $P$ ubicado a lo largo del eje de esta línea.

> **[Figura]:** Ejes $x$–$y$. El punto $P$ está en el origen. La barra está sobre el eje $x$, desde $x=a$ hasta $x=a+\ell$ (en la figura la longitud se denota $\ell$, igual a $L$). Un elemento de longitud $dx$ ubicado a distancia $x$ de $P$ tiene carga $dq=\lambda\,dx$. El campo $\vec E$ en $P$ apunta hacia $-x$ (hacia la izquierda, alejándose de la barra).

*Para pensar:* ¿cómo cambia este problema si la línea fuese infinita?

Respuesta (diapositiva): $\vec{E}=-k \left( \dfrac{Q}{a^{2}+L a} \right)\hat{i}$

**Resolución**

*Idea:* usar $\vec E=k\int dq\,\hat r/r^2$ (sección 2). Como todos los elementos están sobre el eje $x$ a la derecha de $P$, cada $d\vec E$ apunta en $-\hat i$ (para $\lambda>0$): no hay que descomponer, basta sumar magnitudes.

1. Elemento de carga: $dq=\lambda\,dx$, a distancia $r=x$ de $P$. Unitario desde la carga hacia $P$: $\hat r=-\hat i$.
2. Contribución:
   $$d\vec E = k\frac{\lambda\,dx}{x^2}(-\hat i)$$
3. Integrando de $x=a$ a $x=a+L$:
   $$\vec E=-k\lambda\,\hat i\int_a^{a+L}\frac{dx}{x^2}=-k\lambda\left[-\frac1x\right]_a^{a+L}\hat i=-k\lambda\left(\frac1a-\frac1{a+L}\right)\hat i$$
4. Simplificando: $\dfrac1a-\dfrac1{a+L}=\dfrac{L}{a(a+L)}$, y como $\lambda L=Q$:
   $$\boxed{\vec E=-\,\frac{kQ}{a(a+L)}\,\hat i=-k\frac{Q}{a^2+La}\,\hat i}$$

Coincide con la respuesta de la diapositiva.

*Verificación / interpretación:*
- Unidades: $kQ/\text{m}^2$ → N/C. ✔
- Límite $a\gg L$: $E\to kQ/a^2$, el campo de una carga puntual $Q$. ✔
- *Para pensar (línea infinita):* si la barra se extiende indefinidamente ($L\to\infty$, semi-infinita desde $x=a$), la carga total diverge, pero el campo es finito: $E=k\lambda\left(\frac1a-0\right)=\dfrac{k\lambda}{a}$. Ya no se puede expresar en función de $Q$; se debe usar $\lambda$. Si la línea fuese infinita en ambos sentidos y $P$ estuviese sobre ella, el campo en $P$ no estaría definido (P estaría sobre la carga). El caso físicamente relevante de línea infinita con $P$ **fuera** de ella da $E=2k\lambda/r$ (ver Ejercicio 1 y Ejemplo 5).

### Ejemplo 2: Campo eléctrico de un anillo (punto en el eje)

Considere un anillo de radio $R$ uniforme y carga total $Q$. Calcule el campo eléctrico debido a este sobre el punto $P$ que está a una distancia $z$ desde su centro.

> **[Figura]:** Anillo de radio $R$ en el plano $xy$, centrado en el origen. El punto $P$ está sobre el eje $z$ a altura $z$. Un elemento $dq$ del anillo está en el ángulo azimutal $\phi'$; la distancia de $dq$ a $P$ es $r=\sqrt{z^2+R^2}$. El vector $d\vec E$ en $P$ apunta a lo largo de la recta que une $dq$ con $P$, alejándose de $dq$ (tiene componente hacia $+z$ y una componente radial horizontal).

Respuesta (diapositiva): $\vec{E}( z)=k \dfrac{Q z}{\left( z^{2}+R^{2} \right)^{3/2}}\hat{k}$

**Resolución**

*Idea:* superposición continua + simetría. Cada elemento $dq$ tiene un compañero diametralmente opuesto cuya componente horizontal de $d\vec E$ es igual y opuesta; las componentes horizontales se cancelan y sólo sobrevive $E_z$.

1. Todos los elementos están a la misma distancia $r=\sqrt{z^2+R^2}$ de $P$, por lo que $|d\vec E|=k\,dq/(z^2+R^2)$.
2. La componente $z$ se obtiene con el coseno del ángulo $\theta$ entre $d\vec E$ y el eje $z$: $\cos\theta=\dfrac{z}{r}=\dfrac{z}{\sqrt{z^2+R^2}}$.
   $$dE_z=k\frac{dq}{z^2+R^2}\cdot\frac{z}{\sqrt{z^2+R^2}}=k\frac{z\,dq}{(z^2+R^2)^{3/2}}$$
3. Como $z$ y $R$ son constantes al recorrer el anillo, el factor sale de la integral y $\int dq=Q$:
   $$\boxed{\vec E(z)=k\frac{Qz}{(z^2+R^2)^{3/2}}\,\hat k}$$

Coincide con la diapositiva.

*Verificación / interpretación:*
- En el centro ($z=0$): $E=0$, por simetría (todas las contribuciones se cancelan). ✔
- Para $z\gg R$: $E\approx kQ/z^2$ (carga puntual). ✔
- Para $z<0$ el resultado cambia de signo automáticamente: el campo apunta en $-\hat k$, alejándose del anillo. ✔
- El campo es máximo en $z=R/\sqrt2$ (derivando e igualando a cero).

### Ejercicio 1: Campo de una línea de carga (punto en la mediatriz)

Una carga eléctrica $Q$ positiva está distribuida uniformemente a lo largo de una línea con longitud $2a$ que se ubica sobre el eje $y$, entre $y=-a$ y $y=+a$. Calcule el campo eléctrico en el punto $P$ sobre el eje $x$, a una distancia $x$ del origen.

> **[Figura]:** Barra vertical sobre el eje $y$ entre $-a$ y $+a$, con carga total $Q$. Un elemento $dy$ a altura $y$ tiene carga $dQ$. El punto $P$ está sobre el eje $x$ a distancia $x$ del origen $O$. La distancia de $dQ$ a $P$ es $r$, y la línea $dQ$–$P$ forma un ángulo $\alpha$ con el eje $x$. En $P$, el vector $d\vec E$ apunta alejándose de $dQ$ (hacia abajo a la derecha), con componentes $dE_x$ (hacia $+x$) y $dE_y$ (hacia $-y$); $\alpha$ es el ángulo entre $d\vec E$ y el eje $x$.

Respuesta (diapositiva): $\vec{E}(P)=k\dfrac{Q}{x\,(x^{2}+a^{2})^{1/2}}\, \hat{i}$

**Resolución**

*Idea:* superposición continua (sección 2) con simetría respecto del eje $x$: el elemento en $+y$ y el elemento en $-y$ producen componentes $dE_y$ opuestas que se cancelan. Sólo queda $E_x$.

1. Densidad: $\lambda=\dfrac{Q}{2a}$, $dQ=\lambda\,dy$.
2. Distancia: $r=\sqrt{x^2+y^2}$; $\cos\alpha=\dfrac{x}{\sqrt{x^2+y^2}}$.
3. Componente $x$:
   $$dE_x=k\frac{dQ}{r^2}\cos\alpha=k\lambda\frac{x\,dy}{(x^2+y^2)^{3/2}}$$
4. Integral (con $\displaystyle\int\frac{dy}{(x^2+y^2)^{3/2}}=\frac{y}{x^2\sqrt{x^2+y^2}}$, que se obtiene con $y=x\tan\theta$):
   $$E_x=k\lambda x\left[\frac{y}{x^2\sqrt{x^2+y^2}}\right]_{-a}^{a}=k\lambda x\cdot\frac{2a}{x^2\sqrt{x^2+a^2}}=\frac{k(2a\lambda)}{x\sqrt{x^2+a^2}}$$
5. Con $2a\lambda=Q$:
   $$\boxed{\vec E(P)=\frac{kQ}{x\sqrt{x^2+a^2}}\,\hat i}$$

Coincide con la diapositiva.

*Verificación / interpretación:*
- Para $x\gg a$: $E\approx kQ/x^2$ (carga puntual). ✔
- **Línea infinita** ($a\gg x$): $\sqrt{x^2+a^2}\approx a$, luego $E\approx \dfrac{kQ}{xa}=\dfrac{k\,2a\lambda}{xa}=\dfrac{2k\lambda}{x}=\dfrac{\lambda}{2\pi\varepsilon_0 x}$. Este resultado se recuperará con la ley de Gauss en el Ejemplo 5. ✔

### Ejercicio 2: Campo de un disco con carga uniforme

Encuentre el campo eléctrico que genera un disco de radio $R$ con densidad superficial de carga positiva y uniforme $\sigma$, en un punto a lo largo del eje del disco a una distancia $x$ de su centro. Suponga que $x$ es positiva.

> **[Figura]:** Disco de radio $R$ en el plano perpendicular al eje $x$, centrado en $O$. Se marca un anillo delgado de radio $r$ y ancho $dr$, con carga $dQ$. El punto $P$ está sobre el eje $x$ a distancia $x$ de $O$; la contribución $dE_x$ del anillo en $P$ apunta hacia $+x$.

Respuesta (diapositiva): $\vec{E}(P)=\dfrac{\sigma }{2\varepsilon_0}\left( 1-\dfrac{x}{\left( x^{2}+R^{2} \right)^{1/2}} \right)\hat{i}=2\pi k\sigma \left( 1-\dfrac{x}{\left( x^{2}+R^{2} \right)^{1/2}} \right)\hat{i}$

**Resolución**

*Idea:* descomponer el disco en anillos concéntricos y usar el resultado del **Ejemplo 2** (campo de un anillo en su eje) como bloque elemental; luego sumar (integrar) los anillos.

1. Un anillo de radio interior $r$ y exterior $r+dr$ tiene área $dA=2\pi r\,dr$ y carga
   $$dQ=\sigma\,dA=2\pi\sigma r\,dr$$
2. Campo del anillo en su eje (Ejemplo 2, con $Q\to dQ$, $R\to r$, $z\to x$):
   $$dE_x=k\frac{x\,dQ}{(x^2+r^2)^{3/2}}=\frac{1}{4\pi\varepsilon_0}\frac{(2\pi\sigma r\,dr)\,x}{(x^2+r^2)^{3/2}}$$
   Cada anillo sólo tiene componente a lo largo del eje, así que $E_y=E_z=0$.
3. Se integra sobre $r$ de $0$ a $R$ (no de $-R$ a $R$), con $x$ constante:
   $$E_x=\frac{\sigma x}{2\varepsilon_0}\int_0^R\frac{r\,dr}{(x^2+r^2)^{3/2}}$$
4. Sustitución $u=x^2+r^2$, $du=2r\,dr$:
   $$\int_0^R\frac{r\,dr}{(x^2+r^2)^{3/2}}=\frac12\int_{x^2}^{x^2+R^2}u^{-3/2}du=\left[-u^{-1/2}\right]_{x^2}^{x^2+R^2}=\frac1x-\frac{1}{\sqrt{x^2+R^2}}$$
5. Entonces:
   $$E_x=\frac{\sigma x}{2\varepsilon_0}\left[\frac1x-\frac1{\sqrt{x^2+R^2}}\right]$$
   $$\boxed{\vec E(P)=\frac{\sigma}{2\varepsilon_0}\left(1-\frac{x}{\sqrt{x^2+R^2}}\right)\hat i=\frac{\sigma}{2\varepsilon_0}\left[1-\frac{1}{\sqrt{(R^2/x^2)+1}}\right]\hat i}$$

Como $\frac{1}{2\varepsilon_0}=2\pi k$, es igual a la forma $2\pi k\sigma(\dots)$ de la diapositiva. ✔

*Verificación / interpretación:*
- **Plano infinito** ($R\gg x$): el término $1/\sqrt{R^2/x^2+1}\to0$ y
  $$E=\frac{\sigma}{2\varepsilon_0}$$
  independiente de la distancia al plano. La dirección es perpendicular al plano, alejándose de él (si $\sigma>0$). Para $x<0$ el campo tiene la misma magnitud pero apunta hacia $-\hat i$. No existe una lámina infinita real, pero si sus dimensiones son mucho mayores que la distancia $x$, el campo se aproxima muy bien por este valor.
- Lejos del disco ($x\gg R$): usando $(1+R^2/x^2)^{-1/2}\approx1-\frac{R^2}{2x^2}$, $E\approx\frac{\sigma}{2\varepsilon_0}\frac{R^2}{2x^2}=\frac{k(\sigma\pi R^2)}{x^2}=\frac{kQ}{x^2}$ (carga puntual). ✔

**Complemento: dos láminas infinitas con carga opuesta.** Dos láminas planas infinitas y paralelas, separadas una distancia $d$; la inferior (lámina 1) con $+\sigma$ y la superior (lámina 2) con $-\sigma$. Por superposición, cada lámina produce $E=\sigma/2\varepsilon_0$: la lámina 1 apunta alejándose de ella, la lámina 2 apunta hacia ella.

> **[Figura]:** Vista de canto de las dos láminas horizontales. Arriba de la lámina 2: $\vec E_1$ hacia arriba y $\vec E_2$ hacia abajo → $\vec E=0$. Entre ambas: $\vec E_1$ y $\vec E_2$ hacia arriba → se suman. Debajo de la lámina 1: $\vec E_1$ hacia abajo y $\vec E_2$ hacia arriba → $\vec E=0$.

$$\vec E_{\text{entre}}=\frac{\sigma}{\varepsilon_0}\,\hat j\ (\text{de la placa } +\sigma \text{ hacia la } -\sigma),\qquad \vec E_{\text{fuera}}=0$$

Esta es la configuración del condensador de placas paralelas (Clase 06).

---

## 4. Lo aprendido hasta ahora sobre el campo eléctrico

- Las cargas eléctricas estáticas son fuentes de campos eléctricos, capaces de interactuar con otras cargas.
- El campo generado por una carga puntual está dado por la ley de Coulomb: su magnitud es proporcional a la carga e inversamente proporcional al cuadrado de la distancia.
- Si hay más de una carga, el campo total es la suma vectorial de los campos generados por cada carga individualmente.

$$\textbf{Electrostática} = \text{Ley de Coulomb} + \text{Principio de superposición}$$

La ley de Gauss ofrece una forma alternativa (y equivalente) de expresar esta relación entre cargas y campos.

---

## 5. Flujo de campo eléctrico

### 5.1 Motivación: ¿cómo medir la carga dentro de una caja sin abrirla?

Planteamos la pregunta inversa a la de la sección 2: *si se conoce el campo eléctrico en una región, ¿qué podemos decir de la distribución de carga en esa región?*

> **[Figura]:** (a) Una caja cerrada que contiene una cantidad desconocida de carga (marcada con "?"). (b) Una carga de prueba $q_0$ se mueve alrededor de la caja; en distintas posiciones se mide la fuerza y se dibujan vectores $\vec E=\vec F/q_0$, todos apuntando radialmente hacia fuera de la caja, como el campo de una carga puntual positiva.

Imaginemos que la caja es una **superficie cerrada imaginaria** (una superficie que encierra por completo un volumen). Moviendo una carga de prueba $q_0$ alrededor de ella y midiendo $\vec F$, se construye el mapa $\vec E=\vec F/q_0$ fuera de la caja. En realidad, basta medir $\vec E$ **sobre la superficie** de la caja.

> **[Figura]:** Cuatro cajas: (a) una carga $+q$ dentro: el campo sobre la superficie apunta hacia fuera (flujo hacia fuera). (b) dos cargas $+q$: también hacia fuera, con más líneas. (c) una carga $-q$: el campo apunta hacia dentro (flujo hacia dentro). (d) dos cargas $-q$: hacia dentro, con más líneas.

Conclusiones cualitativas:
- Carga neta positiva dentro → flujo neto hacia fuera; carga neta negativa → flujo neto hacia dentro.
- Al duplicar la carga encerrada se duplica el flujo: **el flujo neto es proporcional a la carga neta encerrada**.
- Cargas fuera de la superficie no producen flujo neto (las líneas que entran también salen).
- El flujo neto no depende del tamaño de la superficie cerrada.

### 5.2 Flujo de un campo uniforme a través de una superficie plana

El flujo de un campo vectorial se interpreta como la cantidad de líneas de campo que atraviesan una sección transversal. Si el campo es uniforme y **perpendicular** a una superficie de área $A$:

$$\Phi_E=EA$$

> **[Figura]:** Un rectángulo de área $A$ atravesado perpendicularmente por líneas de campo $\vec E$ paralelas y uniformes.

Se define el **vector de área** $\vec A=A\,\hat n$, donde $\hat n$ es el vector unitario normal a la superficie. Una superficie tiene dos lados, por lo que hay que especificar cuál de las dos normales se elige. **Para una superficie cerrada se elige siempre $\hat n$ hacia el exterior**: el flujo hacia fuera es positivo y el flujo hacia dentro es negativo.

> **[Figura]:** Tres casos con campo uniforme horizontal $\vec E$:
> (a) Superficie de frente al campo: $\vec E\parallel\vec A$, $\phi=0$, $\Phi_E=EA$.
> (b) Superficie inclinada un ángulo $\phi$: el ángulo entre $\vec E$ y $\vec A$ es $\phi$; el área proyectada perpendicular al campo es $A_\perp=A\cos\phi$, y $\Phi_E=EA\cos\phi$.
> (c) Superficie de canto: $\vec E\perp\vec A$, $\phi=90^\circ$, $\Phi_E=EA\cos90^\circ=0$.

$$\Phi_E=ES\cos\theta = \vec{E}\cdot \left( S\hat{n} \right)=\vec{E}\cdot \vec{S}$$

donde $\theta$ es el ángulo que forma el campo con el vector normal a la superficie. La unidad SI del flujo eléctrico es $1\ \text{N·m}^2/\text{C}$.

### 5.3 Flujo de un campo no uniforme o a través de una superficie curva

Se divide la superficie en elementos $dA$ con vector de área $d\vec A=\hat n\,dA$, se calcula el flujo en cada uno y se integra:

$$\Phi_E=\int E\cos\phi\,dA=\int E_\perp\,dA=\int \vec{E}\cdot d\vec{S}\qquad\text{(definición general del flujo eléctrico)}$$

Esta integral es la **integral de superficie** de la componente normal $E_\perp$. El flujo $\int E_\perp dA$ es igual al valor medio de la componente perpendicular del campo multiplicado por el área. Para una superficie cerrada se escribe $\oint\vec E\cdot d\vec A$.

---

## 6. Ley de Gauss (forma integral)

El flujo eléctrico total a través de **cualquier superficie cerrada** es proporcional a la carga neta encerrada; la constante de proporcionalidad es $1/\varepsilon_0$ (permitividad del vacío, $\varepsilon_0=8{,}854\times10^{-12}\ \text{C}^2/\text{N·m}^2$):

$$\boxed{\Phi_E=\oint \vec E\cdot d\vec A=\frac{q_{\text{enc}}}{\varepsilon_0}}$$

> **[Figura]:** (a) Una carga puntual $+q$ en el centro de una superficie gaussiana esférica de radio $r$. (b) La misma carga dentro de una superficie cerrada de forma irregular. El flujo es el mismo, $q/\varepsilon_0$, en ambos casos.

**Justificación para una carga puntual.** Para una esfera de radio $R$ centrada en $q$: $E=\frac{1}{4\pi\varepsilon_0}\frac{q}{R^2}$ es igual en todos los puntos y $\vec E$ es paralelo a $d\vec A$ (radial, hacia fuera). Entonces
$$\Phi_E=E\oint dA=\frac{1}{4\pi\varepsilon_0}\frac{q}{R^2}\cdot4\pi R^2=\frac{q}{\varepsilon_0}$$
El radio se cancela: el resultado no depende del tamaño. Como las líneas de campo son continuas, cualquier otra superficie que encierre $q$ es atravesada por las mismas líneas, por lo que el flujo tampoco depende de la forma. Por superposición, vale para cualquier distribución.

*Ejemplo numérico (texto de referencia):* una carga $q=3{,}0\ \mu\text{C}$ rodeada por una esfera de radio $0{,}20$ m centrada en ella. $E=kq/r^2=(9{,}0\times10^9)(3{,}0\times10^{-6})/(0{,}20)^2=6{,}75\times10^5$ N/C; $\Phi_E=E\cdot4\pi r^2=(6{,}75\times10^5)(4\pi)(0{,}20)^2=3{,}4\times10^5\ \text{N·m}^2/\text{C}$, igual a $q/\varepsilon_0=3{,}39\times10^5\ \text{N·m}^2/\text{C}$. Se obtendría lo mismo con una esfera de 2,0 m o de 200 m de radio.

### 6.1 Ley de Gauss vs. ley de Coulomb

> **[Figura]:** Comparación de dos métodos. Izquierda ("Gauss"): esfera gaussiana centrada en una carga, con $\vec E$ y $d\vec A$ paralelos en cada punto. Derecha ("Coulomb"): una distribución irregular dividida en elementos $\Delta q$, cada uno con su $\Delta\vec E=k\Delta q\,\hat r/r^2$ en el punto $P$, sumados vectorialmente: $\vec E=k\int dq\,\hat r/r^2$.

- **Coulomb + superposición**: siempre válido, pero requiere una integral vectorial (a veces difícil).
- **Gauss**: siempre es verdadera, pero sólo es **útil para calcular $\vec E$** cuando la distribución tiene alta simetría (esférica, cilíndrica o plana).

### 6.2 Consideraciones importantes

- Los campos eléctricos creados por cargas que se encuentran **fuera** de la superficie de Gauss no contribuyen al flujo total (aunque sí contribuyen al campo en cada punto de la superficie).
- Para despejar $E$ se necesita una superficie de Gauss en la que, por simetría, en cada parte $\vec E$ sea **perpendicular** a la superficie (paralelo a $d\vec A$) con magnitud constante, o bien **tangente** a ella ($\vec E\cdot d\vec A=0$). Sólo entonces
  $$\int \vec{E}\cdot d\vec{S}=E\int dS=\frac{q_{\text{enc}}}{\varepsilon_0}$$

**Receta para aplicar la ley de Gauss:**
1. Identificar la simetría y deducir la dirección de $\vec E$ y de qué coordenada depende su magnitud.
2. Elegir una superficie gaussiana que pase por el punto de interés y respete la simetría.
3. Calcular el flujo (sólo $E\times$ área en las partes donde $\vec E\parallel d\vec A$).
4. Calcular $q_{\text{enc}}$ (integrando la densidad si es necesario).
5. Despejar $E$.

---

## 7. Aplicaciones de la ley de Gauss

### Ejemplo 3: Carga puntual

Determinar el campo eléctrico en todo el espacio, generado por una carga puntual $q$, utilizando la ley de Gauss.

> **[Figura]:** Carga $+q$ en el centro de una esfera gaussiana de radio $r$; el elemento de área $d\vec A$ apunta radialmente hacia fuera, igual que $\vec E$.

Respuesta (diapositiva): $\vec{E}(r)=\dfrac{1}{4\pi \varepsilon_0} \dfrac{q}{r^{2}}\hat{r}$

**Resolución**

*Idea:* simetría esférica → $\vec E=E(r)\,\hat r$. Superficie gaussiana: esfera de radio $r$ centrada en la carga.

1. En la esfera, $\vec E\parallel d\vec A$ y $E(r)$ es constante: $\oint\vec E\cdot d\vec A=E(r)\cdot4\pi r^2$.
2. Carga encerrada: $q_{\text{enc}}=q$.
3. Ley de Gauss: $E\cdot4\pi r^2=q/\varepsilon_0$.
$$\boxed{\vec E(r)=\frac{1}{4\pi\varepsilon_0}\frac{q}{r^2}\,\hat r}$$

*Verificación:* recupera la ley de Coulomb (Clase 02), lo que muestra la equivalencia entre ambas leyes. Para $q<0$, $\vec E$ apunta hacia $-\hat r$. ✔

### Ejemplo 4: Esfera maciza con carga uniforme

Determinar el campo eléctrico en todo el espacio, generado por una esfera cargada de radio $R$ y carga $Q$ (distribuida uniformemente en el volumen; en la respuesta el radio se denota $a$).

> **[Figura]:** (a) Esfera aislante de radio $a$ y carga $Q$, rodeada por una esfera gaussiana concéntrica de radio $r>a$ (línea discontinua). (b) La misma esfera con una esfera gaussiana interior de radio $r<a$.

Respuesta (diapositiva):
$\vec{E}(r)= \begin{cases}\dfrac{1}{4\pi \varepsilon_0} \dfrac{Q}{r^{2}}\hat{r} , & r>a \\[2mm] \dfrac{1}{4\pi \varepsilon_0} \dfrac{Q r}{a^{3}}\hat{r} , & r\leq a\end{cases}$

**Resolución**

*Idea:* simetría esférica, $\vec E=E(r)\hat r$; esferas gaussianas concéntricas. La densidad es $\rho=\dfrac{Q}{\frac43\pi a^3}$.

**Exterior ($r>a$):** la esfera gaussiana encierra toda la carga.
$$E\cdot4\pi r^2=\frac{Q}{\varepsilon_0}\ \Rightarrow\ E=\frac{Q}{4\pi\varepsilon_0r^2}=k\frac{Q}{r^2}$$
Fuera, la esfera se comporta como una carga puntual ubicada en su centro.

**Interior ($r\le a$):** sólo se encierra la carga dentro del radio $r$:
$$q_{\text{enc}}=\rho\cdot\frac43\pi r^3=\frac{Q}{\frac43\pi a^3}\cdot\frac43\pi r^3=Q\frac{r^3}{a^3}$$
$$E\cdot4\pi r^2=\frac{Q r^3}{\varepsilon_0a^3}\ \Rightarrow\ E=\frac{Qr}{4\pi\varepsilon_0a^3}=\frac{\rho}{3\varepsilon_0}\,r$$

$$\boxed{\vec E(r)=\begin{cases}\dfrac{1}{4\pi\varepsilon_0}\dfrac{Q}{r^2}\,\hat r, & r>a\\[2mm]\dfrac{1}{4\pi\varepsilon_0}\dfrac{Qr}{a^3}\,\hat r, & r\le a\end{cases}}$$

*Verificación:* en $r=a$ ambas expresiones dan $kQ/a^2$: el campo es continuo (no hay carga superficial). En el centro $E=0$ por simetría. Crece linealmente dentro y decae como $1/r^2$ fuera. ✔

### Ejemplo 5: Alambre infinito

Determinar el campo eléctrico en todo el espacio, generado por un alambre infinito de densidad lineal de carga $\lambda$.

> **[Figura]:** Superficie gaussiana cilíndrica (coaxial con el alambre), de radio $r$ y longitud $L$, con sus dos tapas planas.

Respuesta (diapositiva): $\vec{E}(r)=\dfrac{1}{4\pi \varepsilon_0} \dfrac{2\lambda}{r}\hat{r}$

**Resolución**

*Idea:* simetría cilíndrica: el campo es radial respecto del alambre ($\hat r$ perpendicular al alambre) y sólo depende de la distancia $r$. Superficie gaussiana: cilindro coaxial de radio $r$ y longitud $L$.

1. Flujo por las tapas: $\vec E$ es tangente a ellas → $\vec E\cdot d\vec A=0$.
2. Flujo por el manto: $\vec E\parallel d\vec A$, $E$ constante → $\Phi=E\cdot2\pi rL$.
3. Carga encerrada: $q_{\text{enc}}=\lambda L$.
4. Gauss: $E\cdot2\pi rL=\lambda L/\varepsilon_0$.
$$\boxed{\vec E(r)=\frac{\lambda}{2\pi\varepsilon_0r}\,\hat r=\frac{1}{4\pi\varepsilon_0}\frac{2\lambda}{r}\,\hat r}$$

*Verificación:* coincide con la diapositiva y con el límite $a\to\infty$ del Ejercicio 1 ($2k\lambda/x$), obtenido allí con una integral. La longitud $L$ arbitraria se cancela. ✔

### Ejemplo 6: Cilindro infinito macizo

Determinar el campo eléctrico en todo el espacio, generado por un cilindro infinito de radio $R$ y densidad volumétrica de carga $\rho$ (uniforme).

Respuesta (diapositiva):
$\vec{E}(r)= \begin{cases}\dfrac{\rho R^{2}}{2\varepsilon_0r} \hat{r} , & r>R \\[2mm] \dfrac{\rho r}{2\varepsilon_0} \hat{r} , & r\leq R\end{cases}$

**Resolución**

*Idea:* misma simetría y superficie que en el Ejemplo 5 (cilindro coaxial de radio $r$, largo $L$); lo único que cambia es la carga encerrada.

Flujo en ambos casos: $\Phi=E\cdot2\pi rL$.

**Interior ($r\le R$):** $q_{\text{enc}}=\rho\,\pi r^2L$.
$$E\cdot2\pi rL=\frac{\rho\pi r^2L}{\varepsilon_0}\Rightarrow E=\frac{\rho r}{2\varepsilon_0}$$

**Exterior ($r>R$):** $q_{\text{enc}}=\rho\,\pi R^2L$.
$$E\cdot2\pi rL=\frac{\rho\pi R^2L}{\varepsilon_0}\Rightarrow E=\frac{\rho R^2}{2\varepsilon_0r}$$

$$\boxed{\vec E(r)=\begin{cases}\dfrac{\rho R^2}{2\varepsilon_0 r}\,\hat r, & r>R\\[2mm]\dfrac{\rho r}{2\varepsilon_0}\,\hat r, & r\le R\end{cases}}$$

*Verificación:* continuidad en $r=R$: ambas dan $\rho R/2\varepsilon_0$. ✔ Fuera, con $\lambda=\rho\pi R^2$ (carga por unidad de largo), $E=\lambda/(2\pi\varepsilon_0r)$: igual al alambre del Ejemplo 5. ✔

### Ejercicio 3: Cilindro con dos densidades

Se tiene un cilindro macizo muy largo de radio $b$ con densidad de carga $\rho_1$ cuando $0<r<a$ y $\rho_2$ cuando $a<r<b$ ($a<b$). Calcular el campo eléctrico en todo el espacio.

Respuesta (diapositiva):
$\vec{E}(r)= \begin{cases}\dfrac{1}{2\varepsilon_0r}\left( \rho_1a^{2}+\rho_2\left( b^{2}-a^{2} \right) \right)\hat{r} , & r>b \\[2mm] \dfrac{1}{2\varepsilon_0r}\left( \rho_1a^{2}+\rho_2\left( r^{2}-a^{2} \right) \right)\hat{r}, & a<r\le b \\[2mm] \dfrac{\rho_1r}{2\varepsilon_0}\hat{r}, & r\le a\end{cases}$

**Resolución**

*Idea:* ley de Gauss con cilindro coaxial de radio $r$ y largo $L$ (Ejemplos 5 y 6). Flujo: $E\cdot2\pi rL$. La carga encerrada se calcula sumando las capas: $q_{\text{enc}}=\int\rho\,dV$ con $dV=2\pi r'L\,dr'$, o directamente con áreas de anillos.

**Región $r\le a$:** $q_{\text{enc}}=\rho_1\pi r^2L$
$$E=\frac{\rho_1\pi r^2L}{\varepsilon_0\,2\pi rL}=\frac{\rho_1r}{2\varepsilon_0}$$

**Región $a<r\le b$:** todo el núcleo más la parte de la corteza entre $a$ y $r$:
$$q_{\text{enc}}=\rho_1\pi a^2L+\rho_2\pi(r^2-a^2)L$$
$$E=\frac{\pi L\left[\rho_1a^2+\rho_2(r^2-a^2)\right]}{\varepsilon_0\,2\pi rL}=\frac{\rho_1a^2+\rho_2(r^2-a^2)}{2\varepsilon_0r}$$

**Región $r>b$:** se encierra toda la carga:
$$q_{\text{enc}}=\rho_1\pi a^2L+\rho_2\pi(b^2-a^2)L\ \Rightarrow\ E=\frac{\rho_1a^2+\rho_2(b^2-a^2)}{2\varepsilon_0r}$$

$$\boxed{\vec E(r)=\begin{cases}\dfrac{\rho_1 r}{2\varepsilon_0}\,\hat r, & r\le a\\[2mm]\dfrac{\rho_1a^2+\rho_2(r^2-a^2)}{2\varepsilon_0 r}\,\hat r, & a<r\le b\\[2mm]\dfrac{\rho_1a^2+\rho_2(b^2-a^2)}{2\varepsilon_0 r}\,\hat r, & r>b\end{cases}}$$

Coincide con la diapositiva.

*Verificación:* en $r=a$ las dos primeras dan $\rho_1a/2\varepsilon_0$; en $r=b$ las dos últimas coinciden: el campo es continuo. Si $\rho_1=\rho_2=\rho$, se recupera el Ejemplo 6 con $R=b$. ✔

### Ejercicio 4: Plano infinito

Determinar el campo eléctrico sobre un disco infinito (plano infinito) de densidad superficial de carga $\sigma$.

Respuesta (diapositiva): $E=\dfrac{\sigma }{2\varepsilon_0}$

**Resolución**

*Idea:* simetría plana: el campo es perpendicular al plano, apunta alejándose de él (si $\sigma>0$) a ambos lados, y su magnitud sólo puede depender de la distancia al plano. Superficie gaussiana: un cilindro ("pastillero") de área de tapa $A$ que atraviesa el plano, con tapas a la misma distancia a cada lado.

1. Manto: $\vec E$ es tangente → flujo nulo.
2. Tapas: en cada una $\vec E\parallel d\vec A$ (ambos hacia fuera) → flujo $EA$ por tapa, total $2EA$.
3. Carga encerrada: la porción del plano dentro del cilindro, $q_{\text{enc}}=\sigma A$.
4. Gauss: $2EA=\sigma A/\varepsilon_0$.
$$\boxed{E=\frac{\sigma}{2\varepsilon_0}}\qquad \vec E=\pm\frac{\sigma}{2\varepsilon_0}\hat n\ \text{(alejándose del plano a cada lado)}$$

*Verificación:* coincide con el límite $R\to\infty$ del disco (Ejercicio 2), obtenido allí por integración directa. No depende de la distancia, lo que es consistente con que el flujo por las tapas no dependa de su ubicación. ✔

---

## 8. Cargas en conductores en equilibrio electrostático

En un conductor, las cargas libres se mueven ante cualquier campo. En una situación **electrostática** (todas las cargas en reposo):

1. **$\vec E=0$ en todo punto del interior del material conductor.** Si no fuese cero, las cargas libres se moverían.
2. **Toda carga en exceso se ubica en la superficie**, no en el interior. *Demostración:* se toma una superficie gaussiana totalmente dentro del material (superficie $A$ en la figura). Como $\vec E=0$ en todos sus puntos, el flujo es cero y la carga neta encerrada es cero. Encogiendo la superficie hasta un punto arbitrario $P$, la carga en ese punto es cero. Por tanto no puede haber carga en exceso en ningún punto interior.

> **[Figura]:** Corte transversal de un conductor sólido de forma irregular con cargas "+" distribuidas sobre su borde exterior. Una superficie gaussiana $A$ (línea morada) está dibujada completamente dentro del material, justo bajo la superficie.

3. **Justo fuera de la superficie, $\vec E$ es perpendicular a ella** y vale $E=\sigma/\varepsilon_0$. (Complemento: con un pastillero pequeño que atraviesa la superficie, el flujo sólo sale por la tapa exterior, porque dentro $\vec E=0$ y la componente tangencial es nula: $EA=\sigma A/\varepsilon_0$.)

### 8.1 Conductores con cavidades

> **[Figura]:** Tres paneles.
> (a) Conductor sólido con carga $q_C$: la carga reside por completo en la superficie exterior y $\vec E=0$ dentro del conductor.
> (b) El mismo conductor con una cavidad interna vacía: una superficie gaussiana arbitraria $A$ rodea la cavidad dentro del material; como $\vec E=0$ en ella, la carga neta en la superficie de la cavidad es cero. La carga $q_C$ sigue en la superficie exterior.
> (c) Se coloca una carga aislada $q$ dentro de la cavidad: la superficie de la cavidad adquiere carga total $-q$ (signos "−") y la superficie exterior queda con $q_C+q$ (signos "+").

- **Cavidad vacía:** la carga neta en la superficie de la cavidad es cero (de hecho, no hay carga en ningún punto de ella).
- **Carga $q$ en la cavidad:** como $\vec E=0$ sobre la superficie gaussiana $A$, la carga total encerrada debe ser cero ⇒ la pared de la cavidad tiene carga **$-q$** (inducida). Por conservación de la carga, la superficie externa tiene **$q_C+q$**.

$$q_{\text{cavidad}}=-q,\qquad q_{\text{exterior}}=q_C+q$$

### Ejemplo 7: Conductor con cavidad

Un conductor sólido con una cavidad tiene una carga total de $+7$ nC. Dentro de la cavidad, aislada del conductor, hay una carga puntual de $-5$ nC. ¿Cuánta carga hay en cada superficie (interna y externa) del conductor?

**Resolución**

*Idea:* conductor en equilibrio ($\vec E=0$ en el material) + ley de Gauss con una superficie dentro del material que rodea la cavidad + conservación de la carga del conductor (sección 8.1).

1. Superficie gaussiana dentro del material del conductor, rodeando la cavidad: $\vec E=0$ ⇒ $\Phi=0$ ⇒ $q_{\text{enc}}=0$.
2. La carga encerrada es la puntual más la de la superficie interna:
   $$-5\ \text{nC}+q_{\text{int}}=0\ \Rightarrow\ q_{\text{int}}=+5\ \text{nC}$$
3. La carga total del conductor es $+7$ nC y está repartida sólo entre sus dos superficies (no hay carga en el interior del material):
   $$q_{\text{int}}+q_{\text{ext}}=7\ \text{nC}\ \Rightarrow\ q_{\text{ext}}=7-5=+2\ \text{nC}$$

$$\boxed{q_{\text{interna}}=+5\ \text{nC},\qquad q_{\text{externa}}=+2\ \text{nC}}$$

*Verificación:* una superficie gaussiana que encierre todo el sistema contiene $7-5=+2$ nC, igual a la carga externa: el campo exterior es el que produciría $+2$ nC. ✔

### Ejemplo 8: Esfera conductora hueca con carga en la cavidad

Una esfera hueca, conductora, con radio exterior de $0{,}250$ m y radio interior de $0{,}200$ m tiene una densidad superficial de carga de $+6{,}37\times10^{-6}$ C/m². Se introduce una carga de $-0{,}500\ \mu$C en la cavidad interna de la esfera.
a) ¿Cuál es la nueva densidad de carga apenas afuera de la esfera?
b) Calcule la intensidad del campo eléctrico justo fuera de la esfera.
c) ¿Cuál es el flujo eléctrico a través de una superficie esférica apenas dentro de la superficie interior de la esfera?

**Resolución**

*Idea:* en un conductor en equilibrio la carga en exceso está en la superficie exterior (inicialmente no hay carga en la cavidad, así que la densidad dada corresponde a la superficie exterior). Al introducir la carga en la cavidad se induce $-q$ en la pared interior (sección 8.1). Campo justo fuera de un conductor: $E=\sigma/\varepsilon_0$. Flujo: ley de Gauss.

**Carga inicial del conductor.** Área exterior: $A_{\text{ext}}=4\pi(0{,}250)^2=0{,}7854\ \text{m}^2$.
$$Q=\sigma A_{\text{ext}}=(6{,}37\times10^{-6})(0{,}7854)=5{,}00\times10^{-6}\ \text{C}=5{,}00\ \mu\text{C}$$

**a)** Con $q=-0{,}500\ \mu$C en la cavidad, la superficie interior adquiere $+0{,}500\ \mu$C. Por conservación:
$$q_{\text{ext}}=Q-q_{\text{int}}=5{,}00-0{,}500=4{,}50\ \mu\text{C}$$
$$\sigma_{\text{nueva}}=\frac{4{,}50\times10^{-6}}{0{,}7854}$$
$$\boxed{\sigma_{\text{nueva}}=5{,}73\times10^{-6}\ \text{C/m}^2}$$

**b)** Justo fuera de la superficie del conductor:
$$E=\frac{\sigma}{\varepsilon_0}=\frac{5{,}73\times10^{-6}}{8{,}854\times10^{-12}}$$
$$\boxed{E=6{,}47\times10^{5}\ \text{N/C}\ \text{(radial, hacia fuera)}}$$

*(Equivalente: Gauss con una esfera de radio $0{,}250^+$ m encierra $Q+q=4{,}50\ \mu$C, y $E=k(4{,}50\times10^{-6})/(0{,}250)^2=6{,}47\times10^5$ N/C.)*

**c)** Una esfera gaussiana apenas dentro de la superficie interior (en la cavidad, $r=0{,}200^-$ m) sólo encierra la carga puntual $-0{,}500\ \mu$C (la carga inducida está sobre la pared, fuera de esta superficie):
$$\Phi_E=\frac{q_{\text{enc}}}{\varepsilon_0}=\frac{-0{,}500\times10^{-6}}{8{,}854\times10^{-12}}$$
$$\boxed{\Phi_E=-5{,}65\times10^{4}\ \text{N·m}^2/\text{C}}$$

*Verificación / interpretación:* el flujo es negativo porque el campo dentro de la cavidad apunta hacia la carga negativa (hacia dentro). La densidad exterior disminuye porque parte de la carga positiva del conductor fue atraída hacia la pared de la cavidad. Unidades: C/(C²/N·m²) = N·m²/C. ✔

---

## Resumen de fórmulas

| Resultado | Expresión |
|---|---|
| Superposición discreta | $\vec E=k\sum_i \dfrac{q_i}{r_i^2}\hat r_i$ |
| Distribución continua | $\vec E=k\displaystyle\int\frac{dq}{r^2}\hat r$, con $dq=\lambda\,d\ell,\ \sigma\,dA,\ \rho\,dV$ |
| Barra de largo $L$, punto en el eje a distancia $a$ del extremo | $E=\dfrac{kQ}{a(a+L)}$ |
| Barra de largo $2a$, punto en la mediatriz a distancia $x$ | $E=\dfrac{kQ}{x\sqrt{x^2+a^2}}$ |
| Anillo, punto en el eje | $E_z=\dfrac{kQz}{(z^2+R^2)^{3/2}}$ |
| Disco, punto en el eje | $E=\dfrac{\sigma}{2\varepsilon_0}\left(1-\dfrac{x}{\sqrt{x^2+R^2}}\right)$ |
| Plano infinito | $E=\dfrac{\sigma}{2\varepsilon_0}$ |
| Dos placas $\pm\sigma$ (entre ellas / fuera) | $E=\dfrac{\sigma}{\varepsilon_0}$ / $0$ |
| Flujo eléctrico | $\Phi_E=\displaystyle\int\vec E\cdot d\vec A$; uniforme: $\Phi_E=EA\cos\theta$ |
| Ley de Gauss | $\displaystyle\oint\vec E\cdot d\vec A=\frac{q_{\text{enc}}}{\varepsilon_0}$ |
| Carga puntual / exterior de esfera | $E=\dfrac{Q}{4\pi\varepsilon_0r^2}$ |
| Interior de esfera uniforme | $E=\dfrac{Qr}{4\pi\varepsilon_0a^3}=\dfrac{\rho r}{3\varepsilon_0}$ |
| Línea infinita | $E=\dfrac{\lambda}{2\pi\varepsilon_0r}=\dfrac{2k\lambda}{r}$ |
| Cilindro macizo (dentro / fuera) | $E=\dfrac{\rho r}{2\varepsilon_0}$ / $\dfrac{\rho R^2}{2\varepsilon_0r}$ |
| Conductor en equilibrio | $\vec E_{\text{int}}=0$; carga en la superficie; $E_{\text{fuera}}=\dfrac{\sigma}{\varepsilon_0}$ (normal) |
| Conductor con carga $q$ en la cavidad | $q_{\text{cavidad}}=-q$, $q_{\text{ext}}=q_C+q$ |
| Constantes | $k=8{,}99\times10^9\ \text{N·m}^2/\text{C}^2$, $\varepsilon_0=8{,}854\times10^{-12}\ \text{C}^2/\text{N·m}^2$ |
