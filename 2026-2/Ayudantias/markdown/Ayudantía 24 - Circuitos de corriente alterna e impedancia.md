# Ayudantía 24 — Circuitos de corriente alterna e impedancia

> Clases relacionadas: [Clase 14 - Inductancia](../../Clases/markdown/Clase%2014%20-%20Inductancia.md)

---

## Problema 1

Un circuito contiene dos resistencias $R$, dos inductancias $L$ y una capacitancia $C$. Estos elementos están conectados a una fuente de voltaje alterna $V(t) = V_0 \cos(\omega t)$ como se observa en la figura. Se pide:

a) La impedancia vista desde la fuente de voltaje.  
b) El fasor de corriente del circuito y el fasor de voltaje $\hat{V}_L$.  
c) Determine la frecuencia $\omega_0$ que debe tener la fuente de voltaje, de modo que la amplitud de la corriente que sale de la fuente sea máxima. Además calcule cuál será dicha amplitud máxima.

> **[Figura]:** Circuito de malla única en serie. En la rama vertical izquierda se ubica la fuente de voltaje alterno $V(t) = V_0 \cos(\omega t)$. La rama horizontal superior contiene una resistencia $R$ en serie con un condensador $C$. La rama vertical derecha contiene un inductor $L$, con terminales de prueba y una flecha azul etiquetada como $V_L$ orientada hacia arriba (del nodo inferior al superior). La rama horizontal inferior contiene un inductor $L$ en serie con una segunda resistencia $R$, cerrando la malla hacia el terminal inferior de la fuente.

### Solución

**Idea:** Todos los elementos del circuito están conectados en serie en una única malla cerrada. Representando las impedancias complejas de cada elemento mediante la unidad imaginaria $j$ ($j^2 = -1$, con $Z_R = R$, $Z_L = j\omega L$ y $Z_C = \frac{1}{j\omega C}$), la impedancia equivalente $Z_{\text{eq}}$ es la suma directa de las impedancias en serie. A partir de $Z_{\text{eq}}$ se obtienen el fasor de corriente $\hat{I}$ y el fasor de voltaje $\hat{V}_L$, y la amplitud máxima de corriente se alcanza en la condición de resonancia serie donde la reactancia inductiva total iguala a la reactancia capacitiva.

#### Parte a) Impedancia vista desde la fuente de voltaje

La impedancia equivalente en serie será la suma de las impedancias de cada elemento a lo largo de la malla:
$$Z_{\text{eq}} = R + \frac{1}{j\omega C} + j\omega L + R + j\omega L$$

Simplificando y agrupando términos resistivos e inductivos:
$$\boxed{Z_{\text{eq}} = 2R + 2j\omega L + \frac{1}{j\omega C}}$$

*(Equivalentemente, usando $\frac{1}{j} = -j$, se escribe $Z_{\text{eq}} = 2R + j\left(2\omega L - \frac{1}{\omega C}\right)$).*

---

#### Parte b) Fasor de corriente $\hat{I}$ y fasor de voltaje $\hat{V}_L$

1. **Fasor de corriente del circuito $\hat{I}$:**  
   Tomando el voltaje de la fuente como referencia ($\hat{V} = V_0$), el fasor de corriente será el fasor de voltaje dividido por la impedancia equivalente:
   $$\hat{I} = \frac{\hat{V}}{Z_{\text{eq}}} = \frac{V_0}{2R + 2j\omega L + \frac{1}{j\omega C}}$$

   Para simplificar, llevamos la impedancia a notación polar definiendo las reactancias totales $X_L = 2\omega L$ y $X_C = \frac{1}{\omega C}$:
   $$Z_{\text{eq}} = 2R + j(X_L - X_C) = \sqrt{4R^2 + (X_L - X_C)^2}\, e^{j\phi}$$
   con ángulo de fase:
   $$\phi = \arctan\left(\frac{X_L - X_C}{2R}\right), \qquad X_L = 2\omega L, \qquad X_C = \frac{1}{\omega C}$$

   Con esto, el fasor de corriente se puede escribir como:
   $$\boxed{\hat{I} = \frac{V_0}{\sqrt{4R^2 + (X_L - X_C)^2}}\, e^{-j\phi}}$$

2. **Fasor de voltaje $\hat{V}_L$:**  
   Usando $\hat{V}_L = Z_L \hat{I}$ con $Z_L = j\omega L = \omega L\, e^{j\pi/2}$, se encuentra que:
   $$\boxed{\hat{V}_L = j\omega L \hat{I} = \frac{V_0 \omega L}{\sqrt{4R^2 + (X_L - X_C)^2}}\, e^{j\left(-\phi + \frac{\pi}{2}\right)}}$$

---

#### Parte c) Frecuencia $\omega_0$ y amplitud máxima de corriente

La corriente instantánea en función del tiempo debe ser:
$$i(t) = \text{Re}\left(\hat{I} e^{j\omega t}\right) = \frac{V_0}{\sqrt{4R^2 + (X_L - X_C)^2}} \cos(\omega t - \phi)$$

La amplitud de la corriente será máxima cuando el denominador sea mínimo, lo cual ocurre cuando $X_L = X_C$:
$$2\omega_0 L = \frac{1}{\omega_0 C} \implies \omega_0^2 = \frac{1}{2LC}$$

Es decir, cuando $\omega$ es igual a:
$$\boxed{\omega_0 = \sqrt{\frac{1}{2LC}}}$$

En dicho caso ($X_L - X_C = 0$), la amplitud máxima de la corriente corresponde a:
$$\boxed{I_{\max} = \frac{V_0}{2R}}$$

**Verificación:**
- **Unidades:** $[\omega_0] = 1/\sqrt{\text{H}\cdot\text{F}} = 1/\text{s} = \text{rad/s}$; $[I_{\max}] = \text{V}/\Omega = \text{A}$. Correcto.
- **Fase en resonancia:** En $\omega = \omega_0$, se tiene $X_L = X_C$ y $\phi = 0$, por lo que $i(t) = \frac{V_0}{2R}\cos(\omega_0 t)$ oscila en fase con la fuente y el voltaje en el inductor $\hat{V}_L = j\omega_0 L \frac{V_0}{2R}$ queda adelantado en $\pi/2$.

---

## Problema 2

Dado el circuito RLC en la figura:

1. ¿Cuál es la impedancia entre los terminales de conexión?  
2. Se aplica el voltaje alterno $U(t) = U_0 \cos(\omega t)$ a los terminales de conexión. Calcule la amplitud de oscilación de la corriente alterna $I(t)$ que entra al circuito.  
3. ¿Cuál es la potencia que se disipa en el circuito durante un período de oscilación del voltaje alterno cuando la frecuencia angular del voltaje es $\omega = 1/(LC)$?

> **[Figura]:** Circuito con dos terminales de entrada abiertos a la izquierda. El riel conductor superior se conecta a dos ramas verticales en paralelo que bajan hacia el riel inferior:
> - Rama central: contiene una resistencia $R$.
> - Rama derecha: contiene en serie una resistencia $R$, un inductor $L$ y un condensador $C$.
> Ambas ramas confluyen en el riel inferior que regresa al terminal de conexión inferior.

### Solución

**Idea:** El circuito consta de una rama puramente resistiva de impedancia $R$ en paralelo con una rama serie $RLC$. Expresamos la reactancia del inductor y del condensador en función de la frecuencia característica $\omega_{LC} = 1/\sqrt{LC}$, combinamos ambas ramas en paralelo para hallar la impedancia equivalente $Z$, aplicamos la ley de Ohm en amplitudes complejas $\tilde{U}_0 = Z\tilde{I}_0$ para obtener $I_0$, y evaluamos la potencia promedio disipada en resonancia.

#### Parte 1) Impedancia entre los terminales de conexión

La resistencia $R$, inductancia $L$ y capacitancia $C$ en serie de la rama derecha tienen la impedancia:
$$R + i\omega L + \frac{1}{i\omega C} = R + i\omega L\left[1 - \left(\frac{\omega_{LC}}{\omega}\right)^2\right]$$
donde $\omega_{LC} = 1/\sqrt{LC}$ es la frecuencia angular característica del circuito $LC$.

Con la resistencia $R$ de la rama central en paralelo, la impedancia total resulta como:
$$Z = \left(\frac{1}{R} + \frac{1}{R + i\omega L\left[1 - \left(\frac{\omega_{LC}}{\omega}\right)^2\right]}\right)^{-1}$$

Combinando las fracciones e invirtiendo:
$$Z = \left(\frac{R + i\omega L\left[1 - \left(\frac{\omega_{LC}}{\omega}\right)^2\right] + R}{R\left(R + i\omega L\left[1 - \left(\frac{\omega_{LC}}{\omega}\right)^2\right]\right)}\right)^{-1}$$

$$\boxed{Z = R\,\frac{R + i\omega L\left[1 - \left(\frac{\omega_{LC}}{\omega}\right)^2\right]}{2R + i\omega L\left[1 - \left(\frac{\omega_{LC}}{\omega}\right)^2\right]}}$$

---

#### Parte 2) Amplitud de oscilación de la corriente $I(t)$

Definimos las amplitudes complejas de voltaje $\tilde{U}_0$ y corriente $\tilde{I}_0$ mediante la representación fasorial:
$$U(t) = U_0 \cos(\omega t) = \text{Re}\left(\underbrace{U_0}_{=\tilde{U}_0} e^{i\omega t}\right)$$
$$I(t) = I_0 \cos(\omega t + \varphi) = \text{Re}\left(\underbrace{I_0 e^{i\varphi}}_{=\tilde{I}_0} e^{i\omega t}\right)$$

Por la «ley de Ohm» para amplitudes complejas:
$$\tilde{U}_0 = Z \tilde{I}_0 \implies \tilde{I}_0 = \frac{\tilde{U}_0}{Z}$$

Tomando el módulo para obtener la amplitud real $I_0 = |\tilde{I}_0|$:
$$I_0 = \left|\frac{U_0}{R}\,\frac{2R + i\omega L\left[1 - \left(\frac{\omega_{LC}}{\omega}\right)^2\right]}{R + i\omega L\left[1 - \left(\frac{\omega_{LC}}{\omega}\right)^2\right]}\right|$$

Como el módulo de un cociente es el cociente de los módulos ($|a + ib| = \sqrt{a^2 + b^2}$), por lo tanto la amplitud es:
$$\boxed{I_0 = \frac{U_0}{R}\sqrt{\frac{(2R)^2 + (\omega L)^2\left[1 - \left(\frac{\omega_{LC}}{\omega}\right)^2\right]^2}{R^2 + (\omega L)^2\left[1 - \left(\frac{\omega_{LC}}{\omega}\right)^2\right]^2}}}$$

---

#### Parte 3) Potencia disipada durante un período en resonancia

Suponiendo la definición dimensionalmente correcta de la frecuencia de resonancia $\omega_{LC} = 1/\sqrt{LC}$ (dado que $1/(LC)$ tiene unidades de $\text{s}^{-2}$ y no de $\text{s}^{-1}$):

Para $\omega = \omega_{LC}$, el término $\left[1 - (\omega_{LC}/\omega)^2\right]$ se anula, por lo que $Z = R/2$ es puramente real, la fase es $\varphi = 0$ y la amplitud de corriente resulta:
$$I_0 = \frac{U_0}{R}\sqrt{\frac{4R^2}{R^2}} = \frac{2 U_0}{R}$$

Por consiguiente, la potencia promedio disipada en un período resulta:
$$\boxed{\overline{P} = \frac{U_0 I_0}{2}\cos\varphi = \frac{U_0^2}{R}}$$

**Verificación:**
- **Unidades:** $[Z] = \Omega$; $[I_0] = \text{V}/\Omega = \text{A}$; $[\overline{P}] = \text{V}^2/\Omega = \text{W}$. Correcto.
- **Límites de frecuencia:** Para $\omega \to 0$ o $\omega \to \infty$, la rama $RLC$ se vuelve de impedancia infinita (abierta) y toda la corriente pasa por la resistencia central $R$, dando $Z \to R$ e $I_0 \to U_0/R$. En $\omega = \omega_{LC}$, la rama $LC$ resuena con reactancia nula, quedando dos resistencias $R$ en paralelo ($Z = R/2$, $I_0 = 2U_0/R$), y la energía total disipada durante un período completo $T = 2\pi\sqrt{LC}$ sería $W = \overline{P}T = \frac{2\pi U_0^2 \sqrt{LC}}{R}$.

---

## Problema 3

Considere el circuito eléctrico de la figura, que es alimentado por una fuente de voltaje alterno $V(t) = V_0 \cos \omega t$. Determine:

a) La impedancia equivalente de la configuración, especificando claramente su parte real e imaginaria.  
b) La frecuencia de resonancia $\omega_0$ del circuito, tal que haga máxima la corriente que sale de la fuente.  
c) La corriente que circula por la resistencia $R$ en función del tiempo (ie. escriba la corriente de la forma $I(t) = I_0 \cos(\omega t - \phi)$, especificando claramente los valores de $I_0$ y $\phi$).  
d) La potencia promedio entregada por la fuente.

> **[Figura]:** Fuente de voltaje alterno $V_0$ con polaridad superior positiva ($+$) e inferior negativa ($-$). Desde el terminal superior, la corriente atraviesa en serie una resistencia $R$ y luego llega a un nodo que se divide en dos ramas en paralelo:
> - Rama central: inductor $L$ en serie con un condensador $C_1$.
> - Rama derecha: un condensador $C_2$.
> Ambas ramas se unen en el riel inferior, regresando al polo negativo de la fuente.

### Solución

**Idea:** El circuito consiste en la resistencia $R$ en serie con el arreglo en paralelo de la rama serie $L-C_1$ y la rama capacitiva $C_2$. Usando la unidad imaginaria $j$ ($j^2 = -1$) y las reactancias $X_L = \omega L$, $X_{C_1} = \frac{1}{\omega C_1}$ y $X_{C_2} = \frac{1}{\omega C_2}$, sumamos en paralelo las impedancias puramente reactivas y luego las añadimos en serie con $R$. La resonancia de corriente máxima se produce cuando la parte imaginaria de la impedancia equivalente se anula, minimizando $|Z|$.

#### Parte a) Impedancia equivalente de la configuración

Sean las reactancias de cada elemento $X_L = \omega L$, $X_{C_1} = \frac{1}{\omega C_1}$ y $X_{C_2} = \frac{1}{\omega C_2}$. La rama central tiene impedancia $j X_L - j X_{C_1} = j(X_L - X_{C_1})$ y la rama derecha tiene impedancia $-j X_{C_2}$.

La impedancia equivalente total está dada por:
$$Z = R + \left(\frac{1}{j X_L - j X_{C_1}} + \frac{1}{-j X_{C_2}}\right)^{-1}$$

Sumando las admitancias de las dos ramas en paralelo (usando $j \cdot (-j) = 1$):
$$Z = R + \left(\frac{-j X_{C_2} + j X_L - j X_{C_1}}{(X_L - X_{C_1}) X_{C_2}}\right)^{-1}$$

Invirtiendo la fracción y multiplicando numerador y denominador por $-j$ (recordando $\frac{1}{j} = -j$):
$$Z = R + \frac{(X_L - X_{C_1}) X_{C_2}}{j(X_L - X_{C_1} - X_{C_2})} = R + j\,\frac{(X_L - X_{C_1}) X_{C_2}}{X_{C_2} + X_{C_1} - X_L}$$

Sustituyendo $X_L = \omega L$, $X_{C_1} = \frac{1}{\omega C_1}$ y $X_{C_2} = \frac{1}{\omega C_2}$:
$$Z = R + j\,\frac{\left(\omega L - \frac{1}{\omega C_1}\right)\frac{1}{\omega C_2}}{\frac{1}{\omega C_2} + \frac{1}{\omega C_1} - \omega L} = R + j\,\frac{\frac{\omega^2 L C_1 - 1}{\omega^2 C_1 C_2}}{\frac{C_1 + C_2 - \omega^2 L C_1 C_2}{\omega C_1 C_2}}$$

$$\boxed{Z = R + j\,\frac{\omega^2 L C_1 - 1}{\omega\left(C_1 + C_2 - \omega^2 L C_1 C_2\right)}}$$

Especificando sus partes real e imaginaria:
$$\text{Re}\{Z\} = R, \qquad \text{Im}\{Z\} = \frac{\omega^2 L C_1 - 1}{\omega\left(C_1 + C_2 - \omega^2 L C_1 C_2\right)}$$

---

#### Parte b) Frecuencia de resonancia $\omega_0$

La frecuencia de resonancia es tal que la parte imaginaria de la impedancia se vuelve nula ($\text{Im}\{Z\} = 0$), es decir:
$$X_L = X_{C_1} \implies \omega_0 L = \frac{1}{\omega_0 C_1} \implies \boxed{\omega_0 = \frac{1}{\sqrt{L C_1}}}$$

Al elegir esta frecuencia, el módulo de la impedancia se vuelve mínimo ($|Z(\omega_0)| = R$), y en consecuencia, se maximiza el módulo de la corriente que sale de la fuente ($I_{0,\max} = V_0/R$).

---

#### Parte c) Corriente que circula por la resistencia $R$ en función del tiempo

Como toda la corriente que entrega la fuente pasa por $R$, la corriente instantánea que circula por la resistencia es:
$$I(t) = \text{Re}\left\{\frac{V_0 e^{j\omega t}}{Z}\right\} = \text{Re}\left\{\frac{V_0 e^{j\omega t}}{|Z| e^{j\phi}}\right\} = \frac{V_0}{|Z|} \cos(\omega t - \phi)$$

$$\boxed{I(t) = \frac{V_0}{|Z|} \cos(\omega t - \phi)}$$

De la forma $I(t) = I_0 \cos(\omega t - \phi)$, con $I_0 = \frac{V_0}{|Z|}$, donde de la parte anterior se tiene que los valores de $|Z|$ y $\phi$ son:
$$\boxed{|Z| = \sqrt{R^2 + \left(\frac{\omega^2 L C_1 - 1}{\omega\left(C_1 + C_2 - \omega^2 L C_1 C_2\right)}\right)^2}}$$
$$\boxed{\phi = \arctan\left(\frac{\omega^2 L C_1 - 1}{R\omega\left(C_1 + C_2 - \omega^2 L C_1 C_2\right)}\right)}$$

*(Por tanto, la amplitud de la corriente es $I_0 = \frac{V_0}{\sqrt{R^2 + \left(\frac{\omega^2 L C_1 - 1}{\omega(C_1 + C_2 - \omega^2 L C_1 C_2)}\right)^2}}$).*

---

#### Parte d) Potencia promedio entregada por la fuente

Finalmente, la potencia media que entrega la fuente es:
$$\langle P \rangle = \frac{V_0 I_0}{2}\cos\phi = \frac{V_0^2}{2|Z|}\cos\phi$$

Usando $\cos\phi = \frac{\text{Re}\{Z\}}{|Z|}$:
$$\langle P \rangle = \frac{V_0^2}{2|Z|^2}\text{Re}\{Z\}$$

Sustituyendo $\text{Re}\{Z\} = R$ y $|Z|^2 = R^2 + \left(\frac{\omega^2 L C_1 - 1}{\omega(C_1 + C_2 - \omega^2 L C_1 C_2)}\right)^2$:
$$\boxed{\langle P \rangle = \frac{V_0^2 R}{2R^2 + 2\left(\dfrac{\omega^2 L C_1 - 1}{\omega\left(C_1 + C_2 - \omega^2 L C_1 C_2\right)}\right)^2}}$$

**Verificación:**
- **Unidades:** $[\text{Im}\{Z\}] = \frac{1}{\text{s}^{-1}\cdot\text{F}} = \Omega$; $[\langle P \rangle] = \text{V}^2 \cdot \Omega / \Omega^2 = \text{W}$. Correcto.
- **Límites:** En $\omega = \omega_0 = 1/\sqrt{L C_1}$, se anula $\text{Im}\{Z\}$, por lo que $|Z| = R$, $\phi = 0$, $I_0 = V_0/R$ y $\langle P \rangle = \frac{V_0^2}{2R}$. Cuando $\omega^2 \to \frac{C_1 + C_2}{L C_1 C_2}$ (antirresonancia del bloque paralelo), $|Z| \to \infty$, $I_0 \to 0$ y $\langle P \rangle \to 0$.

---

## Resumen de resultados

| Problema | Magnitud requerida | Resultado analítico |
| :--- | :--- | :--- |
| **P1 (a)** | Impedancia equivalente $Z_{\text{eq}}$ | $Z_{\text{eq}} = 2R + 2j\omega L + \dfrac{1}{j\omega C}$ |
| **P1 (b)** | Fasor de corriente $\hat{I}$ | $\hat{I} = \dfrac{V_0}{\sqrt{4R^2 + (X_L - X_C)^2}}\,e^{-j\phi}, \quad X_L = 2\omega L,\; X_C = \dfrac{1}{\omega C}$ |
| **P1 (b)** | Fasor de voltaje $\hat{V}_L$ | $\hat{V}_L = \dfrac{V_0 \omega L}{\sqrt{4R^2 + (X_L - X_C)^2}}\,e^{j\left(-\phi + \frac{\pi}{2}\right)}$ |
| **P1 (c)** | Frecuencia de resonancia $\omega_0$ | $\omega_0 = \sqrt{\dfrac{1}{2LC}}$ |
| **P1 (c)** | Amplitud máxima de corriente $I_{\max}$ | $I_{\max} = \dfrac{V_0}{2R}$ |
| **P2 (1)** | Impedancia equivalente $Z$ | $Z = R\,\dfrac{R + i\omega L\left[1 - \left(\omega_{LC}/\omega\right)^2\right]}{2R + i\omega L\left[1 - \left(\omega_{LC}/\omega\right)^2\right]}, \quad \omega_{LC} = \dfrac{1}{\sqrt{LC}}$ |
| **P2 (2)** | Amplitud de corriente $I_0$ | $I_0 = \dfrac{U_0}{R}\sqrt{\dfrac{(2R)^2 + (\omega L)^2\left[1 - (\omega_{LC}/\omega)^2\right]^2}{R^2 + (\omega L)^2\left[1 - (\omega_{LC}/\omega)^2\right]^2}}$ |
| **P2 (3)** | Potencia promedio disipada $\overline{P}$ | $\overline{P} = \dfrac{U_0^2}{R} \quad (\text{en resonancia } \omega = \omega_{LC} = 1/\sqrt{LC})$ |
| **P3 (a)** | Impedancia equivalente $Z$ | $Z = R + j\,\dfrac{\omega^2 L C_1 - 1}{\omega\left(C_1 + C_2 - \omega^2 L C_1 C_2\right)}$ |
| **P3 (b)** | Frecuencia de resonancia $\omega_0$ | $\omega_0 = \dfrac{1}{\sqrt{L C_1}}$ |
| **P3 (c)** | Corriente $I(t) = \frac{V_0}{|Z|}\cos(\omega t - \phi)$ | $\|Z\| = \sqrt{R^2 + \left(\dfrac{\omega^2 L C_1 - 1}{\omega(C_1 + C_2 - \omega^2 L C_1 C_2)}\right)^2}, \quad \phi = \arctan\left(\dfrac{\omega^2 L C_1 - 1}{R\omega(C_1 + C_2 - \omega^2 L C_1 C_2)}\right)$ |
| **P3 (d)** | Potencia promedio $\langle P \rangle$ | $\langle P \rangle = \dfrac{V_0^2 R}{2R^2 + 2\left(\dfrac{\omega^2 L C_1 - 1}{\omega(C_1 + C_2 - \omega^2 L C_1 C_2)}\right)^2}$ |
