# Ayudantía 21 — Ley de Faraday-Lenz

> Clases relacionadas: [Clase 12 - Ley de Ampere](../../Clases/markdown/Clase%2012%20-%20Ley%20de%20Ampere.md), [Clase 13 - Inducción Magnética](../../Clases/markdown/Clase%2013%20-%20Inducci%C3%B3n%20Magn%C3%A9tica.md)

---

## Problema 1

Si una espira rectangular de lados $a$ y $b$ se aleja con velocidad constante $\vec{v}$ de un alambre infinito por el que circula una corriente $I$, como se muestra en la figura, determine la fuerza electromotriz inducida en la espira como función del tiempo. Suponga que en $t = 0$, la distancia del lado más cercano de la espira al alambre es $r = h$.

> **[Figura]:** Alambre recto infinito sobre el eje vertical $Z$ por el que circula una corriente estacionaria $I$ en sentido positivo ($+\hat{z}$). El eje horizontal $X$ es perpendicular al alambre y apunta hacia la derecha. En el plano $XZ$ (plano de la hoja) se sitúa una espira rectangular con dimensiones $a$ (ancho horizontal en $x$) y $b$ (alto vertical en $z$, paralelo al alambre). La espira se aleja horizontalmente del alambre con vector velocidad constante $\vec{v} = v\,\hat{x}$. En $t = 0$, la distancia entre el alambre y el lado vertical más cercano es $x = h$, por lo que la posición instantánea de dicho lado es $r(t) = h + vt$, y la del lado más alejado es $r(t) + a = h + a + vt$. En todo el semiplano $x > 0$, el campo magnético $\vec{B}$ producido por la corriente entra perpendicularmente al plano de la hoja ($\otimes$, dirección $-\hat{y}$).

### Solución

**Idea:** La corriente constante que circula por el alambre recto genera un campo magnético estático e inhomogeneous que decae inversamente con la distancia radial $x$. Al desplazarse la espira con velocidad constante $\vec{v}$, el área permanece constante pero el campo magnético medio sobre ella varía con el tiempo, modificando el flujo magnético $\Phi_B(t)$ enlazado. Por la ley de Faraday-Lenz, dicha variación temporal induce una fuerza electromotriz (fem) dada por $\mathcal{E} = -\frac{d\Phi_B}{dt}$. El sentido de circulación de la corriente inducida se determina mediante la ley de Lenz.

---

#### 1. Campo magnético producido por el alambre rectilíneo

Aplicando la ley de Ampère a una circunferencia concéntrica de radio $x$ perpendicular al alambre:
$$\oint \vec{B} \cdot d\vec{\ell} = B(x) \cdot 2\pi x = \mu_0 I_{\text{enc}} = \mu_0 I \implies B(x) = \frac{\mu_0 I}{2\pi x}$$

Por la regla de la mano derecha con corriente en $+\hat{z}$, en la región $x > 0$ del plano de la espira el campo apunta hacia el interior de la página (dirección $-\hat{y}$):
$$\vec{B}(x) = -\frac{\mu_0 I}{2\pi x}\,\hat{y}$$

---

#### 2. Cinemática de la espira y flujo magnético

La espira realiza un movimiento rectilíneo uniforme (MRU) con rapidez constante $v$:
- Posición del lado vertical más cercano: $x_{\text{cercano}}(t) = h + vt$.
- Posición del lado vertical más lejano: $x_{\text{lejano}}(t) = h + a + vt$.

Tomando como vector normal a la superficie de la espira la dirección que entra a la hoja, $d\vec{A} = b\,dx(-\hat{y})$:
$$\Phi_B(t) = \int_{\text{espira}} \vec{B} \cdot d\vec{A} = \int_{h+vt}^{h+a+vt} \left(\frac{\mu_0 I}{2\pi x}\right) b\,dx$$
$$\Phi_B(t) = \frac{\mu_0 I b}{2\pi} \int_{h+vt}^{h+a+vt} \frac{dx}{x} = \frac{\mu_0 I b}{2\pi} \Big[ \ln(x) \Big]_{h+vt}^{h+a+vt}$$
$$\Phi_B(t) = \frac{\mu_0 I b}{2\pi} \ln\left( \frac{h+a+vt}{h+vt} \right)$$

---

#### 3. Cálculo de la fuerza electromotriz inducida

Por la ley de Faraday-Lenz:
$$\mathcal{E}(t) = -\frac{d\Phi_B(t)}{dt}$$

Derivamos el término logarítmico con respecto al tiempo:
$$\frac{d}{dt} \left[ \ln(h+a+vt) - \ln(h+vt) \right] = \frac{v}{h+a+vt} - \frac{v}{h+vt} = \frac{v(h+vt) - v(h+a+vt)}{(h+vt)(h+a+vt)} = -\frac{a v}{(h+vt)(h+a+vt)}$$

Sustituyendo en la expresión de la fem:
$$\mathcal{E}(t) = - \frac{\mu_0 I b}{2\pi} \left( -\frac{a v}{(h+vt)(h+a+vt)} \right)$$

$$\boxed{\mathcal{E}(t) = \frac{\mu_0 I a b v}{2\pi (h+vt)(h+a+vt)}}$$

---

#### 4. Sentido de la corriente inducida (Ley de Lenz)

A medida que la espira se aleja del alambre ($v > 0$), la intensidad del campo magnético disminuye progresivamente en cada punto de la espira, haciendo que el flujo magnético hacia el interior de la página ($\otimes$) disminuya con el tiempo ($d\Phi_B/dt < 0$).

De acuerdo con la ley de Lenz, la corriente inducida debe generar un campo magnético inducido $\vec{B}_{\text{ind}}$ que se oponga a dicha disminución, es decir, debe apuntar en el mismo sentido que el campo externo: **hacia adentro de la página ($\otimes$)**.

Por la regla de la mano derecha (pulgar apuntando hacia la hoja), la corriente inducida debe circular en **sentido horario** a lo largo de la espira rectangular:
- Tramo inferior: hacia la derecha ($+\hat{x}$).
- Tramo derecho: hacia abajo ($-\hat{z}$).
- Tramo superior: hacia la izquierda ($-\hat{x}$).
- Tramo izquierdo: hacia arriba ($+\hat{z}$).

**Verificación:**
- **Unidades:**
  $$[\mathcal{E}] = \frac{[\mu_0][I][a][b][v]}{[\text{longitud}]^2} = \frac{(\text{T}\cdot\text{m}/\text{A})(\text{A})(\text{m})(\text{m})(\text{m}/\text{s})}{\text{m}^2} = \frac{\text{T}\cdot\text{m}^2}{\text{s}} = \frac{\text{Wb}}{\text{s}} = \text{V}$$
  Dimensionalmente correcto.
- **Comportamiento asintótico:**
  - Si $v = 0$ (espira en reposo): $\mathcal{E} = 0$, consistente con la ausencia de variación temporal de flujo.
  - Para $t \to \infty$: $\mathcal{E}(t) \propto \frac{1}{t^2} \to 0$, ya que a distancias asintóticamente grandes el gradiente del campo magnético tiende a cero.

---

## Problema 2

Una bobina muy larga de radio $b$ tiene $m$ vueltas por unidad de largo y lleva corriente $I(t) = I_0 \sin(\omega t)$.

1. Encuentre el campo magnético dentro de la bobina.
2. Encuentre el campo eléctrico dentro de la bobina y fuera de la bobina.

> **[Figura]:** Bobina cilíndrica (solenoide ideal) muy larga de radio $b$, con devanado uniforme compacto de $m$ vueltas por unidad de longitud a lo largo del eje $z$. Por las espiras circula una corriente armónica dependiente del tiempo $I(t) = I_0 \sin(\omega t)$ orientada circunferencialmente en dirección azimutal ($\hat{\theta}$).

### Solución

**Idea:** En la aproximación cuasiestática (las dimensiones espaciales son mucho menores que la longitud de onda asociada $\lambda = 2\pi c/\omega$), el campo magnético instantáneo dentro de un solenoide infinito se calcula mediante la ley de Ampère en función del valor instantáneo de la corriente. La tasa de variación temporal de este campo magnético genera un campo eléctrico inducido no conservativo governed por la ley de Faraday en forma integral: $\oint \vec{E} \cdot d\vec{\ell} = -\frac{d\Phi_B}{dt}$. La simetría cilíndrica dicta que las líneas de $\vec{E}$ sean circunferencias concéntricas azimutales.

---

#### 1. Campo magnético dentro de la bobina

Para una bobina muy larga (solenoide ideal de radio $b$ y densidad lineal de espiras $m$), el campo magnético es uniforme y puramente axial en el interior, y nulo en el exterior:
$$\vec{B}_{\text{fuera}} = \vec{0}$$
$$\vec{B}_{\text{dentro}}(t) = B(t)\,\hat{z}$$

Tomamos un lazo amperiano rectangular de longitud $\ell$ paralelo al eje $z$: un tramo vertical de longitud $\ell$ dentro de la bobina, dos tramos radiales perpendiculares al eje, y un tramo de cierre en el exterior (donde $\vec{B} = \vec{0}$).  
Aplicando la ley de Ampère:
$$\oint \vec{B} \cdot d\vec{\ell} = B(t)\cdot \ell = \mu_0 I_{\text{enc}} = \mu_0 (m \ell I(t))$$

Cancelando $\ell$ y reemplazando $I(t) = I_0 \sin(\omega t)$:
$$B(t) = \mu_0 m I_0 \sin(\omega t)$$

En forma vectorial para $r < b$:
$$\boxed{\vec{B}(r < b, t) = \mu_0 m I_0 \sin(\omega t)\,\hat{z}}$$
$$\vec{B}(r > b, t) = \vec{0}$$

---

#### 2. Campo eléctrico dentro y fuera de la bobina

Por simetría cilíndrica, el campo eléctrico inducido es exclusivamente tangencial (azimutal) y depende únicamente de la distancia radial $r$ al eje del solenoide:
$$\vec{E}(r, t) = E(r, t)\,\hat{\theta}$$

Tomamos una curva cerrada circular amperiana $\Gamma$ de radio $r$ concéntrica con el eje del solenoide, con vector tangente $d\vec{\ell} = r\,d\theta\,\hat{\theta}$ y vector normal de superficie $\hat{n} = \hat{z}$:
$$\oint_\Gamma \vec{E} \cdot d\vec{\ell} = E(r, t) \int_0^{2\pi} r\,d\theta = 2\pi r E(r, t)$$

Por la ley de Maxwell-Faraday:
$$2\pi r E(r, t) = -\frac{d\Phi_B}{dt} = -\frac{d}{dt} \iint_S \vec{B} \cdot d\vec{A}$$

Analizamos el flujo según la región:

- **Dentro de la bobina ($r < b$):**  
  Todo el círculo de radio $r$ se encuentra en la región donde el campo magnético es uniforme $\vec{B} = \mu_0 m I_0 \sin(\omega t)\,\hat{z}$:
  $$\Phi_B(r, t) = B(t) \cdot (\pi r^2) = \mu_0 m I_0 \sin(\omega t) \cdot \pi r^2$$
  $$\frac{d\Phi_B}{dt} = \mu_0 m I_0 \pi r^2 \omega \cos(\omega t)$$

  Igualando la circulación al negativo de la derivada del flujo:
  $$2\pi r E(r, t) = -\mu_0 m I_0 \pi r^2 \omega \cos(\omega t)$$
  $$E(r, t) = - \frac{\mu_0 m I_0 \omega r}{2} \cos(\omega t)$$

  Vectorialmente:
  $$\boxed{\vec{E}(r < b, t) = - \frac{\mu_0 m I_0 \omega r}{2} \cos(\omega t)\,\hat{\theta}}$$

- **Fuera de la bobina ($r > b$):**  
  Como el campo magnético es estrictamente nulo fuera de la bobina ($r > b$), el flujo magnético total que atraviesa cualquier circunferencia de radio $r > b$ proviene exclusivamente del área interior del solenoide de radio $b$:
  $$\Phi_B(r, t) = B(t) \cdot (\pi b^2) = \mu_0 m I_0 \sin(\omega t) \cdot \pi b^2$$
  $$\frac{d\Phi_B}{dt} = \mu_0 m I_0 \pi b^2 \omega \cos(\omega t)$$

  Igualando con la circulación a radio $r$:
  $$2\pi r E(r, t) = -\mu_0 m I_0 \pi b^2 \omega \cos(\omega t)$$
  $$E(r, t) = - \frac{\mu_0 m I_0 \omega b^2}{2r} \cos(\omega t)$$

  Vectorialmente:
  $$\boxed{\vec{E}(r > b, t) = - \frac{\mu_0 m I_0 \omega b^2}{2r} \cos(\omega t)\,\hat{\theta}}$$

En resumen:
$$\vec{E}(r, t) = \begin{cases}
- \dfrac{\mu_0 m I_0 \omega r}{2} \cos(\omega t)\,\hat{\theta}, & r < b \\[2ex]
- \dfrac{\mu_0 m I_0 \omega b^2}{2r} \cos(\omega t)\,\hat{\theta}, & r > b
\end{cases}$$

**Verificación:**
- **Continuidad en la frontera $r = b$:**
  - Evaluando el campo interior cuando $r \to b^-$:
    $$E(b^-, t) = -\frac{\mu_0 m I_0 \omega b}{2} \cos(\omega t)$$
  - Evaluando el campo exterior cuando $r \to b^+$:
    $$E(b^+, t) = -\frac{\mu_0 m I_0 \omega b^2}{2b} \cos(\omega t) = -\frac{\mu_0 m I_0 \omega b}{2} \cos(\omega t)$$
  El campo eléctrico tangencial es estrictamente continuo a través de la superficie $r = b$.
- **Unidades:**
  $$[\mu_0 m I_0 \omega r] = \left(\frac{\text{T}\cdot\text{m}}{\text{A}}\right) \left(\frac{1}{\text{m}}\right) (\text{A}) \left(\frac{1}{\text{s}}\right) (\text{m}) = \frac{\text{T}\cdot\text{m}}{\text{s}} = \frac{\text{N}\cdot\text{s}}{\text{C}\cdot\text{m}} \cdot \frac{\text{m}}{\text{s}} = \frac{\text{N}}{\text{C}} = \frac{\text{V}}{\text{m}}$$
  Dimensionalmente correcto.

---

## Problema 3

Una espira rectangular de resistencia $R$, ancho $a$, largo $L$ (muy grande) y de masa $m$ cae bajo efecto de la gravedad bajo un campo magnético $\vec{B}$ perpendicular al plano de la espira y no nulo solo en la parte inferior del plano. Asuma que una parte de la espira siempre está fuera de la región de campo magnético, determine la velocidad terminal y sentido de la corriente inducida en la espira.

> **[Figura]:** Sistema cartesiano con eje horizontal $x$ apuntando a la derecha y eje vertical $y$ apuntando hacia arriba. Una recta horizontal delimita la frontera del campo magnético: para $y < 0$ (zona inferior) existe un campo magnético uniforme y constante perpendicular que entra a la hoja ($\vec{B} = -B\,\hat{z}$); para $y > 0$ (zona superior) el campo magnético es nulo ($\vec{B} = \vec{0}$). Una espira rectangular de masa $m$, resistencia eléctrica total $R$, ancho horizontal $a$ y altura $L$ cae verticalmente debido a la fuerza gravitacional ($\vec{g} = -g\,\hat{y}$). El lado horizontal inferior se encuentra sumergido en la región con campo magnético, mientras que el lado horizontal superior permanece en todo momento en la región libre de campo.

### Solución

**Idea:** A medida que la espira cae acelerada por la gravedad, el área del lazo inmersa en la región con campo magnético aumenta gradualmente, incrementando el flujo magnético hacia el interior de la página. Por la ley de Faraday y la ley de Ohm, esto induce una fuerza electromotriz y una corriente inducida $I_{\text{ind}}$. Por la ley de Lorentz, la corriente que circula horizontalmente por el lado inferior sumergido experimenta una fuerza magnética vertical dirigida hacia arriba ($\vec{F}_m = I \vec{\ell} \times \vec{B}$), que actúa como amortiguamiento magnético oponiéndose al peso. La velocidad terminal $v_t$ se alcanza en el régimen estacionario cuando la fuerza magnética equilibra exactamente a la fuerza de gravedad ($\sum F_y = 0$).

---

#### 1. Flujo magnético y fuerza electromotriz inducida

Sea $y_{\text{in}}(t)$ la longitud vertical de la porción de la espira que se encuentra inmersa dentro del campo magnético en el instante $t$.  
La velocidad instantánea de caída de la espira (rapidez vertical hacia abajo) es:
$$v = \frac{dy_{\text{in}}}{dt} \ge 0$$

El área sumergida de la espira es $A(t) = a \cdot y_{\text{in}}(t)$.  
Tomando la normal a la superficie en el sentido entrante ($\hat{n} = -\hat{z}$), el flujo magnético enlazado es:
$$\Phi_B(t) = \iint \vec{B} \cdot d\vec{A} = (-B\,\hat{z}) \cdot (-a y_{\text{in}}(t)\,\hat{z}) = B a y_{\text{in}}(t)$$

Por la ley de inducción de Faraday, la magnitud de la fuerza electromotriz inducida es:
$$|\mathcal{E}| = \frac{d\Phi_B}{dt} = B a \frac{dy_{\text{in}}}{dt} = B a v$$

---

#### 2. Corriente inducida y sentido de circulación (Ley de Lenz)

Por la ley de Ohm, la corriente inducida en la espira de resistencia $R$ tiene una magnitud de:
$$I_{\text{ind}} = \frac{|\mathcal{E}|}{R} = \frac{B a v}{R}$$

**Sentido de la corriente:**  
Al caer la espira, el flujo del campo magnético entrante ($\otimes$) se incrementa continuamente. Por la ley de Lenz, la corriente inducida produce un campo magnético que se opone a dicho incremento, por lo cual debe generar un campo magnético inducido dirigido hacia afuera de la página ($\odot$).  
Aplicando la regla de la mano derecha con el pulgar apuntando hacia afuera de la página, la corriente inducida circula en **sentido antihorario**:
- Lado horizontal inferior (sumergido): hacia la derecha ($+\hat{x}$).
- Lado vertical derecho: hacia arriba ($+\hat{y}$).
- Lado horizontal superior (fuera del campo): hacia la izquierda ($-\hat{x}$).
- Lado vertical izquierdo: hacia abajo ($-\hat{y}$).

---

#### 3. Fuerzas magnéticas sobre cada segmento de la espira

La fuerza magnética que actúa sobre un conductor filiforme recorrido por corriente es $\vec{F}_m = I \int d\vec{\ell} \times \vec{B}$:

1. **Lado horizontal superior:**  
   Se encuentra enteramente en la región donde $\vec{B} = \vec{0}$, por lo que:
   $$\vec{F}_{\text{sup}} = \vec{0}$$

2. **Lados verticales (izquierdo y derecho):**  
   En la porción sumergida de longitud $y_{\text{in}}$, la corriente circula hacia abajo ($-\hat{y}$) en el lado izquierdo y hacia arriba ($+\hat{y}$) en el lado derecho:
   $$\vec{F}_{\text{izq}} = I_{\text{ind}} (-y_{\text{in}}\,\hat{y}) \times (-B\,\hat{z}) = I_{\text{ind}} y_{\text{in}} B (\hat{y} \times \hat{z}) = + I_{\text{ind}} y_{\text{in}} B\,\hat{x}$$
   $$\vec{F}_{\text{der}} = I_{\text{ind}} (+y_{\text{in}}\,\hat{y}) \times (-B\,\hat{z}) = - I_{\text{ind}} y_{\text{in}} B (\hat{y} \times \hat{z}) = - I_{\text{ind}} y_{\text{in}} B\,\hat{x}$$
   Estas dos fuerzas son horizontales, de igual magnitud y sentidos opuestos, por lo que se anulan mutuamente:
   $$\vec{F}_{\text{izq}} + \vec{F}_{\text{der}} = \vec{0}$$

3. **Lado horizontal inferior (sumergido, longitud $a$ con corriente hacia $+\hat{x}$):**
   $$d\vec{\ell} = dx\,\hat{x}$$
   $$\vec{F}_{\text{inf}} = I_{\text{ind}} (a\,\hat{x}) \times (-B\,\hat{z}) = - I_{\text{ind}} a B (\hat{x} \times \hat{z}) = + I_{\text{ind}} a B\,\hat{y}$$

   La fuerza magnética neta sobre la espira apunta verticalmente hacia arriba:
   $$\vec{F}_m = I_{\text{ind}} a B\,\hat{y} = \left(\frac{B a v}{R}\right) a B\,\hat{y} = \frac{B^2 a^2 v}{R}\,\hat{y}$$

---

#### 4. Ecuación dinámica y velocidad terminal

Aplicamos la segunda ley de Newton en el eje vertical $Y$:
$$\sum F_y = F_m - m g = m a_y = m \left( -\frac{dv}{dt} \right)$$
$$\frac{B^2 a^2 v}{R} - m g = - m \frac{dv}{dt}$$

Cuando la espira alcanza la condición estacionaria de velocidad terminal ($v \to v_t$), la aceleración se hace nula ($\frac{dv}{dt} = 0$):
$$\frac{B^2 a^2 v_t}{R} - m g = 0$$

Despejando la velocidad terminal $v_t$:
$$\frac{B^2 a^2 v_t}{R} = m g \implies \boxed{v_t = \frac{m g R}{B^2 a^2}}$$

**Verificación:**
- **Sentido físico:** La corriente en sentido antihorario produce una fuerza de frenado ascensional $+\hat{y}$, oponiéndose a la aceleración gravitacional $-\hat{y}$, lo que permite alcanzar una velocidad límite constante.
- **Unidades:**
  $$[v_t] = \frac{[m][g][R]}{[B]^2 [a]^2} = \frac{(\text{kg})(\text{m}/\text{s}^2)(\Omega)}{\text{T}^2 \cdot \text{m}^2} = \frac{\text{N} \cdot (\text{V}/\text{A})}{(\text{N}/(\text{A}\cdot\text{m}))^2 \cdot \text{m}^2} = \frac{\text{N} \cdot \text{V}/\text{A}}{\text{N}^2 / \text{A}^2} = \frac{\text{V}\cdot\text{A}}{\text{N}} = \frac{\text{W}}{\text{N}} = \frac{\text{N}\cdot\text{m}/\text{s}}{\text{N}} = \text{m}/\text{s}$$
  Dimensionalmente correcto.
- **Casos límite:**
  - Si la resistencia es infinita ($R \to \infty$, circuito abierto sin corriente): $v_t \to \infty$, la espira cae en caída libre con aceleración $g$.
  - Si el campo magnético es nulo ($B \to 0$): $v_t \to \infty$.
  - Si la espira tiene resistencia nula ($R \to 0$, superconductor): $v_t \to 0$, no puede penetrar en la región con campo.

---

## Resumen de resultados

| Problema | Parte / Pregunta | Parámetro / Variable | Resultado Final |
| :--- | :--- | :--- | :--- |
| **Problema 1** | — | Fem inducida en la espira $\mathcal{E}(t)$ | $\displaystyle \mathcal{E}(t) = \frac{\mu_0 I a b v}{2\pi (h+vt)(h+a+vt)}$ |
| | — | Sentido de la corriente inducida | **Horario** |
| **Problema 2** | 1. | Campo $\vec{B}$ dentro de la bobina ($r < b$) | $\displaystyle \vec{B} = \mu_0 m I_0 \sin(\omega t)\,\hat{z}$ |
| | 2. | Campo $\vec{E}$ dentro de la bobina ($r < b$) | $\displaystyle \vec{E} = - \frac{\mu_0 m I_0 \omega r}{2} \cos(\omega t)\,\hat{\theta}$ |
| | 2. | Campo $\vec{E}$ fuera de la bobina ($r > b$) | $\displaystyle \vec{E} = - \frac{\mu_0 m I_0 \omega b^2}{2r} \cos(\omega t)\,\hat{\theta}$ |
| **Problema 3** | — | Velocidad terminal $v_t$ | $\displaystyle v_t = \frac{m g R}{B^2 a^2}$ |
| | — | Sentido de la corriente inducida | **Antihorario** |
