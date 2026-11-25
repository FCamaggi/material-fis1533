# Pauta Examen — FIS1533 (2024-2)

> **Evaluación:** Examen (Respuestas Forma 1) | **Semestre:** 2024-2 | **Fecha:** 09 de diciembre de 2024  
> **Temas:** Ley de Ampère, fuerza magnética entre corrientes e inductancia mutua; ley de Biot-Savart y momento dipolar magnético; circuitos RLC de corriente alterna e impedancia; ley de Faraday-Lenz

---

## Problema 1

Considere un alambre infinito por el que circula una corriente $I_1$ y una espira rectangular de lados $a$ y $b$, coplanar con el alambre y tal que el lado $a$ es paralelo a este y a una distancia $h$ del alambre. Suponga que por la espira rectangular circula una corriente $I_2$.

a) *(2 puntos)* Calcular el vector campo magnético $\vec{B}_1$ inducido por la corriente $I_1$ en función a la distancia al eje del alambre infinito.  
b) *(2 puntos)* ¿Cuál es la fuerza neta que ejerce la corriente $I_1$ sobre la espira rectangular que conduce la corriente $I_2$?  
c) *(2 puntos)* Calcular la inductancia mutua entre la espira y el alambre.

> **[Figura]:** Sistema de coordenadas en el plano $xy$ (con el eje $+x$ hacia la derecha, $+y$ hacia arriba y $+z$ saliendo de la página). Sobre el eje $x$ yace un alambre infinito con corriente $I_1$ hacia la derecha ($+\hat{x}$). En el primer cuadrante ($x \ge 0$, $y > 0$) se ubica una espira rectangular de ancho horizontal $a$ y altura vertical $b$, con su lado inferior a altura $y = h$ y su lado superior a altura $y = h + b$. La corriente $I_2$ circula por la espira en sentido **horario**: sube por el lado izquierdo, va hacia la derecha en $y = h + b$, baja por el lado derecho y va hacia la izquierda en $y = h$.

---

### Solución

**Idea:** Se calcula el campo magnético del alambre infinito por ley de Ampère. La fuerza neta sobre la espira se obtiene sumando $\int I_2\,d\vec{\ell}\times\vec{B}_1$ sobre sus cuatro tramos: las fuerzas en los lados verticales se cancelan por simetría y en los horizontales compiten la atracción del lado superior y la repulsión del lado inferior (más cercano al alambre). La inductancia mutua se deduce de $M = \Phi_2/I_1$ integrando el flujo magnético de $\vec{B}_1$ sobre el área rectangular.

#### Parte a) Vector campo magnético $\vec{B}_1$ del alambre infinito

El campo magnético inducido por la corriente $I_1$ en el alambre infinito se calcula mediante la ley de Ampère:

$$\oint_C \vec{B}_1 \cdot d\vec{\ell} = \mu_0 I_{\text{enc}} \qquad \text{(0.5 pts.)}$$

Escogemos como trayectoria de integración $C$ una circunferencia de radio $r$ concéntrica al alambre infinito (en el plano $x = 0$, es decir, el plano $yz$), cuyo sentido de recorrido obedece la regla de la mano derecha respecto a la corriente $I_1$ en $+\hat{x}$ y que encierra $I_{\text{enc}} = I_1$ *(0.5 pts.)*:

$$B_1(r)(2\pi r) = \mu_0 I_1 \implies B_1(r) = \frac{\mu_0 I_1}{2\pi r}$$

En particular, sobre el semiplano $z = 0$ con $y > 0$ (donde $r = y$ es la distancia al eje del alambre infinito y la regla de la mano derecha da dirección $+\hat{z}$):

$$\boxed{\vec{B}_1(y) = \frac{\mu_0 I_1}{2\pi y}\,\hat{z}} \qquad \text{(1.0 pts.)}$$

*(En coordenadas cilíndricas alrededor del eje $x$, de forma general para toda distancia $r$ al eje del alambre, $\vec{B}_1(r) = \frac{\mu_0 I_1}{2\pi r}\,\hat{\phi}$.)*

---

#### Parte b) Fuerza neta sobre la espira rectangular

La fuerza magnética sobre el circuito cerrado de corriente $I_2$ viene dada por:

$$\vec{F} = \oint \left(I_2\,d\vec{\ell} \times \vec{B}_1(y)\right) \qquad \text{(0.5 pts.)}$$

Los lados verticales de la espira (paralelos al eje $y$) experimentan fuerzas opuestas de igual magnitud ($\vec{F}_{\text{izq}} + \vec{F}_{\text{der}} = \vec{0}$), ya que tienen corrientes opuestas y atraviesan el mismo perfil de campo $B_1(y)$. Para los lados horizontales (paralelos al eje $x$), con $d\vec{\ell} = dx\,\hat{x}$ en el segmento superior ($y = h + b$, recorrido de $0$ a $a$) y en el inferior ($y = h$, recorrido de $a$ a $0$):

$$\vec{F} = \int_0^a \left(I_2\,dx\,\hat{x} \times \vec{B}_1(y = h + b)\right) + \int_a^0 \left(I_2\,dx\,\hat{x} \times \vec{B}_1(y = h)\right) \qquad \text{(0.5 pts.)}$$

*(Nota: en la pauta oficial se redacta por lapsus «elemento de corriente del alambre infinito», refiriéndose en realidad a un elemento de corriente de los tramos horizontales de la espira rectangular.)*

Sustituyendo $\vec{B}_1(y) = \frac{\mu_0 I_1}{2\pi y}\,\hat{z}$ y usando $\hat{x} \times \hat{z} = -\hat{y}$:

$$\vec{F} = \left(I_2 a\,\frac{\mu_0 I_1}{2\pi(h + b)} - I_2 a\,\frac{\mu_0 I_1}{2\pi h}\right)(-\hat{y}) = \frac{\mu_0 I_1 I_2 a}{2\pi}\left(\frac{1}{h} - \frac{1}{h + b}\right)\hat{y}$$

Simplificando:

$$\boxed{\vec{F} = \frac{\mu_0 I_1 I_2 ab}{2\pi h(h + b)}\,\hat{y}} \qquad \text{(1.0 pts.)}$$

---

#### Parte c) Inductancia mutua $M$ entre la espira y el alambre

Por definición, la inductancia mutua $M$ cumple:

$$M I_1 = \Phi_2 \qquad \text{(0.5 pts.)}$$

donde $\Phi_2$ es el flujo magnético del campo $\vec{B}_1$ a través del área $A_2$ encerrada por la espira rectangular. Así:

$$M = \frac{1}{I_1}\int_{A_2} \vec{B}_1 \cdot d\vec{A}_2 \qquad \text{(0.5 pts.)}$$

En este cálculo la corriente $I_2$ y su sentido son irrelevantes; elegimos el diferencial de área de modo que el flujo sea positivo, $d\vec{A}_2 = dx\,dy\,\hat{z}$:

$$M = \frac{1}{I_1}\int_{A_2} \frac{\mu_0 I_1}{2\pi y}\,\hat{z} \cdot dx\,dy\,\hat{z} = \frac{\mu_0}{2\pi}\int_0^a dx \int_h^{h+b} \frac{1}{y}\,dy = \frac{\mu_0 a}{2\pi}\Big[\ln y\Big]_h^{h+b}$$

Finalmente obtenemos:

$$\boxed{M = \frac{\mu_0 a}{2\pi}\ln\left(\frac{h + b}{h}\right)} \qquad \text{(1.0 pts.)}$$

**Verificación:** Como el tramo inferior de la espira (más cercano al alambre) lleva corriente antiparalela a $I_1$, sufre repulsión ($+\hat{y}$) más intensa que la atracción ($-\hat{y}$) sobre el tramo superior, resultando una fuerza neta en $+\hat{y}$. En el límite $h \gg b$, $\vec{F} \approx \frac{\mu_0 I_1 I_2 ab}{2\pi h^2}\hat{y}$ y $M \approx \frac{\mu_0 ab}{2\pi h} = \frac{B_1(h)\cdot(ab)}{I_1}$, coherentes con campo casi uniforme sobre la espira.

---

## Problema 2

Una corriente $I$ circula por la espira de radios $b$ y $a$ ($b > a$) mostrada en la figura. Ambas semicircunferencias tienen un origen común en $P$.

Con esta información, calcule:

a) *(4 puntos)* El vector campo magnético en el punto $P$.  
b) *(2 puntos)* El vector momento dipolar magnético de la espira.

> **[Figura]:** En el plano $xy$ con origen en $P$ ($x$ hacia la derecha, $y$ hacia arriba), la espira cerrada está compuesta por cuatro tramos recorridos por la corriente $I$ en sentido **horario**: una semicircunferencia superior de radio $b$ (en $y \ge 0$, yendo de izquierda a derecha), un segmento recto horizontal derecho sobre el eje $+x$ desde $x = b$ hasta $x = a$, una semicircunferencia inferior de radio $a$ (en $y \le 0$, yendo de $(a,0)$ a $(-a,0)$ en sentido horario), y un segmento recto horizontal izquierdo sobre el eje $-x$ desde $x = -a$ hasta $x = -b$. Se dibujan también los vectores unitarios polares $\hat{\rho}$ (radial hacia afuera) y $\hat{\theta}$ (tangencial antihorario).

---

### Solución

**Idea:** Se aplica la ley de Biot-Savart sumando las contribuciones de los cuatro tramos: los dos segmentos rectos pasan por la recta que contiene a $P$, por lo que $d\vec{\ell} \parallel (\vec{r}-\vec{r}')$ y su aporte es nulo; los dos arcos semicirculares con corriente horaria generan campos que apuntan ambos en $-\hat{k}$. El momento dipolar magnético se obtiene como $\vec{\mu} = I A\,\hat{n}$ con el área total encerrada $A = \frac{\pi}{2}(b^2 + a^2)$ y normal $-\hat{k}$ por regla de la mano derecha.

#### Parte a) Vector campo magnético en el punto $P$

Aplicamos la ley de Biot-Savart:

$$\vec{B} = \frac{\mu_0}{4\pi}\int \frac{I\,d\vec{\ell}\times(\vec{r} - \vec{r}')}{|\vec{r} - \vec{r}'|^3}$$

El campo magnético total en $P$ es la superposición de los campos generados por las dos semicircunferencias ($\cap$ y $\cup$) y las dos secciones rectas ($-$) *(0.5 pts.)*:

$$\vec{B}_P = \vec{B}_\cap + \vec{B}_\cup + \vec{B}_- + \vec{B}_-$$

Para las secciones rectas horizontales sobre el eje $x$, tanto $d\vec{\ell} \propto \hat{\imath}$ como $\vec{r} - \vec{r}' \propto \hat{\imath}$ son colineales, de modo que $d\vec{\ell} \times (\vec{r} - \vec{r}') = \vec{0}$ y su contribución al campo en $P$ es nula.

Para las porciones circulares evaluadas en el origen $P$ ($\vec{r} = \vec{0}$), de acuerdo con la figura:

- **Para $\cap$ (semicircunferencia superior de radio $b$):** *(0.5 pts.)*
  $$d\vec{\ell} = b\,d\theta\,(-\hat{\theta}), \qquad \vec{r} = \vec{0}, \qquad \vec{r}' = b\,\hat{\rho}$$
- **Para $\cup$ (semicircunferencia inferior de radio $a$):** *(0.5 pts.)*
  $$d\vec{\ell} = a\,d\theta\,(-\hat{\theta}), \qquad \vec{r} = \vec{0}, \qquad \vec{r}' = a\,\hat{\rho}$$

Sustituyendo en Biot-Savart con $\theta \in [0, \pi]$ (o parametrizando en el sentido de la corriente con $d\vec{\ell} = r'\,d\theta\,\hat{\theta}$ desde $\pi$ hasta $0$ para $\cap$, y desde $0$ hasta $-\pi$ para $\cup$):

$$\vec{B}_\cap = \frac{\mu_0}{4\pi}\int_0^\pi \frac{I b\,d\theta\,(-\hat{\theta})\times(-b)\hat{\rho}}{b^3} = \frac{\mu_0}{4\pi}\int_\pi^0 \frac{I b\,d\theta\,\hat{\theta}\times(-b)\hat{\rho}}{b^3} \qquad \text{(0.5 pts.)}$$

$$\vec{B}_\cup = \frac{\mu_0}{4\pi}\int_0^\pi \frac{I a\,d\theta\,(-\hat{\theta})\times(-a)\hat{\rho}}{a^3} = \frac{\mu_0}{4\pi}\int_0^{-\pi} \frac{I a\,d\theta\,\hat{\theta}\times(-a)\hat{\rho}}{a^3} \qquad \text{(0.5 pts.)}$$

En cualquier caso, utilizando la identidad $\hat{\theta} \times \hat{\rho} = -\hat{k}$ (dado que $\hat{\rho}\times\hat{\theta} = +\hat{k}$):

$$\vec{B}_\cap = \frac{\mu_0 I}{4\pi b}\int_0^\pi (-\hat{k})\,d\theta = -\frac{\mu_0 I}{4b}\,\hat{k} \qquad \text{(0.5 pts.)}$$

$$\vec{B}_\cup = \frac{\mu_0 I}{4\pi a}\int_0^\pi (-\hat{k})\,d\theta = -\frac{\mu_0 I}{4a}\,\hat{k} \qquad \text{(0.5 pts.)}$$

Sumando ambas contribuciones:

$$\boxed{\vec{B}_P = -\frac{\mu_0 I}{4}\left(\frac{1}{a} + \frac{1}{b}\right)\hat{k}} \qquad \text{(0.5 pts.)}$$

---

#### Parte b) Vector momento dipolar magnético de la espira

El momento dipolar magnético de una espira plana de corriente $I$ y área $A$ está dado por:

$$\vec{\mu} = I A\,\hat{n}$$

El área encerrada es la suma de dos semicírculos de radios $b$ y $a$: $A = \frac{\pi b^2}{2} + \frac{\pi a^2}{2} = \frac{\pi}{2}(b^2 + a^2)$. Como la corriente circula en sentido horario en el plano $xy$, la regla de la mano derecha determina la normal $\hat{n} = -\hat{k}$ *(1 pto. por la magnitud, 1 pto. por la dirección)*:

$$\boxed{\vec{\mu} = -I\frac{\pi}{2}(b^2 + a^2)\,\hat{k}} \qquad \text{(2 pts.)}$$

**Verificación:** Si $a = b$, la espira completa un círculo de radio $b$ con corriente horaria, recuperándose $\vec{B}_P = -\frac{\mu_0 I}{2b}\hat{k}$ y $\vec{\mu} = -I\pi b^2 \hat{k}$.

---

## Problema 3

Considere el circuito de la figura con una fuente de voltaje $V(t) = V_0 \cos(\omega t)$, una resistencia $R$, una inductancia $L$ y dos condensadores $C_1$ y $C_2$ con $C_1 = C$ y $C_2 = 2C$.

a) *(1.5 puntos)* Encuentre la ecuación diferencial (de segundo grado) que deben satisfacer las corrientes del circuito.  
b) *(1.5 puntos)* Determine la impedancia equivalente del sistema.  
c) *(3 puntos)* Encuentre la expresión para la corriente alterna en función del tiempo. Además, determine el valor de $C$, en términos de $\omega$ y $L$, que maximiza la amplitud de la corriente.

> **[Figura]:** Circuito RLC de una sola malla en serie. En la rama izquierda se ubica la fuente de voltaje alterno $V(t)$; en la rama superior, la resistencia $R$; en la rama derecha, el condensador $C_1$ en serie con la inductancia $L$; y en la rama inferior, el condensador $C_2$.

---

### Solución

**Idea:** Todos los elementos están conectados en serie, por lo que comparten la misma corriente $I(t)$. Al aplicar la regla de mallas de Kirchhoff y derivar respecto al tiempo se obtiene una EDO lineal de segundo orden para $I(t)$. En régimen estacionario sinusoidal, la impedancia equivalente es la suma de las impedancias individuales, y la amplitud de corriente se maximiza en resonancia cuando la reactancia total se anula ($\text{Im}(Z_{\text{eq}}) = 0$).

*(Nota de la pauta: en algunas secciones del curso se utilizó la letra $j$ en vez de $i$ para denotar la unidad imaginaria.)*

#### Parte a) Ecuación diferencial para la corriente

Por la regla de mallas de Kirchhoff (con $Q_1$ y $Q_2$ las cargas en $C_1$ y $C_2$):

$$V(t) = I R + \frac{Q_2}{C_2} + \dot{I} L + \frac{Q_1}{C_1} \qquad \text{(0.5 pts.)}$$

Derivando la expresión respecto al tiempo y usando $\dot{Q}_1 = \dot{Q}_2 = I$:

$$\dot{V}(t) = \dot{I} R + \frac{I}{C_1} + \frac{I}{C_2} + \ddot{I} L \qquad \text{(0.5 pts.)}$$

Evaluando el inverso de la capacitancia equivalente en serie con $C_1 = C$ y $C_2 = 2C$:

$$\frac{1}{C_1} + \frac{1}{C_2} = \frac{1}{C}\left(1 + \frac{1}{2}\right) = \frac{3}{2C}$$

Dado que $V(t) = V_0\cos(\omega t)$, tenemos $\dot{V}(t) = -\omega V_0 \sin(\omega t)$, por lo que la ecuación diferencial resulta:

$$\boxed{-\omega V_0 \sin(\omega t) = \ddot{I}L + \dot{I}R + \frac{3}{2C}I} \qquad \text{(0.5 pts.)}$$

---

#### Parte b) Impedancia equivalente del sistema

Dado que todos los elementos están en serie:

$$Z_{\text{eq}} = Z_R + Z_{C_1} + Z_L + Z_{C_2} \qquad \text{(0.5 pts.)}$$

Sustituyendo las impedancias individuales ($Z_R = R$, $Z_L = i\omega L$, $Z_{C_k} = \frac{1}{i\omega C_k} = -\frac{i}{\omega C_k}$):

$$Z_{\text{eq}} = R - \frac{i}{\omega C_1} + i\omega L - \frac{i}{\omega C_2} \qquad \text{(0.5 pts.)}$$

Con $C_1 = C$ y $C_2 = 2C$:

$$\boxed{Z_{\text{eq}} = R + i\omega L - \frac{3i}{2\omega C} = R + i\left(\omega L - \frac{3}{2\omega C}\right)} \qquad \text{(0.5 pts.)}$$

---

#### Parte c) Corriente alterna $I(t)$ y valor de $C$ que maximiza su amplitud

Por definición fasorial:

$$\tilde{V}(t) = \tilde{I}(t)\,Z_{\text{eq}}, \qquad \text{con } \tilde{V}(t) = V_0 e^{i\omega t} \qquad \text{(0.5 pts.)}$$

De donde:

$$I(t) = \Re\{\tilde{I}(t)\} = \Re\left\{\frac{\tilde{V}(t)}{Z_{\text{eq}}}\right\} \qquad \text{(0.5 pts.)}$$

Escribiendo la impedancia en forma polar $Z_{\text{eq}} = |Z_{\text{eq}}|e^{i\varphi}$, su módulo y fase son:

$$|Z_{\text{eq}}| = \sqrt{R^2 + \left(\omega L - \frac{3}{2\omega C}\right)^2} \qquad \text{(0.5 pts.)}$$

$$\tan\varphi = \frac{\omega L - \frac{3}{2\omega C}}{R} \qquad \text{(0.5 pts.)}$$

Entonces:

$$I(t) = \Re\left\{\frac{V_0 e^{i\omega t}}{|Z_{\text{eq}}|e^{i\varphi}}\right\} = \frac{V_0}{|Z_{\text{eq}}|}\Re\left\{e^{i(\omega t - \varphi)}\right\}$$

$$\boxed{I(t) = \frac{V_0}{\sqrt{R^2 + \left(\omega L - \frac{3}{2\omega C}\right)^2}}\cos(\omega t - \varphi), \qquad \varphi = \arctan\!\left(\frac{\omega L - \frac{3}{2\omega C}}{R}\right)} \qquad \text{(0.5 pts.)}$$

La amplitud de $I(t)$ es máxima cuando $|Z_{\text{eq}}|$ es mínimo. Como podemos ajustar $C$ para anular la reactancia total:

$$\omega L - \frac{3}{2\omega C} = 0 \implies \boxed{C = \frac{3}{2\omega^2 L}} \qquad \text{(0.5 pts.)}$$

*(Nota: la pauta oficial redacta por lapsus «libertad para ajustar los valores de $L$ y $\omega$» cuando se despeja $C$ en términos de $\omega$ y $L$; el resultado $C = \frac{3}{2\omega^2 L}$ es completamente correcto.)*

**Verificación:** La capacitancia equivalente serie de $C_1=C$ y $C_2=2C$ es $C_{\text{eq}} = \frac{2}{3}C$. La condición de resonancia $\omega = \frac{1}{\sqrt{L C_{\text{eq}}}}$ da $C_{\text{eq}} = \frac{1}{\omega^2 L} \implies C = \frac{3}{2\omega^2 L}$.

---

## Problema 4

Una espira circular de radio pequeño $r$ está fija en el espacio. Una gran espira de radio $R$ está situada en un plano paralelo a la primera, es coaxial con ella y se le acerca con una velocidad constante $\vec{v} = v\hat{z}$. Las dos espiras son conductores óhmicos. Por la espira grande circula una corriente constante $I$ como se muestra en la figura, y en el instante $t = 0$ la distancia entre las dos espiras es $z$.

a) *(2 puntos)* Calcular cómo cambia con el tiempo el flujo del campo magnético generado por la espira grande a través de la espira pequeña. Se asume que $r \ll R$ de manera que el campo magnético en el interior de la espira pequeña se puede considerar uniforme e igual a su valor a lo largo del eje.  
b) *(2 puntos)* Calcular la f.e.m. inducida en la espira pequeña en un instante $t$ cualquiera.  
c) *(2 puntos)* Argumentar en qué dirección fluye la corriente inducida en la espira pequeña en comparación con el sentido de $d\vec{\ell}$ que se muestra en la figura cuando la espira grande se encuentra a la izquierda y a la derecha de la espira pequeña. Calcular la corriente inducida en la espira pequeña cuando las dos espiras están en el mismo plano y cuando $t \to +\infty$.

> **[Figura]:** Vista en perspectiva de dos espiras circulares coaxiales paralelas con eje de simetría común $z$ apuntando hacia la derecha. A la izquierda se encuentra la espira grande de radio $R$, moviéndose hacia la derecha con velocidad $\vec{v}$, por la que circula una corriente $I$ (indicada con una flecha hacia abajo en el arco izquierdo). A la derecha, fija y separada una distancia inicial $z$ en $t = 0$, se encuentra la espira pequeña de radio $r$, con una flecha de orientación $d\vec{\ell}$ hacia abajo en su arco izquierdo (mismo sentido de circulación que $I$).

---

### Solución

**Idea:** Como $r \ll R$, el flujo magnético a través de la espira pequeña se aproxima por $\Phi(t) = B_z(t)\cdot \pi r^2$, donde $B_z(t)$ es el campo en el eje de una espira circular a distancia $d(t) = z - vt$. Derivando $\Phi(t)$ respecto a $t$ mediante la ley de Faraday-Lenz se obtiene la f.e.m. inducida $\mathcal{E}(t)$, cuyo signo indica si la corriente inducida es concordante u opuesta a $d\vec{\ell}$.

#### Parte a) Flujo magnético en función del tiempo

El campo magnético producido por la espira grande de radio $R$ y corriente $I$ sobre su eje, a una distancia genérica $d$ de su centro, es:

$$\vec{B}(0, 0, d) = \frac{\mu_0 I R^2}{2(R^2 + d^2)^{3/2}}\,\hat{z} \qquad \text{(0.5 pts.)}$$

En un instante genérico $t$, la distancia axial desde la espira grande hacia la espira pequeña es $d(t) = z - vt$ *(0.5 pts.)*. Usando la aproximación $r \ll R$, el flujo a través de la espira pequeña (con $d\vec{s}$ orientado en $+\hat{z}$, concordante con $d\vec{\ell}$) es:

$$\Phi(t) = \int_S d\vec{s}\cdot\vec{B}\big(0,0,d(t)\big) = \int_S ds\,\big|\vec{B}\big(0,0,d(t)\big)\big| = \big|\vec{B}\big(0,0,d(t)\big)\big|\pi r^2 \qquad \text{(0.5 pts.)}$$

Así:

$$\boxed{\Phi(t) = \frac{\mu_0 I R^2}{2\left[R^2 + (z - vt)^2\right]^{3/2}}\,\pi r^2} \qquad \text{(0.5 pts.)}$$

> **Nota oficial:** También se considera correcta la solución con signo negativo si el/la estudiante interpretó en la perspectiva que la corriente en la espira grande gira hacia atrás (produciendo campo en $-\hat{z}$).

---

#### Parte b) Fuerza electromotriz inducida en un instante $t$

Por la ley de Faraday-Lenz, la f.e.m. inducida en la espira pequeña debido a la variación temporal del flujo es:

$$\mathcal{E}(t) = -\frac{d\Phi}{dt} \qquad \text{(0.5 pts.)}$$

Derivando respecto a $t$:

$$\mathcal{E}(t) = -\frac{\mu_0 I R^2 \pi r^2}{2}\left(-\frac{3}{2}\right)\left[R^2 + (z - vt)^2\right]^{-5/2}\frac{d}{dt}(z - vt)^2$$

$$\mathcal{E}(t) = \frac{3}{2}\frac{\mu_0 I R^2}{2\left[R^2 + (z - vt)^2\right]^{5/2}}\,\pi r^2\,\frac{d}{dt}(z - vt)^2 \qquad \text{(0.5 pts.)}$$

Como $\frac{d}{dt}(z - vt)^2 = 2(z - vt)(-v) = -2v(z - vt)$:

$$\boxed{\mathcal{E}(t) = -\frac{3\mu_0 I R^2 v (z - vt)}{2\left[R^2 + (z - vt)^2\right]^{5/2}}\,\pi r^2} \qquad \text{(1.0 pts.)}$$

> **Nota oficial:** También se considera correcta la solución con signo positivo si el/la estudiante consideró la orientación opuesta de la corriente en la parte a).

---

#### Parte c) Dirección de la corriente inducida y casos límite

- **Espira grande a la izquierda ($z - vt > 0$):** La espira grande se acerca hacia la pequeña, de modo que el flujo $\Phi(t)$ es creciente y $\mathcal{E}(t) < 0$. Por la ley de Lenz, la corriente inducida debe generar un campo magnético que se oponga al aumento del flujo. Por lo tanto, la corriente inducida fluye en **sentido opuesto a $d\vec{\ell}$** *(0.5 pts.)*.
- **Espira grande a la derecha ($z - vt < 0$):** La espira grande ya sobrepasó a la pequeña y se aleja de ella, de modo que el flujo $\Phi(t)$ es decreciente y $\mathcal{E}(t) > 0$. Por la ley de Lenz, la corriente inducida intenta compensar la disminución del flujo, fluyendo en **sentido concordante con $d\vec{\ell}$** *(0.5 pts.)*.
- **Ambas espiras en el mismo plano ($z - vt = 0$):** En el instante $t_0 = z/v$, el flujo alcanza su valor máximo y su derivada se anula, por lo que $\mathcal{E}(t_0) = 0$ y la corriente inducida es **cero** *(0.5 pts.)*:
  $$\boxed{I_{\text{ind}}(t_0 = z/v) = 0}$$
- **Cuando $t \to +\infty$:**
  $$\lim_{t\to\infty}\mathcal{E}(t) = -\frac{3\mu_0 I R^2 v \pi r^2}{2}\lim_{t\to\infty}\frac{z - vt}{\left[R^2 + (z - vt)^2\right]^{5/2}} = 0 \qquad \text{(0.5 pts.)}$$
  Por lo tanto, como la espira es óhmica ($I_{\text{ind}} = \mathcal{E}/R_{\text{esp}}$), la corriente inducida cuando $t \to \infty$ también es **cero**:
  $$\boxed{\lim_{t\to\infty} I_{\text{ind}}(t) = 0}$$

**Verificación:** Para $z - vt > 0$, $\mathcal{E}(t) < 0$ corresponde a una corriente inducida antiparalela a $I$, lo cual genera repulsión magnética entre las espiras oponiéndose al acercamiento, en acuerdo con la ley de Lenz.

---

## Resumen de resultados

| Problema / Inciso | Resultado final |
| :--- | :--- |
| **1a)** Campo magnético del alambre | $\vec{B}_1(y) = \dfrac{\mu_0 I_1}{2\pi y}\,\hat{z}$ (en $z=0, y>0$) |
| **1b)** Fuerza neta sobre la espira | $\vec{F} = \dfrac{\mu_0 I_1 I_2 ab}{2\pi h(h+b)}\,\hat{y}$ |
| **1c)** Inductancia mutua | $M = \dfrac{\mu_0 a}{2\pi}\ln\left(\dfrac{h+b}{h}\right)$ |
| **2a)** Campo magnético en $P$ | $\vec{B}_P = -\dfrac{\mu_0 I}{4}\left(\dfrac{1}{a} + \dfrac{1}{b}\right)\hat{k}$ |
| **2b)** Momento dipolar magnético | $\vec{\mu} = -I\dfrac{\pi}{2}(b^2 + a^2)\,\hat{k}$ |
| **3a)** EDO del circuito | $-\omega V_0\sin(\omega t) = \ddot{I}L + \dot{I}R + \dfrac{3}{2C}I$ |
| **3b)** Impedancia equivalente | $Z_{\text{eq}} = R + i\omega L - \dfrac{3i}{2\omega C}$ |
| **3c)** Corriente alterna y $C$ resonante | $I(t) = \dfrac{V_0}{|Z_{\text{eq}}|}\cos(\omega t - \varphi)$ ; $\quad C = \dfrac{3}{2\omega^2 L}$ |
| **4a)** Flujo magnético $\Phi(t)$ | $\Phi(t) = \dfrac{\mu_0 I R^2 \pi r^2}{2\left[R^2 + (z - vt)^2\right]^{3/2}}$ |
| **4b)** F.e.m. inducida $\mathcal{E}(t)$ | $\mathcal{E}(t) = -\dfrac{3\mu_0 I R^2 v (z - vt)\pi r^2}{2\left[R^2 + (z - vt)^2\right]^{5/2}}$ |
| **4c)** Sentido y límites de $I_{\text{ind}}$ | Izquierda: opuesto a $d\vec{\ell}$ ; Derecha: concordante con $d\vec{\ell}$ ; $t_0=z/v$: $0$ ; $t\to\infty$: $0$ |
