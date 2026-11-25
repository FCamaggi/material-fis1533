# Ayudantía 15 — Circuitos RC y transitorios

> Clases relacionadas: [Clase 06 - Condensadores](../../Clases/markdown/Clase%2006%20-%20Condensadores.md), [Clase 08 - Corriente electrica y resistencias](../../Clases/markdown/Clase%2008%20-%20Corriente%20electrica%20y%20resistencias.md), [Clase 09 - Potencia, circuitos de resistencias y circuito RC](../../Clases/markdown/Clase%2009%20-%20Potencia%2C%20circuitos%20de%20resistencias%20y%20circuito%20RC.md)

---

## Problema 1

Considere un condensador de capacitancia $C$ inicialmente descargado, el cual se comienza a cargar al conectar (en $t = 0$) el interruptor $S$ del circuito mostrado en la figura.

a) Obtenga la ecuación diferencial para el voltaje $V_C(t)$ entre los terminales del condensador.  
b) Obtenga la solución de la ecuación diferencial obtenida en a), incorporando la condición inicial correspondiente.  
c) Para $t \to \infty$ el condensador estará completamente cargado y el voltaje $V_C$ alcanzará su valor máximo. Usando el resultado de b) obtenga este valor máximo.

Note que $\varepsilon$, $C$, $R_1$ y $R_2$ son datos del problema.

> **[Figura]:** Circuito de dos mallas formado por una fuente de voltaje ideal de fem $\varepsilon$ en la rama vertical izquierda (borne positivo hacia arriba, borne negativo hacia abajo). El riel superior contiene un interruptor $S$ en serie con la fuente y, a continuación, un resistor de resistencia $R_2$. Posteriormente, el circuito se ramifica en dos ramas verticales en paralelo: una rama central que contiene una resistencia $R_1$ y una rama extrema derecha que contiene un condensador de capacitancia $C$. El riel horizontal inferior conecta los terminales inferiores de $R_1$, $C$ y el borne negativo de la fuente $\varepsilon$.

### Solución

**Idea:** Tras cerrar el interruptor en $t = 0$, el circuito opera como una red transitoria de primer orden. Podemos modelar la dinámica aplicando la Ley de Voltajes de Kirchhoff (LVK) mediante el método de corrientes de malla o, de forma equivalente, determinando el equivalente de Thévenin visto desde los terminales del condensador. La corriente por la rama capacitiva obedece a la relación constitutiva $i_C(t) = C \frac{dV_C}{dt}$. Al reemplazarla en la ecuación de mallas se obtiene una ecuación diferencial ordinaria (EDO) lineal de primer orden para $V_C(t)$, que se resuelve por separación de variables sujeta a la condición de reposo $V_C(0) = 0$.

#### Parte a) Ecuación diferencial para el voltaje $V_C(t)$

1. **Definición de corrientes de malla:**  
   Definimos dos corrientes de malla ficticias ambas en sentido horario:
   - $i_1(t)$ para la malla 1 (izquierda), compuesta por la fuente $\varepsilon$, el resistor $R_2$ y el resistor compartido $R_1$.
   - $i_2(t)$ para la malla 2 (derecha), compuesta por el resistor $R_1$ y el condensador $C$.

2. **Ecuaciones de Kirchhoff de voltaje (LVK):**  
   - Para la malla 1, recorriendo en sentido horario:
     $$-\varepsilon + i_1 R_2 + (i_1 - i_2) R_1 = 0$$
     $$i_1(R_1 + R_2) - i_2 R_1 = \varepsilon \implies i_1 = \frac{\varepsilon + i_2 R_1}{R_1 + R_2}$$

   - Para la malla 2, recorriendo en sentido horario:
     $$(i_2 - i_1) R_1 + V_C = 0$$

3. **Eliminación de $i_1$ y obtención de la EDO:**  
   Sustituimos la expresión de $i_1$ en la ecuación de la malla 2:
   $$i_2 R_1 - \left(\frac{\varepsilon + i_2 R_1}{R_1 + R_2}\right) R_1 + V_C = 0$$

   Agrupando los términos que multiplican a $i_2$:
   $$i_2 \left(R_1 - \frac{R_1^2}{R_1 + R_2}\right) - \frac{\varepsilon R_1}{R_1 + R_2} + V_C = 0$$

   Operando el paréntesis:
   $$R_1 - \frac{R_1^2}{R_1 + R_2} = \frac{R_1(R_1 + R_2) - R_1^2}{R_1 + R_2} = \frac{R_1 R_2}{R_1 + R_2}$$

   Obtenemos:
   $$i_2 \left(\frac{R_1 R_2}{R_1 + R_2}\right) + V_C = \varepsilon \frac{R_1}{R_1 + R_2}$$

   > **Nota:** En el manuscrito original se transcribe en un paso intermedio un error tipográfico de signos al escribir $i_2 \left(\frac{R_1 R_2}{R_1 + R_2}\right) - \frac{\varepsilon R_1}{R_1 + R_2} - V_C = 0$, pero en el paso inmediatamente posterior el autor restablece correctamente $+V_C$. El desarrollo riguroso presentado aquí preserva los signos de manera exacta.

   Puesto que la corriente por la rama derecha es exclusivamente $i_2(t)$, la relación constitutiva del condensador es:
   $$i_2 = C \frac{dV_C}{dt}$$

   Sustituyendo $i_2$ en la expresión anterior, llegamos a la ecuación diferencial buscada:
   $$\left(\frac{R_1 R_2}{R_1 + R_2} C\right) \frac{dV_C}{dt} + V_C = \varepsilon \frac{R_1}{R_1 + R_2}$$

$$\boxed{\left(\frac{R_1 R_2}{R_1 + R_2} C\right) \frac{dV_C}{dt} + V_C = \varepsilon \frac{R_1}{R_1 + R_2}}$$

---

#### Parte b) Solución de la ecuación diferencial con condición inicial

1. **Separación de variables:**  
   Reescribimos la ecuación diferencial en la forma estándar:
   $$\frac{dV_C}{dt} = \frac{\varepsilon \frac{R_1}{R_1 + R_2} - V_C}{\left(\frac{R_1 R_2}{R_1 + R_2} C\right)}$$
   $$\frac{dV_C}{\varepsilon \frac{R_1}{R_1 + R_2} - V_C} = \frac{dt}{\left(\frac{R_1 R_2}{R_1 + R_2} C\right)}$$

2. **Integración con condición inicial $V_C(0) = 0$:**  
   Como el condensador se encuentra inicialmente descargado, en $t = 0$ se tiene $V_C(0) = 0$. Integrando entre el reposo inicial y un instante genérico $t$:
   $$\int_0^{V_C(t)} \frac{dv}{\varepsilon \frac{R_1}{R_1 + R_2} - v} = \int_0^t \frac{d\tau}{\left(\frac{R_1 R_2}{R_1 + R_2} C\right)}$$

   Efectuando las integrales:
   $$\left[ -\ln\left(\varepsilon \frac{R_1}{R_1 + R_2} - v\right) \right]_0^{V_C(t)} = \frac{t}{\left(\frac{R_1 R_2}{R_1 + R_2} C\right)}$$
   $$\ln\left(\frac{\varepsilon \frac{R_1}{R_1 + R_2} - V_C(t)}{\varepsilon \frac{R_1}{R_1 + R_2}}\right) = -\frac{t}{\left(\frac{R_1 R_2}{R_1 + R_2} C\right)}$$

3. **Despeje de $V_C(t)$:**  
   Aplicando la función exponencial en ambos miembros:
   $$\frac{\varepsilon \frac{R_1}{R_1 + R_2} - V_C(t)}{\varepsilon \frac{R_1}{R_1 + R_2}} = \exp\left(-\frac{t}{\left(\frac{R_1 R_2}{R_1 + R_2} C\right)}\right)$$
   $$V_C(t) = \varepsilon \frac{R_1}{R_1 + R_2} \left[1 - \exp\left(-\frac{t}{\left(\frac{R_1 R_2}{R_1 + R_2} C\right)}\right)\right]$$

$$\boxed{V_C(t) = \varepsilon \frac{R_1}{R_1 + R_2} \left[ 1 - e^{-\frac{t}{\left(\frac{R_1 R_2}{R_1 + R_2} C\right)}} \right]}$$

---

#### Parte c) Valor máximo de $V_C$ para $t \to \infty$

Cuando $t \to \infty$, el condensador alcanza su estado estacionario y queda completamente cargado (actuando como un circuito abierto, $i_2(\infty) = 0$):
$$V_{C,\text{máx}} = \lim_{t \to \infty} V_C(t) = \lim_{t \to \infty} \left\{ \varepsilon \frac{R_1}{R_1 + R_2} \left[ 1 - e^{-\frac{t}{\tau}} \right] \right\} = \varepsilon \frac{R_1}{R_1 + R_2} [1 - 0]$$

$$\boxed{V_{C,\text{máx}} = \varepsilon \frac{R_1}{R_1 + R_2}}$$

**Verificación:**
- **Equivalente de Thévenin:** Visto desde los bornes del condensador (retirando $C$), el voltaje a circuito abierto es el divisor de tensión formado por $\varepsilon$, $R_2$ y $R_1$: $V_{\text{Th}} = \varepsilon \frac{R_1}{R_1 + R_2}$. Apagando la fuente de voltaje independiente (cortocircuito), la resistencia equivalente vista por el condensador es el paralelo entre $R_1$ y $R_2$: $R_{\text{Th}} = \frac{R_1 R_2}{R_1 + R_2}$. Por ende, el circuito se reduce a un circuito RC serie clásico con constante de tiempo $\tau = R_{\text{Th}} C$ y voltaje asintótico $V_{\text{Th}}$, lo que valida idénticamente la EDO y la solución obtenida.

---

## Problema 2

Considere un circuito compuesto por una pila eléctrica de fuerza electromotriz (FEM) $\mathcal{E}$ y tres elementos, denominados ①, ② y ③, tal como se muestra en la figura.  
Los elementos ① y ② consisten en bloques de material homogéneo con conductividad eléctrica $\sigma_1$ (elemento ①) y $\sigma_2$ (elemento ②). Ambos bloques tienen la misma área transversal $A$ y el mismo espesor $h$.  
El elemento ③ está formado por dos placas conductoras ideales y paralelas, separadas una distancia $h$. El espacio entre las placas está completamente ocupado por un material de permitividad eléctrica $\epsilon > \epsilon_0$, donde $\epsilon_0$ es la permitividad del vacío. El área de cada placa es $A$.

a) Determine las resistencias $R_1$ y $R_2$ de los elementos ① y ②, respectivamente.  
b) Determine la capacitancia $C_3$ del elemento ③.  
c) De acá en adelante suponga conocidos los valores de $R_1$, $R_2$ y $C_3$. Dibuje el circuito usando los símbolos eléctricos. En el circuito identifique un nodo del sistema y defina las corrientes que entran y salen de este.  
d) Escriba las ecuaciones de Kirchhoff del circuito equivalente.  
e) Suponga además que $C_3$ se encuentra inicialmente descargado. Si en el instante $t = 0$ se cierra el interruptor, determine la evolución temporal de la carga en $C_3$.

> **[Figura]:** Dispositivo físico tridimensional compuesto por:
> - Una fuente de fem continua $\mathcal{E}$ (pila vertical) con borne positivo superior y borne negativo inferior.
> - Un interruptor que se cierra en $t = 0$, ubicado en el conductor conectado al borne positivo.
> - **Elemento ①:** Bloque paralelepípedo homogéneo de base rectangular de área horizontal $A$, espesor vertical $h$ y conductividad $\sigma_1$. La corriente entra por su cara conductora superior y sale por su cara conductora inferior en la dirección del eje vertical descendente $z$.
> - **Nivel inferior:** Al salir del elemento ①, el cable conductor conecta con un nodo que se divide en dos ramas en paralelo:
>   - **Elemento ②:** Bloque paralelepípedo de igual geometría (área horizontal $A$, espesor vertical $h$) y conductividad $\sigma_2$.
>   - **Elemento ③:** Condensador de placas planas y paralelas horizontales de área $A$, separadas una distancia vertical $h$, con dieléctrico lineal de permitividad $\epsilon$ entre ellas.
> - Un riel conductor horizontal inferior común conecta la cara inferior de ② y la placa inferior de ③ de regreso al borne negativo de la pila $\mathcal{E}$.

### Solución

**Idea:** La corriente fluye perpendicularmente a través de las caras planas de área $A$ a lo largo del espesor $h$, de modo que los elementos conductores se comportan como resistencias óhmicas volumétricas $R = \frac{h}{\sigma A}$. El elemento ③ es un condensador plano con dieléctrico de capacitancia $C = \frac{\epsilon A}{h}$. La topología circuital sitúa al elemento ① en serie con la combinación en paralelo de ② y ③. Planteando las leyes de Kirchhoff en el circuito equivalente, se obtiene la ecuación diferencial transitoria que gobierna la carga $q(t)$ del condensador.

#### Parte a) Resistencias $R_1$ y $R_2$ de los bloques ① y ②

La resistencia de un conductor cilíndrico o prismático de sección transversal constante $A$, longitud $h$ y conductividad uniforme $\sigma$ recorrida por una densidad de corriente uniforme viene dada por:
$$R = \int_{\Gamma} \frac{d\ell}{\sigma A(\ell)}$$

Como la trayectoria de la corriente es puramente rectilínea a lo largo del espesor vertical ($d\ell = dz$ desde $z = 0$ hasta $z = h$), con $A(z) = A = \text{cte}$ y conductividad $\sigma_k$:
$$R_k = \frac{1}{\sigma_k A} \int_0^h dz = \frac{h}{\sigma_k A} \quad (k = 1, 2)$$

Por lo tanto:
$$\boxed{R_1 = \frac{h}{\sigma_1 A}}$$
$$\boxed{R_2 = \frac{h}{\sigma_2 A}}$$

---

#### Parte b) Capacitancia $C_3$ del elemento ③

Para un condensador de placas plano-paralelas de área $A$, separación entre armaduras $h$ y completamente lleno con un material homogéneo e isótropo de permitividad $\epsilon$:
$$C = \frac{\epsilon A}{d}$$

Con $d = h$:
$$\boxed{C_3 = \frac{\epsilon A}{h}}$$

---

#### Parte c) Circuito equivalente esquemático, nodos y corrientes

El circuito equivalente está constituido por:
- La fuente de fem $\mathcal{E}$ en la rama izquierda (+ arriba, - abajo).
- El interruptor en serie sobre el riel superior que se cierra en $t = 0$.
- La resistencia $R_1$ sobre el riel superior.
- Un nodo principal intermedio a potencial $v_C(t)$ con respecto a la tierra de referencia (riel inferior).
- Dos ramas en paralelo que bajan hacia el riel inferior:
  - Una rama central resistiva con la resistencia $R_2$.
  - Una rama derecha capacitiva con el condensador $C_3$.

Definimos las corrientes:
- $i_1(t)$: corriente que fluye por la rama principal (resistencia $R_1$) e ingresa al nodo intermedio.
- $i_2(t)$: corriente que sale del nodo intermedio hacia abajo a través de la resistencia $R_2$.
- $i_C(t)$: corriente que sale del nodo intermedio hacia la derecha a través del condensador $C_3$.

Por la Ley de Corrientes de Kirchhoff en el nodo intermedio:
$$i_1(t) = i_2(t) + i_C(t)$$

---

#### Parte d) Ecuaciones de Kirchhoff del circuito equivalente

1. **Ecuación de nodo (LCK):**  
   $$i_1 = i_2 + i_C$$
   donde la corriente que carga el condensador es la tasa de variación temporal de su carga:
   $$i_C = \frac{dq}{dt}$$

2. **Ecuación de la malla principal (LVK, fuente y $R_1$, $R_2$):**  
   Recorriendo la malla izquierda en sentido horario:
   $$\mathcal{E} - i_1 R_1 - i_2 R_2 = 0$$

3. **Ecuación de la malla secundaria (LVK, paralelo entre $R_2$ y $C_3$):**  
   El voltaje entre los terminales de $R_2$ es idéntico al voltaje entre las placas del condensador $C_3$:
   $$v_C = i_2 R_2 = \frac{q}{C_3} \implies -\frac{q}{C_3} + i_2 R_2 = 0$$

$$\boxed{\begin{aligned} i_1 &= i_2 + i_C \\ \mathcal{E} - i_1 R_1 - i_2 R_2 &= 0 \\ -\frac{q}{C_3} + i_2 R_2 &= 0 \end{aligned}}$$

---

#### Parte e) Evolución temporal de la carga en $C_3$

1. **Despeje de $i_2$ en función de $i_C$:**  
   Sustituyendo $i_1 = i_2 + i_C$ en la ecuación de la malla principal:
   $$\mathcal{E} - (i_2 + i_C) R_1 - i_2 R_2 = 0$$
   $$\mathcal{E} - i_C R_1 - i_2(R_1 + R_2) = 0 \implies i_2 = \frac{\mathcal{E} - i_C R_1}{R_1 + R_2}$$

2. **Formulación de la ecuación diferencial:**  
   Sustituimos $i_2$ en la ecuación del lazo secundario $-\frac{q}{C_3} + i_2 R_2 = 0$:
   $$-\frac{q}{C_3} + \left(\frac{\mathcal{E} - i_C R_1}{R_1 + R_2}\right) R_2 = 0$$

   Multiplicando por $C_3$:
   $$-q + \left(\frac{R_2}{R_1 + R_2}\right) \mathcal{E} C_3 - \left(\frac{R_1 R_2}{R_1 + R_2} C_3\right) i_C = 0$$

   Definimos el voltaje asintótico del condensador ($t \to \infty$) y el tiempo característico de relajación $\tau$:
   $$v_C(\infty) = \frac{R_2}{R_1 + R_2} \mathcal{E}$$
   $$\tau = \left(\frac{R_1 R_2}{R_1 + R_2}\right) C_3$$

   Sustituyendo $i_C = \frac{dq}{dt}$:
   $$-q + v_C(\infty) C_3 - \tau \frac{dq}{dt} = 0 \implies \tau \frac{dq}{dt} = v_C(\infty) C_3 - q$$

3. **Integración con $q(0) = 0$:**  
   Separando variables:
   $$\frac{dq}{q - v_C(\infty) C_3} = -\frac{dt}{\tau}$$

   Integrando desde $t = 0$ (donde $q = 0$) hasta un tiempo arbitrario $t$:
   $$\int_0^{q(t)} \frac{dq'}{q' - v_C(\infty) C_3} = -\int_0^t \frac{dt'}{\tau}$$
   $$\ln\left(\frac{q(t) - v_C(\infty) C_3}{-v_C(\infty) C_3}\right) = -\frac{t}{\tau}$$
   $$\frac{q(t) - v_C(\infty) C_3}{-v_C(\infty) C_3} = e^{-t/\tau} \implies q(t) = v_C(\infty) C_3 \left(1 - e^{-t/\tau}\right)$$

   Reemplazando la expresión explícita de $v_C(\infty)$:
   $$q(t) = \left(\frac{R_2}{R_1 + R_2}\right) \mathcal{E} C_3 \left(1 - e^{-t/\tau}\right)$$
   con $\tau = \left(\frac{R_1 R_2}{R_1 + R_2}\right) C_3$.

$$\boxed{q(t) = \frac{R_2}{R_1 + R_2} \mathcal{E} C_3 \left(1 - e^{-\frac{t}{\tau}}\right), \qquad \text{con } \tau = \frac{R_1 R_2}{R_1 + R_2} C_3}$$

**Verificación:**
- En $t = 0$, $q(0) = 0$, consistente con el condensador inicialmente descargado.
- En $t \to \infty$, $q(\infty) = C_3 v_C(\infty) = C_3 \mathcal{E} \frac{R_2}{R_1 + R_2}$, que coincide con la carga adquirida cuando por la rama del condensador deja de fluir corriente y la tensión sobre este es la dada por el divisor resistivo formado por $R_1$ y $R_2$.

---

## Problema 3

El circuito de la figura se usa para medir la rapidez de la flecha. En la práctica $V_f = 24\text{ V}$, $C = 20\text{ pF}$, $R_1 = 2\text{ M}\Omega$, $R_2 = 3\text{ M}\Omega$, y $d = 69\text{ cm}$. En todos los cálculos numéricos mantenga 3 cifras significativas.

a) Cuando se cierra el interruptor $S$ el condensador está totalmente descargado y la flecha se encuentra a la izquierda del circuito. Explique lo que sucede con el condensador. ¿Cuánto tiempo debe transcurrir para que el condensador quede a $0{,}1\,\%$ de su carga máxima? Entregue primero una fórmula algebraica para el tiempo, y luego evalúe con los valores indicados antes. Considere la aproximación $\ln 1000 \approx 6{,}9$.  
b) En el instante $t = 0$ la flecha corta el circuito en la sección AC (asuma que el condensador tiene en ese momento su carga máxima). Explique lo que sucede con el condensador. Calcule su voltaje en función del tiempo.  
c) En un instante posterior $t > 0$ la flecha corta la sección BD. Explique lo que sucede con el condensador. Si el voltaje final del condensador es $V_C^{\text{fin}}$ (voltaje en el momento del corte) encuentre la rapidez de la flecha. Entregue primero una fórmula algebraica para la rapidez, y luego evalúe con los valores indicados antes. Suponga que $V_C^{\text{fin}} = V_C^{\text{max}}/2$ (donde $V_C^{\text{max}}$ es el voltaje máximo del condensador), y use que $\ln 2 \approx 0{,}69$.

> **[Figura]:** Dispositivo experimental para cronometrar la rapidez de un proyectil (flecha):
> - **Lazo de carga:** Fuente continua de voltaje $V_f = 24\text{ V}$ con interruptor $S$ en su terminal positivo.
> - **Secciones vulnerables:** La flecha se desplaza en vuelo horizontal hacia la derecha a lo largo de una línea recta que cruza dos tramos conductores verticales:
>   - Tramo vertical $AC$ situado a la salida del borne negativo de la fuente de alimentación.
>   - Tramo vertical $BD$ situado a una distancia horizontal $d = 69\text{ cm}$ a la derecha del tramo $AC$.
> - **Resistores y condensador:** Conectada entre el riel superior y el nodo $D$ se encuentra la resistencia vertical $R_2 = 3\text{ M}\Omega$. Más a la derecha, en el riel superior, se ubica la resistencia $R_1 = 2\text{ M}\Omega$, cerrando el lazo derecho con el condensador vertical $C = 20\text{ pF}$.
> - Al volar la flecha, primero secciona mecánicamente el tramo $AC$, aislando la fuente del resto del circuito. Luego de recorrer la distancia $d$, secciona el tramo $BD$, desconectando la resistencia $R_2$ y congelando el proceso de descarga.

### Solución

**Idea:** El problema se descompone cronológicamente en tres regímenes circuitales bien diferenciados:
1. **Fase de carga:** Con la fuente conectada, el condensador se carga a través de la resistencia $R_1$. Al ser la fuente ideal, la presencia de $R_2$ en paralelo no afecta la tensión aplicada a la rama de carga $R_1\text{-}C$.
2. **Fase de descarga (vuelo entre $AC$ y $BD$):** Al cortar la flecha el tramo $AC$, la fuente queda desconectada; el condensador se descarga a través de las resistencias $R_1$ y $R_2$ conectadas ahora en serie.
3. **Fase de retención de carga (corte en $BD$):** Al seccionar el tramo $BD$, el circuito de descarga se abre definitivamente; la corriente cesa instantáneamente y la carga remanente queda atrapada en el condensador. Midiendo el voltaje final residual $V_C^{\text{fin}}$, se deduce el tiempo de vuelo y la rapidez de la flecha $v = d / t_v$.

#### Parte a) Carga del condensador y tiempo para alcanzar el $99{,}9\,\%$ de la carga máxima

1. **Circuito equivalente de carga:**  
   Al cerrar el interruptor $S$, la fuente $V_f$ entrega corriente al condensador a través de la resistencia $R_1$. La resistencia $R_2$ está en paralelo con la fuente ideal $V_f$, por lo que solo consume corriente adicional de la fuente sin modificar el voltaje entregado a la rama $R_1\text{-}C$.  
   Por la Ley de Voltajes de Kirchhoff en el lazo de carga:
   $$V_{R_1} + V_C = V_f$$

   Dado que por la rama circula una única corriente $I$:
   $$V_{R_1} = R_1 I$$
   $$Q_C = C V_C \implies I = C \frac{dV_C}{dt}$$

   Sustituyendo:
   $$R_1 C \frac{dV_C}{dt} + V_C = V_f$$

2. **Solución transitoria de carga:**  
   Con la condición inicial $V_C(0) = 0$:
   $$V_C(t) = V_f \left(1 - e^{-t / (R_1 C)}\right)$$

3. **Tiempo para quedar a $0{,}1\,\%$ de su carga máxima:**  
   El voltaje máximo asintótico es $V_{C,\text{máx}} = V_f$. El condensador se encuentra a un $0{,}1\,\%$ de su carga máxima cuando ha adquirido el $99{,}9\,\%$ de dicha carga, es decir, cuando la diferencia faltante es $10^{-3}$:
   $$1 - e^{-T / (R_1 C)} = 0{,}999 \implies e^{-T / (R_1 C)} = 0{,}001 = \frac{1}{1000}$$
   $$\frac{T}{R_1 C} = \ln 1000 \implies T = R_1 C \ln 1000$$

4. **Evaluación numérica:**  
   Con $R_1 = 2\text{ M}\Omega = 2 \times 10^6\,\Omega$, $C = 20\text{ pF} = 20 \times 10^{-12}\text{ F}$ y $\ln 1000 \approx 6{,}9$:
   $$T \approx (2 \times 10^6\,\Omega)(20 \times 10^{-12}\text{ F})(6{,}9) = (40 \times 10^{-6}\text{ s})(6{,}9) = 2{,}76 \times 10^{-4}\text{ s}$$

$$\boxed{T = R_1 C \ln 1000 \approx 2{,}76 \times 10^{-4}\text{ s}}$$

*(Este tiempo es de tan solo $0{,}276\text{ ms}$, lo que garantiza experimentalmente que antes de la llegada del proyectil el condensador se encuentra efectivamente cargado al máximo).*

---

#### Parte b) Desconexión en la sección AC y descarga del condensador

1. **Circuito de descarga:**  
   En $t = 0$, la flecha secciona el conductor $AC$. La fuente $V_f$ queda totalmente desconectada del sistema. El lazo cerrado remanente está compuesto por el condensador $C$ cargado a un voltaje inicial $V_C(0) = V_f$, en serie con las resistencias $R_1$ y $R_2$.  
   Por la Ley de Voltajes de Kirchhoff en el lazo cerrado de descarga:
   $$V_{R_1} + V_{R_2} + V_C = 0$$

   Con una corriente de descarga $I'$:
   $$V_{R_1} = R_1 I', \qquad V_{R_2} = R_2 I', \qquad I' = C \frac{dV_C}{dt}$$

2. **Ecuación diferencial y voltaje en el tiempo:**  
   $$(R_1 + R_2) C \frac{dV_C}{dt} + V_C = 0$$

   La solución para la descarga con voltaje inicial $V_C(0) = V_f$ es:
   $$V_C(t) = V_f \exp\left(-\frac{t}{(R_1 + R_2)C}\right)$$

$$\boxed{V_C(t) = V_f e^{-\frac{t}{(R_1 + R_2)C}}}$$

---

#### Parte c) Corte en la sección BD y cálculo de la rapidez de la flecha

1. **Interrupción de la descarga:**  
   Al cortar la flecha la sección $BD$, la rama que contiene la resistencia $R_2$ se abre. El circuito queda abierto y la descarga cesa instantáneamente; el condensador retiene congelado el voltaje residual $V_C^{\text{fin}}$ que poseía en ese preciso instante.

2. **Tiempo de vuelo $t_v$ de la flecha:**  
   Sea $t_v$ el intervalo de tiempo transcurrido entre el corte de $AC$ y el corte de $BD$:
   $$V_C(t_v) = V_C^{\text{fin}} = V_f e^{-\frac{t_v}{(R_1 + R_2)C}}$$
   $$e^{\frac{t_v}{(R_1 + R_2)C}} = \frac{V_f}{V_C^{\text{fin}}} \implies t_v = (R_1 + R_2)C \ln\left(\frac{V_f}{V_C^{\text{fin}}}\right)$$

   Como el enunciado especifica que $V_C^{\text{fin}} = \frac{V_{C,\text{máx}}}{2} = \frac{V_f}{2}$:
   $$\frac{V_f}{V_C^{\text{fin}}} = 2 \implies t_v = (R_1 + R_2)C \ln 2$$

3. **Rapidez de la flecha:**  
   La flecha recorre la distancia $d$ a rapidez constante $v_{\text{flecha}}$ durante el tiempo de vuelo $t_v$:
   $$v_{\text{flecha}} = \frac{d}{t_v} = \frac{d}{(R_1 + R_2) C \ln\left(\frac{V_f}{V_C^{\text{fin}}}\right)} = \frac{d}{(R_1 + R_2) C \ln 2}$$

4. **Evaluación numérica:**  
   Datos:
   - $d = 69\text{ cm} = 0{,}69\text{ m}$
   - $R_1 + R_2 = 2\text{ M}\Omega + 3\text{ M}\Omega = 5\text{ M}\Omega = 5 \times 10^6\,\Omega$
   - $C = 20\text{ pF} = 20 \times 10^{-12}\text{ F}$
   - $\ln 2 \approx 0{,}69$

   Sustituyendo:
   $$(R_1 + R_2) C = (5 \times 10^6\,\Omega)(20 \times 10^{-12}\text{ F}) = 100 \times 10^{-6}\text{ s} = 10^{-4}\text{ s}$$
   $$v_{\text{flecha}} = \frac{0{,}69\text{ m}}{(10^{-4}\text{ s})(0{,}69)} = \frac{1}{10^{-4}}\text{ m/s} = 10^4\text{ m/s}$$

$$\boxed{v_{\text{flecha}} = \frac{d}{(R_1 + R_2) C \ln 2} \approx 10^4\text{ m/s} = 10\text{ km/s}}$$

**Verificación:**
- **Unidades:** $[d / (R C)] = [\text{m} / (\Omega \cdot \text{F})] = [\text{m} / \text{s}]$, dimensionalmente correcto.
- **Sentido físico:** Si la flecha viajara infinitamente rápido ($t_v \to 0$), el condensador no alcanzaría a descargarse y $V_C^{\text{fin}} \to V_f$. Si viajara infinitamente lento ($t_v \to \infty$), el condensador se descargaría totalmente ($V_C^{\text{fin}} \to 0$).

---

## Resumen de resultados

| Problema | Inciso | Magnitud / Variable | Expresión / Valor numérico |
| :--- | :--- | :--- | :--- |
| **Problema 1** | a) | Ecuación diferencial para $V_C(t)$ | $\left(\dfrac{R_1 R_2}{R_1 + R_2} C\right) \dfrac{dV_C}{dt} + V_C = \varepsilon \dfrac{R_1}{R_1 + R_2}$ |
| | b) | Voltaje en el tiempo $V_C(t)$ | $\varepsilon \dfrac{R_1}{R_1 + R_2} \left[ 1 - e^{-t / \left(\frac{R_1 R_2}{R_1 + R_2} C\right)} \right]$ |
| | c) | Voltaje máximo $V_{C,\text{máx}}$ | $\varepsilon \dfrac{R_1}{R_1 + R_2}$ |
| **Problema 2** | a) | Resistencias $R_1$ y $R_2$ | $R_1 = \dfrac{h}{\sigma_1 A}, \quad R_2 = \dfrac{h}{\sigma_2 A}$ |
| | b) | Capacitancia $C_3$ | $C_3 = \dfrac{\epsilon A}{h}$ |
| | c) | Ecuación de nodo | $i_1(t) = i_2(t) + i_C(t)$ |
| | d) | Ecuaciones de mallas (Kirchhoff) | $\mathcal{E} - i_1 R_1 - i_2 R_2 = 0, \quad -\dfrac{q}{C_3} + i_2 R_2 = 0$ |
| | e) | Evolución de carga $q(t)$ | $\dfrac{R_2}{R_1 + R_2}\mathcal{E} C_3 \left(1 - e^{-t/\tau}\right), \quad \tau = \left(\dfrac{R_1 R_2}{R_1 + R_2}\right) C_3$ |
| **Problema 3** | a) | Tiempo para $99{,}9\,\%$ de carga | $T = R_1 C \ln 1000 \approx 2{,}76 \times 10^{-4}\text{ s}$ |
| | b) | Voltaje de descarga $V_C(t)$ | $V_C(t) = V_f e^{-t / ((R_1 + R_2)C)}$ |
| | c) | Rapidez de la flecha $v_{\text{flecha}}$ | $v_{\text{flecha}} = \dfrac{d}{(R_1 + R_2)C \ln 2} \approx 10^4\text{ m/s}$ |
