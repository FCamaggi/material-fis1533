# Ayudantía 09 — Dieléctricos

> Clases relacionadas: [Clase 06 - Condensadores](../../Clases/markdown/Clase%2006%20-%20Condensadores.md), [Clase 07 - Dieléctricos](../../Clases/markdown/Clase%2007%20-%20Diel%C3%A9ctricos.md)

---

## Problema 1

Considere un cable coaxial compuesto por dos materiales dieléctricos lineales e isotrópicos, con permitividades $\epsilon_1$ y $\epsilon_2$, entre dos conductores de espesor despreciable, sobre los cuales se aplica una diferencia de potencial $V_0$, como se muestra en la figura.

a) El vector desplazamiento en todo el espacio.  
b) El campo eléctrico en todo el espacio.  
c) El vector de polarización en todo el espacio.

> **[Figura]:** Sección transversal de un cable coaxial cilíndrico formado por dos conductores coaxiales de espesor despreciable: un conductor interior de radio $a$ y un conductor exterior de radio $c$. La región comprendida entre $r = a$ y $r = b$ está ocupada por un dieléctrico de permitividad $\epsilon_1$. La región entre $r = b$ y $r = c$ está ocupada por un dieléctrico de permitividad $\epsilon_2$. Una fuente de voltaje continuo aplica una diferencia de potencial $V_0$ entre los conductores, con el terminal positivo conectado al conductor exterior ($r = c$) y el terminal negativo conectado al conductor interior ($r = a$).

### Solución

**Idea:** En medios dieléctricos con simetría cilíndrica, la ley de Gauss en medios materiales relaciona directamente el flujo del vector desplazamiento eléctrico $\vec{D}$ con la carga libre encerrada $Q_{\text{libre}}$. Al tratarse de dieléctricos lineales e isotrópicos, el campo eléctrico se obtiene mediante la relación constitutiva $\vec{D} = \epsilon \vec{E}$. Integrando radialmente el campo eléctrico entre los electrodos se vincula la carga libre con la diferencia de potencial impuesta $V_0$. Finalmente, el vector de polarización se calcula a través de $\vec{P} = (\epsilon - \varepsilon_0)\vec{E}$.

#### 1. Ley de Gauss para el desplazamiento eléctrico $\vec{D}$

Consideramos un tramo de longitud $L$ del cable coaxial ($L \gg c$) para despreciar efectos de borde. Por simetría cilíndrica azimutal y longitudinal, el desplazamiento eléctrico es estrictamente radial:
$$\vec{D}(r) = D_r(r)\,\hat{r}$$

Tomando como superficie gaussiana un cilindro coaxial de radio $r$ y longitud $L$:
$$\oint \vec{D} \cdot d\vec{A} = Q_{\text{libre, enc}}$$

El flujo en las tapas basales es cero. En la superficie lateral ($d\vec{A} = \hat{r}\,r\,d\phi\,dz$):
$$\iint D_r(r)\,r\,d\phi\,dz = D_r(r) \cdot 2\pi r L = Q_{\text{libre, enc}}$$

Por tanto, para una carga libre total $Q$ en el conductor interior a lo largo de la longitud $L$:
$$D_r(r) = \frac{Q}{2\pi r L}$$

Evaluando por regiones en función de la carga libre $Q$:
- Para $r < a$ (interior del conductor central): $Q_{\text{libre, enc}} = 0 \implies \vec{D} = 0$.
- Para $a < r < b$ (medio con $\epsilon_1$): $Q_{\text{libre, enc}} = Q \implies \vec{D}_1(r) = \dfrac{Q}{2\pi r L}\,\hat{r}$.
- Para $b < r < c$ (medio con $\epsilon_2$): $Q_{\text{libre, enc}} = Q \implies \vec{D}_2(r) = \dfrac{Q}{2\pi r L}\,\hat{r}$.
- Para $r > c$ (exterior del conductor externo): la carga neta libre de ambos conductores es cero ($Q_{\text{libre, enc}} = Q + (-Q) = 0$) $\implies \vec{D} = 0$.

#### 2. Relación con la diferencia de potencial $V_0$

Los campos eléctricos en cada región dieléctrica son:
$$\vec{E}_1(r) = \frac{\vec{D}_1(r)}{\epsilon_1} = \frac{Q}{2\pi \epsilon_1 L r}\,\hat{r} \quad (a < r < b)$$
$$\vec{E}_2(r) = \frac{\vec{D}_2(r)}{\epsilon_2} = \frac{Q}{2\pi \epsilon_2 L r}\,\hat{r} \quad (b < r < c)$$

La diferencia de potencial aplicada por la batería establece que el conductor exterior ($r=c$) está a un potencial $V_0$ respecto al conductor interior ($r=a$), es decir, $V(c) - V(a) = V_0$:
$$V_0 = V(c) - V(a) = - \int_a^c \vec{E} \cdot d\vec{r} = - \left[\int_a^b \vec{E}_1 \cdot d\vec{r} + \int_b^c \vec{E}_2 \cdot d\vec{r}\right]$$

Sustituyendo los campos radiales:
$$V_0 = - \left[\int_a^b \frac{Q}{2\pi \epsilon_1 L r}\,dr + \int_b^c \frac{Q}{2\pi \epsilon_2 L r}\,dr\right] = - \frac{Q}{2\pi L} \left[\frac{\ln(b/a)}{\epsilon_1} + \frac{\ln(c/b)}{\epsilon_2}\right]$$

Sumando las fracciones en el corchete:
$$V_0 = - \frac{Q}{2\pi L} \left[\frac{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)}{\epsilon_1 \epsilon_2}\right]$$

Despejando la carga libre $Q$:
$$Q = - \frac{2\pi L V_0 \epsilon_1 \epsilon_2}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)}$$

El signo negativo refleja que, al estar el conductor exterior al potencial más alto ($+V_0$), el conductor interior acumula carga libre negativa para que el campo eléctrico apunte hacia adentro ($-\hat{r}$), de mayor a menor potencial.

#### Parte a) Vector desplazamiento en todo el espacio
Reemplazando $Q$ en la expresión de $\vec{D}$:
$$\boxed{\vec{D}(r) = \begin{cases} 0 & r < a \\[1ex] - \dfrac{V_0 \epsilon_1 \epsilon_2}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)} \dfrac{1}{r}\,\hat{r} & a < r < c \\[1ex] 0 & r > c \end{cases}}$$

#### Parte b) Campo eléctrico en todo el espacio
Dividiendo $\vec{D}(r)$ por la permitividad correspondiente:
- En $a < r < b$, dividimos por $\epsilon_1$:
  $$\vec{E}_1(r) = - \frac{V_0 \epsilon_2}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)} \frac{1}{r}\,\hat{r}$$
- En $b < r < c$, dividimos por $\epsilon_2$:
  $$\vec{E}_2(r) = - \frac{V_0 \epsilon_1}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)} \frac{1}{r}\,\hat{r}$$

$$\boxed{\vec{E}(r) = \begin{cases} 0 & r < a \\[1ex] - \dfrac{V_0 \epsilon_2}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)} \dfrac{1}{r}\,\hat{r} & a < r < b \\[1ex] - \dfrac{V_0 \epsilon_1}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)} \dfrac{1}{r}\,\hat{r} & b < r < c \\[1ex] 0 & r > c \end{cases}}$$

#### Parte c) Vector de polarización en todo el espacio
Para un medio lineal e isotrópico, $\vec{P} = \vec{D} - \varepsilon_0 \vec{E} = (\epsilon - \varepsilon_0)\vec{E}$. En los conductores y en el vacío exterior la polarización es nula ($\vec{P} = 0$).

- Para $a < r < b$:
  $$\vec{P}_1(r) = (\epsilon_1 - \varepsilon_0)\vec{E}_1(r) = - \frac{V_0 (\epsilon_1 - \varepsilon_0)\epsilon_2}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)} \frac{1}{r}\,\hat{r}$$

- Para $b < r < c$:
  $$\vec{P}_2(r) = (\epsilon_2 - \varepsilon_0)\vec{E}_2(r) = - \frac{V_0 (\epsilon_2 - \varepsilon_0)\epsilon_1}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)} \frac{1}{r}\,\hat{r}$$

$$\boxed{\vec{P}(r) = \begin{cases} 0 & r < a \\[1ex] - \dfrac{V_0 (\epsilon_1 - \varepsilon_0)\epsilon_2}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)} \dfrac{1}{r}\,\hat{r} & a < r < b \\[1ex] - \dfrac{V_0 (\epsilon_2 - \varepsilon_0)\epsilon_1}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)} \dfrac{1}{r}\,\hat{r} & b < r < c \\[1ex] 0 & r > c \end{cases}}$$

**Verificación:**
- **Continuidad de la componente normal de $\vec{D}$:** En la interfaz dieléctrica $r = b$, no existe carga libre interfacial ($\sigma_{\text{libre}} = 0$). La componente normal $D_{1r}(b) = D_{2r}(b)$ es perfectamente continua, cumpliendo las condiciones de borde.
- **Discontinuidad de $\vec{E}$:** $\epsilon_1 E_{1r}(b) = \epsilon_2 E_{2r}(b)$, lo cual concuerda con la existencia de una densidad de carga de polarización ligada superficial en la interfaz: $\sigma_p = (\vec{P}_2 - \vec{P}_1) \cdot \hat{r}\big|_{r=b} = \varepsilon_0 [E_{1r}(b) - E_{2r}(b)]$.

---

## Problema 2

Considere un cable coaxial de longitud $L$, el cual tiene una sección transversal como la mostrada en la figura. Este cable consiste de un alambre macizo de cobre de radio $R$ rodeado por dos mantos (cascarones) cilíndricos sucesivos concéntricos de material dieléctrico de constantes dieléctricas (permitividad relativa) $\kappa_1$ y $\kappa_2$, respectivamente, y un envoltorio (cascarón) cilíndrico metálico de radio interior $3R$ y espesor $R/4$.

a) Calcule la capacitancia del sistema, considerando que $L \gg R$.  
b) Si una batería de $12\text{ V}$ es conectada con su polo positivo al conductor macizo y su terminal negativo al conductor exterior, ¿cuál es la carga neta almacenada en el conductor macizo?  
c) ¿Cuál es la energía almacenada en el condensador cuando está completamente cargado?

> **[Figura]:** Sección transversal circular de un cable coaxial:
> - Núcleo central macizo de cobre (conductor) de radio $R$.
> - Primer manto dieléctrico concéntrico de radio interior $R$, radio exterior $2R$ y constante dieléctrica $\kappa_1$.
> - Segundo manto dieléctrico concéntrico de radio interior $2R$, radio exterior $3R$ y constante dieléctrica $\kappa_2$.
> - Envoltorio exterior metálico (conductor) con radio interior $3R$ y espesor de pared $R/4$ (radio exterior $3{,}25R$).

### Solución

**Idea:** La disposición concéntrica de dos dieléctricos distintos entre los conductores equivale a dos condensadores cilíndricos conectados en serie. Se puede determinar la capacitancia equivalente asociando las capacitancias en serie o, equivalentemente, calculando desde primeros principios el campo de desplazamiento $\vec{D}$, los campos $\vec{E}_1$ y $\vec{E}_2$, integrando la diferencia de potencial $\Delta V$ y evaluando $C = Q/\Delta V$. La carga y la energía almacenada se obtienen a partir de las relaciones fundamentales $Q = C V$ y $U = \frac{1}{2} C V^2$.

#### Parte a) Capacitancia del sistema

##### Método 1: Asociación de condensadores en serie
La capacitancia de un condensador cilíndrico de longitud $L$ con radios interior $R_i$ y exterior $R_f$ lleno de dieléctrico de constante $\kappa$ es:
$$C = \kappa \frac{2\pi \varepsilon_0 L}{\ln(R_f / R_i)}$$

Para las dos capas cilíndricas:
- Capa 1 ($R \le r \le 2R$):
  $$C_1 = \kappa_1 \frac{2\pi \varepsilon_0 L}{\ln(2R / R)} = \frac{2\pi \varepsilon_0 L \kappa_1}{\ln(2)}$$
- Capa 2 ($2R \le r \le 3R$):
  $$C_2 = \kappa_2 \frac{2\pi \varepsilon_0 L}{\ln(3R / 2R)} = \frac{2\pi \varepsilon_0 L \kappa_2}{\ln(3/2)}$$

Al estar dispuestas sucesivamente en dirección radial, la conexión es en serie:
$$\frac{1}{C} = \frac{1}{C_1} + \frac{1}{C_2} = \frac{\ln(2)}{2\pi \varepsilon_0 L \kappa_1} + \frac{\ln(3/2)}{2\pi \varepsilon_0 L \kappa_2} = \frac{1}{2\pi \varepsilon_0 L \kappa_1 \kappa_2} \left[\kappa_2 \ln(2) + \kappa_1 \ln(3/2)\right]$$

Invirtiendo la expresión:
$$\boxed{C = \frac{2\pi \varepsilon_0 L \kappa_1 \kappa_2}{\kappa_2 \ln(2) + \kappa_1 \ln(3/2)}}$$

##### Demostración alternativa desde primeros principios
Suponiendo una carga libre $+Q$ en el conductor interior y $-Q$ en el conductor exterior:
Por la ley de Gauss en medios dieléctricos con superficie cilíndrica de radio $r$ y longitud $L$:
$$D(r) \cdot 2\pi r L = Q \implies D(r) = \frac{Q}{2\pi r L}$$

El campo eléctrico en cada manto es $\vec{E} = \frac{\vec{D}}{\varepsilon_0 \kappa}$:
- Región 1 ($R < r < 2R$): $E_1(r) = \dfrac{Q}{2\pi \varepsilon_0 \kappa_1 L r}$
- Región 2 ($2R < r < 3R$): $E_2(r) = \dfrac{Q}{2\pi \varepsilon_0 \kappa_2 L r}$

La diferencia de potencial $\Delta V = V(R) - V(3R)$ es:
$$\Delta V = \int_R^{3R} E(r)\,dr = \int_R^{2R} E_1(r)\,dr + \int_{2R}^{3R} E_2(r)\,dr$$
$$\Delta V = \frac{Q}{2\pi \varepsilon_0 L} \left[\frac{1}{\kappa_1} \int_R^{2R} \frac{dr}{r} + \frac{1}{\kappa_2} \int_{2R}^{3R} \frac{dr}{r}\right] = \frac{Q}{2\pi \varepsilon_0 L} \left[\frac{\ln(2)}{\kappa_1} + \frac{\ln(3/2)}{\kappa_2}\right]$$

Por definición, $C = \frac{Q}{\Delta V}$:
$$C = \frac{Q}{\dfrac{Q}{2\pi \varepsilon_0 L}\left[\dfrac{\ln(2)}{\kappa_1} + \dfrac{\ln(3/2)}{\kappa_2}\right]} = \frac{2\pi \varepsilon_0 L}{\dfrac{\ln(2)}{\kappa_1} + \dfrac{\ln(3/2)}{\kappa_2}} = \frac{2\pi \varepsilon_0 L \kappa_1 \kappa_2}{\kappa_2 \ln(2) + \kappa_1 \ln(3/2)}$$
lo que confirma formalmente el resultado.

#### Parte b) Carga neta en el conductor macizo
Con una diferencia de potencial aplicada $V = 12\text{ V}$, donde el polo positivo está conectado al conductor central:
$$Q_+ = C \cdot V = (12\text{ V}) \cdot C$$

Sustituyendo $C$:
$$\boxed{Q_+ = \frac{24\pi \varepsilon_0 L \kappa_1 \kappa_2}{\kappa_2 \ln(2) + \kappa_1 \ln(3/2)} \text{ [C]}}$$

#### Parte c) Energía almacenada en el condensador
La energía electrostática almacenada en el sistema cargado es:
$$U = \frac{1}{2} Q V = \frac{1}{2} C V^2$$

Con $V = 12\text{ V}$:
$$U = \frac{(12\text{ V})^2}{2} C = 72\,C = 72 \cdot \frac{2\pi \varepsilon_0 L \kappa_1 \kappa_2}{\kappa_2 \ln(2) + \kappa_1 \ln(3/2)}$$

$$\boxed{U = \frac{144\pi \varepsilon_0 L \kappa_1 \kappa_2}{\kappa_2 \ln(2) + \kappa_1 \ln(3/2)} \text{ [J]}}$$

**Verificación:**
- **Espesor del conductor exterior:** El espesor $R/4$ del conductor metálico exterior no interviene en la capacitancia porque en electrostática la carga libre se confina a la superficie interior ($r = 3R$) que encara al dieléctrico, y el campo eléctrico en el seno del conductor es idénticamente nulo.
- **Consistencia dimensional:** $[Q] = [\text{F}] \cdot [\text{V}] = \text{C}$, y $[U] = [\text{F}] \cdot [\text{V}^2] = \text{J}$.

---

## Problema 3

Una esfera dieléctrica de radio $b$ y permitividad de carga $\epsilon$ contienen en un interior una densidad de carga libre
$$\rho(r) = \begin{cases} \rho_0 r & 0 < r < b \\ 0 & r > b \end{cases}$$

a) Calcule las densidades de carga de polarización en volumen $\rho_p$ y superficial $\sigma_p$ en las zonas donde existan.  
b) Calcule la energía electrostática del sistema de cargas.

> **[Figura]:** Esfera dieléctrica homogénea de radio $b$ con permitividad $\epsilon$, inmersa en vacío ($\varepsilon_0$). En su interior alberga una distribución de carga libre con simetría esférica dada por $\rho(r) = \rho_0 r$ para $0 < r < b$, y nula en el exterior ($r > b$).

### Solución

**Idea:** La simetría esférica permite aplicar la ley de Gauss para el vector desplazamiento eléctrico $\vec{D}$ con superficies gaussianas esféricas concéntricas. A partir de $\vec{D}$, se determina el campo eléctrico $\vec{E}$ dentro y fuera de la esfera considerando las respectivas permitividades ($\epsilon$ dentro y $\varepsilon_0$ fuera). El vector polarización $\vec{P} = \vec{D} - \varepsilon_0 \vec{E}$ genera densidad superficial de carga ligada $\sigma_p = \vec{P} \cdot \hat{n}$ en la frontera y densidad volumétrica $\rho_p = -\nabla \cdot \vec{P}$ en el volumen. La energía electrostática total se calcula integrando la densidad de energía $u = \frac{1}{2} \vec{D} \cdot \vec{E}$ en todo el espacio.

#### 1. Cálculo de los campos $\vec{D}$ y $\vec{E}$

Por simetría esférica, $\vec{D}(r) = D(r)\,\hat{r}$ y $\vec{E}(r) = E(r)\,\hat{r}$. Tomando una superficie gaussiana esférica de radio $r$:
$$\oint \vec{D} \cdot d\vec{A} = Q_{\text{libre, enc}} \implies D(r) \cdot 4\pi r^2 = Q_{\text{libre, enc}}$$

- **Región interior ($r \le b$):**
  $$Q_{\text{libre, enc}} = \int_0^r \rho(r') 4\pi r'^2\,dr' = 4\pi \rho_0 \int_0^r r'^3\,dr' = 4\pi \rho_0 \frac{r^4}{4} = \pi \rho_0 r^4$$
  $$D(r) \cdot 4\pi r^2 = \pi \rho_0 r^4 \implies \vec{D}(r) = \frac{\rho_0 r^2}{4}\,\hat{r}$$
  El campo eléctrico en el medio dieléctrico ($\vec{D} = \epsilon \vec{E}$):
  $$\vec{E}(r) = \frac{\rho_0 r^2}{4\epsilon}\,\hat{r}$$

- **Región exterior ($r > b$):**
  La carga libre total contenida en la esfera es:
  $$Q_{\text{libre, tot}} = 4\pi \rho_0 \int_0^b r'^3\,dr' = \pi \rho_0 b^4$$
  $$D(r) \cdot 4\pi r^2 = \pi \rho_0 b^4 \implies \vec{D}(r) = \frac{\rho_0 b^4}{4r^2}\,\hat{r}$$
  En el exterior hay vacío ($\vec{D} = \varepsilon_0 \vec{E}$):
  $$\vec{E}(r) = \frac{\rho_0 b^4}{4\varepsilon_0 r^2}\,\hat{r}$$

#### Parte a) Densidades de carga de polarización $\rho_p$ y $\sigma_p$

En el exterior ($r > b$), no existe medio material polarizable, de modo que $\vec{P} = 0$.

En el interior de la esfera ($r \le b$):
$$\vec{P}(r) = \vec{D}(r) - \varepsilon_0 \vec{E}(r) = (\epsilon - \varepsilon_0)\vec{E}(r) = \frac{(\epsilon - \varepsilon_0)\rho_0 r^2}{4\epsilon}\,\hat{r}$$

1. **Densidad superficial de polarización $\sigma_p$ en $r = b$:**  
   El vector normal unitario exterior a la superficie es $\hat{n} = \hat{r}$:
   $$\sigma_p = \vec{P} \cdot \hat{n}\Big|_{r=b} = P_r(b)$$
   $$\boxed{\sigma_p = \frac{(\epsilon - \varepsilon_0)\rho_0 b^2}{4\epsilon}}$$

2. **Densidad volumétrica de polarización $\rho_p$ en $0 < r < b$:**  
   En coordenadas esféricas, la divergencia de un campo radial $\vec{P} = P_r(r)\,\hat{r}$ es:
   $$\rho_p = - \nabla \cdot \vec{P} = - \frac{1}{r^2}\frac{\partial}{\partial r}\left(r^2 P_r\right)$$
   Sustituyendo $P_r(r) = \dfrac{(\epsilon - \varepsilon_0)\rho_0 r^2}{4\epsilon}$:
   $$\rho_p = - \frac{1}{r^2}\frac{\partial}{\partial r}\left(\frac{(\epsilon - \varepsilon_0)\rho_0 r^4}{4\epsilon}\right) = - \frac{1}{r^2} \left[\frac{4(\epsilon - \varepsilon_0)\rho_0 r^3}{4\epsilon}\right]$$
   $$\boxed{\rho_p = - \frac{(\epsilon - \varepsilon_0)\rho_0 r}{\epsilon}}$$

> **Verificación de neutralidad:** La carga total de polarización debe ser nula ($Q_{p,\text{tot}} = 0$):
> $$Q_{p,\text{vol}} = \int_0^b \rho_p (4\pi r^2)\,dr = - \frac{4\pi(\epsilon - \varepsilon_0)\rho_0}{\epsilon} \int_0^b r^3\,dr = - \frac{\pi(\epsilon - \varepsilon_0)\rho_0 b^4}{\epsilon}$$
> $$Q_{p,\text{sup}} = \sigma_p (4\pi b^2) = \frac{(\epsilon - \varepsilon_0)\rho_0 b^2}{4\epsilon} (4\pi b^2) = + \frac{\pi(\epsilon - \varepsilon_0)\rho_0 b^4}{\epsilon}$$
> $$Q_p = Q_{p,\text{vol}} + Q_{p,\text{sup}} = 0$$
> Comprobándose exactamente la conservación de la carga ligada inducida.

#### Parte b) Energía electrostática del sistema

La energía electrostática total almacenada en el campo es:
$$U = \frac{1}{2} \iiint_{\text{todo el espacio}} \vec{D} \cdot \vec{E}\,dV$$

Separando la integral en la región interior ($0 \le r \le b$) y exterior ($b < r < \infty$), con el elemento de volumen en simetría esférica $dV = 4\pi r^2 dr$:
$$U = \frac{1}{2} \int_0^b D(r) E(r) \cdot 4\pi r^2\,dr + \frac{1}{2} \int_b^\infty D(r) E(r) \cdot 4\pi r^2\,dr$$

- **Integral interior ($0 \le r \le b$):**
  $$D(r) E(r) = \left(\frac{\rho_0 r^2}{4}\right)\left(\frac{\rho_0 r^2}{4\epsilon}\right) = \frac{\rho_0^2 r^4}{16\epsilon}$$
  $$U_{\text{int}} = 2\pi \int_0^b \frac{\rho_0^2 r^4}{16\epsilon} r^2\,dr = \frac{2\pi \rho_0^2}{16\epsilon} \int_0^b r^6\,dr = \frac{\pi \rho_0^2}{8\epsilon} \left[\frac{b^7}{7}\right] = \frac{\pi \rho_0^2 b^7}{56\epsilon}$$

- **Integral exterior ($b < r < \infty$):**
  $$D(r) E(r) = \left(\frac{\rho_0 b^4}{4r^2}\right)\left(\frac{\rho_0 b^4}{4\varepsilon_0 r^2}\right) = \frac{\rho_0^2 b^8}{16\varepsilon_0 r^4}$$
  $$U_{\text{ext}} = 2\pi \int_b^\infty \frac{\rho_0^2 b^8}{16\varepsilon_0 r^4} r^2\,dr = \frac{2\pi \rho_0^2 b^8}{16\varepsilon_0} \int_b^\infty \frac{dr}{r^2} = \frac{\pi \rho_0^2 b^8}{8\varepsilon_0} \left[-\frac{1}{r}\right]_b^\infty = \frac{\pi \rho_0^2 b^8}{8\varepsilon_0} \left(0 + \frac{1}{b}\right) = \frac{\pi \rho_0^2 b^7}{8\varepsilon_0}$$

Sumando ambas contribuciones:
$$U = U_{\text{int}} + U_{\text{ext}} = \frac{\pi \rho_0^2 b^7}{8} \left(\frac{1}{7\epsilon} + \frac{1}{\varepsilon_0}\right)$$

$$\boxed{U = \frac{\pi \rho_0^2 b^7}{8} \left(\frac{1}{7\epsilon} + \frac{1}{\varepsilon_0}\right)}$$

**Verificación:**
- **Unidades:** $[\rho_0] = \text{C}/\text{m}^4$, $[\rho_0^2] = \text{C}^2/\text{m}^8$. Con $[b^7] = \text{m}^7$ y $[1/\varepsilon_0] = \text{N}\cdot\text{m}^2/\text{C}^2$:
  $$[\rho_0^2 b^7 / \varepsilon_0] = \frac{\text{C}^2}{\text{m}^8} \cdot \text{m}^7 \cdot \frac{\text{N}\cdot\text{m}^2}{\text{C}^2} = \text{N}\cdot\text{m} = \text{J}$$
  lo que confirma unidades de energía.
- **Límite de vacío:** Si $\epsilon \to \varepsilon_0$, el factor entre paréntesis se reduce a $\frac{1}{7\varepsilon_0} + \frac{1}{\varepsilon_0} = \frac{8}{7\varepsilon_0}$, dando $U = \frac{\pi \rho_0^2 b^7}{7\varepsilon_0}$, que coincide exactamente con la energía de una distribución de carga en vacío $\rho = \rho_0 r$.

---

## Resumen de resultados

| Problema / Inciso | Descripción | Resultado final |
| :--- | :--- | :--- |
| **Problema 1 a)** | Desplazamiento eléctrico $\vec{D}(r)$ | $\vec{D}(r) = \begin{cases} - \dfrac{V_0 \epsilon_1 \epsilon_2}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)}\dfrac{1}{r}\,\hat{r} & a < r < c \\ 0 & r < a \text{ o } r > c \end{cases}$ |
| **Problema 1 b)** | Campo eléctrico $\vec{E}(r)$ | $\vec{E}(r) = \begin{cases} - \dfrac{V_0 \epsilon_2}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)}\dfrac{1}{r}\,\hat{r} & a < r < b \\[1ex] - \dfrac{V_0 \epsilon_1}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)}\dfrac{1}{r}\,\hat{r} & b < r < c \\[1ex] 0 & r < a \text{ o } r > c \end{cases}$ |
| **Problema 1 c)** | Vector polarización $\vec{P}(r)$ | $\vec{P}(r) = \begin{cases} - \dfrac{V_0(\epsilon_1-\varepsilon_0)\epsilon_2}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)}\dfrac{1}{r}\,\hat{r} & a < r < b \\[1ex] - \dfrac{V_0(\epsilon_2-\varepsilon_0)\epsilon_1}{\epsilon_2 \ln(b/a) + \epsilon_1 \ln(c/b)}\dfrac{1}{r}\,\hat{r} & b < r < c \\[1ex] 0 & r < a \text{ o } r > c \end{cases}$ |
| **Problema 2 a)** | Capacitancia del cable coaxial de dos dieléctricos | $C = \dfrac{2\pi \varepsilon_0 L \kappa_1 \kappa_2}{\kappa_2 \ln(2) + \kappa_1 \ln(3/2)}$ |
| **Problema 2 b)** | Carga en conductor macizo con batería de $12\text{ V}$ | $Q_+ = \dfrac{24\pi \varepsilon_0 L \kappa_1 \kappa_2}{\kappa_2 \ln(2) + \kappa_1 \ln(3/2)} \text{ [C]}$ |
| **Problema 2 c)** | Energía almacenada con batería de $12\text{ V}$ | $U = \dfrac{144\pi \varepsilon_0 L \kappa_1 \kappa_2}{\kappa_2 \ln(2) + \kappa_1 \ln(3/2)} \text{ [J]}$ |
| **Problema 3 a)** | Densidad de polarización volumétrica $\rho_p$ | $\rho_p(r) = -\dfrac{(\epsilon - \varepsilon_0)\rho_0 r}{\epsilon} \quad (0 < r < b)$ |
| **Problema 3 a)** | Densidad de polarización superficial $\sigma_p$ | $\sigma_p = \dfrac{(\epsilon - \varepsilon_0)\rho_0 b^2}{4\epsilon} \quad (r = b)$ |
| **Problema 3 b)** | Energía electrostática del sistema | $U = \dfrac{\pi \rho_0^2 b^7}{8}\left(\dfrac{1}{7\epsilon} + \dfrac{1}{\varepsilon_0}\right)$ |
