# Ayudantía 22 — Inducción electromagnética y fem de movimiento

> Clases relacionadas: [Clase 13 - Inducción Magnética](../../Clases/markdown/Clase%2013%20-%20Inducci%C3%B3n%20Magn%C3%A9tica.md), [Clase 14 - Inductancia](../../Clases/markdown/Clase%2014%20-%20Inductancia.md)

---

## Problema 1

Un generador de corriente $G$ produce una corriente $I(t)$ en un circuito formado por un riel conductor sin roce, en forma de U y una barra conductora de masa $m$ que atraviesa los rieles en dirección perpendicular. Un campo magnético constante y uniforme $\vec{B}$ que apunta perpendicular al plano del circuito existe en todo el espacio. La corriente $I(t)$ que circula en el circuito varía en el tiempo de acuerdo con:
$$I(t) = \begin{cases} 0 & t < 0 \\ bt & 0 < t < T \\ 0 & T < t \end{cases}$$

Para $t \le T$, determine la fuerza electromotriz inducida en el circuito y la velocidad de la barra en función del tiempo.

> **[Figura]:** Circuito rectangular horizontal formado por dos rieles conductores paralelos sin fricción separados una distancia $L$ y cerrados en su extremo izquierdo por una fuente/generador de corriente $G$. Una barra conductora vertical de masa $m$ y largo mayor que $L$ se apoya transversalmente sobre los rieles, cerrando el circuito a una distancia $x(t)$ de la fuente. La corriente $I(t)$ sale de la fuente por el riel superior hacia la derecha, baja por la barra móvil hacia el riel inferior y regresa a la fuente por el riel inferior (sentido horario). Existe un campo magnético uniforme $\vec{B} = -B\hat{z}$ perpendicular al plano, dirigido hacia dentro de la página (indicado por cruces $\times$).

### Solución

**Idea:** La corriente forzada por el generador a través de la barra conductora en presencia del campo magnético perpendicular produce una fuerza magnética de Lorentz ($\vec{F} = I\vec{L}\times\vec{B}$). Por la segunda ley de Newton, esta fuerza acelera la barra. A medida que la barra se desplaza, el área del circuito aumenta linealmente con su posición $x(t)$, produciendo una variación del flujo magnético en el tiempo. Por la ley de Faraday-Lenz, dicha variación induce una fuerza electromotriz (fem) de movimiento en el circuito.

#### 1. Fuerza magnética sobre la barra móvil

Definimos un sistema de coordenadas cartesiano donde:
- El eje $X$ coincide con la dirección de los rieles, apuntando positivamente hacia la derecha ($\hat{x}$).
- El eje $Y$ es perpendicular a los rieles en el plano del circuito, apuntando hacia arriba ($\hat{y}$).
- El eje $Z$ es perpendicular al plano del circuito, saliendo de la página ($\hat{z}$).

El campo magnético uniforme entrante al plano se escribe como:
$$\vec{B} = -B\,\hat{z} \qquad (B > 0)$$

La corriente $I(t)$ circula en sentido horario. En la barra conductora (ubicada en $x(t)$), la corriente fluye desde el riel superior ($y = L$) hacia el riel inferior ($y = 0$), es decir, en la dirección $-\hat{y}$:
$$d\vec{l} = -dy\,\hat{y}$$

El elemento diferencial de fuerza magnética sobre la barra es:
$$d\vec{F} = I(t)\, d\vec{l} \times \vec{B} = I(t)(-dy\,\hat{y}) \times (-B\,\hat{z}) = B I(t)\, dy (\hat{y} \times \hat{z}) = B I(t)\, dy\,\hat{x}$$

Integrando a lo largo de la barra entre los rieles ($y = 0$ a $y = L$):
$$\vec{F}(t) = \int_0^L B I(t)\, dy\,\hat{x} = B L I(t)\,\hat{x}$$

La fuerza neta sobre la barra apunta hacia la derecha ($+\hat{x}$).

#### 2. Ecuación de movimiento y velocidad de la barra

Aplicando la segunda ley de Newton a la barra de masa $m$, considerando movimiento unidimensional a lo largo del eje $X$ sin roce:
$$m \frac{dv}{dt} = B L I(t)$$

Para $t < 0$, la corriente es nula ($I(t) = 0$), por lo que la barra permanece en reposo:
$$v(t) = 0 \qquad (t < 0)$$

Para el intervalo $0 < t \le T$, la corriente es $I(t) = bt$. Separando variables e integrando desde la condición inicial $v(0) = 0$:
$$m \frac{dv}{dt} = B L bt \implies \int_0^{v(t)} dv = \frac{BLb}{m} \int_0^t t'\, dt'$$

$$v(t) = \frac{BLb}{m} \left[\frac{t^2}{2}\right] = \frac{B L b t^2}{2m} \qquad (0 < t \le T)$$

#### 3. Fuerza electromotriz inducida

Consideramos la espira orientada en sentido horario (acorde a la corriente impuesta). Tomando el vector unitario normal al plano en la dirección entrante $\hat{n} = -\hat{z}$ (regla de la mano derecha con sentido horario), el vector área diferencial es $d\vec{A} = -dx\, dy\,\hat{z}$.

El flujo magnético que atraviesa el circuito delimitado por la fuente en $x = 0$ y la barra en $x(t)$ es:
$$\Phi(t) = \int \vec{B} \cdot d\vec{A} = \int_0^{x(t)} dx \int_0^L dy\, (-B\,\hat{z}) \cdot (-\hat{z}) = B L x(t)$$

Alternativamente, tomando $\hat{n} = +\hat{z}$ saliente de la página:
$$\Phi(t) = \int_0^L \int_0^{x(t)} (-B\,\hat{z})\cdot(dx\,dy\,\hat{z}) = -BLx(t)$$

Por la ley de inducción de Faraday, la magnitud de la fem inducida generada por la variación del flujo magnético es:
$$\varepsilon(t) = -\frac{d\Phi}{dt} = -\frac{d}{dt}\left[-B L x(t)\right] = B L \frac{dx}{dt} = B L v(t)$$

Sustituyendo la velocidad obtenida para cada intervalo:
- Para $t < 0$: como $v(t) = 0$, se tiene $\varepsilon(t) = 0$.
- Para $0 < t \le T$:
$$\varepsilon(t) = B L \left(\frac{B L b t^2}{2m}\right) = \frac{B^2 L^2 b t^2}{2m}$$

Por lo tanto:
$$\boxed{v(t) = \begin{cases} 0 & t < 0 \\ \dfrac{B L b t^2}{2m} & 0 < t \le T \end{cases}}$$

$$\boxed{\varepsilon(t) = \begin{cases} 0 & t < 0 \\ \dfrac{B^2 L^2 b t^2}{2m} & 0 < t \le T \end{cases}}$$

**Verificación:**
- **Unidades:**
  - Velocidad: $[B L b t^2 / (2m)] = \text{T} \cdot \text{m} \cdot (\text{A/s}) \cdot \text{s}^2 / \text{kg} = (\text{N}/(\text{A}\cdot\text{m})) \cdot \text{m} \cdot \text{A} \cdot \text{s} / \text{kg} = \text{N}\cdot\text{s}/\text{kg} = \text{m/s}$. Correcto.
  - Fem: $[B^2 L^2 b t^2 / (2m)] = [B L v] = \text{T} \cdot \text{m} \cdot (\text{m/s}) = (\text{V}\cdot\text{s}/\text{m}^2) \cdot \text{m}^2/\text{s} = \text{V}$. Correcto.
- **Límites físicos:** Si $b \to 0$ (no hay corriente) o $B \to 0$ (no hay campo magnético), la fuerza se anula y la barra permanece en reposo ($v = 0, \varepsilon = 0$), tal como se espera.

---

## Problema 2

Un alambre recto con masa $m$ puede moverse en dirección del eje $x$ sobre dos rieles de conductores perfectos en un campo magnético uniforme $\vec{B}$, ver figura. Entre los contactos con los rieles el alambre tiene la resistencia $R$. La distancia entre los rieles es $d$. Así se construye un circuito en forma de un rectángulo. Al tiempo inicial $t_0 = 0$ el alambre se encuentra en la posición inicial $x_0$, con una velocidad inicial $v_0 > 0$.  
Durante el movimiento del alambre, se induce una corriente, y por lo tanto, debido a la presencia del campo $\vec{B}$ aparece una fuerza de Lorentz. Esta fuerza frena el alambre y así disminuye la velocidad durante el movimiento hasta que el alambre deja de moverse.

a) Calcular la corriente inducida en el circuito como función del tiempo suponiendo una trayectoria del alambre general $x(t)$. ¿Cuál es el sentido de dicha corriente?  
b) Usando el resultado de a), calcular la fuerza que actúa en el alambre como función del tiempo.  
c) Usando los resultados anteriores, escriba la ecuación de movimiento para la posición $x(t)$ del alambre y resuélvala usando las condiciones iniciales $x_0$ y $v_0$ en el tiempo $t = 0$.

> **[Figura]:** Dos rieles conductores horizontales paralelos separados una distancia $d$, unidos por un conductor ideal en el extremo izquierdo ($x = 0$), formando una U que se extiende a lo largo del eje $+x$. Una barra conductora vertical de masa $m$ y resistencia $R$ se desliza sobre los rieles con velocidad $\vec{v}(t) = v(t)\,\hat{i}$. Un campo magnético uniforme $\vec{B} = B\,\hat{z}$ sale perpendicularmente de la página (marcado con el símbolo $\odot$).

### Solución

**Idea:** El desplazamiento de la barra móvil modifica el área y por ende el flujo magnético que atraviesa el circuito cerrado. Por la ley de Faraday-Lenz, se genera una fem inducida que impulsa una corriente a través de la resistencia de la barra. Esta corriente, en presencia del campo magnético, experimenta una fuerza magnética opuesta al sentido del movimiento (fuerza de frenado magnético), lo que conduce a una desaceleración exponencial del alambre.

#### Parte a) Corriente inducida y sentido de circulación

1. **Cálculo del flujo magnético:**  
   Tomamos como sentido positivo de circulación el sentido antihorario. Por la regla de la mano derecha, el vector normal al plano apunta hacia afuera de la página: $\hat{n} = +\hat{z}$, de modo que el vector de área es $d\vec{A} = dA\,\hat{z}$.  
   El área abarcada por el rectángulo en el instante $t$ es $A(t) = d \cdot x(t)$. Como el campo magnético uniforme es $\vec{B} = B\,\hat{z}$:
   $$\Phi(t) = \int \vec{B} \cdot d\vec{A} = B \cdot A(t) = B d x(t)$$

2. **Fuerza electromotriz inducida:**  
   Por la ley de inducción de Faraday:
   $$\varepsilon(t) = -\frac{d\Phi}{dt} = -B d \dot{x}(t)$$

3. **Corriente inducida:**  
   Aplicando la ley de Ohm con la resistencia $R$ del alambre (los rieles tienen resistencia nula):
   $$I(t) = \frac{\varepsilon(t)}{R} = -\frac{B d \dot{x}(t)}{R}$$

4. **Sentido de la corriente:**  
   Dado que $\dot{x}(t) = v(t) > 0$, el valor algebraico de $I(t)$ es estrictamente negativo con respecto a la convención antihoraria adoptada. Esto significa que **la corriente circula en sentido horario**.  
   *Justificación por ley de Lenz:* Al avanzar el alambre hacia la derecha, el área del circuito aumenta y el flujo magnético saliente ($\odot$) se incrementa. Para oponerse a este incremento, la corriente inducida debe generar un campo magnético inducido que apunte hacia adentro de la página ($\otimes$). Por la regla de la mano derecha, un campo inducido entrante es producido por una corriente que circula en sentido horario.

$$\boxed{I(t) = -\frac{B d \dot{x}(t)}{R} \quad \text{(sentido horario)}}$$

---

#### Parte b) Fuerza magnética sobre el alambre

En el alambre conductor (que se extiende a lo largo de la coordenada $y$ de $0$ a $d$), la corriente circula en sentido horario, es decir, de arriba hacia abajo ($-\hat{y}$):
$$I \vec{L} = |I|(-d\,\hat{y}) = - |I| d\,\hat{y}$$

O bien, usando la corriente algebraica $I(t) = -\frac{Bd\dot{x}}{R}$ asociada a la dirección antihoraria ($d\vec{l} = dy\,\hat{y}$):
$$\vec{F}(t) = \int_0^d I(t)\, dy\,\hat{y} \times B\,\hat{z} = I(t) d B (\hat{y} \times \hat{z}) = I(t) d B\,\hat{x}$$

Reemplazando la expresión de $I(t)$:
$$\vec{F}(t) = \left(-\frac{B d \dot{x}(t)}{R}\right) d B\,\hat{x} = -\frac{(Bd)^2 \dot{x}(t)}{R}\,\hat{x}$$

$$\boxed{\vec{F}(t) = -\frac{(Bd)^2 \dot{x}(t)}{R}\,\hat{x}}$$

La fuerza apunta en la dirección $-\hat{x}$, actuando como una fuerza disipativa viscosa que frena el movimiento del alambre.

---

#### Parte c) Ecuación de movimiento y solución

1. **Ecuación diferencial:**  
   Aplicando la segunda ley de Newton sobre el alambre en el eje $X$:
   $$m \ddot{x} = -\frac{(Bd)^2}{R} \dot{x} \implies m \frac{dv}{dt} = -\frac{(Bd)^2}{R} v$$

   Definiendo la constante de tiempo característica del frenado:
   $$\tau = \frac{m R}{(Bd)^2}$$

   La ecuación se reduce a:
   $$\frac{dv}{dt} = -\frac{1}{\tau} v$$

2. **Cálculo de la velocidad $v(t)$:**  
   Separando variables e integrando desde $t = 0$ con $v(0) = v_0$:
   $$\int_{v_0}^{v(t)} \frac{dv}{v} = -\frac{1}{\tau} \int_0^t dt' \implies \ln\left(\frac{v(t)}{v_0}\right) = -\frac{t}{\tau}$$

   $$v(t) = v_0 \exp\left(-\frac{t}{\tau}\right) = v_0 \exp\left(-\frac{(Bd)^2}{mR} t\right)$$

3. **Cálculo de la posición $x(t)$:**  
   Como $v(t) = \frac{dx}{dt}$, integramos con la condición inicial $x(0) = x_0$:
   $$\int_{x_0}^{x(t)} dx' = \int_0^t v_0 \exp\left(-\frac{t'}{\tau}\right) dt'$$

   $$x(t) - x_0 = v_0 \left[-\tau \exp\left(-\frac{t'}{\tau}\right)\right]_0^t = v_0 \tau \left(1 - \exp\left(-\frac{t}{\tau}\right)\right)$$

   Reemplazando $\tau = \frac{mR}{(Bd)^2}$:
   $$x(t) = x_0 + \frac{v_0 m R}{(Bd)^2} \left[1 - \exp\left(-\frac{(Bd)^2}{mR} t\right)\right]$$

4. **Posición final del alambre:**  
   El alambre se detiene cuando $t \to \infty$ ($v \to 0$):
   $$x_{\text{final}} = \lim_{t \to \infty} x(t) = x_0 + \frac{v_0 m R}{(Bd)^2}$$

$$\boxed{x(t) = x_0 + \frac{v_0 m R}{(Bd)^2} \left[1 - \exp\left(-\frac{(Bd)^2}{mR} t\right)\right]}$$

$$\boxed{x_{\text{final}} = x_0 + \frac{v_0 m R}{(Bd)^2}}$$

**Verificación:**
- **Unidades:**
  - $[\tau] = [\text{kg} \cdot \Omega / (\text{T}^2 \cdot \text{m}^2)] = \text{s}$.
  - $[v_0 \tau] = (\text{m/s}) \cdot \text{s} = \text{m}$, consistente con dimensiones de posición.
- **Límites:** En $t = 0$, $x(0) = x_0$ y $v(0) = v_0$. Si $B \to 0$ o $R \to \infty$, la fuerza de frenado desaparece ($\tau \to \infty$), recuperando el movimiento rectilíneo uniforme $x(t) = x_0 + v_0 t$.

---

## Problema 3

Una barra conductora de masa $m$ desliza sin roce sobre dos rieles conductores paralelos separados una distancia $b$. El circuito posee un switch que puede cambiar entre dos posiciones. Si el switch se encuentra en la posición 1, los rieles quedan conectados únicamente mediante una resistencia $R$, mientras que si se mueve a la posición 2, los rieles quedan conectados por la misma resistencia $R$ y una batería que provee una diferencia de potencial $V_0$ (ver Figura). Hay un campo magnético uniforme $\vec{B} = B_0\,\hat{z}$ perpendicular al plano de la Figura.

a) Considere que inicialmente el switch se encuentra en la posición 1 y se le imparte una velocidad $v_0$ a la barra en $t = 0$. Determine la velocidad en función del tiempo de la barra y el desplazamiento máximo que alcanza la misma.  
b) Suponiendo que la barra alcanzó su máximo desplazamiento, el switch se cambia a la posición 2 y se reinicia el tiempo. Determine nuevamente la velocidad de la barra en el tiempo.

> **[Figura]:** Circuito con dos rieles conductores horizontales paralelos separados una distancia $b$. A la izquierda, un conmutador (switch) permite conectar la barra a través del riel inferior a dos ramas:
> - Posición 1: la rama izquierda contiene únicamente una resistencia $R$ conectada al riel superior.
> - Posición 2: la rama inferior añade en serie con $R$ una fuente de voltaje continua $V_0$, orientada con el terminal positivo conectado hacia el riel inferior (hacia la derecha/barra) y el terminal negativo hacia el switch/resistencia $R$.
> Sobre los rieles desliza una barra vertical de masa $m$ ubicada a la derecha. En toda la región existe un campo magnético uniforme saliente $\vec{B} = B_0\,\hat{z}$ (representado por puntos $\bullet$).

### Solución

**Idea:** En la posición 1, el circuito actúa como un freno magnético pasivo donde la energía cinética de la barra se disipa por efecto Joule en la resistencia $R$. En la posición 2, la fuente de poder $V_0$ introduce una corriente externa que impulsa a la barra hacia adelante mediante una fuerza de Lorentz motriz, hasta alcanzar una velocidad límite donde la fem inducida de movimiento contrarresta exactamente la fem de la batería.

#### Parte a) Switch en la posición 1

1. **Fem y corriente inducida:**  
   Tomando la orientación antihoraria como positiva:
   $$\Phi(t) = B_0 b x(t) \implies \varepsilon(t) = -\frac{d\Phi}{dt} = -B_0 b \dot{x}(t)$$
   La corriente que circula por la resistencia $R$ es:
   $$I(t) = \frac{\varepsilon(t)}{R} = -\frac{B_0 b \dot{x}(t)}{R}$$
   El signo negativo indica que la corriente fluye en sentido horario (hacia abajo por la barra, $-\hat{y}$).

2. **Fuerza magnética y ecuación de movimiento:**  
   La fuerza magnética que experimenta la barra conductora es:
   $$\vec{F} = \int_0^b I(t)\, dy\,\hat{y} \times B_0\,\hat{z} = I(t) b B_0\,\hat{x} = -\frac{(B_0 b)^2 \dot{x}(t)}{R}\,\hat{x}$$
   Por la segunda ley de Newton:
   $$m \frac{dv}{dt} = -\frac{(B_0 b)^2}{R} v$$

3. **Cálculo de la velocidad y desplazamiento máximo:**  
   Integrando con la condición inicial $v(0) = v_0$:
   $$\int_{v_0}^{v(t)} \frac{dv}{v} = -\frac{(B_0 b)^2}{mR} \int_0^t dt' \implies v(t) = v_0 \exp\left(-\frac{(B_0 b)^2}{mR} t\right)$$

   Integrando la velocidad para obtener la trayectoria, tomando la posición de partida como el origen ($x(0) = 0$):
   $$x(t) = \int_0^t v(t')\, dt' = v_0 \int_0^t \exp\left(-\frac{(B_0 b)^2}{mR} t'\right) dt' = \frac{v_0 m R}{(B_0 b)^2} \left[1 - \exp\left(-\frac{(B_0 b)^2}{mR} t\right)\right]$$

   El desplazamiento máximo alcanzado se obtiene cuando la barra se detiene ($t \to \infty$):
   $$x_{\text{final}} = \lim_{t \to \infty} x(t) = \frac{v_0 m R}{(B_0 b)^2}$$

$$\boxed{v(t) = v_0 \exp\left(-\frac{(B_0 b)^2}{mR} t\right)}$$

$$\boxed{\Delta x_{\max} = \frac{v_0 m R}{(B_0 b)^2}}$$

---

#### Parte b) Switch en la posición 2

1. **Condición inicial y corrientes en el circuito:**  
   Al conmutar a la posición 2, la barra parte del reposo: $v(0) = 0$, y se reinicia el reloj ($t = 0$).  
   La batería $V_0$ está conectada de tal forma que empuja corriente desde su terminal positivo hacia el riel inferior y hacia arriba por la barra (sentido antihorario). La corriente impuesta por la batería es:
   $$I_0 = +\frac{V_0}{R} \quad \text{(sentido antihorario)}$$

   A medida que la barra adquiere velocidad hacia la derecha ($\dot{x} > 0$), la fem inducida se opone al aumento de flujo saliente, aportando una corriente inducida en sentido horario:
   $$I_{\text{ind}}(t) = -\frac{B_0 b \dot{x}(t)}{R}$$

   La corriente neta que circula por la barra en sentido antihorario ($+\hat{y}$) es:
   $$I_{\text{neto}}(t) = I_0 + I_{\text{ind}}(t) = \frac{V_0}{R} - \frac{B_0 b \dot{x}(t)}{R}$$

2. **Fuerza total sobre la barra:**  
   $$\vec{F} = \int_0^b I_{\text{neto}}(t)\, dy\,\hat{y} \times B_0\,\hat{z} = I_{\text{neto}}(t) b B_0\,\hat{x} = \left(\frac{V_0 B_0 b}{R} - \frac{(B_0 b)^2 \dot{x}}{R}\right)\hat{x}$$

3. **Ecuación diferencial y resolución:**  
   Aplicando la segunda ley de Newton:
   $$m \frac{dv}{dt} = \frac{V_0 B_0 b}{R} - \frac{(B_0 b)^2}{R} v$$

   Reordenando en forma canónica lineal:
   $$\frac{dv}{dt} + \frac{(B_0 b)^2}{mR} v = \frac{V_0 B_0 b}{mR}$$

   Multiplicando por el factor integrante $\mu(t) = \exp\left(\frac{(B_0 b)^2}{mR} t\right)$:
   $$\frac{d}{dt}\left[v(t) \exp\left(\frac{(B_0 b)^2}{mR} t\right)\right] = \frac{V_0 B_0 b}{mR} \exp\left(\frac{(B_0 b)^2}{mR} t\right)$$

   Integrando a ambos lados entre $0$ y $t$, e imponiendo que la barra parte del reposo ($v(0) = 0$):
   $$v(t) \exp\left(\frac{(B_0 b)^2}{mR} t\right) = \frac{V_0 B_0 b}{mR} \int_0^t \exp\left(\frac{(B_0 b)^2}{mR} t'\right) dt'$$

   $$v(t) \exp\left(\frac{(B_0 b)^2}{mR} t\right) = \frac{V_0 B_0 b}{mR} \cdot \frac{mR}{(B_0 b)^2} \left[\exp\left(\frac{(B_0 b)^2}{mR} t\right) - 1\right] = \frac{V_0}{B_0 b} \left[\exp\left(\frac{(B_0 b)^2}{mR} t\right) - 1\right]$$

   Multiplicando por $\exp\left(-\frac{(B_0 b)^2}{mR} t\right)$:
   $$v(t) = \frac{V_0}{B_0 b} \left[1 - \exp\left(-\frac{(B_0 b)^2}{mR} t\right)\right]$$

$$\boxed{v(t) = \frac{V_0}{B_0 b} \left[1 - \exp\left(-\frac{(B_0 b)^2}{mR} t\right)\right]}$$

**Verificación:**
- **Comportamiento asintótico:** Cuando $t \to \infty$, la velocidad tiende a una velocidad terminal constante:
  $$v_{\infty} = \lim_{t \to \infty} v(t) = \frac{V_0}{B_0 b}$$
  A esta velocidad, la fem de movimiento generada es $\varepsilon_{\text{mov}} = B_0 b v_{\infty} = V_0$, la cual equilibra exactamente el voltaje de la fuente $V_0$. En consecuencia, la corriente neta en el circuito se reduce a cero ($I_{\text{neto}} = 0$) y la aceleración se extingue, manteniendo la barra a velocidad constante.
- **Unidades:** $[V_0 / (B_0 b)] = \text{V} / (\text{T} \cdot \text{m}) = \text{V} / ((\text{V}\cdot\text{s}/\text{m}^2)\cdot\text{m}) = \text{m/s}$. Correcto.

---

## Resumen de resultados

| Problema | Magnitud requerida | Resultado analítico |
| :--- | :--- | :--- |
| **P1** | Velocidad de la barra $v(t)$ ($0 < t \le T$) | $v(t) = \dfrac{B L b t^2}{2m}$ |
| **P1** | Fem inducida $\varepsilon(t)$ ($0 < t \le T$) | $\varepsilon(t) = \dfrac{B^2 L^2 b t^2}{2m}$ |
| **P2 (a)** | Corriente inducida $I(t)$ | $I(t) = -\dfrac{B d \dot{x}(t)}{R} \quad \text{(sentido horario)}$ |
| **P2 (b)** | Fuerza de Lorentz sobre el alambre $\vec{F}(t)$ | $\vec{F}(t) = -\dfrac{(Bd)^2 \dot{x}(t)}{R}\,\hat{x}$ |
| **P2 (c)** | Posición en el tiempo $x(t)$ | $x(t) = x_0 + \dfrac{v_0 m R}{(Bd)^2} \left[1 - \exp\left(-\dfrac{(Bd)^2}{mR} t\right)\right]$ |
| **P2 (c)** | Posición final $x_{\text{final}}$ | $x_{\text{final}} = x_0 + \dfrac{v_0 m R}{(Bd)^2}$ |
| **P3 (a)** | Velocidad de la barra $v(t)$ (Switch en pos. 1) | $v(t) = v_0 \exp\left(-\dfrac{(B_0 b)^2}{mR} t\right)$ |
| **P3 (a)** | Desplazamiento máximo $\Delta x_{\max}$ | $\Delta x_{\max} = \dfrac{v_0 m R}{(B_0 b)^2}$ |
| **P3 (b)** | Velocidad de la barra $v(t)$ (Switch en pos. 2) | $v(t) = \dfrac{V_0}{B_0 b} \left[1 - \exp\left(-\dfrac{(B_0 b)^2}{mR} t\right)\right]$ |
| **P3 (b)** | Velocidad terminal asintótica $v_{\infty}$ | $v_{\infty} = \dfrac{V_0}{B_0 b}$ |
