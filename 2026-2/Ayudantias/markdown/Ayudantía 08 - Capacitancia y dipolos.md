# Ayudantía 08 — Capacitancia y dipolos

> Clases relacionadas: [Clase 05 - Potencial electroestático](../../Clases/markdown/Clase%2005%20-%20Potencial%20electroest%C3%A1tico.md), [Clase 06 - Condensadores](../../Clases/markdown/Clase%2006%20-%20Condensadores.md)

---

## Problema 1

Considere dos condensadores cilíndricos como se indican en la figura. Los condensadores tienen radios $R_1$ y $R_2$ y el otro $R_3$ y $R_4$ (ver figura), determinar la capacitancia equivalente entre los puntos $A$ y $B$. Suponga que $R_1, R_2, R_3, R_4 \ll L$.

> **[Figura]:** Dos condensadores cilíndricos de longitud $L$ dispuestos verticalmente uno al lado del otro. El primer condensador (a la izquierda) posee una armadura cilíndrica interior de radio $R_1$ conectada al terminal $A$, y una armadura cilíndrica exterior de radio $R_2$. El segundo condensador (a la derecha) posee una armadura interior de radio $R_3$ conectada al terminal $B$, y una armadura exterior de radio $R_4$. Las armaduras exteriores de ambos condensadores ($r=R_2$ y $r=R_4$) se encuentran unidas eléctricamente mediante un alambre conductor ideal en la parte superior.

### Solución

**Idea:** Debido a que los radios son mucho menores que la longitud ($R_i \ll L$), se desprecian los efectos de borde y se aplica la ley de Gauss cilíndrica para determinar el campo eléctrico y la diferencia de potencial en un condensador cilíndrico genérico. Luego, analizando la topología del circuito, se identifica que ambos condensadores están conectados en serie a través de sus placas exteriores, permitiendo calcular la capacitancia equivalente.

#### 1. Capacitancia de un condensador cilíndrico

Consideremos un condensador cilíndrico de longitud $L$ con armadura interna de radio $R_{\text{int}}$ portando carga $+Q$, y armadura externa de radio $R_{\text{ext}}$ portando carga $-Q$.

Por simetría cilíndrica, elegimos una superficie gaussiana cilíndrica coaxial de radio $r$ ($R_{\text{int}} \le r < R_{\text{ext}}$) y largo $L$. Aplicando la ley de Gauss:
$$\oint \vec{E} \cdot d\vec{A} = \frac{Q_{\text{enc}}}{\varepsilon_0}$$

El flujo a través de las tapas planas es nulo debido a la dirección puramente radial del campo ($\vec{E} = E(r)\,\hat{r}$). En el manto lateral:
$$E(r) \cdot 2\pi r L = \frac{Q}{\varepsilon_0} \implies \vec{E}(r) = \frac{Q}{2\pi \varepsilon_0 L r}\,\hat{r}$$

La diferencia de potencial entre la armadura exterior e interior es:
$$\Delta V = - \int_{R_{\text{int}}}^{R_{\text{ext}}} \vec{E} \cdot d\vec{r} = - \int_{R_{\text{int}}}^{R_{\text{ext}}} \frac{Q}{2\pi \varepsilon_0 L r}\,dr = - \frac{Q}{2\pi \varepsilon_0 L} \ln\left(\frac{R_{\text{ext}}}{R_{\text{int}}}\right)$$

Tomando la magnitud de la diferencia de potencial $|\Delta V|$:
$$|\Delta V| = \frac{Q}{2\pi \varepsilon_0 L} \ln\left(\frac{R_{\text{ext}}}{R_{\text{int}}}\right)$$

Por definición de capacidad ($C = \frac{Q}{|\Delta V|}$):
$$C = \frac{Q}{\dfrac{Q}{2\pi \varepsilon_0 L} \ln\left(\dfrac{R_{\text{ext}}}{R_{\text{int}}}\right)} = \frac{2\pi \varepsilon_0 L}{\ln(R_{\text{ext}}/R_{\text{int}})}$$

Aplicando este resultado a cada condensador:
$$C_1 = \frac{2\pi \varepsilon_0 L}{\ln(R_2 / R_1)}$$
$$C_2 = \frac{2\pi \varepsilon_0 L}{\ln(R_4 / R_3)}$$

#### 2. Capacitancia equivalente de la conexión

Los condensadores $C_1$ y $C_2$ están conectados en serie. Esto se debe a que la armadura exterior del primer condensador se une directamente con la armadura exterior del segundo cilindro mediante un conductor aislado del resto del circuito. Una carga $+Q$ en el terminal $A$ (armadura $R_1$) induce $-Q$ en la armadura $R_2$, lo que a su vez induce $+Q$ en la armadura interna $R_3$ conectada al terminal $B$ (o $-Q$ en la armadura $R_4$), garantizando que ambos condensadores sostengan la misma carga $Q$.

Para condensadores en serie:
$$\frac{1}{C_{\text{eq}}} = \frac{1}{C_1} + \frac{1}{C_2}$$

Sustituyendo los valores:
$$\frac{1}{C_{\text{eq}}} = \frac{\ln(R_2 / R_1)}{2\pi \varepsilon_0 L} + \frac{\ln(R_4 / R_3)}{2\pi \varepsilon_0 L} = \frac{\ln(R_2 / R_1) + \ln(R_4 / R_3)}{2\pi \varepsilon_0 L}$$

Usando las propiedades del logaritmo ($\ln(a) + \ln(b) = \ln(ab)$):
$$\ln\left(\frac{R_2}{R_1}\right) + \ln\left(\frac{R_4}{R_3}\right) = \ln(R_2) - \ln(R_1) + \ln(R_4) - \ln(R_3) = \ln\left(\frac{R_2 R_4}{R_1 R_3}\right)$$

Invirtiendo la expresión:
$$\boxed{C_{\text{eq}} = \frac{2\pi \varepsilon_0 L}{\ln\left(\dfrac{R_2 R_4}{R_1 R_3}\right)}}$$

> **Nota:** En el manuscrito original, en la línea de sustitución se escribió formalmente $C_{\text{eq}} = \frac{\ln(R_2/R_1)}{2\pi\varepsilon_0 L} + \dots$ por una omisión tipográfica del exponente $-1$ o de la fracción $1/C_{\text{eq}}$, pero en el paso inmediatamente posterior el autor invierte la expresión de manera correcta para arribar al resultado final aquí mostrado.

**Verificación:**
- **Unidades:** $[\varepsilon_0] \cdot [L] = (\text{F/m}) \cdot \text{m} = \text{F}$, lo cual corresponde a unidades de capacitancia.
- **Límites:** Si $R_2 \to R_1$ o $R_4 \to R_3$ (espesor de separación nulo), el argumento del logaritmo tiende a 1, $\ln(1) = 0$, y la capacidad tiende a infinito ($C_{\text{eq}} \to \infty$), tal como se espera al colapsar la distancia entre placas. Si $C_1 = C_2$ (geometrías idénticas con $R_2/R_1 = R_4/R_3 = \eta$), $C_{\text{eq}} = \frac{2\pi \varepsilon_0 L}{2\ln\eta} = \frac{C_1}{2}$, consistente con dos condensadores idénticos en serie.

---

## Problema 2

Considere dos esferas de radio $b$ y densidades de carga $\rho_0$ y $-\rho_0$, las cuales están dispuestas en el eje $z$, a una distancia $2a$ entre ellas, según se muestra en la figura. Se pide:

a) Estimar el potencial en el punto $(0, L, 0)$, suponiendo $L \gg a, b$.  
b) Si se ubica una carga $q$ en la posición $(0, L, 0)$, estime la fuerza sobre la carga.  
c) Calcule el trabajo necesario para llevar la carga desde la posición $(0, L, 0)$ a $(L, 0, 0)$.

> **[Figura]:** Sistema de coordenadas cartesiano tridimensional $(x, y, z)$. Sobre el eje $z$ se disponen dos esferas de radio $b$: una esfera superior centrada en $(0, 0, a)$ con densidad volumétrica uniforme $+\rho_0$, y una esfera inferior centrada en $(0, 0, -a)$ con densidad volumétrica uniforme $-\rho_0$. La separación centro a centro entre las esferas es $2a$. El eje $y$ contiene el punto de observación $(0, L, 0)$ a una distancia $L$ del origen. El plano horizontal formado por los ejes $x$ e $y$ corresponde al plano de simetría $z = 0$.

### Solución

**Idea:** La carga total de cada esfera se calcula integrando su densidad volumétrica uniforme. A distancias grandes respecto al radio ($L \gg b$), el teorema de Gauss asegura que el campo y el potencial exterior de una distribución con simetría esférica son idénticos a los de una carga puntual concentrada en su centro. Por tanto, el sistema equivale a un dipolo eléctrico de cargas $\pm Q$ separadas por $2a$. A distancias $L \gg a$, se emplean aproximaciones multipolares o superposición de fuerzas coulombianas. Para el trabajo, se utiliza la propiedad conservativa del campo electrostático evaluando el potencial en el plano ecuatorial $z=0$.

#### Carga total de las esferas
La carga total de cada esfera se obtiene integrando en su volumen esférico:
$$Q^+ = \iiint \rho_0\,dV = \rho_0 \left(\frac{4}{3}\pi b^3\right) \equiv Q$$
$$Q^- = \iiint (-\rho_0)\,dV = -\rho_0 \left(\frac{4}{3}\pi b^3\right) = -Q$$

A grandes distancias ($L \gg b$), las esferas se comportan como cargas puntuales $+Q$ en $\vec{r}_+ = (0, 0, a)$ y $-Q$ en $\vec{r}_- = (0, 0, -a)$.

#### Parte a) Potencial en $(0, L, 0)$

El punto de observación es $\vec{r} = (0, L, 0)$. Por el principio de superposición:
$$V(L) = V_{Q^+}(L) + V_{Q^-}(L)$$

Las distancias desde cada carga al punto $(0, L, 0)$ son:
$$r_+ = |\vec{r} - \vec{r}_+| = \sqrt{0^2 + L^2 + (0 - a)^2} = \sqrt{L^2 + a^2}$$
$$r_- = |\vec{r} - \vec{r}_-| = \sqrt{0^2 + L^2 + (0 - (-a))^2} = \sqrt{L^2 + a^2}$$

Como ambas distancias son exactamente iguales ($r_+ = r_-$):
$$V(0, L, 0) = \frac{1}{4\pi \varepsilon_0}\frac{Q}{\sqrt{L^2 + a^2}} + \frac{1}{4\pi \varepsilon_0}\frac{(-Q)}{\sqrt{L^2 + a^2}} = \frac{Q}{4\pi \varepsilon_0}\left(\frac{1}{\sqrt{L^2 + a^2}} - \frac{1}{\sqrt{L^2 + a^2}}\right) = 0$$

$$\boxed{V(0, L, 0) = 0}$$

#### Parte b) Fuerza sobre una carga $q$ en $(0, L, 0)$

Calculamos el campo eléctrico generado por cada carga en el punto $\vec{r} = L\hat{j}$:

Para la carga $+Q$ en $\vec{r}_+ = a\hat{k}$:
$$\vec{r} - \vec{r}_+ = L\hat{j} - a\hat{k}$$
$$\vec{E}_+ = \frac{1}{4\pi \varepsilon_0} \frac{Q(\vec{r} - \vec{r}_+)}{|\vec{r} - \vec{r}_+|^3} = \frac{Q}{4\pi \varepsilon_0} \frac{L\hat{j} - a\hat{k}}{(L^2 + a^2)^{3/2}}$$

Dado que $L \gg a$, aproximamos al orden dominante:
$$(L^2 + a^2)^{3/2} = L^3 \left(1 + \frac{a^2}{L^2}\right)^{3/2} \approx L^3$$
$$\vec{E}_+ \approx \frac{Q}{4\pi \varepsilon_0 L^3}(L\hat{j} - a\hat{k})$$

Para la carga $-Q$ en $\vec{r}_- = -a\hat{k}$:
$$\vec{r} - \vec{r}_- = L\hat{j} + a\hat{k}$$
$$\vec{E}_- = \frac{1}{4\pi \varepsilon_0} \frac{(-Q)(\vec{r} - \vec{r}_-)}{|\vec{r} - \vec{r}_-|^3} \approx \frac{-Q}{4\pi \varepsilon_0 L^3}(L\hat{j} + a\hat{k})$$

Sumando ambos campos vectoriales:
$$\vec{E} = \vec{E}_+ + \vec{E}_- = \frac{Q}{4\pi \varepsilon_0 L^3}[(L\hat{j} - a\hat{k}) - (L\hat{j} + a\hat{k})] = - \frac{2Qa}{4\pi \varepsilon_0 L^3}\,\hat{k}$$

Las componentes en $\hat{j}$ se cancelan por simetría, quedando únicamente componente en $-\hat{k}$ ($-\hat{z}$).

Sustituyendo el valor de $Q = \frac{4}{3}\pi \rho_0 b^3$:
$$\vec{E} = - \frac{2a\left(\frac{4}{3}\pi \rho_0 b^3\right)}{4\pi \varepsilon_0 L^3}\,\hat{k} = - \frac{2\rho_0 a b^3}{3\varepsilon_0 L^3}\,\hat{k}$$

La fuerza sobre una carga $q$ ubicada en dicha posición es $\vec{F} = q\vec{E}$:
$$\boxed{\vec{F} = - \frac{2 q \rho_0 a b^3}{3\varepsilon_0 L^3}\,\hat{z}}$$

> **Método alternativo (aproximación dipolar):** El momento dipolar del sistema es $\vec{p} = Q(2a)\,\hat{k} = \frac{8}{3}\pi \rho_0 a b^3\,\hat{k}$. En el plano ecuatorial ($\theta = \pi/2$), el campo dipolar es $\vec{E} = - \frac{\vec{p}}{4\pi \varepsilon_0 L^3} = - \frac{2\rho_0 a b^3}{3\varepsilon_0 L^3}\,\hat{k}$, lo que confirma con exactitud la fuerza calculada.

#### Parte c) Trabajo para trasladar la carga desde $(0, L, 0)$ a $(L, 0, 0)$

El campo electrostático es conservativo, por lo que el trabajo requerido por una fuerza externa para mover la carga con velocidad constante depende únicamente de la diferencia de potencial electrostático entre los puntos final e inicial:
$$W = q \left[V(L, 0, 0) - V(0, L, 0)\right]$$

El plano $z = 0$ (plano $XY$) es el plano mediatriz entre las cargas $+Q$ en $(0, 0, a)$ y $-Q$ en $(0, 0, -a)$. Para cualquier punto $(x, y, 0)$ perteneciente a este plano, la distancia a $+Q$ es:
$$d_+ = \sqrt{x^2 + y^2 + a^2}$$
y la distancia a $-Q$ es:
$$d_- = \sqrt{x^2 + y^2 + (-a)^2} = \sqrt{x^2 + y^2 + a^2} = d_+$$

Por lo tanto, el potencial en cualquier punto del plano $z=0$ es estrictamente cero:
$$V(x, y, 0) = \frac{1}{4\pi \varepsilon_0}\left(\frac{Q}{d_+} - \frac{Q}{d_-}\right) = 0$$

El plano $z=0$ es una superficie equipotencial con potencial nulo. En particular:
$$V(0, L, 0) = 0 \quad \text{y} \quad V(L, 0, 0) = 0$$

Por ende, el trabajo es nulo:
$$\boxed{W = 0}$$

**Verificación:**
- **Simetría:** En el plano $z=0$, el campo eléctrico total $\vec{E}$ es perpendicular al plano en todo punto ($\vec{E} \propto -\hat{k}$). Cualquier desplazamiento contenido en el plano $XY$ tiene vector diferencial $d\vec{r} = dx\,\hat{i} + dy\,\hat{j}$. El producto escalar $\vec{E} \cdot d\vec{r} = 0$, demostrando directamente que $\int \vec{E}\cdot d\vec{r} = 0$ a lo largo de cualquier trayectoria en dicho plano.

---

## Problema 3

Una carga $+Q$ se encuentra inserta en un alambre conductor de largo $L$ y radio $R_0$ muy pequeño. Un cascarón cilíndrico conductor neutro de radios interno $R_1$ y externo $R_2$ y largo $L$ es ubicado simétricamente alrededor del alambre (ver figura). Tener en cuenta que: $R_0 \ll R_1, R_2 \ll L$. Calcule:

a) La densidad lineal de carga $\lambda$ del alambre.  
b) La densidad superficial de carga en la capa interna y externa del cascarón; y la densidad volumétrica de carga dentro del conductor.  
c) El campo eléctrico en todo el espacio.

Ahora deposite una carga $-Q$ en el cascarón cilíndrico, calcule:

d) Las nuevas densidades de carga superficiales en las capas interna y externa del cascarón, y también la densidad volumétrica dentro de éste.  
e) El nuevo campo eléctrico en todo el espacio.  
f) La diferencia de potencial entre el cilindro y el alambre $\Delta V = V_{\text{cilindro}} - V_{\text{alambre}}$.  
g) La capacidad (o capacitancia) del sistema.  
h) La energía almacenada en el sistema.

> **[Figura]:** Sección transversal de un sistema cilíndrico coaxial de longitud $L$. En el centro se ubica un alambre conductor de radio $R_0$ que lleva una carga $+Q$. Rodeándolo concéntricamente se encuentra un cascarón cilíndrico conductor con radio interno $R_1$ y radio externo $R_2$. El espacio entre $R_0$ y $R_1$ y el espacio exterior a $R_2$ corresponden a vacío.

### Solución

**Idea:** La condición de equilibrio electrostático impone que al interior de todo material conductor el campo eléctrico es idénticamente nulo ($\vec{E} = 0$), lo cual implica que no existe carga volumétrica neta en su seno ($\rho = 0$) y que toda carga se distribuye en sus superficies. Aplicando la ley de Gauss cilíndrica con superficies coaxiales de longitud $L$, se determinan las cargas inducidas, los campos en cada región y las diferencias de potencial por integración radial.

---

### Cascarón cilíndrico neutro

#### Parte a) Densidad lineal de carga $\lambda$ del alambre
La carga total $+Q$ está distribuida uniformemente a lo largo de la longitud $L$ del alambre:
$$\boxed{\lambda = \frac{Q}{L}}$$

#### Parte b) Densidades de carga en el cascarón neutro
En el interior del cascarón conductor ($R_1 < r < R_2$), en equilibrio electrostático se tiene:
$$\vec{E} = 0$$

Considerando una superficie cilíndrica gaussiana de radio $r \in (R_1, R_2)$ y longitud $L$:
$$\oint \vec{E} \cdot d\vec{A} = 0 \implies Q_{\text{enc}} = 0$$

La carga encerrada comprende la carga del alambre $+Q$ más la carga $Q_{\text{int}}$ inducida en la superficie interna del cascarón ($r = R_1$):
$$Q_{\text{enc}} = Q + Q_{\text{int}} = 0 \implies Q_{\text{int}} = -Q$$

Como el área lateral interna es $A_1 = 2\pi R_1 L$, la densidad superficial interna es:
$$\boxed{\sigma_{\text{int}} = -\frac{Q}{2\pi R_1 L}}$$

El cascarón es originalmente neutro ($Q_{\text{cascarón}} = Q_{\text{int}} + Q_{\text{ext}} = 0$):
$$Q_{\text{ext}} = -Q_{\text{int}} = +Q$$

Con área lateral externa $A_2 = 2\pi R_2 L$:
$$\boxed{\sigma_{\text{ext}} = \frac{Q}{2\pi R_2 L}}$$

Dentro del material conductor ($R_1 < r < R_2$):
$$\boxed{\rho = 0}$$

#### Parte c) Campo eléctrico en todo el espacio
Por la ley de Gauss cilíndrica, para un cilindro de radio $r$ y longitud $L$:
$$E(r) \cdot 2\pi r L = \frac{Q_{\text{enc}}}{\varepsilon_0} \implies E(r) = \frac{Q_{\text{enc}}}{2\pi \varepsilon_0 L r}$$

Evaluando por regiones:
- Para $r < R_0$ (interior del alambre conductor):
  $$\vec{E}(r) = 0$$
- Para $R_0 < r < R_1$: $Q_{\text{enc}} = Q = \lambda L$, por lo que:
  $$\vec{E}(r) = \frac{\lambda}{2\pi \varepsilon_0 r}\,\hat{r} = \frac{Q}{2\pi \varepsilon_0 L r}\,\hat{r}$$
- Para $R_1 < r < R_2$ (interior del cascarón conductor):
  $$\vec{E}(r) = 0$$
- Para $r > R_2$: $Q_{\text{enc}} = Q + Q_{\text{int}} + Q_{\text{ext}} = Q - Q + Q = Q = \lambda L$, por lo que:
  $$\vec{E}(r) = \frac{\lambda}{2\pi \varepsilon_0 r}\,\hat{r} = \frac{Q}{2\pi \varepsilon_0 L r}\,\hat{r}$$

En resumen:
$$\boxed{\vec{E}(r) = \begin{cases} 0 & r < R_0 \\[1ex] \dfrac{\lambda}{2\pi \varepsilon_0 r}\,\hat{r} & R_0 < r < R_1 \\[1ex] 0 & R_1 < r < R_2 \\[1ex] \dfrac{\lambda}{2\pi \varepsilon_0 r}\,\hat{r} & r > R_2 \end{cases}}$$

---

### Cascarón cilíndrico con carga $-Q$

#### Parte d) Nuevas densidades de carga
Al depositar una carga neta de $-Q$ sobre el cascarón conductor:
1. En el interior del conductor ($R_1 < r < R_2$), se mantiene la condición de equilibrio electrostático $\vec{E} = 0$. Por ley de Gauss a través de una superficie en su interior:
   $$Q_{\text{enc}} = Q + Q_{\text{int}} = 0 \implies Q_{\text{int}} = -Q$$
   Por tanto, la densidad de carga en la superficie interior permanece invariante:
   $$\boxed{\sigma_{\text{int}} = -\frac{Q}{2\pi R_1 L}}$$

2. Por conservación de carga sobre el cascarón, la carga neta es ahora $-Q$:
   $$Q_{\text{int}} + Q_{\text{ext}} = -Q \implies -Q + Q_{\text{ext}} = -Q \implies Q_{\text{ext}} = 0$$
   De donde se deduce:
   $$\boxed{\sigma_{\text{ext}} = 0}$$

3. Dentro del conductor la densidad volumétrica sigue siendo nula:
   $$\boxed{\rho = 0}$$

#### Parte e) Nuevo campo eléctrico en todo el espacio
- Para $r < R_0$: $\vec{E}(r) = 0$.
- Para $R_0 < r < R_1$: $Q_{\text{enc}} = Q \implies \vec{E}(r) = \dfrac{\lambda}{2\pi \varepsilon_0 r}\,\hat{r} = \dfrac{Q}{2\pi \varepsilon_0 L r}\,\hat{r}$.
- Para $R_1 < r < R_2$: conductor $\implies \vec{E}(r) = 0$.
- Para $r > R_2$: $Q_{\text{enc}} = Q + Q_{\text{cascarón}} = Q + (-Q) = 0 \implies \vec{E}(r) = 0$.

En resumen:
$$\boxed{\vec{E}(r) = \begin{cases} 0 & r < R_0 \\[1ex] \dfrac{\lambda}{2\pi \varepsilon_0 r}\,\hat{r} & R_0 < r < R_1 \\[1ex] 0 & R_1 < r < R_2 \\[1ex] 0 & r > R_2 \end{cases}}$$

#### Parte f) Diferencia de potencial $\Delta V = V_{\text{cilindro}} - V_{\text{alambre}}$
Integrando el campo eléctrico a lo largo del radio desde el alambre ($r = R_0$) hasta la cara interna del cilindro ($r = R_1$):
$$\Delta V = V(R_1) - V(R_0) = - \int_{R_0}^{R_1} \vec{E} \cdot d\vec{r} = - \int_{R_0}^{R_1} \frac{\lambda}{2\pi \varepsilon_0 r}\,dr = - \frac{\lambda}{2\pi \varepsilon_0} \ln\left(\frac{R_1}{R_0}\right)$$

Expresando en función de $Q$ ($\lambda = Q/L$):
$$\boxed{\Delta V = - \frac{Q}{2\pi \varepsilon_0 L}\ln\left(\frac{R_1}{R_0}\right)}$$

Como $R_1 > R_0$, $\ln(R_1/R_0) > 0$, lo que confirma que el cilindro se encuentra a menor potencial que el alambre con carga positiva ($\Delta V < 0$).

#### Parte g) Capacidad del sistema
La capacitancia se define respecto al valor absoluto de la diferencia de potencial entre los conductores:
$$C = \frac{Q}{|\Delta V|} = \frac{Q}{\dfrac{Q}{2\pi \varepsilon_0 L}\ln(R_1/R_0)}$$

$$\boxed{C = \frac{2\pi \varepsilon_0 L}{\ln(R_1 / R_0)}}$$

#### Parte h) Energía almacenada en el sistema
La energía electrostática total almacenada en el condensador cilíndrico es:
$$U = \frac{1}{2} \frac{Q^2}{C} = \frac{Q^2}{2 \left(\dfrac{2\pi \varepsilon_0 L}{\ln(R_1/R_0)}\right)}$$

$$\boxed{U = \frac{Q^2 \ln(R_1 / R_0)}{4\pi \varepsilon_0 L}}$$

> **Demostración por trabajo de carga:** Para cargar el condensador trayendo cargas $dq$ incrementales:
> $$dW = \Delta V(q)\,dq = \frac{q}{C}\,dq \implies W = \int_0^Q \frac{q}{C}\,dq = \frac{1}{2}\frac{Q^2}{C}$$
> que coincide plenamente con la expresión de la energía almacenada.

**Verificación:**
- **Conservación de la carga:** La suma de densidades superficiales integradas reproduce exactamente las cargas totales asignadas: $Q_{\text{int}} + Q_{\text{ext}} = -Q + 0 = -Q$.
- **Discontinuidad del campo:** En $r = R_1$, el salto de campo normal es $\Delta E_r = E(R_1^+) - E(R_1^-) = 0 - \frac{Q}{2\pi \varepsilon_0 L R_1} = \frac{\sigma_{\text{int}}}{\varepsilon_0}$, satisfaciendo la condición de borde electrostática. En $r = R_2$, como $\sigma_{\text{ext}} = 0$, el campo exterior es nulo y no hay discontinuidad ($\Delta E_r = 0$).

---

## Resumen de resultados

| Problema / Inciso | Descripción | Resultado final |
| :--- | :--- | :--- |
| **Problema 1** | Capacitancia equivalente de dos cilindros en serie | $C_{\text{eq}} = \dfrac{2\pi \varepsilon_0 L}{\ln\left(\dfrac{R_2 R_4}{R_1 R_3}\right)}$ |
| **Problema 2 a)** | Potencial dipolar en $(0, L, 0)$ con $L \gg a, b$ | $V(0, L, 0) = 0$ |
| **Problema 2 b)** | Fuerza sobre carga $q$ en $(0, L, 0)$ | $\vec{F} = - \dfrac{2 q \rho_0 a b^3}{3\varepsilon_0 L^3}\,\hat{z}$ |
| **Problema 2 c)** | Trabajo para llevar $q$ de $(0, L, 0)$ a $(L, 0, 0)$ | $W = 0$ |
| **Problema 3 a)** | Densidad lineal del alambre | $\lambda = \dfrac{Q}{L}$ |
| **Problema 3 b)** | Densidades en cascarón neutro | $\sigma_{\text{int}} = -\dfrac{Q}{2\pi R_1 L}, \quad \sigma_{\text{ext}} = \dfrac{Q}{2\pi R_2 L}, \quad \rho = 0$ |
| **Problema 3 c)** | Campo eléctrico (cascarón neutro) | $\vec{E}(r) = \begin{cases} \dfrac{Q}{2\pi\varepsilon_0 L r}\,\hat{r} & r \in (R_0, R_1) \cup (R_2, \infty) \\ 0 & r < R_0 \text{ o } r \in (R_1, R_2) \end{cases}$ |
| **Problema 3 d)** | Densidades en cascarón cargado con $-Q$ | $\sigma_{\text{int}} = -\dfrac{Q}{2\pi R_1 L}, \quad \sigma_{\text{ext}} = 0, \quad \rho = 0$ |
| **Problema 3 e)** | Campo eléctrico (cascarón con $-Q$) | $\vec{E}(r) = \begin{cases} \dfrac{Q}{2\pi\varepsilon_0 L r}\,\hat{r} & R_0 < r < R_1 \\ 0 & r < R_0 \text{ o } r > R_1 \end{cases}$ |
| **Problema 3 f)** | Diferencia de potencial $V_{\text{cilindro}} - V_{\text{alambre}}$ | $\Delta V = -\dfrac{Q}{2\pi\varepsilon_0 L}\ln\left(\dfrac{R_1}{R_0}\right)$ |
| **Problema 3 g)** | Capacitancia del sistema | $C = \dfrac{2\pi \varepsilon_0 L}{\ln(R_1 / R_0)}$ |
| **Problema 3 h)** | Energía almacenada | $U = \dfrac{Q^2 \ln(R_1 / R_0)}{4\pi \varepsilon_0 L}$ |
