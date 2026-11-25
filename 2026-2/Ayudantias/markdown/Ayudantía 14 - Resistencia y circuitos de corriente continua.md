# Ayudantía 14 — Resistencia y circuitos de corriente continua

> Clases relacionadas: [Clase 08 - Corriente electrica y resistencias](../../Clases/markdown/Clase%2008%20-%20Corriente%20electrica%20y%20resistencias.md), [Clase 09 - Potencia, circuitos de resistencias y circuito RC](../../Clases/markdown/Clase%2009%20-%20Potencia%2C%20circuitos%20de%20resistencias%20y%20circuito%20RC.md)

---

## Problema 1

Considere un tronco de cono recto con radios $a = 1\text{ mm}$, $b = 5\text{ mm}$ y altura $h = 10\text{ cm}$, fabricado de grafito con resistividad $\rho = 3 \times 10^{-3}\,\Omega\cdot\text{m}$. En las dos superficies circulares del tronco se depositan capas delgadas de un conductor perfecto para obtener dos contactos. Se conectan los contactos con una pila de $9\text{ V}$ y un resistor de $100\,\Omega$ en serie. Determine los siguientes valores numéricos:

a) La resistencia entre los dos contactos del tronco de cono recto.  
b) La potencia disipada en el tronco de cono recto.

> **[Figura]:** Tronco de cono recto orientado a lo largo de un eje vertical $z$. La cara circular inferior se sitúa en $z = 0$ y posee un radio menor $a = 1\text{ mm}$; la cara circular superior se sitúa en $z = h = 10\text{ cm}$ y posee un radio mayor $b = 5\text{ mm}$. Ambas superficies planas circulares están recubiertas de capas delgadas metálicas de conductor perfecto (resistencia nula), que funcionan como terminales de contacto. El tronco de cono se conecta en serie mediante cables conductores con un resistor fijo de resistencia $R_s = 100\,\Omega$ y una fuente de fem continua $V = 9\text{ V}$.

### Solución

**Idea:** Para calcular la resistencia de un cuerpo conductor con sección transversal no uniforme a lo largo de la dirección de la corriente, se divide el conductor en rebanadas diferenciales de espesor $dz$ perpendiculares a las líneas de corriente. Cada rebanada tiene una resistencia incremental $dR = \rho \frac{dz}{A(z)}$. La resistencia total se obtiene integrando desde $z = 0$ hasta $z = h$. Luego, la corriente del circuito serie se determina mediante la ley de Ohm ($I = \frac{V}{R_{\text{eq}}}$) y la potencia disipada por efecto Joule en el tronco se calcula mediante $P_c = I^2 R_c$.

#### Parte a) Resistencia del tronco de cono recto

1. **Variación del radio y del área transversal con la altura:**  
   Definimos un eje $z$ que coincide con el eje de simetría del cono, con $z = 0$ en la base de radio menor $a$ y $z = h$ en la base de radio mayor $b$. La variación del radio $r(z)$ es lineal:
   $$r(z) = a + \left(\frac{b - a}{h}\right) z$$

   El área transversal circular a una altura $z$ es:
   $$A(z) = \pi [r(z)]^2 = \pi \left(a + \frac{b - a}{h} z\right)^2$$

2. **Integración de la resistencia:**  
   Considerando cada elemento infinitesimal de altura $dz$ como un resistor en serie de sección transversal $A(z)$:
   $$dR = \rho \frac{dz}{A(z)} = \frac{\rho}{\pi \left(a + \frac{b - a}{h} z\right)^2}\, dz$$

   La resistencia total entre ambas caras conductoras es:
   $$R_c = \int_0^h \frac{\rho}{\pi \left(a + \frac{b - a}{h} z\right)^2}\, dz$$

   Efectuamos el cambio de variable:
   $$u = a + \frac{b - a}{h} z \implies du = \left(\frac{b - a}{h}\right) dz \implies dz = \frac{h}{b - a}\, du$$

   Los límites de integración se transforman en $u(0) = a$ y $u(h) = b$:
   $$R_c = \frac{\rho h}{\pi (b - a)} \int_a^b \frac{du}{u^2} = \frac{\rho h}{\pi (b - a)} \left[ -\frac{1}{u} \right]_a^b = \frac{\rho h}{\pi (b - a)} \left(\frac{1}{a} - \frac{1}{b}\right)$$

   Simplificando la diferencia de fracciones:
   $$\frac{1}{a} - \frac{1}{b} = \frac{b - a}{ab}$$

   Por lo tanto, los factores $(b - a)$ se cancelan exactamente:
   $$R_c = \frac{\rho h}{\pi ab}$$

3. **Evaluación numérica:**  
   Datos del enunciado:
   - $a = 1\text{ mm} = 10^{-3}\text{ m}$
   - $b = 5\text{ mm} = 5 \times 10^{-3}\text{ m}$
   - $h = 10\text{ cm} = 0{,}1\text{ m}$
   - $\rho = 3 \times 10^{-3}\,\Omega\cdot\text{m}$

   Reemplazando:
   $$R_c = \frac{(3 \times 10^{-3}\,\Omega\cdot\text{m})(0{,}1\text{ m})}{\pi (10^{-3}\text{ m})(5 \times 10^{-3}\text{ m})} = \frac{3 \times 10^{-4}}{5\pi \times 10^{-6}}\,\Omega = \frac{300}{5\pi}\,\Omega = \frac{60}{\pi}\,\Omega$$

   Aproximando con decimales:
   $$R_c = \frac{60}{\pi}\,\Omega \approx 19{,}0986\,\Omega \approx 19{,}10\,\Omega$$

$$\boxed{R_c = \frac{60}{\pi}\,\Omega \approx 19{,}10\,\Omega}$$

---

#### Parte b) Potencia disipada en el tronco de cono recto

1. **Resistencia equivalente del circuito:**  
   La pila de voltaje $V = 9\text{ V}$, el resistor fijo $R_s = 100\,\Omega$ y el tronco de cono $R_c$ forman un circuito de una sola malla en serie:
   $$R_{\text{eq}} = R_s + R_c = 100 + \frac{60}{\pi}\,\Omega \approx 100 + 19{,}10 = 119{,}10\,\Omega$$

2. **Corriente eléctrica en el circuito:**  
   Por la ley de Ohm:
   $$I = \frac{V}{R_{\text{eq}}} = \frac{9\text{ V}}{100 + \frac{60}{\pi}\,\Omega} = \frac{9}{119{,}10}\text{ A} \approx 0{,}07557\text{ A}$$

3. **Potencia disipada en el tronco de cono:**  
   La potencia disipada en forma de calor por efecto Joule exclusivamente en el tronco de cono es:
   $$P_c = I^2 R_c = \left(\frac{9}{100 + \frac{60}{\pi}}\right)^2 \left(\frac{60}{\pi}\right)$$
   $$P_c \approx (0{,}075568\text{ A})^2 \times (19{,}0986\,\Omega) \approx 0{,}10906\text{ W} \approx 0{,}109\text{ W} = 109\text{ mW}$$

$$\boxed{P_c \approx 0{,}109\text{ W} = 109\text{ mW}}$$

**Verificación:**
- **Unidades:** En parte a), $[\rho h / (\pi a b)] = [\Omega\cdot\text{m}\cdot\text{m}/\text{m}^2] = [\Omega]$, consistente. En parte b), $[I^2 R] = [\text{A}^2 \cdot \Omega] = [\text{W}]$, consistente.
- **Caso límite:** Si $a = b$ (cilindro circular recto de radio $a$), $R_c = \frac{\rho h}{\pi a^2}$, que coincide con la fórmula de Poiseuille/Ohm habitual $R = \rho L / A$.

---

## Problema 2

En el circuito indicado en la figura se piden determinar los siguientes valores numéricos:

a) El voltaje (diferencia de potencial) entre los puntos A y B.  
b) La potencia total disipada en forma de calor por el circuito.

> **[Figura]:** Circuito de dos mallas formado por tres ramas paralelas conectadas entre un nodo superior central $A$ y un nodo inferior central $B$:
> - **Rama izquierda:** Se extiende entre $A$ y $B$. Contiene una resistencia superior de $1\,\Omega$, una fuente ideal de fem de $2\text{ V}$ conectada en el tramo vertical con el terminal positivo hacia arriba (hacia $A$) y el terminal negativo hacia abajo, y una resistencia inferior de $1\,\Omega$. La resistencia total de la rama es $R_{\text{izq}} = 1 + 1 = 2\,\Omega$.
> - **Rama central:** Conecta directamente los nodos $A$ y $B$ mediante una resistencia de $4\,\Omega$ en serie con una fuente ideal de fem de $4\text{ V}$. La fuente está orientada con el terminal positivo hacia abajo (conectado al nodo $B$) y el terminal negativo hacia arriba (conectado al resistor de $4\,\Omega$).
> - **Rama derecha:** Idéntica y simétrica a la rama izquierda. Contiene una resistencia superior de $1\,\Omega$, una fuente de fem de $2\text{ V}$ vertical con el terminal positivo hacia arriba (hacia $A$) y el terminal negativo hacia abajo, y una resistencia inferior de $1\,\Omega$. La resistencia total de la rama es $R_{\text{der}} = 1 + 1 = 2\,\Omega$.

### Solución

**Idea:** Dado que el circuito posee solo dos nodos esenciales ($A$ y $B$) a los cuales confluyen tres ramas en paralelo, el método de tensiones nodales (Ley de Corrientes de Kirchhoff en el nodo $A$) es el camino más directo. Fijando el potencial del nodo $B$ como referencia ($V_B = 0\text{ V}$), determinamos $V_A$ y con ello las corrientes en cada una de las tres ramas. Finalmente, la potencia disipada en forma de calor es la suma de las pérdidas por efecto Joule ($P = I^2 R$) en todas las resistencias del circuito.

#### Parte a) Voltaje entre los puntos A y B

1. **Definición de referencia y potenciales de rama:**  
   Fijamos el nodo $B$ como tierra:
   $$V_B = 0\text{ V}$$
   El voltaje buscado es $V_{AB} = V_A - V_B = V_A$.

2. **Corrientes salientes desde el nodo A:**  
   Definimos las corrientes de cada rama saliendo del nodo $A$ hacia el nodo $B$:
   - **Rama izquierda:** Las dos resistencias de $1\,\Omega$ están en serie, $R_{\text{izq}} = 1\,\Omega + 1\,\Omega = 2\,\Omega$. Al descender de $A$ a $B$, la fuente de $2\text{ V}$ tiene su terminal positivo hacia $A$, por lo que el potencial intermedio bajo la fuente es $+2\text{ V}$ respecto a $B$. La caída resistiva es $V_A - 2\text{ V}$:
     $$I_{\text{izq}} = \frac{V_A - 2}{2}$$
   - **Rama central:** La resistencia es $R_{\text{cen}} = 4\,\Omega$. La fuente de $4\text{ V}$ tiene su polo positivo en $B$ y el negativo hacia arriba, por lo que el potencial en el punto inmediatamente inferior a la resistencia de $4\,\Omega$ es $-4\text{ V}$ con respecto a $B$. La corriente descendente es:
     $$I_{\text{cen}} = \frac{V_A - (-4)}{4} = \frac{V_A + 4}{4}$$
   - **Rama derecha:** Por simetría con la rama izquierda ($R_{\text{der}} = 2\,\Omega$ y fem de $2\text{ V}$ con polo positivo arriba):
     $$I_{\text{der}} = \frac{V_A - 2}{2}$$

3. **Ley de Corrientes de Kirchhoff (LCK) en el nodo A:**  
   $$\sum I_{\text{salen}} = 0 \implies I_{\text{izq}} + I_{\text{cen}} + I_{\text{der}} = 0$$
   $$\frac{V_A - 2}{2} + \frac{V_A + 4}{4} + \frac{V_A - 2}{2} = 0$$

   Multiplicando toda la ecuación por $4$:
   $$2(V_A - 2) + (V_A + 4) + 2(V_A - 2) = 0$$
   $$2V_A - 4 + V_A + 4 + 2V_A - 4 = 0$$
   $$5V_A - 4 = 0 \implies 5V_A = 4 \implies V_A = \frac{4}{5} = 0{,}8\text{ V}$$

   Por lo tanto:
   $$V_{AB} = V_A - V_B = 0{,}8\text{ V} - 0\text{ V} = 0{,}8\text{ V}$$

$$\boxed{V_{AB} = 0{,}8\text{ V}}$$

---

#### Parte b) Potencia total disipada en forma de calor por el circuito

1. **Cálculo de las corrientes en cada rama:**  
   Sustituyendo $V_A = 0{,}8\text{ V}$ en las expresiones de corriente:
   - **Rama izquierda:**
     $$I_{\text{izq}} = \frac{0{,}8 - 2}{2} = \frac{-1{,}2}{2} = -0{,}6\text{ A}$$
     El signo negativo indica que una corriente de magnitud $|I_{\text{izq}}| = 0{,}6\text{ A}$ fluye hacia arriba (desde $B$ hacia $A$).
   - **Rama central:**
     $$I_{\text{cen}} = \frac{0{,}8 + 4}{4} = \frac{4{,}8}{4} = 1{,}2\text{ A}$$
     Fluye hacia abajo (desde $A$ hacia $B$).
   - **Rama derecha:**
     $$I_{\text{der}} = \frac{0{,}8 - 2}{2} = -0{,}6\text{ A}$$
     Fluye hacia arriba (desde $B$ hacia $A$) con magnitud $|I_{\text{der}}| = 0{,}6\text{ A}$.

   *(Nótese que en el nodo $A$: $0{,}6\text{ A} + 0{,}6\text{ A} = 1{,}2\text{ A}$, satisfaciendo la LCK).*

2. **Potencia disipada en las resistencias de cada rama ($P = I^2 R$):**  
   - **Rama izquierda ($R_{\text{izq}} = 2\,\Omega$):**
     $$P_{\text{izq}} = (0{,}6\text{ A})^2 \times 2\,\Omega = 0{,}36 \times 2 = 0{,}72\text{ W}$$
   - **Rama central ($R_{\text{cen}} = 4\,\Omega$):**
     $$P_{\text{cen}} = (1{,}2\text{ A})^2 \times 4\,\Omega = 1{,}44 \times 4 = 5{,}76\text{ W}$$
   - **Rama derecha ($R_{\text{der}} = 2\,\Omega$):**
     $$P_{\text{der}} = (0{,}6\text{ A})^2 \times 2\,\Omega = 0{,}36 \times 2 = 0{,}72\text{ W}$$

3. **Potencia total disipada:**  
   $$P_{\text{total}} = P_{\text{izq}} + P_{\text{cen}} + P_{\text{der}} = 0{,}72\text{ W} + 5{,}76\text{ W} + 0{,}72\text{ W} = 7{,}20\text{ W}$$

$$\boxed{P_{\text{total}} = 7{,}2\text{ W}}$$

**Verificación:**
- **Balance de potencia con las fuentes:**
  - Las fuentes de $2\text{ V}$ de las ramas izquierda y derecha tienen corrientes que ingresan por su borne negativo y salen por el positivo (entregan potencia):
    $$P_{\text{fuente, izq}} = (2\text{ V})(0{,}6\text{ A}) = 1{,}2\text{ W}$$
    $$P_{\text{fuente, der}} = (2\text{ V})(0{,}6\text{ A}) = 1{,}2\text{ W}$$
  - La fuente de $4\text{ V}$ en la rama central tiene una corriente de $1{,}2\text{ A}$ que va de $A$ a $B$, es decir, entra por su borne negativo (arriba) y sale por su borne positivo (abajo), por lo que también entrega potencia:
    $$P_{\text{fuente, cen}} = (4\text{ V})(1{,}2\text{ A}) = 4{,}8\text{ W}$$
  - Potencia total suministrada por las fuentes:
    $$P_{\text{suministrada}} = 1{,}2\text{ W} + 1{,}2\text{ W} + 4{,}8\text{ W} = 7{,}2\text{ W}$$
  Coincide de manera exacta con la potencia total disipada por calor en las resistencias ($7{,}2\text{ W}$).

---

## Problema 3

En la Figura adjunta, $R_1 = R_2 = 2\,\Omega$, $R_3 = 4\,\Omega$, $R_4 = 3\,\Omega$, $R_5 = 1\,\Omega$ y $R_6 = R_7 = R_8 = 8\,\Omega$. Las baterías son ideales, cuyas fem son $\varepsilon_1 = 16\text{ V}$ y $\varepsilon_2 = 8\text{ V}$.

a) Determine la resistencia equivalente de las 6 resistencias que se ubican a la izquierda de la batería $\varepsilon_1$, es decir, de las resistencias $R_1$, $R_2$, $R_3$, $R_6$, $R_7$ y $R_8$.  
b) Determine el valor y la dirección de la corriente $i_1$.  
c) ¿Cuál es la potencia que entregan las baterías 1 y 2? ¿La energía está siendo entregada o absorbida por las baterías 1 y 2?

> **[Figura]:** Red circuital plana compuesta por dos sectores separados por una rama vertical central:
> - **Rama vertical central:** Contiene la batería ideal $\varepsilon_1 = 16\text{ V}$ orientada con el polo positivo arriba y el polo negativo abajo. Por esta rama se define una corriente $i_1$ con flecha dirigida verticalmente hacia arriba.
> - **Sector izquierdo (a la izquierda de $\varepsilon_1$):**
>   - En el lazo vertical izquierdo inferior se encuentran dos resistencias de $8\,\Omega$ en paralelo: $R_8 = 8\,\Omega$ en la rama vertical exterior y $R_7 = 8\,\Omega$ en una rama vertical adyacente.
>   - Directamente sobre este conjunto paralelo, en la rama vertical izquierda, se sitúa la resistencia $R_1 = 2\,\Omega$.
>   - En el riel superior izquierdo horizontal se encuentra $R_2 = 2\,\Omega$.
>   - Una rama vertical intermedia contiene $R_6 = 8\,\Omega$.
>   - Conectando el nodo superior de $R_6$ con el terminal positivo de $\varepsilon_1$ se encuentra la resistencia horizontal $R_3 = 4\,\Omega$.
>   - El riel inferior horizontal común conecta las bases de $R_8$, $R_7$, $R_6$ y el terminal negativo de $\varepsilon_1$.
> - **Sector derecho (a la derecha de $\varepsilon_1$):**
>   - El riel superior contiene $R_4 = 3\,\Omega$.
>   - La rama vertical derecha exterior contiene $R_5 = 1\,\Omega$.
>   - El riel inferior contiene una segunda batería ideal $\varepsilon_2 = 8\text{ V}$ orientada horizontalmente con el polo negativo a la izquierda y el polo positivo a la derecha.

### Solución

**Idea:** Para la parte a), aplicamos reducciones sucesivas serie-paralelo de izquierda a derecha. Para la parte b), observamos que la batería ideal $\varepsilon_1$ fija la diferencia de potencial sobre la resistencia equivalente izquierda y sobre el lazo derecho. Mediante la Ley de Mallas de Kirchhoff (LVK) en el lazo derecho y la Ley de Corrientes de Kirchhoff (LCK) en el nodo superior de $\varepsilon_1$, obtenemos $i_1$. En la parte c), calculamos $P = I\varepsilon$ para cada fuente y determinamos si entregan o absorben energía analizando el sentido relativo entre la corriente y la fem.

#### Parte a) Resistencia equivalente de las 6 resistencias a la izquierda de $\varepsilon_1$

1. **Paralelo entre $R_7$ y $R_8$:**  
   Ambas resistencias de $8\,\Omega$ comparten sus terminales superior e inferior:
   $$R_{78} = \frac{R_7 R_8}{R_7 + R_8} = \frac{(8\,\Omega)(8\,\Omega)}{8\,\Omega + 8\,\Omega} = \frac{64}{16}\,\Omega = 4\,\Omega$$

2. **Rama izquierda en serie ($R_{78}$, $R_1$ y $R_2$):**  
   Al estar conectadas en una única trayectoria sin bifurcaciones:
   $$R_A = R_{78} + R_1 + R_2 = 4\,\Omega + 2\,\Omega + 2\,\Omega = 8\,\Omega$$

3. **Paralelo entre $R_A$ y $R_6$:**  
   La rama compuesta $R_A$ queda conectada en paralelo con la resistencia vertical $R_6 = 8\,\Omega$:
   $$R_{A6} = \frac{R_A R_6}{R_A + R_6} = \frac{(8\,\Omega)(8\,\Omega)}{8\,\Omega + 8\,\Omega} = 4\,\Omega$$

4. **Resistencia equivalente total con $R_3$ en serie:**  
   Finalmente, este conjunto $R_{A6}$ se encuentra en serie con la resistencia horizontal $R_3 = 4\,\Omega$ que conduce directamente a la batería $\varepsilon_1$:
   $$R_{\text{eq}} = R_{A6} + R_3 = 4\,\Omega + 4\,\Omega = 8\,\Omega$$

$$\boxed{R_{\text{eq}} = 8\,\Omega}$$

---

#### Parte b) Valor y dirección de la corriente $i_1$

1. **Corriente hacia el subcircuito izquierdo ($i_{\text{izq}}$):**  
   La batería $\varepsilon_1 = 16\text{ V}$ está conectada directamente en paralelo entre el nodo superior y el riel inferior del subcircuito izquierdo. Por la ley de Ohm:
   $$i_{\text{izq}} = \frac{\varepsilon_1}{R_{\text{eq}}} = \frac{16\text{ V}}{8\,\Omega} = 2\text{ A}$$
   Esta corriente sale del nodo superior hacia la izquierda.

2. **Corriente en el lazo derecho ($i_2$):**  
   Definimos una corriente de malla $i_2$ en sentido horario en el lazo derecho (sale del nodo superior hacia la derecha, recorre $R_4$ y $R_5$, atraviesa la fuente $\varepsilon_2$ hacia la izquierda y retorna al nodo inferior de $\varepsilon_1$).  
   Aplicando la Ley de Voltajes de Kirchhoff (LVK) en el lazo derecho en sentido horario:
   $$\varepsilon_1 - i_2 R_4 - i_2 R_5 - \varepsilon_2 = 0$$

   *(Nótese que en el tramo inferior, al recorrer en sentido horario de derecha a izquierda, se entra por el terminal positivo de $\varepsilon_2$ y se sale por el negativo, produciendo una caída $-\varepsilon_2$).*

   Despejando $i_2$:
   $$i_2 = \frac{\varepsilon_1 - \varepsilon_2}{R_4 + R_5} = \frac{16\text{ V} - 8\text{ V}}{3\,\Omega + 1\,\Omega} = \frac{8\text{ V}}{4\,\Omega} = 2\text{ A}$$

3. **Corriente $i_1$ a través de $\varepsilon_1$:**  
   Aplicando la LCK en el nodo superior sobre la batería $\varepsilon_1$:
   $$i_1 = i_{\text{izq}} + i_2 = 2\text{ A} + 2\text{ A} = 4\text{ A}$$

   Dado que el resultado es positivo, la corriente $i_1$ fluye en el sentido asumido en el diagrama: **hacia arriba** (en dirección al nodo superior).

$$\boxed{i_1 = 4\text{ A}\quad\text{(hacia arriba)}}$$

---

#### Parte c) Potencia de las baterías 1 y 2

1. **Batería 1 ($\varepsilon_1 = 16\text{ V}$):**  
   Por la batería 1 circula la corriente $i_1 = 4\text{ A}$ dirigida hacia arriba. La corriente sale por el terminal positivo (potencial mayor) y entra por el terminal negativo:
   $$P_1 = i_1 \varepsilon_1 = (4\text{ A})(16\text{ V}) = 64\text{ W}$$
   Dado que la corriente fluye en el sentido de aumento de potencial electroquímico, la **batería 1 entrega energía** al circuito.

$$\boxed{P_1 = 64\text{ W}\quad\text{(entrega energía)}}$$

2. **Batería 2 ($\varepsilon_2 = 8\text{ V}$):**  
   La corriente que atraviesa la batería 2 es la corriente del lazo derecho $i_2 = 2\text{ A}$, la cual recorre el tramo inferior de derecha a izquierda. Esto significa que la corriente **entra por el terminal positivo** y sale por el negativo de la fuente $\varepsilon_2$:
   $$P_2 = i_2 \varepsilon_2 = (2\text{ A})(8\text{ V}) = 16\text{ W}$$
   Al entrar corriente por su polo positivo, la **batería 2 absorbe energía** (se está cargando).

$$\boxed{P_2 = 16\text{ W}\quad\text{(absorbe energía)}}$$

**Verificación:**
- **Balance global de potencia:**  
  - Potencia entregada neta: $P_{\text{neta, fuentes}} = P_1 - P_2 = 64\text{ W} - 16\text{ W} = 48\text{ W}$.
  - Potencia disipada en el sector izquierdo: $P_{\text{izq}} = i_{\text{izq}}^2 R_{\text{eq}} = (2\text{ A})^2 (8\,\Omega) = 32\text{ W}$.
  - Potencia disipada en el sector derecho: $P_{\text{der}} = i_2^2 (R_4 + R_5) = (2\text{ A})^2 (4\,\Omega) = 16\text{ W}$.
  - Total disipado: $32\text{ W} + 16\text{ W} = 48\text{ W}$.  
  El balance de energía es exacto: $P_{\text{entregada}} = P_{\text{absorbida}} + P_{\text{disipada}}$.

---

## Resumen de resultados

| Problema | Inciso | Magnitud / Variable | Valor / Expresión |
| :--- | :--- | :--- | :--- |
| **Problema 1** | a) | Resistencia del tronco de cono $R_c$ | $\dfrac{60}{\pi}\,\Omega \approx 19{,}10\,\Omega$ |
| | b) | Potencia disipada en el tronco $P_c$ | $\approx 0{,}109\text{ W} = 109\text{ mW}$ |
| **Problema 2** | a) | Diferencia de potencial $V_{AB}$ | $0{,}8\text{ V}$ |
| | b) | Potencia total disipada en calor $P_{\text{total}}$ | $7{,}2\text{ W}$ |
| **Problema 3** | a) | Resistencia equivalente izquierda $R_{\text{eq}}$ | $8\,\Omega$ |
| | b) | Corriente $i_1$ | $4\text{ A}$ (hacia arriba) |
| | c) | Potencia batería 1 ($P_1$) | $64\text{ W}$ (entrega energía) |
| | c) | Potencia batería 2 ($P_2$) | $16\text{ W}$ (absorbe energía) |
