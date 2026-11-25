# Ayudantía 02 — Campo eléctrico y Ley de Coulomb

> Clases relacionadas: [Clase 02 - Carga eléctrica, ley de Coulomb, Campo eléctrico](../../Clases/markdown/Clase%2002%20-%20Carga%20el%C3%A9ctrica%2C%20ley%20de%20Coulomb%2C%20Campo%20el%C3%A9ctrico.md), [Clase 03 - Distribuciones continuas y Gauss](../../Clases/markdown/Clase%2003%20-%20Distribuciones%20continuas%20y%20Gauss.md)

---

## Problema 1

Dos cargas puntuales $q_1$ y $q_2$ se colocan a una distancia de $4{,}50\text{ cm}$ entre sí. Otra carga puntual $Q = -1{,}75\,\mu\text{C}$ con masa de $5{,}00\text{ g}$ se sitúa inicialmente a $3{,}00\text{ cm}$ de cada una de estas cargas y se libera del reposo (*en el original: "se libera del resto"*). Usted observa que la aceleración inicial de $Q$ es de $324\text{ m/s}^2$ hacia arriba, paralela a la línea que une las dos cargas puntuales. Encuentre $q_1$ y $q_2$.

> **[Figura]:** Triángulo isósceles en el plano vertical. Dos cargas $q_1$ y $q_2$ están ubicadas sobre una recta vertical separadas por una distancia $d = 4{,}50\text{ cm}$ ($q_1$ arriba y $q_2$ abajo). A la izquierda de esta recta, a una distancia de $r = 3{,}00\text{ cm}$ de ambas cargas, se sitúa la carga $Q = -1{,}75\,\mu\text{C}$ con masa $m = 5{,}00\text{ g}$. El vector aceleración $\vec{a}$ de la carga $Q$ apunta directamente hacia arriba, de magnitud $a = 324\text{ m/s}^2$, en dirección paralela a la recta vertical que une $q_1$ y $q_2$.

### Solución

**Idea:** Aplicar la segunda ley de Newton ($\sum \vec{F} = m\vec{a}$) y la ley de Coulomb para fuerzas electrostáticas. Dado que la aceleración inicial de $Q$ es exclusivamente vertical hacia arriba, la fuerza neta debe tener solo componente vertical positiva y su componente horizontal debe ser estrictamente nula ($\sum F_x = 0$). Como $Q$ es equidistante a ambas cargas, la anulación de la componente horizontal exige que las fuerzas ejercidas por $q_1$ y $q_2$ tengan igual magnitud ($|q_1| = |q_2| = q$) y signos opuestos. Para que la componente vertical apunte hacia arriba (hacia $q_1$), la carga $q_1$ debe atraer a $Q$ y $q_2$ debe repeler a $Q$; siendo $Q < 0$, esto determina que $q_1 > 0$ y $q_2 < 0$.

#### 1. Dinámica y fuerza neta requerida

Definimos un sistema de coordenadas cartesiano donde:
- El eje $Y$ coincide con la recta vertical que une las cargas, apuntando hacia arriba, con el origen en el punto medio entre $q_1$ y $q_2$.
- El eje $X$ es horizontal, perpendicular a la recta de las cargas, apuntando hacia la derecha.

Las posiciones de las cargas son:
$$\vec{r}_1 = \left(0,\, \frac{d}{2}\right) = (0,\, 2{,}25\text{ cm})$$
$$\vec{r}_2 = \left(0,\, -\frac{d}{2}\right) = (0,\, -2{,}25\text{ cm})$$
$$\vec{r}_Q = (-x_0,\, 0)$$

Donde la distancia horizontal $x_0$ se obtiene por el teorema de Pitágoras:
$$x_0 = \sqrt{r^2 - \left(\frac{d}{2}\right)^2} = \sqrt{(3{,}00\text{ cm})^2 - (2{,}25\text{ cm})^2} = \sqrt{9{,}00 - 5{,}0625}\text{ cm} = \sqrt{3{,}9375}\text{ cm} \approx 1{,}984\text{ cm}$$

Por la segunda ley de Newton:
$$\sum \vec{F} = m \vec{a}$$

Con $m = 5{,}00\text{ g} = 5{,}00 \times 10^{-3}\text{ kg}$ y $\vec{a} = 324\text{ m/s}^2\,\hat{j}$:
$$\sum \vec{F} = (5{,}00 \times 10^{-3}\text{ kg}) (324\text{ m/s}^2)\,\hat{j} = 1{,}62\text{ N}\,\hat{j}$$

Por lo tanto:
$$\sum F_x = 0$$
$$\sum F_y = 1{,}62\text{ N}$$

#### 2. Condición sobre las magnitudes y signos de las cargas

Sea $\theta$ el ángulo que forma cada segmento de longitud $r$ con la horizontal:
$$\sin\theta = \frac{d/2}{r} = \frac{2{,}25\text{ cm}}{3{,}00\text{ cm}} = \frac{3}{4} = 0{,}75$$
$$\cos\theta = \frac{x_0}{r} = \frac{\sqrt{3{,}9375}}{3{,}00} \approx 0{,}6614$$

Las fuerzas de Coulomb ejercidas por $q_1$ y $q_2$ sobre $Q$ tienen magnitudes:
$$F_1 = \frac{k |q_1| |Q|}{r^2}, \qquad F_2 = \frac{k |q_2| |Q|}{r^2}$$

Para que la componente horizontal se anule:
$$\sum F_x = 0 \implies F_{1x} + F_{2x} = 0$$
Como ambas cargas están al mismo lado en $X$ y equidistantes, esto requiere $F_1 = F_2 \equiv F$, lo que implica:
$$|q_1| = |q_2| \equiv q$$

Asimismo, una de las fuerzas debe tirar hacia la derecha y la otra empujar hacia la izquierda. Esto ocurre si y solo si una carga ejerce atracción y la otra repulsión sobre $Q$.

Para que la componente vertical total apunte hacia $+Y$ (arriba):
- La fuerza de $q_1$ sobre $Q$ debe apuntar hacia arriba y hacia la derecha (fuerza atractiva hacia $q_1$). Como $Q = -1{,}75\,\mu\text{C} < 0$, para que sea atractiva se requiere que **$q_1 > 0$**.
- La fuerza de $q_2$ sobre $Q$ debe apuntar hacia arriba y hacia la izquierda (fuerza repulsiva desde $q_2$). Para que sea repulsiva con $Q < 0$, se requiere que **$q_2 < 0$**.

#### 3. Cálculo de la magnitud de la fuerza y de la carga

Las componentes verticales de ambas fuerzas apuntan en $+\hat{j}$ y se suman:
$$\sum F_y = F_1 \sin\theta + F_2 \sin\theta = 2 F \sin\theta$$

Igualando a la fuerza neta:
$$2 F \sin\theta = 1{,}62\text{ N}$$
$$2 F (0{,}75) = 1{,}62\text{ N} \implies 1{,}50\,F = 1{,}62\text{ N}$$
$$F = \frac{1{,}62\text{ N}}{1{,}50} = 1{,}08\text{ N}$$

A partir de la ley de Coulomb ($k = \frac{1}{4\pi\varepsilon_0} \approx 8{,}99 \times 10^9\text{ N}\cdot\text{m}^2/\text{C}^2$):
$$F = \frac{k q |Q|}{r^2} \implies q = \frac{F r^2}{k |Q|}$$

Reemplazando los valores numéricos con $r = 3{,}00\text{ cm} = 0{,}0300\text{ m}$ y $|Q| = 1{,}75 \times 10^{-6}\text{ C}$:
$$q = \frac{(1{,}08\text{ N})(0{,}0300\text{ m})^2}{(8{,}99 \times 10^9\text{ N}\cdot\text{m}^2/\text{C}^2)(1{,}75 \times 10^{-6}\text{ C})} = \frac{1{,}08 \times 9{,}00 \times 10^{-4}}{1{,}573 \times 10^4} = 6{,}17 \times 10^{-8}\text{ C}$$

Por lo tanto:
$$\boxed{q_1 = +6{,}17 \times 10^{-8}\text{ C} = +61{,}7\text{ nC}}$$
$$\boxed{q_2 = -6{,}17 \times 10^{-8}\text{ C} = -61{,}7\text{ nC}}$$

**Verificación:**
- **Unidades:** $[\text{N}] \cdot [\text{m}^2] / ([\text{N}\cdot\text{m}^2/\text{C}^2] \cdot [\text{C}]) = [\text{C}]$, dimensionalmente correcto.
- **Signos y dirección:** Con $q_1 > 0$ y $Q < 0$, la fuerza $\vec{F}_1$ atrae a $Q$ hacia $(0, d/2)$ con componentes $(+F\cos\theta,\, +F\sin\theta)$. Con $q_2 < 0$ y $Q < 0$, la fuerza $\vec{F}_2$ repele a $Q$ desde $(0, -d/2)$ con componentes $(-F\cos\theta,\, +F\sin\theta)$. La suma es $(0,\, 2F\sin\theta) = (0,\, 1{,}62\text{ N})$, exactamente en $+\hat{j}$.

---

## Problema 2

Se lanza un electrón con rapidez inicial $v_0 = 1{,}60 \times 10^6\text{ m/s}$ hacia el interior de un campo uniforme entre las placas paralelas como lo muestra la figura. Suponga que el campo entre las placas es uniforme y está dirigido verticalmente hacia abajo, y que el campo fuera de las placas es igual a cero. El electrón ingresa al campo en un punto equidistante de las dos placas.

a) Si el electrón apenas libra la placa superior al salir del campo, encuentre la magnitud del campo eléctrico.  
b) Suponga que en la figura el electrón es sustituido por un protón con la misma rapidez inicial $v_0$. ¿Golpearía el protón alguna de las placas? Si el protón no golpea ninguna de las placas, ¿cuáles serían la magnitud y la dirección de su desplazamiento vertical, a medida que sale de la región entre las placas?  
c) ¿Cuál es la rapidez del electrón cuando sale del campo eléctrico?

> **[Figura]:** Dos placas metálicas paralelas y horizontales de longitud $L = 2{,}00\text{ cm}$, separadas verticalmente por una distancia $d = 1{,}00\text{ cm}$. Entre ellas existe un campo eléctrico uniforme $\vec{E}$ dirigido verticalmente hacia abajo ($-\hat{j}$). Un electrón ingresa por el extremo izquierdo en el punto medio entre ambas placas ($y_0 = 0$, a una distancia vertical de $0{,}50\text{ cm}$ de cada placa) con velocidad horizontal $\vec{v}_0 = v_0\,\hat{i}$ ($v_0 = 1{,}60 \times 10^6\text{ m/s}$). La trayectoria del electrón es un arco de parábola que se curva hacia arriba y sale rozando el borde derecho de la placa superior.

### Solución

**Idea:** La fuerza eléctrica uniforme $\vec{F} = q\vec{E}$ produce una aceleración constante perpendicular a la velocidad inicial. El movimiento se desacopla en un movimiento rectilíneo uniforme (MRU) en el eje $X$ y un movimiento rectilíneo uniformemente acelerado (MRUA) en el eje $Y$, análogo al lanzamiento de proyectiles.

Constantes físicas empleadas:
- Magnitud de la carga elemental: $e = 1{,}60 \times 10^{-19}\text{ C}$
- Masa del electrón: $m_e = 9{,}11 \times 10^{-31}\text{ kg}$
- Masa del protón: $m_p = 1{,}67 \times 10^{-27}\text{ kg}$
- Longitud de las placas: $L = 2{,}00\text{ cm} = 0{,}0200\text{ m}$
- Distancia entre placas: $d = 1{,}00\text{ cm} = 0{,}0100\text{ m}$
- Desplazamiento vertical máximo disponible: $\Delta y = \frac{d}{2} = 0{,}50\text{ cm} = 5{,}00 \times 10^{-3}\text{ m}$

---

#### Parte a) Magnitud del campo eléctrico $E$

1. **Tiempo de permanencia en el campo:**  
   En la dirección horizontal no actúan fuerzas ($F_x = 0$):
   $$x(t) = v_0 t \implies t = \frac{L}{v_0} = \frac{0{,}0200\text{ m}}{1{,}60 \times 10^6\text{ m/s}} = 1{,}25 \times 10^{-8}\text{ s}$$

2. **Aceleración vertical del electrón:**  
   Dado que $\vec{E} = -E\,\hat{j}$ y la carga del electrón es $q = -e$:
   $$\vec{F}_e = q \vec{E} = (-e)(-E\,\hat{j}) = eE\,\hat{j}$$
   La aceleración vertical apunta hacia arriba ($+\hat{j}$):
   $$a_e = \frac{eE}{m_e}$$

   Partiendo del reposo en $Y$ ($v_{0y} = 0$), el desplazamiento vertical al recorrer la longitud $L$ es:
   $$\Delta y = \frac{1}{2} a_e t^2$$
   Para librar justamente la placa superior, debe desplazarse $\Delta y = \frac{d}{2} = 5{,}00 \times 10^{-3}\text{ m}$:
   $$a_e = \frac{2 \Delta y}{t^2} = \frac{2 (5{,}00 \times 10^{-3}\text{ m})}{(1{,}25 \times 10^{-8}\text{ s})^2} = \frac{1{,}00 \times 10^{-2}\text{ m}}{1{,}5625 \times 10^{-16}\text{ s}^2} = 6{,}40 \times 10^{13}\text{ m/s}^2$$

3. **Magnitud del campo eléctrico:**
   $$E = \frac{m_e a_e}{e} = \frac{(9{,}11 \times 10^{-31}\text{ kg})(6{,}40 \times 10^{13}\text{ m/s}^2)}{1{,}60 \times 10^{-19}\text{ C}} \approx 364{,}4\text{ N/C} \approx 364\text{ N/C}$$

$$\boxed{E = 364\text{ N/C}}$$

---

#### Parte b) Caso del protón sustituyendo al electrón

1. **Fuerza y aceleración sobre el protón:**  
   El protón tiene carga $q = +e$, por lo que la fuerza eléctrica apunta en la misma dirección del campo (hacia abajo, $-\hat{j}$):
   $$\vec{F}_p = q \vec{E} = -eE\,\hat{j}$$
   $$\|\vec{F}_p\| = eE = (1{,}60 \times 10^{-19}\text{ C})(364\text{ N/C}) \approx 5{,}83 \times 10^{-17}\text{ N}$$

   Debido a su mayor inercia ($m_p = 1{,}67 \times 10^{-27}\text{ kg}$):
   $$a_p = \frac{eE}{m_p} = \frac{5{,}83 \times 10^{-17}\text{ N}}{1{,}67 \times 10^{-27}\text{ kg}} \approx 3{,}49 \times 10^{10}\text{ m/s}^2 \approx 3{,}5 \times 10^{10}\text{ m/s}^2$$

2. **Desplazamiento vertical:**  
   Como la rapidez inicial horizontal es idéntica ($v_0 = 1{,}60 \times 10^6\text{ m/s}$), el tiempo de tránsito es el mismo:
   $$t = 1{,}25 \times 10^{-8}\text{ s}$$
   El desplazamiento vertical experimentado hacia abajo es:
   $$\Delta y_p = \frac{1}{2} a_p t^2 = \frac{1}{2} (3{,}49 \times 10^{10}\text{ m/s}^2)(1{,}25 \times 10^{-8}\text{ s})^2 \approx 2{,}73 \times 10^{-6}\text{ m} = 2{,}73\,\mu\text{m}$$

3. **¿Golpea alguna placa?**  
   Para golpear la placa inferior, el protón necesitaría descender $5{,}00\text{ mm} = 5{,}00 \times 10^{-3}\text{ m}$. Como $\Delta y_p = 2{,}73 \times 10^{-6}\text{ m} = 0{,}00273\text{ mm} \ll 5{,}00\text{ mm}$, **el protón no golpea ninguna de las placas**.

$$\boxed{\text{No golpea ninguna placa;\quad } |\Delta y_p| = 2{,}73 \times 10^{-6}\text{ m} = 2{,}73\,\mu\text{m}\quad\text{hacia abajo }(-\hat{j})}$$

---

#### Parte c) Rapidez del electrón a la salida

1. **Componentes de la velocidad:**
   - Componente horizontal (constante):
     $$v_x = v_0 = 1{,}60 \times 10^6\text{ m/s}$$
   - Componente vertical adquirida al salir:
     $$v_y = a_e t = (6{,}40 \times 10^{13}\text{ m/s}^2)(1{,}25 \times 10^{-8}\text{ s}) = 8{,}00 \times 10^5\text{ m/s} = 0{,}80 \times 10^6\text{ m/s}$$

2. **Rapidez final:**
   $$v = \sqrt{v_x^2 + v_y^2} = \sqrt{(1{,}60 \times 10^6\text{ m/s})^2 + (0{,}80 \times 10^6\text{ m/s})^2}$$
   $$v = 10^6 \sqrt{(1{,}60)^2 + (0{,}80)^2} = 10^6 \sqrt{2{,}56 + 0{,}64} = 10^6 \sqrt{3{,}20} \approx 1{,}789 \times 10^6\text{ m/s} \approx 1{,}79 \times 10^6\text{ m/s}$$

$$\boxed{v \approx 1{,}79 \times 10^6\text{ m/s}}$$

**Verificación:**
- **Relación de masas:** Como $m_p / m_e \approx 1836$, la aceleración del protón es $\approx 1836$ veces menor que la del electrón, por lo que su deflexión es $\Delta y_p = \Delta y_e / 1836 = 5 \times 10^{-3}\text{ m} / 1836 \approx 2{,}72 \times 10^{-6}\text{ m}$, consistente con el resultado.
- **Teorema trabajo-energía:** El trabajo realizado por el campo sobre el electrón es $W = q \Delta V = e E \Delta y = (1{,}60 \times 10^{-19}\text{ C})(364{,}4\text{ N/C})(0{,}005\text{ m}) = 2{,}915 \times 10^{-19}\text{ J}$. El cambio de energía cinética es $\Delta K = \frac{1}{2} m_e v_y^2 = \frac{1}{2}(9{,}11 \times 10^{-31})(8{,}00 \times 10^5)^2 = 2{,}915 \times 10^{-19}\text{ J}$, verificando exactamente la conservación de la energía.

---

## Problema 3

Calcular el campo eléctrico en el punto P, a una distancia $x$ a lo largo de la bisectriz perpendicular que une a las cargas.

> **[Figura]:** Dos cargas puntuales de signos opuestos y misma magnitud: $+q$ ubicada en la posición $(0,\, d/2)$ y $-q$ en $(0,\, -d/2)$, alineadas sobre el eje vertical $Y$ a una distancia $d$ entre sí. El punto $P$ se ubica sobre el eje horizontal $X$ (la bisectriz perpendicular al segmento entre cargas) en las coordenadas $(x,\, 0)$. La distancia de cada carga al punto $P$ es $r = \sqrt{x^2 + (d/2)^2}$. Se ilustra el ángulo $\theta$ medido entre la vertical y la recta que une la carga con el punto $P$. El vector campo eléctrico $\vec{E}_+$ (debido a $+q$) apunta alejándose de $+q$, mientras que $\vec{E}_-$ (debido a $-q$) apunta hacia $-q$. Las componentes horizontales se cancelan y las componentes verticales se suman, dando un campo resultante $\vec{E}$ que apunta verticalmente hacia abajo ($-\hat{j}$).

### Solución

**Idea:** Aplicar el principio de superposición para el campo electrostático creado por un dipolo eléctrico. Por la simetría de la configuración respecto a la bisectriz perpendicular (eje $X$), las componentes del campo paralelas a la bisectriz ($E_x$) se anulan mutuamente, mientras que las componentes perpendiculares a ella y paralelas al eje dipolar ($E_y$) apuntan ambas hacia abajo y se suman.

#### 1. Geometría y distancias

Ubicamos el origen $(0,0)$ en el punto medio entre las dos cargas:
- Posición de $+q$: $\vec{r}_+ = \left(0,\, \frac{d}{2}\right)$
- Posición de $-q$: $\vec{r}_- = \left(0,\, -\frac{d}{2}\right)$
- Posición del punto de observación $P$: $\vec{r}_P = (x,\, 0)$

La distancia de cada carga a $P$ es:
$$r = \sqrt{x^2 + \left(\frac{d}{2}\right)^2}$$

Del triángulo rectángulo formado por el origen, la carga superior y el punto $P$, el ángulo $\theta$ con respecto al eje vertical satisface:
$$\cos\theta = \frac{d/2}{r} = \frac{d}{2\sqrt{x^2 + (d/2)^2}}$$
$$\sin\theta = \frac{x}{r} = \frac{x}{\sqrt{x^2 + (d/2)^2}}$$

#### 2. Campos individuales y descomposición en componentes

La magnitud del campo eléctrico generado por cada carga puntual en $P$ es idéntica:
$$E_+ = E_- = \frac{k q}{r^2} = \frac{k q}{x^2 + (d/2)^2}$$

Descomponiendo en componentes cartesianas:
- **Campo de $+q$ (repulsivo, apunta alejándose de la carga hacia abajo y hacia la derecha):**
  $$\vec{E}_+ = E_+ \sin\theta\,\hat{i} - E_+ \cos\theta\,\hat{j}$$
- **Campo de $-q$ (atractivo, apunta hacia la carga hacia abajo y hacia la izquierda):**
  $$\vec{E}_- = -E_- \sin\theta\,\hat{i} - E_- \cos\theta\,\hat{j}$$

#### 3. Superposición

Sumando componente a componente:
- **Componente horizontal $X$:**
  $$E_x = E_+ \sin\theta - E_- \sin\theta = 0$$
- **Componente vertical $Y$:**
  $$E_y = -E_+ \cos\theta - E_- \cos\theta = -2 E_+ \cos\theta$$

Sustituyendo $E_+$ y $\cos\theta$:
$$E_y = -2 \left(\frac{k q}{r^2}\right) \left(\frac{d/2}{r}\right) = -\frac{k q d}{r^3}$$

Expresando en función de $x$ y $d$:
$$E_y = -\frac{k q d}{\left(x^2 + (d/2)^2\right)^{3/2}} = -\frac{k q d}{\left(x^2 + \frac{d^2}{4}\right)^{3/2}}$$

Utilizando la constante dieléctrica $k = \frac{1}{4\pi\varepsilon_0}$, el vector de campo eléctrico en $P$ es:

$$\boxed{\vec{E}(P) = -\frac{k q d}{\left(x^2 + \frac{d^2}{4}\right)^{3/2}}\,\hat{j} = -\frac{q d}{4\pi\varepsilon_0 \left(x^2 + \frac{d^2}{4}\right)^{3/2}}\,\hat{j}}$$

> **Nota:** En la pauta manuscrita oficial (página 5), se plantea correctamente $E = 2E_y = 2 \frac{kq}{r^2}\cos\theta$ con $\cos\theta = \frac{d/2}{r}$. Sin embargo, en la expresión final manuscrita se observa $E_T = -2 \frac{kq\cdot d}{(x^2+d/2)^{3/2}}\hat{j}$, donde se retuvo erróneamente el factor $2$ (el cual se cancela con el denominador $2$ de $d/2$) y se omitió el cuadrado en el término $(d/2)^2$ del denominador. Lo correcto física y matemáticamente es el resultado canónico del campo ecuatorial de un dipolo eléctrico, $\vec{E} = -\frac{kqd}{(x^2 + d^2/4)^{3/2}}\hat{j}$.

**Verificación:**
- **Límite dipolar a gran distancia ($x \gg d$):**
  $$\vec{E} \approx -\frac{k (qd)}{x^3}\,\hat{j} = -\frac{\vec{p}}{4\pi\varepsilon_0 x^3}$$
  donde $\vec{p} = qd\,\hat{j}$ es el momento dipolar eléctrico. Coincide con la fórmula clásica del campo ecuatorial de un dipolo.
- **Límite en el origen ($x = 0$):** El punto $P$ se ubica en el punto medio entre ambas cargas:
  $$\vec{E}(0) = -\frac{kqd}{(d/2)^3}\,\hat{j} = -\frac{4kq}{d^2}\,\hat{j} = -2\frac{kq}{(d/2)^2}\,\hat{j}$$
  que corresponde exactamente a la suma de los campos de $+q$ y $-q$ en el punto medio (ambos de magnitud $kq/(d/2)^2$ apuntando hacia abajo).

---

## Problema 4

Un alambre infinito con densidad lineal de carga $\lambda$ se dobla en forma de horquilla como se muestra en la figura. Calcular el campo eléctrico en el origen del sistema de referencia.

> **[Figura]:** Alambre delgado en forma de horquilla ubicado en el plano $XY$. Consta de tres secciones continuas cargadas uniformemente con densidad lineal $\lambda > 0$:
> 1. Un tramo recto semi-infinito superior horizontal ubicado en $y = +R$, extendiéndose desde $x = 0$ hasta $x \to +\infty$.
> 2. Un tramo curvo semicircular de radio $R$ centrado en el origen $(0,0)$, que une $(0, R)$ con $(0, -R)$ a través del semiplano izquierdo ($x \le 0$).
> 3. Un tramo recto semi-infinito inferior horizontal ubicado en $y = -R$, extendiéndose desde $x = 0$ hasta $x \to +\infty$.
> El origen $(0,0)$ es el centro de curvatura del semicírculo.

### Solución

**Idea:** Dividir la distribución continua en tres tramos: la semirrecta horizontal superior ($1$), el arco semicircular ($2$) y la semirrecta horizontal inferior ($3$). Aplicar la ley de Coulomb para densidades lineales ($d\vec{E} = \frac{1}{4\pi\varepsilon_0}\frac{dq}{|\vec{r} - \vec{r}'|^3}(\vec{r} - \vec{r}')$) en cada tramo y sumar vectorialmente por el principio de superposición.

---

#### 1. Tramo 1: Semirrecta superior ($y = R$, $x \in [0, \infty)$)

- Posición de un elemento de carga $dq = \lambda dx$:
  $$\vec{r}' = x\,\hat{i} + R\,\hat{j}$$
- Vector que va desde el elemento de carga hacia el origen $(0,0)$:
  $$\vec{r} - \vec{r}' = \vec{0} - (x\,\hat{i} + R\,\hat{j}) = -x\,\hat{i} - R\,\hat{j}$$
- Distancia al origen:
  $$|\vec{r} - \vec{r}'| = \sqrt{x^2 + R^2}$$
- Diferencial de campo eléctrico en el origen:
  $$d\vec{E}_1 = k \frac{dq}{|\vec{r} - \vec{r}'|^3}(\vec{r} - \vec{r}') = k \lambda\,dx\,\frac{-x\,\hat{i} - R\,\hat{j}}{(x^2 + R^2)^{3/2}}$$

Integrando sobre toda la semirrecta ($x$ desde $0$ hasta $\infty$):

- **Componente $X$:**
  $$E_{1x} = -k\lambda \int_0^\infty \frac{x\,dx}{(x^2 + R^2)^{3/2}} = -k\lambda \left[ -\frac{1}{\sqrt{x^2 + R^2}} \right]_0^\infty = -k\lambda \left( 0 - \left(-\frac{1}{R}\right) \right) = -\frac{k\lambda}{R}$$
- **Componente $Y$:**
  $$E_{1y} = -k\lambda R \int_0^\infty \frac{dx}{(x^2 + R^2)^{3/2}}$$
  Usando la sustitución trigonométrica $x = R\tan\theta$, $dx = R\sec^2\theta\,d\theta$, o la primitiva estándar $\int \frac{dx}{(x^2+R^2)^{3/2}} = \frac{x}{R^2\sqrt{x^2+R^2}}$:
  $$E_{1y} = -k\lambda R \left[ \frac{x}{R^2 \sqrt{x^2 + R^2}} \right]_0^\infty = -k\lambda R \left( \frac{1}{R^2} - 0 \right) = -\frac{k\lambda}{R}$$

Por lo tanto:
$$\vec{E}_1 = -\frac{k\lambda}{R}\,\hat{i} - \frac{k\lambda}{R}\,\hat{j}$$

---

#### 2. Tramo 3: Semirrecta inferior ($y = -R$, $x \in [0, \infty)$)

- Posición de un elemento de carga $dq = \lambda dx$:
  $$\vec{r}' = x\,\hat{i} - R\,\hat{j}$$
- Vector hacia el origen:
  $$\vec{r} - \vec{r}' = -x\,\hat{i} + R\,\hat{j}$$

Por simetría directa respecto al eje $X$, la componente horizontal es idéntica y la componente vertical tiene signo contrario:
$$E_{3x} = -\frac{k\lambda}{R}$$
$$E_{3y} = +\frac{k\lambda}{R}$$

Por lo tanto:
$$\vec{E}_3 = -\frac{k\lambda}{R}\,\hat{i} + \frac{k\lambda}{R}\,\hat{j}$$

---

#### 3. Suma de los dos tramos rectos

Al sumar las contribuciones de las dos semirrectas horizontales:
$$\vec{E}_{\text{rectas}} = \vec{E}_1 + \vec{E}_3 = \left(-\frac{k\lambda}{R} - \frac{k\lambda}{R}\right)\hat{i} + \left(-\frac{k\lambda}{R} + \frac{k\lambda}{R}\right)\hat{j} = -\frac{2k\lambda}{R}\,\hat{i}$$

Las componentes verticales se cancelan y las horizontales se refuerzan en dirección $-\hat{i}$.

---

#### 4. Tramo 2: Arco semicircular (radio $R$, semiplano $x \le 0$)

Parametrizamos en coordenadas polares con el ángulo estándar $\theta$ medido desde el semieje $+X$:
El semicírculo se extiende desde $\theta = \frac{\pi}{2}$ hasta $\theta = \frac{3\pi}{2}$:
- Posición del elemento diferencial:
  $$\vec{r}' = R\cos\theta\,\hat{i} + R\sin\theta\,\hat{j}$$
- Elemento de longitud de arco y carga:
  $$ds = R\,d\theta \implies dq = \lambda R\,d\theta$$
- Vector hacia el origen:
  $$\vec{r} - \vec{r}' = -R\cos\theta\,\hat{i} - R\sin\theta\,\hat{j}$$
- Distancia constante: $|\vec{r} - \vec{r}'| = R$.

El diferencial de campo eléctrico en el origen es:
$$d\vec{E}_2 = \frac{k\,dq}{R^2} \left(\frac{\vec{r} - \vec{r}'}{R}\right) = \frac{k(\lambda R\,d\theta)}{R^2} \left(-\cos\theta\,\hat{i} - \sin\theta\,\hat{j}\right) = \frac{k\lambda}{R} \left(-\cos\theta\,\hat{i} - \sin\theta\,\hat{j}\right)d\theta$$

Integrando entre $\theta = \pi/2$ y $\theta = 3\pi/2$:

- **Componente $X$:**
  $$E_{2x} = \frac{k\lambda}{R} \int_{\pi/2}^{3\pi/2} (-\cos\theta)\,d\theta = -\frac{k\lambda}{R} \Big[ \sin\theta \Big]_{\pi/2}^{3\pi/2} = -\frac{k\lambda}{R} \Big( (-1) - (1) \Big) = -\frac{k\lambda}{R}(-2) = +\frac{2k\lambda}{R}$$
- **Componente $Y$:**
  $$E_{2y} = \frac{k\lambda}{R} \int_{\pi/2}^{3\pi/2} (-\sin\theta)\,d\theta = \frac{k\lambda}{R} \Big[ \cos\theta \Big]_{\pi/2}^{3\pi/2} = \frac{k\lambda}{R} (0 - 0) = 0$$

Por lo tanto:
$$\vec{E}_2 = +\frac{2k\lambda}{R}\,\hat{i}$$

> **Nota:** En la pauta manuscrita oficial (página 7), el integrando para la componente $X$ del semicírculo se escribió inicialmente con signo positivo en el coseno ($E_x = \int \frac{k\lambda R\cos\theta d\theta}{R^2}$), lo cual matemáticamente da un resultado negativo $(-2k\lambda/R)$; sin embargo, el ayudante corrigió el signo al final a $+2k\lambda/R\,\hat{i}$ para coincidir con la física del problema (la carga positiva ubicada a la izquierda en $x < 0$ repele alejando hacia la derecha, es decir, en $+\hat{i}$). Planteando correctamente el vector de posición relativa $\vec{r} - \vec{r}' = -R\cos\theta\,\hat{i}$, el signo positivo surge de forma natural.

---

#### 5. Campo eléctrico total en el origen

Sumando las tres contribuciones:
$$\vec{E}(0,0) = \vec{E}_1 + \vec{E}_2 + \vec{E}_3$$
$$\vec{E}(0,0) = \left(-\frac{k\lambda}{R}\,\hat{i} - \frac{k\lambda}{R}\,\hat{j}\right) + \left(+\frac{2k\lambda}{R}\,\hat{i}\right) + \left(-\frac{k\lambda}{R}\,\hat{i} + \frac{k\lambda}{R}\,\hat{j}\right)$$

Agrupando por componentes:
$$\vec{E}(0,0) = \left(-\frac{k\lambda}{R} + \frac{2k\lambda}{R} - \frac{k\lambda}{R}\right)\hat{i} + \left(-\frac{k\lambda}{R} + 0 + \frac{k\lambda}{R}\right)\hat{j} = 0\,\hat{i} + 0\,\hat{j} = \vec{0}$$

$$\boxed{\vec{E}(0,0) = \vec{0}}$$

**Verificación:**
- **Simetría física:** El campo generado por las dos semirrectas ubicadas a la derecha ($x > 0$) empuja hacia la izquierda ($-\hat{i}$), con una magnitud combinada de $2k\lambda/R$. El semicírculo de radio $R$ ubicado a la izquierda ($x < 0$) empuja simétricamente hacia la derecha ($+\hat{i}$) con exactamente la misma magnitud de $2k\lambda/R$. Las fuerzas se equilibran exactamente en el origen, dando un campo nulo.
- **Unidades:** $[k\lambda/R] = \frac{\text{N}\cdot\text{m}^2/\text{C}^2 \cdot \text{C/m}}{\text{m}} = \text{N/C}$, dimensionalmente consistente.

---

## Resumen de resultados

| Problema | Pregunta / Magnitud | Resultado final |
| :--- | :--- | :--- |
| **Problema 1** | Cargas $q_1$ y $q_2$ | $q_1 = +6{,}17 \times 10^{-8}\text{ C} = +61{,}7\text{ nC}$<br>$q_2 = -6{,}17 \times 10^{-8}\text{ C} = -61{,}7\text{ nC}$ |
| **Problema 2** | **a)** Magnitud del campo eléctrico $E$ | $E = 364\text{ N/C}$ |
| | **b)** Desplazamiento y choque del protón | No golpea ninguna placa;<br>$\|\Delta y_p\| \approx 2{,}73 \times 10^{-6}\text{ m} = 2{,}73\,\mu\text{m}$ hacia abajo ($-\hat{j}$) |
| | **c)** Rapidez del electrón al salir | $v \approx 1{,}79 \times 10^6\text{ m/s}$ |
| **Problema 3** | Campo eléctrico dipolar en $P(x,0)$ | $\vec{E}(P) = -\dfrac{q d}{4\pi\varepsilon_0 \left(x^2 + \dfrac{d^2}{4}\right)^{3/2}}\,\hat{j}$ |
| **Problema 4** | Campo eléctrico en el origen $\vec{E}(0,0)$ | $\vec{E}(0,0) = \vec{0}$ |
