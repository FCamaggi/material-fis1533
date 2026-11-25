# Ayudantía 13 — Dieléctricos y Ley de Gauss

> Clases relacionadas: [Clase 03 - Distribuciones continuas y Gauss](../../Clases/markdown/Clase%2003%20-%20Distribuciones%20continuas%20y%20Gauss.md), [Clase 07 - Dieléctricos](../../Clases/markdown/Clase%2007%20-%20Diel%C3%A9ctricos.md)

---

## Problema 1

Una esfera conductora de radio $r_0$ tiene una carga $Q$. La esfera es rodeada por una cáscara no conductora, concéntrica, de radio interno $r_i > r_0$ y radio externo $r_e$, y de constante dieléctrica relativa $\kappa = \varepsilon/\varepsilon_0$. El sistema se encuentra aislado de otros cuerpos.

a) Encuentre el campo eléctrico en todo el espacio.  
b) Calcule el potencial eléctrico de la esfera conductora relativo al potencial cero en el infinito.  
c) Calcule las densidades de carga superficial de polarización en las superficies interna y externa del dieléctrico.

> **[Figura]:** Tres regiones esféricas concéntricas centradas en el origen:
> - Una esfera conductora maciza central de radio $r_0$ (sombreada en color salmón/naranja), portadora de una carga libre neta $Q$.
> - Una capa intermedia de vacío comprendida entre los radios $r_0$ y $r_i$.
> - Una cáscara esférica dieléctrica concéntrica (sombreada en celeste) con radio interior $r_i$ y radio exterior $r_e$, caracterizada por su constante dieléctrica relativa $\kappa = \varepsilon/\varepsilon_0$.
> - Más allá de la superficie exterior de radio $r_e$, se extiende el espacio libre exterior (vacío con permitividad $\varepsilon_0$).

### Solución

**Idea:** La simetría esférica permite aplicar la ley de Gauss para el vector desplazamiento eléctrico $\vec{D}$ con una superficie gaussiana esférica concéntrica de radio $r$, ya que el flujo de $\vec{D}$ depende exclusivamente de la carga libre encerrada $Q_{\text{libre}}$. A partir de las relaciones constitutivas $\vec{D} = \varepsilon_0 \vec{E}$ (en el vacío) y $\vec{D} = \varepsilon \vec{E} = \kappa \varepsilon_0 \vec{E}$ (en el dieléctrico lineal e isótropo), se deduce el campo eléctrico $\vec{E}$ en todas las zonas. El potencial se halla integrando el campo desde el infinito hasta $r_0$, y las densidades superficiales de polarización mediante la proyección del vector polarización $\vec{P}$ sobre la normal unitaria saliente del dieléctrico ($\sigma_p = \vec{P} \cdot \hat{n}$).

#### a) Campo eléctrico en todo el espacio

Por simetría esférica, los vectores $\vec{D}$, $\vec{E}$ y $\vec{P}$ son puramente radiales y sus magnitudes dependen exclusivamente de la coordenada radial $r$:
$$\vec{D} = D(r)\,\hat{r}, \qquad \vec{E} = E(r)\,\hat{r}$$

Tomando como superficie gaussiana $S$ una esfera concéntrica de radio $r$:
$$\oint_{S} \vec{D} \cdot d\vec{A} = D(r) \iint_{S} dA = D(r)(4\pi r^2) = Q_{\text{libre, enc}}$$

Analizamos cada región del espacio:

1. **Región interior del conductor ($r < r_0$):**  
   En equilibrio electrostático, el campo eléctrico en el interior de cualquier material conductor es idénticamente nulo, y toda la carga libre $Q$ reside en su superficie $r = r_0$:
   $$\vec{E} = \vec{0}$$

2. **Región de vacío entre el conductor y el dieléctrico ($r_0 < r < r_i$):**  
   La única carga libre encerrada es la carga $Q$ de la esfera conductora:
   $$D(r)(4\pi r^2) = Q \implies \vec{D}(r) = \frac{Q}{4\pi r^2}\,\hat{r}$$
   En el vacío, $\vec{D} = \varepsilon_0 \vec{E}$, por lo que:
   $$\vec{E}(r) = \frac{Q}{4\pi\varepsilon_0 r^2}\,\hat{r}$$

3. **Región en el interior del dieléctrico ($r_i < r < r_e$):**  
   El dieléctrico no posee cargas libres en su volumen. Por lo tanto, la carga libre encerrada sigue siendo exclusivamente $Q_{\text{libre, enc}} = Q$:
   $$D(r)(4\pi r^2) = Q \implies \vec{D}(r) = \frac{Q}{4\pi r^2}\,\hat{r}$$
   En un dieléctrico lineal, homogéneo e isótropo, la relación constitutiva es $\vec{D} = \varepsilon \vec{E} = \kappa \varepsilon_0 \vec{E}$. En consecuencia:
   $$\vec{E}(r) = \frac{Q}{4\pi\varepsilon r^2}\,\hat{r} = \frac{Q}{4\pi\kappa\varepsilon_0 r^2}\,\hat{r}$$

4. **Región exterior al dieléctrico ($r > r_e$):**  
   La superficie gaussiana encierra al conductor y al dieléctrico completo (que es globalmente neutro). La carga libre total encerrada es $Q$:
   $$D(r)(4\pi r^2) = Q \implies \vec{D}(r) = \frac{Q}{4\pi r^2}\,\hat{r}$$
   Como el medio exterior es vacío ($\vec{D} = \varepsilon_0 \vec{E}$):
   $$\vec{E}(r) = \frac{Q}{4\pi\varepsilon_0 r^2}\,\hat{r}$$

En resumen:
$$\boxed{\vec{E}(r) = \begin{cases} \vec{0} & \text{si } r < r_0 \\[2mm] \dfrac{Q}{4\pi\varepsilon_0 r^2}\,\hat{r} & \text{si } r_0 < r < r_i \\[3mm] \dfrac{Q}{4\pi\kappa\varepsilon_0 r^2}\,\hat{r} & \text{si } r_i < r < r_e \\[3mm] \dfrac{Q}{4\pi\varepsilon_0 r^2}\,\hat{r} & \text{si } r > r_e \end{cases}}$$

---

#### b) Potencial eléctrico de la esfera conductora

Fijando la referencia de potencial cero en el infinito ($V(\infty) = 0$), el potencial eléctrico de la superficie del conductor se define como el trabajo por unidad de carga necesario para trasladar una carga de prueba desde el infinito hasta $r = r_0$:
$$V(r_0) = -\int_{\infty}^{r_0} \vec{E} \cdot d\vec{r} = \int_{r_0}^{\infty} E(r)\,dr$$

Descomponiendo la integral en los tres intervalos donde el campo es no nulo:
$$V(r_0) = \int_{r_0}^{r_i} E(r)\,dr + \int_{r_i}^{r_e} E(r)\,dr + \int_{r_e}^{\infty} E(r)\,dr$$

Sustituyendo los campos de cada región:
$$V(r_0) = \int_{r_0}^{r_i} \frac{Q}{4\pi\varepsilon_0 r^2}\,dr + \int_{r_i}^{r_e} \frac{Q}{4\pi\kappa\varepsilon_0 r^2}\,dr + \int_{r_e}^{\infty} \frac{Q}{4\pi\varepsilon_0 r^2}\,dr$$

Evaluando cada una de las integrales inmediatas ($\int \frac{dr}{r^2} = -\frac{1}{r}$):
$$\int_{r_0}^{r_i} \frac{dr}{r^2} = \left[ -\frac{1}{r} \right]_{r_0}^{r_i} = \frac{1}{r_0} - \frac{1}{r_i}$$
$$\int_{r_i}^{r_e} \frac{dr}{r^2} = \left[ -\frac{1}{r} \right]_{r_i}^{r_e} = \frac{1}{r_i} - \frac{1}{r_e}$$
$$\int_{r_e}^{\infty} \frac{dr}{r^2} = \left[ -\frac{1}{r} \right]_{r_e}^{\infty} = \frac{1}{r_e} - 0 = \frac{1}{r_e}$$

Reemplazando:
$$V(r_0) = \frac{Q}{4\pi\varepsilon_0}\left(\frac{1}{r_0} - \frac{1}{r_i}\right) + \frac{Q}{4\pi\kappa\varepsilon_0}\left(\frac{1}{r_i} - \frac{1}{r_e}\right) + \frac{Q}{4\pi\varepsilon_0}\left(\frac{1}{r_e}\right)$$

Agrupando los términos en común:
$$V(r_0) = \frac{Q}{4\pi\varepsilon_0 r_0} - \frac{Q}{4\pi\varepsilon_0 r_i} + \frac{Q}{4\pi\kappa\varepsilon_0 r_i} - \frac{Q}{4\pi\kappa\varepsilon_0 r_e} + \frac{Q}{4\pi\varepsilon_0 r_e}$$
$$V(r_0) = \frac{Q}{4\pi\varepsilon_0 r_0} + \frac{Q}{4\pi\varepsilon_0}\left(1 - \frac{1}{\kappa}\right)\frac{1}{r_e} - \frac{Q}{4\pi\varepsilon_0}\left(1 - \frac{1}{\kappa}\right)\frac{1}{r_i}$$
$$V(r_0) = \frac{Q}{4\pi\varepsilon_0 r_0} + \frac{Q(\kappa - 1)}{4\pi\kappa\varepsilon_0}\left(\frac{1}{r_e} - \frac{1}{r_i}\right)$$

$$\boxed{V(r_0) = \frac{Q}{4\pi\varepsilon_0 r_0} + \frac{Q}{4\pi\kappa\varepsilon_0}(\kappa - 1)\left(\frac{1}{r_e} - \frac{1}{r_i}\right)}$$

> **Nota:** Como $r_e > r_i$, la diferencia $\left(\frac{1}{r_e} - \frac{1}{r_i}\right)$ es estrictamente negativa. Esto implica que la presencia del cascarón dieléctrico ($\kappa > 1$) reduce el potencial de la esfera con respecto al caso en que solo existiera vacío ($V_{\text{vacío}} = \frac{Q}{4\pi\varepsilon_0 r_0}$), debido a la disminución del campo eléctrico en el interior del dieléctrico por la polarización de la materia.

---

#### c) Densidades de carga superficial de polarización

El vector polarización $\vec{P}$ en el medio dieléctrico lineal ($r_i < r < r_e$) se relaciona con el desplazamiento y el campo eléctrico mediante:
$$\vec{P} = \vec{D} - \varepsilon_0 \vec{E}$$

Sustituyendo $\vec{D} = \frac{Q}{4\pi r^2}\,\hat{r}$ y $\vec{E} = \frac{Q}{4\pi\kappa\varepsilon_0 r^2}\,\hat{r}$:
$$\vec{P}(r) = \frac{Q}{4\pi r^2}\,\hat{r} - \varepsilon_0 \left(\frac{Q}{4\pi\kappa\varepsilon_0 r^2}\,\hat{r}\right) = \frac{Q}{4\pi r^2}\left(1 - \frac{1}{\kappa}\right)\hat{r} = \frac{Q(\kappa - 1)}{4\pi\kappa r^2}\,\hat{r}$$

La densidad superficial de carga ligada o de polarización está dada por:
$$\sigma_p = \vec{P} \cdot \hat{n}$$
donde $\hat{n}$ es el vector unitario normal a la superficie que **apunta hacia afuera del dieléctrico**.

1. **En la superficie interna ($r = r_i$):**  
   La normal que sale del dieléctrico apunta hacia el centro de curvatura (hacia el interior de la cavidad hueca):
   $$\hat{n} = -\hat{r}$$
   Por tanto:
   $$\sigma_p(r_i) = \vec{P}(r_i) \cdot (-\hat{r}) = \left[ \frac{Q}{4\pi r_i^2}\left(1 - \frac{1}{\kappa}\right)\hat{r} \right] \cdot (-\hat{r}) = -\frac{Q}{4\pi r_i^2}\left(1 - \frac{1}{\kappa}\right)$$

   $$\boxed{\sigma_p(r_i) = -\frac{Q}{4\pi r_i^2}\left(1 - \frac{1}{\kappa}\right) = -\frac{Q(\kappa - 1)}{4\pi\kappa r_i^2}}$$

2. **En la superficie externa ($r = r_e$):**  
   La normal que sale del dieléctrico hacia el espacio exterior apunta radialmente hacia afuera:
   $$\hat{n} = +\hat{r}$$
   Por tanto:
   $$\sigma_p(r_e) = \vec{P}(r_e) \cdot (+\hat{r}) = \left[ \frac{Q}{4\pi r_e^2}\left(1 - \frac{1}{\kappa}\right)\hat{r} \right] \cdot (+\hat{r}) = +\frac{Q}{4\pi r_e^2}\left(1 - \frac{1}{\kappa}\right)$$

   $$\boxed{\sigma_p(r_e) = +\frac{Q}{4\pi r_e^2}\left(1 - \frac{1}{\kappa}\right) = +\frac{Q(\kappa - 1)}{4\pi\kappa r_e^2}}$$

**Verificación:**
- **Carga de polarización total:** Integrando las densidades sobre cada superficie esférica:
  $$Q_{p,\text{int}} = \sigma_p(r_i)(4\pi r_i^2) = -Q\left(1 - \frac{1}{\kappa}\right)$$
  $$Q_{p,\text{ext}} = \sigma_p(r_e)(4\pi r_e^2) = +Q\left(1 - \frac{1}{\kappa}\right)$$
  La carga volumétrica de polarización es nula:
  $$\rho_p = -\nabla \cdot \vec{P} = -\frac{1}{r^2}\frac{\partial}{\partial r}\left(r^2 \cdot \frac{C}{r^2}\right) = 0$$
  La carga total inducida ligada en el dieléctrico es $Q_{p,\text{total}} = Q_{p,\text{int}} + Q_{p,\text{ext}} = 0$, conservando la neutralidad de carga del aislante.

---

## Problema 2

Se considera un cilindro no conductor de radio $a$ y longitud infinita, con densidad volumétrica de carga constante y conocida $\rho_0$. Este cilindro está rodeado por un cascarón cilíndrico no conductor de radio interno $a$, radio externo $b$ y longitud infinita, con densidad volumétrica de carga $-\rho_0$. Entre ambas distribuciones se inserta, a $r = a$, un cascarón cilíndrico conductor de espesor despreciable y longitud infinita, que separa las cargas del cilindro y del cascarón externo. Suponga que el cascarón conductor posee una distribución de carga superficial homogénea $\sigma_S$, que es desconocida.

a) Calcule el valor que debe tener la densidad superficial $\sigma_S$ para que el campo eléctrico sea nulo en el exterior del cilindro.  
b) Encuentre el campo eléctrico en todo el espacio.  
c) Calcule la diferencia de potencial eléctrico entre $r = 0$ y $r = b$.

> **[Figura]:** Sistema coaxial infinito compuesto por tres medios cilíndricos concéntricos de eje común vertical:
> - Núcleo interior cilíndrico macizo de radio $a$, con densidad de carga volumétrica uniforme $\rho_0$.
> - En la interfaz $r = a$, un cascarón conductor delgado de espesor despreciable con densidad superficial de carga uniforme $\sigma_s$.
> - Cascarón cilíndrico exterior que abarca desde el radio interno $a$ hasta el radio externo $b$, con densidad volumétrica uniforme $-\rho_0$.
> - Por fuera ($r > b$), se encuentra el vacío exterior.

### Solución

**Idea:** Debido a la simetría traslacional y azimutal del cilindro de longitud infinita, el campo eléctrico depende exclusivamente de la coordenada radial $r$ y apunta en dirección $\hat{r}$. Aplicando la ley de Gauss sobre superficies gaussianas cilíndricas coaxiales de radio $r$ y altura $h$, el campo es proporcional a la carga libre neta encerrada por unidad de longitud. La condición de anulación del campo exterior fija el valor de $\sigma_s$. Luego, la diferencia de potencial se calcula integrando el campo $\vec{E}$ entre $r = 0$ y $r = b$.

#### a) Determinación de $\sigma_S$ para campo exterior nulo

Consideremos una superficie gaussiana cilíndrica de radio $r > b$ y altura $h$, coaxial con el sistema. Por simetría cilíndrica:
$$\vec{E}(r) = E(r)\,\hat{r}$$
El flujo a través de las bases superior e inferior es cero ($\vec{E} \perp \hat{z}$), y a través de la cara lateral es:
$$\oint_{S} \vec{E} \cdot d\vec{A} = E(r)(2\pi r h) = \frac{Q_{\text{enc}}}{\varepsilon_0}$$

Para que el campo eléctrico sea idénticamente cero en todo el exterior ($r > b$), se requiere necesariamente que la carga total neta encerrada en una longitud arbitraria $h$ sea nula:
$$Q_{\text{enc}} = 0$$

Calculamos las tres contribuciones a la carga encerrada para $r \ge b$:
1. **Cilindro interior no conductor ($0 \le r' \le a$):**
   $$Q_1 = \int_{0}^{h} dz \int_{0}^{2\pi} d\phi \int_{0}^{a} \rho_0 r'\,dr' = \rho_0 \pi a^2 h$$

2. **Cascarón conductor en la interfaz ($r' = a$):**
   $$Q_2 = \sigma_s (2\pi a h)$$

3. **Cascarón exterior no conductor ($a \le r' \le b$):**
   $$Q_3 = \int_{0}^{h} dz \int_{0}^{2\pi} d\phi \int_{a}^{b} (-\rho_0) r'\,dr' = -\rho_0 \pi (b^2 - a^2) h$$

La carga total encerrada es la suma de las tres:
$$Q_{\text{enc}} = Q_1 + Q_2 + Q_3 = \pi h \Big[ \rho_0 a^2 + 2 a \sigma_s - \rho_0 (b^2 - a^2) \Big] = \pi h \Big[ \rho_0 (2a^2 - b^2) + 2 a \sigma_s \Big]$$

Imponiendo $Q_{\text{enc}} = 0$:
$$\rho_0 (2a^2 - b^2) + 2 a \sigma_s = 0$$

Despejando $\sigma_s$:
$$2 a \sigma_s = \rho_0 (b^2 - 2a^2) \implies \sigma_s = \frac{\rho_0 (b^2 - 2a^2)}{2a}$$

$$\boxed{\sigma_s = \frac{\rho_0 (b^2 - 2a^2)}{2a}}$$

---

#### b) Campo eléctrico en todo el espacio

Con una superficie gaussiana cilíndrica de radio $r$ y longitud $h$:
$$2\pi r h E(r) = \frac{Q_{\text{enc}}(r)}{\varepsilon_0} \implies E(r) = \frac{Q_{\text{enc}}(r)}{2\pi\varepsilon_0 r h}$$

Evaluamos las distintas regiones:

1. **Región interior ($r < a$):**  
   Solo encierra una porción del núcleo cilíndrico de radio $r$:
   $$Q_{\text{enc}}(r) = \rho_0 (\pi r^2) h$$
   Sustituyendo:
   $$2\pi r h E(r) = \frac{\rho_0 \pi r^2 h}{\varepsilon_0} \implies E(r) = \frac{\rho_0 r}{2\varepsilon_0}$$
   $$\vec{E}(r) = \frac{\rho_0 r}{2\varepsilon_0}\,\hat{r}$$

2. **Región intermedia ($a < r < b$):**  
   Encierra todo el cilindro interior, la carga superficial en $r = a$, y una parte del cascarón exterior entre $a$ y $r$:
   $$Q_{\text{enc}}(r) = \rho_0 \pi a^2 h + \sigma_s (2\pi a h) + \int_{a}^{r} (-\rho_0)(2\pi r' h)\,dr'$$
   $$Q_{\text{enc}}(r) = \rho_0 \pi a^2 h + \sigma_s (2\pi a h) - \rho_0 \pi (r^2 - a^2) h = \pi h \Big[ \rho_0 (2a^2 - r^2) + 2 a \sigma_s \Big]$$

   Sustituyendo el valor obtenido para $\sigma_s$, es decir, $2 a \sigma_s = \rho_0 (b^2 - 2a^2)$:
   $$Q_{\text{enc}}(r) = \pi h \Big[ \rho_0 (2a^2 - r^2) + \rho_0 (b^2 - 2a^2) \Big] = \rho_0 \pi (b^2 - r^2) h$$

   Aplicando Gauss:
   $$2\pi r h E(r) = \frac{\rho_0 \pi (b^2 - r^2) h}{\varepsilon_0} \implies E(r) = \frac{\rho_0 (b^2 - r^2)}{2\varepsilon_0 r}$$
   $$\vec{E}(r) = \frac{\rho_0 (b^2 - r^2)}{2\varepsilon_0 r}\,\hat{r}$$

3. **Región exterior ($r > b$):**  
   Por la elección de $\sigma_s$ efectuada en la parte a), la carga neta total encerrada es cero:
   $$\vec{E}(r) = \vec{0}$$

En resumen:
$$\boxed{\vec{E}(r) = \begin{cases} \dfrac{\rho_0 r}{2\varepsilon_0}\,\hat{r} & \text{si } r < a \\[3mm] \dfrac{\rho_0 (b^2 - r^2)}{2\varepsilon_0 r}\,\hat{r} & \text{si } a < r < b \\[3mm] \vec{0} & \text{si } r > b \end{cases}}$$

---

#### c) Diferencia de potencial eléctrico entre $r = 0$ y $r = b$

La diferencia de potencial se define como:
$$V(0) - V(b) = -\int_{b}^{0} \vec{E} \cdot d\vec{r} = \int_{0}^{b} E(r)\,dr$$

Descomponiendo el camino de integración radial en los dos tramos:
$$V(0) - V(b) = \int_{0}^{a} E(r)\,dr + \int_{a}^{b} E(r)\,dr = \int_{0}^{a} \frac{\rho_0 r}{2\varepsilon_0}\,dr + \int_{a}^{b} \frac{\rho_0 (b^2 - r^2)}{2\varepsilon_0 r}\,dr$$

Calculamos cada término por separado:

- **Primer tramo ($0 \le r \le a$):**
  $$\int_{0}^{a} \frac{\rho_0 r}{2\varepsilon_0}\,dr = \frac{\rho_0}{2\varepsilon_0} \left[ \frac{r^2}{2} \right]_{0}^{a} = \frac{\rho_0 a^2}{4\varepsilon_0}$$

- **Segundo tramo ($a \le r \le b$):**
  $$\int_{a}^{b} \frac{\rho_0 (b^2 - r^2)}{2\varepsilon_0 r}\,dr = \frac{\rho_0}{2\varepsilon_0} \left[ b^2 \int_{a}^{b} \frac{dr}{r} - \int_{a}^{b} r\,dr \right] = \frac{\rho_0}{2\varepsilon_0} \left[ b^2 \ln\left(\frac{b}{a}\right) - \left( \frac{b^2 - a^2}{2} \right) \right]$$

Sumando ambas contribuciones:
$$V(0) - V(b) = \frac{\rho_0 a^2}{4\varepsilon_0} + \frac{\rho_0 b^2}{2\varepsilon_0} \ln\left(\frac{b}{a}\right) - \frac{\rho_0(b^2 - a^2)}{4\varepsilon_0}$$

Agrupando los términos polinomiales:
$$\frac{\rho_0 a^2}{4\varepsilon_0} - \frac{\rho_0(b^2 - a^2)}{4\varepsilon_0} = \frac{\rho_0 (a^2 - b^2 + a^2)}{4\varepsilon_0} = \frac{\rho_0 (2a^2 - b^2)}{4\varepsilon_0}$$

Por lo tanto:
$$V(0) - V(b) = \frac{\rho_0}{4\varepsilon_0} (2a^2 - b^2) + \frac{\rho_0 b^2}{2\varepsilon_0} \ln\left(\frac{b}{a}\right)$$

$$\boxed{V(0) - V(b) = \frac{\rho_0}{4\varepsilon_0} (2a^2 - b^2) + \frac{\rho_0 b^2}{2\varepsilon_0} \ln\left(\frac{b}{a}\right)}$$

**Verificación:**
- **Unidades:**
  $$[V] = \frac{[\rho_0][a^2]}{[\varepsilon_0]} = \frac{(\text{C/m}^3)\cdot \text{m}^2}{\text{C}^2/(\text{N}\cdot\text{m}^2)} = \frac{\text{C/m}}{\text{C}^2/(\text{J}\cdot\text{m})} = \frac{\text{J}}{\text{C}} = \text{V}$$
  La dimensión es volt (V), físicamente exacta.
- **Continuidad de $\vec{E}$ en la frontera $r = b$:**
  Evaluando el campo para $r \to b^-$ en la región intermedia:
  $$E(b^-) = \frac{\rho_0 (b^2 - b^2)}{2\varepsilon_0 b} = 0$$
  lo cual coincide perfectamente con el valor nulo exterior ($E(b^+) = 0$).
- **Discontinuidad en la superficie conductora $r = a$:**
  $$E(a^+) - E(a^-) = \frac{\rho_0 (b^2 - a^2)}{2\varepsilon_0 a} - \frac{\rho_0 a}{2\varepsilon_0} = \frac{\rho_0 (b^2 - 2a^2)}{2\varepsilon_0 a} = \frac{\sigma_s}{\varepsilon_0}$$
  Se cumple con total exactitud la condición de frontera electrostática $\Delta E_n = \frac{\sigma_s}{\varepsilon_0}$.

---

## Resumen de resultados

| Problema | Inciso / Magnitud | Resultado final |
| :--- | :--- | :--- |
| **Problema 1** | **a)** Campo eléctrico $\vec{E}(r)$ en todo el espacio | $\vec{E}(r) = \begin{cases} \vec{0} & r < r_0 \\ \dfrac{Q}{4\pi\varepsilon_0 r^2}\,\hat{r} & r_0 < r < r_i \\ \dfrac{Q}{4\pi\kappa\varepsilon_0 r^2}\,\hat{r} & r_i < r < r_e \\ \dfrac{Q}{4\pi\varepsilon_0 r^2}\,\hat{r} & r > r_e \end{cases}$ |
| | **b)** Potencial de la esfera conductora $V(r_0)$ | $V(r_0) = \dfrac{Q}{4\pi\varepsilon_0 r_0} + \dfrac{Q}{4\pi\kappa\varepsilon_0}(\kappa - 1)\left(\dfrac{1}{r_e} - \dfrac{1}{r_i}\right)$ |
| | **c)** Densidades superficiales de polarización $\sigma_p$ | $\sigma_p(r_i) = -\dfrac{Q(\kappa - 1)}{4\pi\kappa r_i^2}$<br>$\sigma_p(r_e) = +\dfrac{Q(\kappa - 1)}{4\pi\kappa r_e^2}$ |
| **Problema 2** | **a)** Densidad superficial $\sigma_S$ para campo nulo exterior | $\sigma_S = \dfrac{\rho_0 (b^2 - 2a^2)}{2a}$ |
| | **b)** Campo eléctrico $\vec{E}(r)$ en todo el espacio | $\vec{E}(r) = \begin{cases} \dfrac{\rho_0 r}{2\varepsilon_0}\,\hat{r} & r < a \\ \dfrac{\rho_0 (b^2 - r^2)}{2\varepsilon_0 r}\,\hat{r} & a < r < b \\ \vec{0} & r > b \end{cases}$ |
| | **c)** Diferencia de potencial $V(0) - V(b)$ | $V(0) - V(b) = \dfrac{\rho_0}{4\varepsilon_0}(2a^2 - b^2) + \dfrac{\rho_0 b^2}{2\varepsilon_0}\ln\left(\dfrac{b}{a}\right)$ |
