# Ayudantía 10 — Dieléctricos y dipolos

> Clases relacionadas: [Clase 05 - Potencial electroestático](../../Clases/markdown/Clase%2005%20-%20Potencial%20electroest%C3%A1tico.md), [Clase 06 - Condensadores](../../Clases/markdown/Clase%2006%20-%20Condensadores.md), [Clase 07 - Dieléctricos](../../Clases/markdown/Clase%2007%20-%20Diel%C3%A9ctricos.md)

---

## Problema 1

Calcular la capacidad del condensador de la figura, suponiendo que la placa intermedia posee una discontinuidad en el medio.

> **[Figura]:** Condensador de placas planas paralelas rectangulares con separación total $d_1 + d_2$. El volumen entre las armaduras exteriores se encuentra dividido en cuatro cuadrantes:
> - Región superior izquierda: espesor $d_1$, área $S_1$, con dieléctrico de constante $\kappa_1$.
> - Región inferior izquierda: espesor $d_2$, área $S_1$, con dieléctrico de constante $\kappa_2$.
> - Región superior derecha: espesor $d_1$, área $S_2$, vacía ($\kappa = 1$).
> - Región inferior derecha: espesor $d_2$, área $S_2$, con dieléctrico de constante $\kappa_3$.
> En el plano intermedio (en la cota $z = d_2$) existe una discontinuidad física (hendidura o corte longitudinal) que aísla eléctricamente el estrato izquierdo del estrato derecho.

### Solución

**Idea:** La existencia de la discontinuidad intermedia impide que circule carga entre la mitad izquierda y la derecha a través de dicha interfaz. Las armaduras superior e inferior son conductoras continuas, por lo que imponen la misma diferencia de potencial global $\Delta V$ a ambas mitades. El sistema se descompone como dos ramas conectadas en paralelo: la rama izquierda (área $S_1$) y la rama derecha (área $S_2$). En cada rama, los dos estratos dieléctricos apilados verticalmente actúan como condensadores conectados en serie.

#### 1. Rama izquierda (área $S_1$)
La mitad izquierda está conformada por dos condensadores en serie de área de placa común $S_1$:
- Capa superior: espesor $d_1$, constante dieléctrica $\kappa_1$:
  $$C_1 = \frac{\varepsilon_0 \kappa_1 S_1}{d_1}$$
- Capa inferior: espesor $d_2$, constante dieléctrica $\kappa_2$:
  $$C_2 = \frac{\varepsilon_0 \kappa_2 S_1}{d_2}$$

La capacitancia equivalente $C_{\text{eq}, 1}$ de la rama izquierda satisface:
$$\frac{1}{C_{\text{eq}, 1}} = \frac{1}{C_1} + \frac{1}{C_2} = \frac{d_1}{\varepsilon_0 \kappa_1 S_1} + \frac{d_2}{\varepsilon_0 \kappa_2 S_1} = \frac{1}{\varepsilon_0 S_1} \left(\frac{d_1}{\kappa_1} + \frac{d_2}{\kappa_2}\right)$$
$$\frac{1}{C_{\text{eq}, 1}} = \frac{d_1 \kappa_2 + d_2 \kappa_1}{\varepsilon_0 \kappa_1 \kappa_2 S_1}$$

Invirtiendo:
$$C_{\text{eq}, 1} = \frac{\kappa_1 \kappa_2 \varepsilon_0 S_1}{d_1 \kappa_2 + d_2 \kappa_1}$$

#### 2. Rama derecha (área $S_2$)
La mitad derecha está conformada por dos condensadores en serie de área común $S_2$:
- Capa superior (vacío, $\kappa = 1$): espesor $d_1$:
  $$C_3 = \frac{\varepsilon_0 S_2}{d_1}$$
- Capa inferior: espesor $d_2$, constante dieléctrica $\kappa_3$:
  $$C_4 = \frac{\varepsilon_0 \kappa_3 S_2}{d_2}$$

La capacitancia equivalente $C_{\text{eq}, 2}$ de la rama derecha es:
$$\frac{1}{C_{\text{eq}, 2}} = \frac{1}{C_3} + \frac{1}{C_4} = \frac{d_1}{\varepsilon_0 S_2} + \frac{d_2}{\varepsilon_0 \kappa_3 S_2} = \frac{1}{\varepsilon_0 S_2} \left(d_1 + \frac{d_2}{\kappa_3}\right) = \frac{d_1 \kappa_3 + d_2}{\varepsilon_0 \kappa_3 S_2}$$

Invirtiendo:
$$C_{\text{eq}, 2} = \frac{\kappa_3 \varepsilon_0 S_2}{d_1 \kappa_3 + d_2}$$

> **Nota:** En el manuscrito original (página 2, parte superior), el autor escribió transitoriamente $\kappa_2$ en lugar de $\kappa_3$ en el primer renglón del planteamiento de $1/C_{\text{eq}, 2}$; sin embargo, corrigió dicho lapsus en la expresión final del resultado global, restituyendo correctamente la dependencia en $\kappa_3$.

#### 3. Capacitancia total del sistema
Como ambas ramas comparten los mismos conductores externos a potenciales $V_{\text{sup}}$ y $V_{\text{inf}}$, están asociadas en paralelo:
$$C_{\text{eq}} = C_{\text{eq}, 1} + C_{\text{eq}, 2}$$

$$\boxed{C_{\text{eq}} = \frac{\kappa_1 \kappa_2 \varepsilon_0 S_1}{d_1 \kappa_2 + d_2 \kappa_1} + \frac{\kappa_3 \varepsilon_0 S_2}{d_1 \kappa_3 + d_2}}$$

**Verificación:**
- **Límite de vacío homogéneo:** Si $\kappa_1 = \kappa_2 = \kappa_3 = 1$, se obtiene:
  $$C_{\text{eq}, 1} = \frac{\varepsilon_0 S_1}{d_1 + d_2}, \qquad C_{\text{eq}, 2} = \frac{\varepsilon_0 S_2}{d_1 + d_2}$$
  $$C_{\text{eq}} = \frac{\varepsilon_0 (S_1 + S_2)}{d_1 + d_2}$$
  que coincide exactamente con la capacitancia de un condensador plano homogéneo de área total $S_1 + S_2$ y distancia entre placas $d_1 + d_2$.

---

## Problema 2

Se tiene un condensador plano con placas cuadradas de largo $a$ y distancia $d$ entre las placas y una carga total $Q$. Calcular la fuerza que se ejerce sobre un material dieléctrico cuando se encuentra a una distancia $x$ del punto O.

> **[Figura]:** Condensador plano de placas paralelas cuadradas de lado $a$ (área $a^2$), separadas por una distancia $d$. El condensador se encuentra aislado, con carga total $+Q$ en la placa superior y $-Q$ en la placa inferior. El punto $O$ denota el borde izquierdo de las placas. Un bloque dieléctrico de permitividad relativa $\kappa$, espesor $d$ y ancho $a$ se introduce horizontalmente entre las placas. La coordenada $x$ mide la distancia horizontal desde el borde izquierdo $O$ hasta el extremo frontal del dieléctrico. Por tanto, la sección no ocupada por el dieléctrico (vacío) tiene longitud $x$, y la sección ocupada por el dieléctrico tiene longitud $a - x$.

### Solución

**Idea:** Para un sistema aislado a carga constante ($Q = \text{cte}$), la fuerza electrostática ejercida sobre el dieléctrico se obtiene derivando la energía potencial electrostática respecto a la coordenada de desplazamiento: $\vec{F} = -\nabla U = -\frac{dU}{dx}\,\hat{i}$. Como la diferencia de potencial es la misma a lo largo de las placas conductoras, el condensador parcialmente lleno se modela como dos condensadores en paralelo: uno con vacío de largo $x$ y otro con dieléctrico de largo $a - x$.

#### 1. Capacitancia en función de la posición $x$

Las placas tienen dimensiones $a \times a$. Al estar el dieléctrico insertado una distancia $a - x$:
- **Región con vacío ($0 \le z \le x$):** área transversal $A_{\text{vacío}} = a \cdot x$, espesor $d$:
  $$C_{\text{vacío}} = \frac{\varepsilon_0 A_{\text{vacío}}}{d} = \frac{\varepsilon_0 a x}{d}$$
- **Región con dieléctrico ($x \le z \le a$):** área transversal $A_\kappa = a \cdot (a - x)$, espesor $d$:
  $$C_\kappa = \frac{\varepsilon_0 \kappa A_\kappa}{d} = \frac{\varepsilon_0 \kappa a (a - x)}{d}$$

Al estar en paralelo:
$$C(x) = C_{\text{vacío}} + C_\kappa = \frac{\varepsilon_0 a x}{d} + \frac{\varepsilon_0 \kappa a (a - x)}{d} = \frac{\varepsilon_0 a}{d} \left[x + \kappa(a - x)\right]$$

Reagrupando términos:
$$C(x) = \frac{\varepsilon_0 a}{d} \left[\kappa a - (\kappa - 1)x\right]$$

#### 2. Energía potencial electrostática
Dado que el condensador está desconectado y aislado, la carga libre $Q$ permanece estrictamente constante ($Q = \text{cte}$). La energía electrostática almacenada es:
$$U(x) = \frac{1}{2}\frac{Q^2}{C(x)} = \frac{1}{2}\frac{Q^2 d}{\varepsilon_0 a \left[x + \kappa(a - x)\right]}$$

#### 3. Fuerza sobre el dieléctrico
La fuerza electrostática ejercida sobre el dieléctrico es:
$$F_x = -\frac{dU}{dx}$$

Derivando $U(x)$ respecto a $x$:
$$\frac{dU}{dx} = \frac{d}{dx} \left\{\frac{Q^2 d}{2\varepsilon_0 a} \left[x + \kappa a - \kappa x\right]^{-1}\right\}$$
$$\frac{dU}{dx} = \frac{Q^2 d}{2\varepsilon_0 a} (-1)\left[x + \kappa(a - x)\right]^{-2} \cdot \frac{d}{dx}\left[x(1 - \kappa) + \kappa a\right]$$
$$\frac{dU}{dx} = - \frac{Q^2 d}{2\varepsilon_0 a [x + \kappa(a - x)]^2} (1 - \kappa) = \frac{Q^2 d (\kappa - 1)}{2\varepsilon_0 a [x + \kappa(a - x)]^2}$$

Aplicando el signo negativo de la fuerza:
$$F_x = - \frac{dU}{dx} = - \frac{Q^2 d (\kappa - 1)}{2\varepsilon_0 a [x + \kappa(a - x)]^2}$$

En forma vectorial:
$$\boxed{\vec{F} = - \frac{Q^2 d (\kappa - 1)}{2\varepsilon_0 a [x + \kappa(a - x)]^2}\,\hat{i}}$$

**Interpretación física:**
- Dado que para cualquier dieléctrico real $\kappa > 1$, se tiene $(\kappa - 1) > 0$, de modo que $F_x < 0$.
- La fuerza apunta en sentido $-\hat{i}$, es decir, hacia el interior del condensador (hacia donde disminuye $x$ y aumenta la porción insertada del dieléctrico).
- El sistema busca espontáneamente minimizar su energía potencial electrostática; a carga constante, $U \propto 1/C$, por lo que la energía disminuye al maximizar la capacitancia $C$, lo cual ocurre cuando el dieléctrico es succionado hacia el interior.

---

## Problema 3

Calcule el potencial de interacción entre dos dipolos ubicados en $\vec{r}_1$ y $\vec{r}_2$. Calcule la fuerza entre los dipolos.

> **[Figura]:** Plano de coordenadas cartesianas $XY$. Dos momentos dipolares eléctricos ideales $\vec{p}_1$ y $\vec{p}_2$ orientados arbitrariamente en el espacio, situados en las posiciones vectoriales $\vec{r}_1$ y $\vec{r}_2$ respecto al origen. El vector que une el dipolo 1 con el dipolo 2 es $\vec{r}_{21} = \vec{r}_2 - \vec{r}_1$, con magnitud $r = |\vec{r}_{21}|$.

### Solución

**Idea:** Un dipolo ideal puntual $\vec{p}_1$ situado en $\vec{r}_1$ produce un potencial electrostático en el espacio. El campo eléctrico $\vec{E}_1(\vec{r})$ se calcula mediante el gradiente $\vec{E} = -\nabla V$. La energía potencial electrostática (potencial de interacción) de un segundo dipolo $\vec{p}_2$ inmerso en este campo es $U = -\vec{p}_2 \cdot \vec{E}_1(\vec{r}_2)$. Finalmente, la fuerza electrostática neta ejercida sobre el segundo dipolo se obtiene a través del gradiente de la energía respecto a la posición del dipolo 2: $\vec{F}_{21} = -\nabla_{\vec{r}_2} U$.

#### 1. Potencial y campo eléctrico producido por el dipolo 1
El potencial dipolar generado por $\vec{p}_1$ en un punto arbitrario $\vec{r}$ es:
$$V(\vec{r}) = \frac{1}{4\pi \varepsilon_0} \frac{\vec{p}_1 \cdot (\vec{r} - \vec{r}_1)}{|\vec{r} - \vec{r}_1|^3}$$

El campo eléctrico corresponde a $\vec{E}(\vec{r}) = -\nabla V(\vec{r})$. Aplicando la regla del producto para el operador gradiente $\nabla(fg) = (\nabla f)g + f(\nabla g)$ con $f(\vec{r}) = \vec{p}_1 \cdot (\vec{r} - \vec{r}_1)$ y $g(\vec{r}) = |\vec{r} - \vec{r}_1|^{-3}$:
1. $\nabla \left[\vec{p}_1 \cdot (\vec{r} - \vec{r}_1)\right] = \vec{p}_1$ (dado que $\vec{p}_1$ y $\vec{r}_1$ son constantes).
2. Para $g = r'^{-3}$ donde $\vec{r}' = \vec{r} - \vec{r}_1$ y $r' = |\vec{r}'|$:
   $$\nabla (r'^{-3}) = -3 r'^{-4} \nabla(r') = -3 r'^{-4} \frac{\vec{r}'}{r'} = -3 \frac{\vec{r} - \vec{r}_1}{|\vec{r} - \vec{r}_1|^5}$$

Por lo tanto:
$$\nabla V(\vec{r}) = \frac{1}{4\pi \varepsilon_0} \left[\frac{\vec{p}_1}{|\vec{r} - \vec{r}_1|^3} - \frac{3\left[\vec{p}_1 \cdot (\vec{r} - \vec{r}_1)\right](\vec{r} - \vec{r}_1)}{|\vec{r} - \vec{r}_1|^5}\right]$$

Tomando el negativo, el campo eléctrico es:
$$\vec{E}_1(\vec{r}) = \frac{1}{4\pi \varepsilon_0} \left[\frac{3\left[\vec{p}_1 \cdot (\vec{r} - \vec{r}_1)\right](\vec{r} - \vec{r}_1)}{|\vec{r} - \vec{r}_1|^5} - \frac{\vec{p}_1}{|\vec{r} - \vec{r}_1|^3}\right]$$

#### 2. Potencial (energía) de interacción entre los dipolos
Evaluamos el campo generado por el dipolo 1 en la posición del dipolo 2 ($\vec{r} = \vec{r}_2$).  
Definimos el vector de desplazamiento relativo:
$$\vec{r}_{21} = \vec{r}_2 - \vec{r}_1, \qquad r = |\vec{r}_{21}|$$

El campo eléctrico en dicha posición es:
$$\vec{E}_1(\vec{r}_2) = \frac{1}{4\pi \varepsilon_0} \left[\frac{3(\vec{p}_1 \cdot \vec{r}_{21})\vec{r}_{21}}{r^5} - \frac{\vec{p}_1}{r^3}\right]$$

La energía de interacción entre ambos dipolos está dada por:
$$U = -\vec{p}_2 \cdot \vec{E}_1(\vec{r}_2) = - \vec{p}_2 \cdot \left\{\frac{1}{4\pi \varepsilon_0} \left[\frac{3(\vec{p}_1 \cdot \vec{r}_{21})\vec{r}_{21}}{r^5} - \frac{\vec{p}_1}{r^3}\right]\right\}$$

Distribuyendo el producto escalar:
$$\boxed{U = \frac{1}{4\pi \varepsilon_0} \left[\frac{\vec{p}_1 \cdot \vec{p}_2}{r^3} - \frac{3(\vec{p}_1 \cdot \vec{r}_{21})(\vec{p}_2 \cdot \vec{r}_{21})}{r^5}\right]}$$

Nótese que esta expresión es estrictamente simétrica ante el intercambio de los índices $1 \leftrightarrow 2$, ya que al intercambiar los dipolos $\vec{r}_{12} = -\vec{r}_{21}$, y el producto $(-\vec{p}_2 \cdot \vec{r}_{21})(-\vec{p}_1 \cdot \vec{r}_{21}) = (\vec{p}_1 \cdot \vec{r}_{21})(\vec{p}_2 \cdot \vec{r}_{21})$ permanece invariante.

#### 3. Fuerza entre los dipolos
La fuerza que ejerce el dipolo 1 sobre el dipolo 2 se obtiene mediante el gradiente negativo de la energía respecto a la posición del dipolo 2 ($\nabla_2 \equiv \nabla_{\vec{r}_2}$):
$$\vec{F}_{21} = -\nabla_2 U = -\frac{1}{4\pi \varepsilon_0} \left[\nabla_2 \left(\frac{\vec{p}_1 \cdot \vec{p}_2}{r^3}\right) - \nabla_2 \left(\frac{3(\vec{p}_1 \cdot \vec{r}_{21})(\vec{p}_2 \cdot \vec{r}_{21})}{r^5}\right)\right]$$

Calculamos ambos términos separadamente:

##### Primer término:
Como $\vec{p}_1$ y $\vec{p}_2$ son momentos dipolares intrínsecos constantes:
$$\nabla_2 \left(\frac{\vec{p}_1 \cdot \vec{p}_2}{r^3}\right) = (\vec{p}_1 \cdot \vec{p}_2) \nabla_2 (r^{-3}) = (\vec{p}_1 \cdot \vec{p}_2) \left(-3 r^{-4} \frac{\vec{r}_{21}}{r}\right) = - \frac{3(\vec{p}_1 \cdot \vec{p}_2)\vec{r}_{21}}{r^5}$$

##### Segundo término:
Sea $f(\vec{r}_2) = 3(\vec{p}_1 \cdot \vec{r}_{21})(\vec{p}_2 \cdot \vec{r}_{21})$ y $g(\vec{r}_2) = r^{-5}$. Aplicando la regla del producto $\nabla(fg) = (\nabla f)g + f(\nabla g)$:
- Gradiente de $f$:
  $$\nabla_2 (\vec{p}_1 \cdot \vec{r}_{21}) = \vec{p}_1, \qquad \nabla_2 (\vec{p}_2 \cdot \vec{r}_{21}) = \vec{p}_2$$
  $$\nabla_2 f = 3 \left[\vec{p}_1 (\vec{p}_2 \cdot \vec{r}_{21}) + (\vec{p}_1 \cdot \vec{r}_{21}) \vec{p}_2\right]$$
- Gradiente de $g$:
  $$\nabla_2 (r^{-5}) = -5 r^{-6} \frac{\vec{r}_{21}}{r} = - \frac{5\vec{r}_{21}}{r^7}$$

Por tanto:
$$\nabla_2(fg) = \frac{3\left[\vec{p}_1 (\vec{p}_2 \cdot \vec{r}_{21}) + \vec{p}_2 (\vec{p}_1 \cdot \vec{r}_{21})\right]}{r^5} - \frac{15(\vec{p}_1 \cdot \vec{r}_{21})(\vec{p}_2 \cdot \vec{r}_{21})\vec{r}_{21}}{r^7}$$

##### Sustitución en la fuerza:
$$\vec{F}_{21} = -\frac{1}{4\pi \varepsilon_0} \left\{ - \frac{3(\vec{p}_1 \cdot \vec{p}_2)\vec{r}_{21}}{r^5} - \left[\frac{3\left[\vec{p}_1 (\vec{p}_2 \cdot \vec{r}_{21}) + \vec{p}_2 (\vec{p}_1 \cdot \vec{r}_{21})\right]}{r^5} - \frac{15(\vec{p}_1 \cdot \vec{r}_{21})(\vec{p}_2 \cdot \vec{r}_{21})\vec{r}_{21}}{r^7}\right]\right\}$$

Distribuyendo el signo menos global y factorizando $+ \dfrac{3}{4\pi \varepsilon_0}$:
$$\boxed{\vec{F}_{21} = \frac{3}{4\pi \varepsilon_0} \left[\frac{(\vec{p}_1 \cdot \vec{p}_2)\vec{r}_{21} + \vec{p}_1 (\vec{p}_2 \cdot \vec{r}_{21}) + \vec{p}_2 (\vec{p}_1 \cdot \vec{r}_{21})}{r^5} - \frac{5(\vec{p}_1 \cdot \vec{r}_{21})(\vec{p}_2 \cdot \vec{r}_{21})\vec{r}_{21}}{r^7}\right]}$$

**Verificación:**
- **Tercera ley de Newton:** La fuerza que el dipolo 2 ejerce sobre el dipolo 1 es $\vec{F}_{12} = -\nabla_{\vec{r}_1} U$. Puesto que $\nabla_{\vec{r}_1} = -\nabla_{\vec{r}_2}$, se verifica de forma idéntica que $\vec{F}_{12} = -\vec{F}_{21}$, cumpliendo rigurosamente el principio de acción y reacción.
- **Caso colineal:** Si ambos dipolos están alineados a lo largo del eje que los une ($\vec{p}_1 = p_1\,\hat{r}$, $\vec{p}_2 = p_2\,\hat{r}$):
  $$U = \frac{1}{4\pi \varepsilon_0}\left[\frac{p_1 p_2}{r^3} - \frac{3 p_1 p_2}{r^3}\right] = - \frac{2 p_1 p_2}{4\pi \varepsilon_0 r^3}$$
  $$\vec{F}_{21} = -\frac{dU}{dr}\,\hat{r} = - \frac{6 p_1 p_2}{4\pi \varepsilon_0 r^4}\,\hat{r}$$
  Evaluando la fórmula general con $\vec{r}_{21} = r\hat{r}$:
  $$\vec{F}_{21} = \frac{3}{4\pi \varepsilon_0} \left[\frac{p_1 p_2 r + p_1(p_2 r) + p_2(p_1 r)}{r^5} - \frac{5(p_1 r)(p_2 r)r}{r^7}\right]\hat{r} = \frac{3}{4\pi \varepsilon_0}\left[\frac{3 p_1 p_2}{r^4} - \frac{5 p_1 p_2}{r^4}\right]\hat{r} = - \frac{6 p_1 p_2}{4\pi \varepsilon_0 r^4}\,\hat{r}$$
  lo que coincide exactamente, confirmando que dipolos alineados se atraen con una fuerza proporcional a $1/r^4$.

---

## Resumen de resultados

| Problema / Inciso | Descripción | Resultado final |
| :--- | :--- | :--- |
| **Problema 1** | Capacitancia con placa intermedia discontinua | $C_{\text{eq}} = \dfrac{\kappa_1 \kappa_2 \varepsilon_0 S_1}{d_1 \kappa_2 + d_2 \kappa_1} + \dfrac{\kappa_3 \varepsilon_0 S_2}{d_1 \kappa_3 + d_2}$ |
| **Problema 2** | Fuerza sobre dieléctrico insertado | $\vec{F} = - \dfrac{Q^2 d (\kappa - 1)}{2\varepsilon_0 a [x + \kappa(a - x)]^2}\,\hat{i}$ |
| **Problema 3** | Potencial de interacción (energía) dipolar | $U = \dfrac{1}{4\pi \varepsilon_0}\left[\dfrac{\vec{p}_1 \cdot \vec{p}_2}{r^3} - \dfrac{3(\vec{p}_1 \cdot \vec{r}_{21})(\vec{p}_2 \cdot \vec{r}_{21})}{r^5}\right]$ |
| **Problema 3** | Fuerza electrostática entre los dipolos | $\vec{F}_{21} = \dfrac{3}{4\pi \varepsilon_0}\left[\dfrac{(\vec{p}_1 \cdot \vec{p}_2)\vec{r}_{21} + \vec{p}_1(\vec{p}_2 \cdot \vec{r}_{21}) + \vec{p}_2(\vec{p}_1 \cdot \vec{r}_{21})}{r^5} - \dfrac{5(\vec{p}_1 \cdot \vec{r}_{21})(\vec{p}_2 \cdot \vec{r}_{21})\vec{r}_{21}}{r^7}\right]$ |
