---
title: "Ondas Electromagnéticas"
source_pdf: "Electro/2025-2/Clases/Tema5_OndasEM.pdf (+ resumen)"
pages: 54
extraction_mode: "visual_latex_transcription"
---

# Ondas Electromagnéticas

## Ecuaciones de Maxwell

Hasta mediados del siglo XIX, las leyes conocidas que describían los campos eléctricos y magnéticos eran cuatro ecuaciones, expresadas en forma diferencial como:

$$\nabla \cdot \vec{E} = \frac{\rho}{\epsilon_0}, \qquad \nabla \cdot \vec{B} = 0$$

$$\nabla \times \vec{E} = -\frac{\partial \vec{B}}{\partial t}, \qquad \nabla \times \vec{B} = \mu_0 \vec{J}$$

En forma integral, estas mismas leyes correspondían a:

- **Ley de Gauss:**
  $$\oint \vec{E} \cdot d\vec{A} = \frac{Q_{\text{enc}}}{\epsilon_0}$$
- **Ley de Gauss del magnetismo:**
  $$\oint \vec{B} \cdot d\vec{A} = 0$$
- **Ley de Ampère:**
  $$\oint \vec{B} \cdot d\vec{l} = \mu_0 I_{\text{enc}}$$
- **Ley de Faraday:**
  $$\oint \vec{E} \cdot d\vec{l} = -\frac{d\Phi_B}{dt}$$

## Ley de Ampère generalizada y corriente de desplazamiento

### Inconsistencia de la ley de Ampère sin el término de desplazamiento

Las ecuaciones anteriores resultan matemáticamente inconsistentes para campos variables en el tiempo. Al tomar la divergencia de la ley de Faraday se obtiene una identidad consistente:

$$\nabla \cdot (\nabla \times \vec{E}) = \nabla \cdot \left(-\frac{\partial \vec{B}}{\partial t}\right) = -\frac{\partial}{\partial t}(\nabla \cdot \vec{B})$$

Dado que la divergencia de todo rotor es nula ($\nabla \cdot (\nabla \times \vec{E}) = 0$) y $\nabla \cdot \vec{B} = 0$, ambos miembros se anulan ($0 = 0$).

Sin embargo, al aplicar la divergencia a la ley de Ampère estática se obtiene:

$$\nabla \cdot (\nabla \times \vec{B}) = \mu_0 (\nabla \cdot \vec{J})$$

El miembro izquierdo es idénticamente nulo ($\nabla \cdot (\nabla \times \vec{B}) = 0$), mientras que el miembro derecho es $\mu_0(\nabla \cdot \vec{J}) \neq 0$, excepto para corrientes estacionarias (por la ecuación de continuidad $\nabla \cdot \vec{J} = -\partial\rho/\partial t$). Por lo tanto, la ley de Ampère debe incluir un término adicional para describir campos magnéticos variables en el tiempo.

### Corriente de desplazamiento en un capacitor

Consideremos el proceso de carga de un capacitor de placas paralelas:

- Alambres conductores llevan una corriente de conducción $i_C$ hacia una placa (carga $+Q$) y hacia afuera de la otra (carga $-Q$).
- A medida que la carga $Q$ aumenta, el campo eléctrico $\vec{E}$ entre las placas también aumenta.
- La notación $i_C$ indica **corriente de conducción** para distinguirla de la nueva clase de corriente que aparecerá.

> **[Figura]:** Diagrama de un capacitor de placas circulares paralelas durante su carga. Un alambre horizontal lleva corriente $i_C$ hacia la izquierda-derecha entrando en la placa positiva ($+Q$) y saliendo de la placa negativa ($-Q$); entre ambas placas el campo eléctrico $\vec{E}$ es uniforme y apunta de izquierda a derecha. Alrededor del alambre izquierdo se traza una trayectoria circular cerrada para la ley de Ampère con elemento de arco $d\vec{l}$ (dirigido según la regla de la mano derecha respecto de $i_C$). Esta curva delimita dos superficies distintas: una **superficie plana** circular perpendicular al alambre (atravesada por $i_C$) y una **superficie abombada** hacia la derecha que pasa por el espacio entre las placas (no atravesada por el alambre conductor, sino por las líneas de $\vec{E}$).

Aplicando la ley de Ampère original a la trayectoria circular:

$$\oint \vec{B} \cdot d\vec{l} = \mu_0 I_{\text{enc}}$$

Si se elige la superficie plana delimitada por el círculo, la corriente encerrada es $i_C$. Pero la superficie abombada hacia la derecha está delimitada por el mismo círculo y la corriente de conducción a través de ella es cero.

A medida que el capacitor se carga, tanto el campo eléctrico como el flujo eléctrico $\Phi_E$ a través de la superficie abombada aumentan. La carga instantánea $q$ en las placas está dada por:

$$\left.\begin{aligned} q &= CV \\ C &= \frac{\epsilon_0 A}{d} \\ V &= Ed \end{aligned}\right\} \implies q = CV = \frac{\epsilon A}{d}(Ed) = \epsilon E A = \epsilon \Phi_E$$

> **Nota (errata):** En la diapositiva se escribe $V$ en minúscula ($v$) para la diferencia de potencial y se pasa de $\epsilon_0$ en la capacitancia $C = \epsilon_0 A/d$ a $\epsilon$ en la expresión final $q = \epsilon\Phi_E$ (en el vacío, $\epsilon = \epsilon_0$).

Derivando respecto del tiempo se obtiene la **corriente de desplazamiento** $i_D$, introducida en 1865 por James Clerk Maxwell (1831–1879):

$$i_D = \epsilon \frac{d\Phi_E}{dt}$$

Con ella se formula la **ley de Ampère generalizada**:

$$\oint \vec{B} \cdot d\vec{l} = \mu_0 (i_C + i_D)_{\text{enc}}$$

De este modo:

- Para la superficie plana, $i_D = 0$ y la corriente encerrada es $i_C$.
- Para la superficie curva (abombada), $i_C = 0$ y la corriente encerrada es $i_D$.
- El valor de $i_C$ en la superficie plana es igual al de $i_D$ en la superficie curva, resolviendo la ambigüedad.

Se define además la **densidad de corriente de desplazamiento**:

$$j_D = \frac{i_D}{A} \implies j_D = \epsilon \frac{dE}{dt}$$

### Campo magnético entre las placas de un capacitor en carga

Si la corriente de desplazamiento desempeña efectivamente ese papel en la ley de Ampère, entonces debe existir un campo magnético en la región comprendida entre las placas mientras el capacitor se está cargando.

> **[Figura]:** Dos placas circulares paralelas de radio $R$ con cargas $+q$ (izquierda) y $-q$ (derecha), alimentadas por un alambre axial con corriente $i_C$ de izquierda a derecha. En el espacio entre placas, las líneas del campo eléctrico $\vec{E}$ son horizontales de izquierda a derecha. Concéntricas al eje hay líneas circulares del campo magnético $\vec{B}$ (que pasan por puntos $a$ arriba y $b$ abajo en una circunferencia de radio $r < R$, y otra circunferencia exterior), orientadas según la regla de la mano derecha alrededor de la dirección de $i_C$ y $\vec{E}$.

**Resolución para $r < R$:**

- *Idea:* La corriente de desplazamiento total entre las placas es igual a la corriente de conducción $i_C$ y se distribuye uniformemente sobre el área $\pi R^2$. Se aplica la ley de Ampère generalizada a una circunferencia concéntrica de radio $r < R$.
- *Desarrollo:* La corriente de desplazamiento encerrada por la circunferencia de radio $r$ es:
  $$i_{D,\text{enc}} = \left(\frac{i_D}{\pi R^2}\right)(\pi r^2) = \frac{r^2}{R^2} i_C$$
  Por simetría axial, la circulación de $\vec{B}$ vale $2\pi r B$, de modo que:
  $$\oint \vec{B} \cdot d\vec{l} = 2\pi r B = \mu_0 \frac{r^2}{R^2} i_C$$
  Despejando $B$:
  $$\boxed{B = \frac{\mu_0}{2\pi}\frac{r}{R^2} i_C \qquad (r < R)}$$
- *Verificación:* En $r = 0$, $B = 0$ por simetría; en $r = R$, $B = \mu_0 i_C / (2\pi R)$, que coincide con el campo de un alambre recto infinito con corriente $i_C$. Al medir el campo magnético en esta región, se comprueba experimentalmente que realmente está presente.

## Ecuaciones de Maxwell completas y en la materia

### Ecuaciones de Maxwell en el vacío

Al incorporar la corriente de desplazamiento de Maxwell, el sistema completo de ecuaciones de Maxwell en el vacío queda expresado en forma diferencial como:

$$\nabla \cdot \vec{E} = \frac{\rho}{\epsilon_0}, \qquad \nabla \cdot \vec{B} = 0$$

$$\nabla \times \vec{E} = -\frac{\partial \vec{B}}{\partial t}, \qquad \nabla \times \vec{B} = \mu_0 \vec{J} + \epsilon_0 \mu_0 \frac{\partial \vec{E}}{\partial t}$$

Y en forma integral como:

- **Ley de Gauss:**
  $$\oint \vec{E} \cdot d\vec{A} = \frac{Q_{\text{enc}}}{\epsilon_0}$$
- **Ley de Gauss del magnetismo:**
  $$\oint \vec{B} \cdot d\vec{A} = 0$$
- **Ley de Ampère-Maxwell:**
  $$\oint \vec{B} \cdot d\vec{l} = \mu_0 \left(i_C + \epsilon_0 \frac{d\Phi_E}{dt}\right)_{\text{enc}}$$
- **Ley de Faraday:**
  $$\oint \vec{E} \cdot d\vec{l} = -\frac{d\Phi_B}{dt}$$

### Ecuaciones de Maxwell en la materia

Cuando se trabaja con materiales sujetos a polarización eléctrica y/o magnética, conviene escribir las ecuaciones en términos de las cargas y corrientes libres y ligadas:

- La polarización eléctrica $\vec{P}$ produce una densidad de carga ligada:
  $$\rho_b = -\nabla \cdot \vec{P}$$
- La magnetización $\vec{M}$ produce una densidad de corriente ligada:
  $$\vec{J}_b = \nabla \times \vec{M}$$
- Si la polarización depende del tiempo, se incluye además una **corriente de polarización**:
  $$\vec{J}_p = \frac{\partial \vec{P}}{\partial t}$$

Por lo tanto, la densidad de carga total y la densidad de corriente total se separan en:

$$\rho = \rho_f + \rho_b = \rho_f - \nabla \cdot \vec{P}$$

$$\vec{J} = \vec{J}_f + \vec{J}_b + \vec{J}_p = \vec{J}_f + \nabla \times \vec{M} + \frac{\partial \vec{P}}{\partial t}$$

Sustituyendo en la ley de Gauss:

$$\nabla \cdot \vec{E} = \frac{1}{\epsilon_0}\left(\rho_f - \nabla \cdot \vec{P}\right) \implies \nabla \cdot \vec{D} = \rho_f$$

donde $\vec{D} = \epsilon_0 \vec{E} + \vec{P}$ es el **vector desplazamiento eléctrico**.

Sustituyendo en la ley de Ampère-Maxwell:

$$\nabla \times \vec{B} = \mu_0 \left(\vec{J}_f + \nabla \times \vec{M} + \frac{\partial \vec{P}}{\partial t}\right) + \epsilon_0 \mu_0 \frac{\partial \vec{E}}{\partial t} \implies \nabla \times \vec{H} = \vec{J}_f + \frac{\partial \vec{D}}{\partial t}$$

donde $\vec{H} = \frac{1}{\mu_0}\vec{B} - \vec{M}$ es el **vector magnético auxiliar**.

En un medio material, las ecuaciones de Maxwell deben suplementarse con **ecuaciones constituyentes** que relacionen $\vec{D}$ y $\vec{H}$ con $\vec{E}$ y $\vec{B}$. En el caso de un **medio lineal**:

$$\vec{P} = \epsilon_0 \chi_e \vec{E} \implies \vec{D} = \epsilon \vec{E}$$

$$\vec{M} = \chi_m \vec{H} \implies \vec{H} = \frac{1}{\mu}\vec{B}$$

donde $\epsilon = \epsilon_0 (1 + \chi_e)$ y $\mu = \mu_0 (1 + \chi_m)$.

> **Nota (errata):** En la diapositiva aparece escrito $\vec{M} = \chi_m \vec{B}$; la relación constitutiva estándar en términos de la susceptibilidad magnética $\chi_m$ es $\vec{M} = \chi_m \vec{H}$, de la cual se obtiene $\vec{B} = \mu_0(\vec{H}+\vec{M}) = \mu_0(1+\chi_m)\vec{H} = \mu\vec{H}$, y por ende $\vec{H} = \frac{1}{\mu}\vec{B}$ con $\mu = \mu_0(1+\chi_m)$.

Comparación entre las ecuaciones de Maxwell en el vacío y en la materia:

| En el vacío | En la materia |
|---|---|
| $\nabla \cdot \vec{E} = \dfrac{\rho}{\epsilon_0}$ | $\nabla \cdot \vec{D} = \rho_f$ |
| $\nabla \cdot \vec{B} = 0$ | $\nabla \cdot \vec{B} = 0$ |
| $\nabla \times \vec{E} = -\dfrac{\partial \vec{B}}{\partial t}$ | $\nabla \times \vec{E} = -\dfrac{\partial \vec{B}}{\partial t}$ |
| $\nabla \times \vec{B} = \mu_0 \vec{J} + \mu_0 \epsilon_0 \dfrac{\partial \vec{E}}{\partial t}$ | $\nabla \times \vec{H} = \vec{J}_f + \dfrac{\partial \vec{D}}{\partial t}$ |

> **Nota (errata):** En la tabla resumen de la diapositiva 16 se omitió el subíndice $f$ en $\rho$ y $\vec{J}$ en la columna "En la materia"; aquí se conserva $\rho_f$ y $\vec{J}_f$ por consistencia con la derivación previa.

## Teorema de Poynting y vector de Poynting

### Densidad de energía electromagnética

El trabajo necesario para ensamblar una distribución de carga estática (contra la repulsión de Coulomb) es:

$$W_e = \frac{\epsilon_0}{2}\int E^2 \, d\tau$$

El trabajo requerido para establecer las corrientes (contra la fuerza electromotriz) es:

$$W_m = \frac{1}{2\mu_0}\int B^2 \, d\tau$$

Esto sugiere que la densidad total de energía por unidad de volumen almacenada en los campos es:

$$u = \frac{1}{2}\left(\epsilon_0 E^2 + \frac{1}{\mu_0} B^2\right)$$

### Deducción del teorema de Poynting

Consideremos una distribución de cargas y corrientes que producen, en un instante $t$, campos eléctrico y magnético. El trabajo realizado por las fuerzas electromagnéticas sobre una carga $q$ que se desplaza $d\vec{l} = \vec{v}\,dt$ en un intervalo $dt$ es:

$$dW = \vec{F} \cdot d\vec{l} = q(\vec{E} + \vec{v} \times \vec{B}) \cdot \vec{v}\,dt = q\vec{E} \cdot \vec{v}\,dt$$

Para una distribución continua en un volumen $\mathcal{V}$, la potencia transferida a las cargas es:

$$\frac{dW}{dt} = \int_{\mathcal{V}} \rho\,d\tau\,(\vec{E} \cdot \vec{v}) = \int_{\mathcal{V}} (\vec{E} \cdot \rho\vec{v})\,d\tau = \int_{\mathcal{V}} (\vec{E} \cdot \vec{J})\,d\tau$$

De la ley de Ampère-Maxwell $\nabla \times \vec{B} = \mu_0 \vec{J} + \epsilon_0 \mu_0 \frac{\partial \vec{E}}{\partial t}$, multiplicando escalarmente por $\vec{E}$:

$$\vec{E} \cdot (\nabla \times \vec{B}) = \mu_0 \vec{E} \cdot \vec{J} + \epsilon_0 \mu_0 \vec{E} \cdot \frac{\partial \vec{E}}{\partial t} \implies \vec{E} \cdot \vec{J} = \frac{1}{\mu_0}\vec{E} \cdot (\nabla \times \vec{B}) - \epsilon_0 \vec{E} \cdot \frac{\partial \vec{E}}{\partial t}$$

Usando la identidad vectorial $\nabla \cdot (\vec{E} \times \vec{B}) = \vec{B} \cdot (\nabla \times \vec{E}) - \vec{E} \cdot (\nabla \times \vec{B})$ junto con la ley de Faraday $\nabla \times \vec{E} = -\frac{\partial \vec{B}}{\partial t}$:

$$\vec{E} \cdot (\nabla \times \vec{B}) = -\vec{B} \cdot \frac{\partial \vec{B}}{\partial t} - \nabla \cdot (\vec{E} \times \vec{B})$$

Además, $\vec{B} \cdot \frac{\partial \vec{B}}{\partial t} = \frac{1}{2}\frac{\partial}{\partial t}(B^2)$ y $\vec{E} \cdot \frac{\partial \vec{E}}{\partial t} = \frac{1}{2}\frac{\partial}{\partial t}(E^2)$, de modo que:

$$\vec{E} \cdot \vec{J} = -\frac{1}{2}\frac{\partial}{\partial t}\left(\epsilon_0 E^2 + \frac{1}{\mu_0}B^2\right) - \frac{1}{\mu_0}\nabla \cdot (\vec{E} \times \vec{B})$$

Integrando sobre el volumen $\mathcal{V}$ y aplicando el teorema de la divergencia sobre la superficie cerrada $\mathcal{S} = \partial\mathcal{V}$:

$$\frac{dW}{dt} = \int_{\mathcal{V}} (\vec{E} \cdot \vec{J})\,d\tau = -\frac{d}{dt}\int_{\mathcal{V}} \frac{1}{2}\left(\epsilon_0 E^2 + \frac{1}{\mu_0}B^2\right)d\tau - \frac{1}{\mu_0}\oint_{\mathcal{S}} (\vec{E} \times \vec{B}) \cdot d\vec{a}$$

El **teorema de Poynting** establece que el trabajo por unidad de tiempo realizado sobre las cargas por la fuerza electromagnética es igual a la disminución de la energía almacenada en los campos electromagnéticos menos la energía que fluye hacia afuera a través de la superficie.

La energía por unidad de tiempo y por unidad de área transportada por los campos se denomina **vector de Poynting**:

$$\vec{S} = \frac{1}{\mu_0}(\vec{E} \times \vec{B})$$

Con $U_{\text{em}} = \int_{\mathcal{V}} u_{\text{em}}\,d\tau$, el teorema de Poynting en forma integral se escribe:

$$\frac{dW}{dt} = -\frac{dU_{\text{em}}}{dt} - \oint_{\mathcal{S}} \vec{S} \cdot d\vec{a}$$

### Forma diferencial del teorema de Poynting

El trabajo realizado sobre las cargas incrementa su energía mecánica:

$$\frac{dW}{dt} = \frac{d}{dt}\int_{\mathcal{V}} u_{\text{mec}}\,d\tau$$

Por lo tanto:

$$\frac{d}{dt}\int_{\mathcal{V}} (u_{\text{mec}} + u_{\text{em}})\,d\tau = -\oint_{\mathcal{S}} \vec{S} \cdot d\vec{a} = -\int_{\mathcal{V}} (\nabla \cdot \vec{S})\,d\tau$$

donde $u_{\text{em}} = \frac{1}{2}\left(\epsilon_0 E^2 + \frac{1}{\mu_0}B^2\right)$ es la densidad de energía del campo electromagnético. De aquí se deduce la **forma diferencial del teorema de Poynting**:

$$\frac{\partial}{\partial t}(u_{\text{mec}} + u_{\text{em}}) = -\nabla \cdot \vec{S}$$

## Ondas electromagnéticas en el vacío

En el vacío libre de cargas y corrientes ($\rho = 0$, $\vec{J} = \vec{0}$), las ecuaciones de Maxwell se reducen a:

$$\nabla \cdot \vec{E} = 0, \qquad \nabla \cdot \vec{B} = 0$$

$$\nabla \times \vec{E} = -\frac{\partial \vec{B}}{\partial t}, \qquad \nabla \times \vec{B} = \epsilon_0 \mu_0 \frac{\partial \vec{E}}{\partial t}$$

Aplicando el rotor a la ley de Faraday y usando la identidad $\nabla \times (\nabla \times \vec{E}) = \nabla(\nabla \cdot \vec{E}) - \nabla^2 \vec{E} = -\nabla^2 \vec{E}$ (puesto que $\nabla \cdot \vec{E} = 0$):

$$\nabla \times \left(-\frac{\partial \vec{B}}{\partial t}\right) = -\frac{\partial}{\partial t}(\nabla \times \vec{B}) = -\epsilon_0 \mu_0 \frac{\partial^2 \vec{E}}{\partial t^2} \implies \nabla^2 \vec{E} = \epsilon_0 \mu_0 \frac{\partial^2 \vec{E}}{\partial t^2}$$

Análogamente, aplicando el rotor a la ley de Ampère-Maxwell en el vacío y usando $\nabla \cdot \vec{B} = 0$:

$$\nabla \times (\nabla \times \vec{B}) = -\nabla^2 \vec{B} = \epsilon_0 \mu_0 \nabla \times \left(\frac{\partial \vec{E}}{\partial t}\right) = \epsilon_0 \mu_0 \frac{\partial}{\partial t}(\nabla \times \vec{E}) = -\epsilon_0 \mu_0 \frac{\partial^2 \vec{B}}{\partial t^2} \implies \nabla^2 \vec{B} = \epsilon_0 \mu_0 \frac{\partial^2 \vec{B}}{\partial t^2}$$

Estas son dos ecuaciones de onda tridimensionales que describen ondas que se propagan en el vacío con velocidad:

$$c = \frac{1}{\sqrt{\epsilon_0 \mu_0}} = \frac{1}{\sqrt{(8.85419\times 10^{-12}\text{ C}^2/\text{N}\cdot\text{m}^2)(4\pi\times 10^{-7}\text{ T}\cdot\text{m/A})}} = 2.99792 \times 10^8\text{ m/s}$$

## Espectro electromagnético

Las ondas electromagnéticas abarcan un amplio rango de longitudes de onda $\lambda$ y frecuencias $f$ relacionadas mediante $c = \lambda f$. Diferentes frecuencias dentro del rango visible corresponden a distintos colores; las ondas de una sola frecuencia se denominan **monocromáticas**.

> **[Figura]:** Diagrama del espectro electromagnético con dos escalas paralelas horizontales: arriba, longitudes de onda $\lambda$ en metros de $10\text{ m}$ a $10^{-13}\text{ m}$; abajo, frecuencias $f$ en Hz de $10^8\text{ Hz}$ a $10^{22}\text{ Hz}$. Se señalan de izquierda a derecha las bandas: Radio y TV, Microondas, Infrarrojo, Luz visible (ampliada inferiormente entre $700\text{ nm}$ a la izquierda y $400\text{ nm}$ a la derecha), Ultravioleta, Rayos X y Rayos gamma.

**Tabla 32.1: Longitudes de onda de la luz visible**

| Rango de longitud de onda | Color |
|---|---|
| $400\text{ a }440\text{ nm}$ | Violeta |
| $440\text{ a }480\text{ nm}$ | Azul |
| $480\text{ a }560\text{ nm}$ | Verde |
| $560\text{ a }590\text{ nm}$ | Amarillo |
| $590\text{ a }630\text{ nm}$ | Naranja |
| $630\text{ a }700\text{ nm}$ | Rojo |

## Ondas monocromáticas planas

Una **onda plana** que viaja en la dirección $z$ no tiene dependencia en $x$ ni en $y$. En notación compleja:

$$\tilde{\vec{E}}(z,t) = \tilde{\vec{E}}_0 e^{i(kz - \omega t)}, \qquad \tilde{\vec{B}}(z,t) = \tilde{\vec{B}}_0 e^{i(kz - \omega t)}$$

donde los campos físicos corresponden a la parte real.

> **[Figura]:** Sistema de ejes cartesianos tridimensional dextrógiro ($x$ hacia arriba, $y$ hacia abajo-izquierda saliendo de la página, $z$ hacia la derecha). Cuatro planos grises paralelos al plano $xy$ (frentes de onda planos) están espaciados a lo largo del eje $+z$, con un vector de velocidad $\vec{v}$ apuntando en $+z$. Sobre cada frente de onda se dibujan vectores de campo eléctrico $\vec{E}$ paralelos al eje $x$, uniformes en todo el plano y alternando su sentido y magnitud de un plano al siguiente.

- *(del resumen)* Parámetros de la onda:
  - $k = \dfrac{2\pi}{\lambda} = \dfrac{\omega}{c}$: **número de onda** (puede entenderse como una "frecuencia" espacial).
  - $\omega = 2\pi f = \dfrac{2\pi c}{\lambda}$: **frecuencia angular** de la onda.

Al aplicar las ecuaciones de divergencia $\nabla \cdot \vec{E} = 0$ y $\nabla \cdot \vec{B} = 0$:

$$(E_0)_z = (B_0)_z = 0$$

Es decir, las ondas electromagnéticas son **transversales**: los campos eléctrico y magnético son perpendiculares a la dirección de propagación.

Al aplicar la ley de Faraday $\nabla \times \vec{E} = -\frac{\partial \vec{B}}{\partial t}$:

$$-k(E_0)_y = \omega (B_0)_x, \qquad k(E_0)_x = \omega (B_0)_y$$

En forma vectorial:

$$\vec{B}_0 = \frac{k}{\omega}(\hat{z} \times \vec{E}_0)$$

Esto indica que $\vec{E}$ y $\vec{B}$ están en fase y son mutuamente perpendiculares (la ley de Ampère-Maxwell conduce a la misma condición). En magnitud:

$$B_0 = \frac{k}{\omega}E_0 = \frac{1}{c}E_0$$

> **[Figura]:** Onda electromagnética sinusoidal linealmente polarizada en el sistema $(x\text{ arriba}, y\text{ saliendo}, z\text{ derecha})$ propagándose con velocidad $c$ en $+z$. El campo $\vec{E}$ oscila sinusoidalmente a lo largo del eje $x$ (plano $xz$) con amplitud $E_0$; el campo $\vec{B}$ oscila en fase a lo largo del eje $y$ (plano $yz$) con amplitud $E_0/c$. En todo punto, $\vec{E} \perp \vec{B} \perp \hat{z}$.

### Ejemplo de onda monocromática plana

Si la onda plana se propaga en $+\hat{z}$ y su campo eléctrico está polarizado a lo largo de $\hat{x}$:

$$\tilde{\vec{E}}(z,t) = \tilde{E}_0 e^{i(kz - \omega t)}\hat{x}, \qquad \tilde{\vec{B}}(z,t) = \frac{1}{c}\tilde{E}_0 e^{i(kz - \omega t)}\hat{y}$$

Tomando la parte real (con $\tilde{E}_0 = E_0 e^{i\delta}$ y usando $e^{ix} = \cos x + i\sin x$), los campos físicos son:

$$\vec{E}(z,t) = E_0 \cos(kz - \omega t + \delta)\hat{x}, \qquad \vec{B}(z,t) = \frac{1}{c}E_0 \cos(kz - \omega t + \delta)\hat{y}$$

## Polarización

Se dice que una onda electromagnética está **linealmente polarizada** cuando el campo eléctrico yace en un plano fijo. Para una onda que se propaga en la dirección arbitraria $\hat{k}$ con vector de onda $\vec{k} = k\hat{k}$ y dirección de polarización unitaria $\hat{n}$:

$$\tilde{\vec{E}}(\vec{r},t) = \tilde{E}_0 e^{i(\vec{k}\cdot\vec{r} - \omega t)}\hat{n}, \qquad \tilde{\vec{B}}(\vec{r},t) = \frac{1}{c}\tilde{E}_0 e^{i(\vec{k}\cdot\vec{r} - \omega t)}(\hat{k} \times \hat{n}) = \frac{1}{c}\hat{k} \times \tilde{\vec{E}}$$

En forma real:

$$\vec{E}(\vec{r},t) = E_0 \cos(\vec{k}\cdot\vec{r} - \omega t + \delta)\hat{n}, \qquad \vec{B}(\vec{r},t) = \frac{1}{c}E_0 \cos(\vec{k}\cdot\vec{r} - \omega t + \delta)(\hat{k} \times \hat{n})$$

donde la transversalidad exige que la dirección de polarización $\hat{n}$ (definida por $\vec{E}$) sea perpendicular a la dirección de propagación $\hat{k}$:

$$\hat{n} \cdot \hat{k} = 0$$

> **[Figura]:** Tres esquemas de polarización lineal para una onda propagándose con velocidad $v$ en la dirección $+z$ (ejes $x$ arriba, $y$ abajo-izquierda, $z$ derecha):
> **(a) Polarización vertical:** el campo eléctrico oscila en el plano vertical $xz$ (dirección $\hat{x}$).
> **(b) Polarización horizontal:** el campo eléctrico oscila en el plano horizontal $yz$ (dirección $\hat{y}$).
> **(c) Vector de polarización general:** el vector unitario $\hat{n}$ yace en el plano $xy$ formando un ángulo $\theta$ con el eje $x$, y la onda oscila en el plano oblicuo definido por $\hat{n}$ y $\hat{z}$.

## Energía e intensidad en las ondas electromagnéticas

Partiendo del teorema de Poynting y de la relación $B_0 = \frac{1}{c}E_0$ (válida instantáneamente como $B = E/c$ en una onda plana en el vacío, con $\epsilon_0 \mu_0 = 1/c^2$):

$$u = \frac{1}{2}\left(\epsilon_0 E^2 + \frac{1}{\mu_0}B^2\right) = \frac{\epsilon_0}{2}\left(E^2 + \frac{1}{\epsilon_0 \mu_0}B^2\right) = \epsilon_0 E^2 = \frac{1}{\mu_0}B^2$$

Para la onda plana $\vec{E}(z,t) = E_0 \cos(kz - \omega t + \delta)\hat{x}$:

$$u = \epsilon_0 E_0^2 \cos^2(kz - \omega t + \delta)$$

La densidad de energía promedio en un período $T = 2\pi/\omega$ es:

$$\langle u \rangle = \frac{1}{T}\int_0^T \epsilon_0 E_0^2 \cos^2(kz - \omega t + \delta)\,dt = \frac{1}{2}\epsilon_0 E_0^2$$

Por su parte, el vector de Poynting instantáneo vale:

$$\vec{S} = \frac{1}{\mu_0}(\vec{E} \times \vec{B}) = \frac{1}{c\mu_0}E^2\hat{z} = \frac{1}{c\mu_0 \epsilon_0} u\hat{z} = c u \hat{z}$$

La **intensidad** $I$ de la onda es el valor promedio temporal de la magnitud del vector de Poynting:

$$I = \langle S \rangle = \frac{1}{2} c \epsilon_0 E_0^2$$

## Propiedades clave de las ondas electromagnéticas

1. La onda es **transversal**: tanto $\vec{E}$ como $\vec{B}$ son perpendiculares a la dirección de propagación de la onda. Los campos eléctrico y magnético también son perpendiculares entre sí. La dirección de propagación es la dirección del producto vectorial $\vec{E} \times \vec{B}$.
2. Hay una razón definida entre las magnitudes de $\vec{E}$ y $\vec{B}$: $E = cB$.
3. La onda viaja en el vacío con rapidez definida e invariable $c$.
4. A diferencia de las ondas mecánicas, que necesitan de partículas oscilantes de un medio (como el agua o el aire) para transmitirse, las ondas electromagnéticas no requieren un medio: lo que "ondula" en una onda electromagnética son los campos eléctrico y magnético.

> **[Figura]:** Regla de la mano derecha para una onda electromagnética en un sistema dextrógiro con origen $O$: $\vec{E}$ apunta hacia $+y$ (arriba), $\vec{B}$ hacia $+z$ (abajo-izquierda) y la dirección de propagación ($\vec{E} \times \vec{B}$, velocidad $c$) hacia $+x$ (abajo-derecha). Se ilustra una mano derecha con el pulgar apuntando en la dirección de propagación ($+x$) y los dedos girando $90^\circ$ desde $\vec{E}$ hasta $\vec{B}$.

## Ondas electromagnéticas en la materia

En un **medio lineal y homogéneo** sin cargas ni corrientes libres ($\rho_f = 0$, $\vec{J}_f = \vec{0}$), usando las relaciones constitutivas $\vec{D} = \epsilon\vec{E}$ y $\vec{H} = \frac{1}{\mu}\vec{B}$, las ecuaciones de Maxwell toman la forma:

$$\nabla \cdot \vec{E} = 0, \qquad \nabla \cdot \vec{B} = 0$$

$$\nabla \times \vec{E} = -\frac{\partial \vec{B}}{\partial t}, \qquad \nabla \times \vec{B} = \epsilon\mu \frac{\partial \vec{E}}{\partial t}$$

Por lo tanto, en un medio lineal y homogéneo se propagan ondas electromagnéticas con velocidad:

$$v = \frac{1}{\sqrt{\epsilon\mu}} = \frac{c}{n}$$

donde

$$n = \sqrt{\frac{\epsilon\mu}{\epsilon_0 \mu_0}}$$

es el **índice de refracción** del medio. La densidad de energía y el vector de Poynting en el medio están dados por:

$$u = \frac{1}{2}\left(\epsilon E^2 + \frac{1}{\mu}B^2\right), \qquad \vec{S} = \frac{1}{\mu}(\vec{E} \times \vec{B})$$

## Reflexión y transmisión en incidencia normal

### Condiciones de borde y amplitudes reflejada y transmitida

En la interfaz plana ($z = 0$) entre dos medios lineales $1$ ($z < 0$) y $2$ ($z > 0$), las condiciones de borde para los campos totales $\vec{E}_1 = \tilde{\vec{E}}_I + \tilde{\vec{E}}_R$, $\vec{B}_1 = \tilde{\vec{B}}_I + \tilde{\vec{B}}_R$, $\vec{E}_2 = \tilde{\vec{E}}_T$, $\vec{B}_2 = \tilde{\vec{B}}_T$ (sin cargas ni corrientes superficiales libres) son:

$$\text{(i)}\;\epsilon_1 E_1^\perp = \epsilon_2 E_2^\perp, \qquad \text{(ii)}\;B_1^\perp = B_2^\perp, \qquad \text{(iii)}\;\vec{E}_1^\parallel = \vec{E}_2^\parallel, \qquad \text{(iv)}\;\frac{1}{\mu_1}\vec{B}_1^\parallel = \frac{1}{\mu_2}\vec{B}_2^\parallel$$

> **[Figura]:** Ejes tridimensionales ($x$ hacia arriba, $y$ hacia abajo-izquierda, $z$ hacia la derecha) con una interfaz gris plana en $z = 0$ (plano $xy$) que separa el medio 1 ($z < 0$) del medio 2 ($z > 0$). En el medio 1 se muestra la onda incidente propagándose con $\vec{v}_1$ en $+z$ ($\vec{E}_I$ en $+x$, $\vec{B}_I$ en $+y$) y la onda reflejada propagándose con $\vec{v}_1$ en $-z$ ($\vec{E}_R$ en $+x$, $\vec{B}_R$ en $-y$). En el medio 2 se muestra la onda transmitida propagándose con $\vec{v}_2$ en $+z$ ($\vec{E}_T$ en $+x$, $\vec{B}_T$ en $+y$).

Considerando ondas incidentes viajando en $+z$ y polarizadas en $\hat{x}$:

- **Incidente:**
  $$\tilde{\vec{E}}_I(z,t) = \tilde{E}_{0_I} e^{i(k_1 z - \omega t)}\hat{x}, \qquad \tilde{\vec{B}}_I(z,t) = \frac{1}{v_1}\tilde{E}_{0_I} e^{i(k_1 z - \omega t)}\hat{y}$$
- **Reflejada:**
  $$\tilde{\vec{E}}_R(z,t) = \tilde{E}_{0_R} e^{i(-k_1 z - \omega t)}\hat{x}, \qquad \tilde{\vec{B}}_R(z,t) = -\frac{1}{v_1}\tilde{E}_{0_R} e^{i(-k_1 z - \omega t)}\hat{y}$$
- **Transmitida:**
  $$\tilde{\vec{E}}_T(z,t) = \tilde{E}_{0_T} e^{i(k_2 z - \omega t)}\hat{x}, \qquad \tilde{\vec{B}}_T(z,t) = \frac{1}{v_2}\tilde{E}_{0_T} e^{i(k_2 z - \omega t)}\hat{y}$$

En incidencia normal no hay componente perpendicular (por lo que (i) y (ii) se cumplen trivialmente como $0 = 0$). Evaluando (iii) y (iv) en $z = 0$:

$$\tilde{E}_{0_I} + \tilde{E}_{0_R} = \tilde{E}_{0_T}$$

$$\frac{1}{\mu_1}\left(\frac{1}{v_1}\tilde{E}_{0_I} - \frac{1}{v_1}\tilde{E}_{0_R}\right) = \frac{1}{\mu_2}\left(\frac{1}{v_2}\tilde{E}_{0_T}\right) \implies \tilde{E}_{0_I} - \tilde{E}_{0_R} = \beta \tilde{E}_{0_T}$$

donde se define el parámetro adimensional:

$$\beta \equiv \frac{\mu_1 v_1}{\mu_2 v_2} = \frac{\mu_1 n_2}{\mu_2 n_1}$$

Resolviendo el sistema lineal para $\tilde{E}_{0_R}$ y $\tilde{E}_{0_T}$ en función de $\tilde{E}_{0_I}$:

$$\tilde{E}_{0_R} = \left(\frac{1 - \beta}{1 + \beta}\right)\tilde{E}_{0_I}, \qquad \tilde{E}_{0_T} = \left(\frac{2}{1 + \beta}\right)\tilde{E}_{0_I}$$

Si las permeabilidades $\mu_1, \mu_2$ están cerca de su valor en el vacío ($\mu_1 \approx \mu_2 \approx \mu_0$), entonces $\beta = v_1 / v_2$ y las amplitudes resultan:

$$\tilde{E}_{0_R} = \left(\frac{v_2 - v_1}{v_2 + v_1}\right)\tilde{E}_{0_I}, \qquad \tilde{E}_{0_T} = \left(\frac{2v_2}{v_2 + v_1}\right)\tilde{E}_{0_I}$$

## Ejemplo resuelto: Superposición de dos ondas electromagnéticas

**Enunciado:** Dos ondas electromagnéticas en el vacío son emitidas desde dos diferentes fuentes, de modo que:

$$\vec{E}_1(x,t) = E_{10}\cos(kx - \omega t)\hat{y}$$
$$\vec{E}_2(x,t) = E_{20}\cos(kx - \omega t + \phi)\hat{y}$$

a) Encuentre el vector de Poynting asociado a la onda electromagnética resultante.  
b) Encuentre la intensidad de la onda.  
c) Repita el cálculo si la dirección de propagación de la segunda onda electromagnética viaja en la dirección contraria a la primera:

$$\vec{E}_1(x,t) = E_{10}\cos(kx - \omega t)\hat{y}$$
$$\vec{E}_2(x,t) = E_{20}\cos(kx + \omega t + \phi)\hat{y}$$

> **[Figura]:** Ejes $x$ horizontal hacia la derecha e $y$ vertical hacia arriba. Se representan dos ondas sinusoidales superpuestas en el espacio (una roja y una azul, desfasadas entre sí), con dos flechas horizontales superiores marcadas con $c$ (roja y azul) apuntando hacia $+x$, ilustrando la propagación en el mismo sentido para las partes (a) y (b).

**Resolución**

- *Idea:* Por el principio de superposición, los campos totales son $\vec{E} = \vec{E}_1 + \vec{E}_2$ y $\vec{B} = \vec{B}_1 + \vec{B}_2$. Para cada onda plana monocromática en el vacío que se propaga con velocidad $c = \omega/k$ en la dirección unitaria $\hat{u}$, el campo magnético asociado es $\vec{B}_i = \frac{1}{c}(\hat{u}_i \times \vec{E}_i)$. Luego se calcula el vector de Poynting $\vec{S} = \frac{1}{\mu_0}(\vec{E} \times \vec{B})$ y su promedio temporal en un período $T = 2\pi/\omega$ para obtener la intensidad $I = |\langle\vec{S}\rangle|$.

**Parte a) Vector de Poynting resultante (ambas ondas en $+x$)**

1. Ambas ondas se propagan en $+\hat{x}$ (ya que la fase es $kx - \omega t$). Como $\hat{x} \times \hat{y} = \hat{z}$, sus campos magnéticos son:
   $$\vec{B}_1(x,t) = \frac{E_{10}}{c}\cos(kx - \omega t)\hat{z}, \qquad \vec{B}_2(x,t) = \frac{E_{20}}{c}\cos(kx - \omega t + \phi)\hat{z}$$

2. Los campos resultantes son:
   $$\vec{E}(x,t) = \left[E_{10}\cos(kx - \omega t) + E_{20}\cos(kx - \omega t + \phi)\right]\hat{y}$$
   $$\vec{B}(x,t) = \frac{1}{c}\left[E_{10}\cos(kx - \omega t) + E_{20}\cos(kx - \omega t + \phi)\right]\hat{z}$$

3. Calculamos el vector de Poynting $\vec{S} = \frac{1}{\mu_0}(\vec{E} \times \vec{B})$ usando $\hat{y} \times \hat{z} = \hat{x}$ y $\frac{1}{\mu_0 c} = \epsilon_0 c$:

$$\boxed{\vec{S}(x,t) = \epsilon_0 c \left[E_{10}\cos(kx - \omega t) + E_{20}\cos(kx - \omega t + \phi)\right]^2 \hat{x}}$$

**Parte b) Intensidad de la onda resultante**

1. Desarrollamos el cuadrado dentro de $\vec{S}(x,t)$:
   $$\vec{S}(x,t) = \epsilon_0 c \left[E_{10}^2 \cos^2(kx - \omega t) + E_{20}^2 \cos^2(kx - \omega t + \phi) + 2 E_{10} E_{20}\cos(kx - \omega t)\cos(kx - \omega t + \phi)\right]\hat{x}$$

2. Tomamos el promedio temporal en un período $T = 2\pi/\omega$:
   - $\langle \cos^2(kx - \omega t) \rangle = \frac{1}{2}$
   - $\langle \cos^2(kx - \omega t + \phi) \rangle = \frac{1}{2}$
   - Usando $\cos A \cos B = \frac{1}{2}[\cos(A - B) + \cos(A + B)]$:
     $$\cos(kx - \omega t)\cos(kx - \omega t + \phi) = \frac{1}{2}\left[\cos\phi + \cos(2kx - 2\omega t + \phi)\right]$$
     Como el promedio temporal de $\cos(2kx - 2\omega t + \phi)$ sobre un período es cero, queda $\langle\cos(kx - \omega t)\cos(kx - \omega t + \phi)\rangle = \frac{1}{2}\cos\phi$.

3. Sustituyendo en $\langle\vec{S}\rangle$:
   $$\langle\vec{S}\rangle = \frac{1}{2}\epsilon_0 c \left(E_{10}^2 + E_{20}^2 + 2E_{10}E_{20}\cos\phi\right)\hat{x}$$
   Por lo tanto, la intensidad $I = |\langle\vec{S}\rangle|$ es:

$$\boxed{I = \frac{1}{2}\epsilon_0 c \left(E_{10}^2 + E_{20}^2 + 2E_{10}E_{20}\cos\phi\right) = I_1 + I_2 + 2\sqrt{I_1 I_2}\cos\phi}$$

donde $I_1 = \frac{1}{2}\epsilon_0 c E_{10}^2$ e $I_2 = \frac{1}{2}\epsilon_0 c E_{20}^2$.

**Parte c) Segunda onda propagándose en sentido contrario ($-x$)**

1. La primera onda sigue viajando en $+\hat{x}$ con $\vec{B}_1(x,t) = \frac{E_{10}}{c}\cos(kx - \omega t)\hat{z}$. La segunda onda tiene fase $kx + \omega t + \phi$, por lo que viaja en $-\hat{x}$ ($\hat{u}_2 = -\hat{x}$). Como $(-\hat{x}) \times \hat{y} = -\hat{z}$, su campo magnético (verificable con $\nabla \times \vec{E}_2 = -\partial\vec{B}_2/\partial t$) es:
   $$\vec{B}_2(x,t) = -\frac{E_{20}}{c}\cos(kx + \omega t + \phi)\hat{z}$$

2. Los campos resultantes son:
   $$\vec{E}(x,t) = \left[E_{10}\cos(kx - \omega t) + E_{20}\cos(kx + \omega t + \phi)\right]\hat{y}$$
   $$\vec{B}(x,t) = \frac{1}{c}\left[E_{10}\cos(kx - \omega t) - E_{20}\cos(kx + \omega t + \phi)\right]\hat{z}$$

3. El vector de Poynting resulta de un producto de suma por diferencia:
   $$\vec{S}(x,t) = \frac{1}{\mu_0 c}\left[E_{10}\cos(kx - \omega t) + E_{20}\cos(kx + \omega t + \phi)\right]\left[E_{10}\cos(kx - \omega t) - E_{20}\cos(kx + \omega t + \phi)\right]\hat{x}$$

$$\boxed{\vec{S}(x,t) = \epsilon_0 c \left[E_{10}^2\cos^2(kx - \omega t) - E_{20}^2\cos^2(kx + \omega t + \phi)\right]\hat{x}}$$

4. Al promediar en un período $T$, $\langle \cos^2(kx - \omega t) \rangle = \langle \cos^2(kx + \omega t + \phi) \rangle = \frac{1}{2}$, por lo que:
   $$\langle\vec{S}\rangle = \frac{1}{2}\epsilon_0 c (E_{10}^2 - E_{20}^2)\hat{x}$$
   y la magnitud del flujo promedio de energía (intensidad neta) es:

$$\boxed{I = |\langle\vec{S}\rangle| = \frac{1}{2}\epsilon_0 c \left|E_{10}^2 - E_{20}^2\right| = |I_1 - I_2|}$$

- *Verificación:*
  - Unidades: $[\epsilon_0 c E^2] = (\text{C}^2/\text{N}\cdot\text{m}^2)(\text{m/s})(\text{N}/\text{C})^2 = \text{N}/(\text{m}\cdot\text{s}) = \text{W/m}^2$.
  - Casos límite en (b): si $E_{20} = 0$, se recupera $I = \frac{1}{2}\epsilon_0 c E_{10}^2$; si $E_{10} = E_{20} = E_0$ y $\phi = 0$, $I = 4I_1$ (interferencia constructiva); si $\phi = \pi$, $I = 0$ (interferencia destructiva).
  - Caso límite en (c): si $E_{10} = E_{20}$, se forma una onda estacionaria y el flujo neto de energía es nulo ($\langle\vec{S}\rangle = \vec{0}$, $I = 0$).

## Anexo: Derivadas parciales para una onda plana en la dirección $x$

> **Nota:** El subtítulo superior de la diapositiva 54 queda parcialmente oculto por la barra de encabezado; del contexto de las ecuaciones se trata de una onda plana dependiente solo de $x$ y $t$ en un medio lineal homogéneo.

Bajo estas hipótesis, todas las derivadas con respecto a $y$ y $z$ son nulas, y por lo tanto se tiene:

$$\nabla \cdot \vec{E} = \frac{\partial E_x}{\partial x} + \frac{\partial E_y}{\partial y} + \frac{\partial E_z}{\partial z} \implies \frac{\partial E_x}{\partial x} = 0$$

$$\nabla \cdot \vec{B} = \frac{\partial B_x}{\partial x} + \frac{\partial B_y}{\partial y} + \frac{\partial B_z}{\partial z} \implies \frac{\partial B_x}{\partial x} = 0$$

El rotor del campo eléctrico (denotado como $\nabla \wedge \vec{E}$) es:

$$(\nabla \wedge \vec{E})_x = \frac{\partial E_z}{\partial y} - \frac{\partial E_y}{\partial z} = -\frac{\partial B_x}{\partial t} \implies \frac{\partial B_x}{\partial t} = 0$$

$$(\nabla \wedge \vec{E})_y = \frac{\partial E_x}{\partial z} - \frac{\partial E_z}{\partial x} = -\frac{\partial B_y}{\partial t} \implies \frac{\partial B_y}{\partial t} = \frac{\partial E_z}{\partial x}$$

$$(\nabla \wedge \vec{E})_z = \frac{\partial E_y}{\partial x} - \frac{\partial E_x}{\partial y} = -\frac{\partial B_z}{\partial t} \implies \frac{\partial B_z}{\partial t} = -\frac{\partial E_y}{\partial x}$$

El rotor del campo magnético es:

$$(\nabla \wedge \vec{B})_x = \frac{\partial B_z}{\partial y} - \frac{\partial B_y}{\partial z} = \epsilon\mu\frac{\partial E_x}{\partial t} \implies \frac{\partial E_x}{\partial t} = 0$$

$$(\nabla \wedge \vec{B})_y = \frac{\partial B_x}{\partial z} - \frac{\partial B_z}{\partial x} = \epsilon\mu\frac{\partial E_y}{\partial t} \implies \frac{\partial E_y}{\partial t} = -\frac{1}{\epsilon\mu}\frac{\partial B_z}{\partial x}$$

$$(\nabla \wedge \vec{B})_z = \frac{\partial B_y}{\partial x} - \frac{\partial B_x}{\partial y} = \epsilon\mu\frac{\partial E_z}{\partial t} \implies \frac{\partial E_z}{\partial t} = \frac{1}{\epsilon\mu}\frac{\partial B_y}{\partial x}$$

> **Nota (errata):** En la componente $y$ de $\nabla \wedge \vec{B}$, la diapositiva escribe $\frac{\partial v_z}{\partial x}$ en lugar de $\frac{\partial B_z}{\partial x}$.

## Resumen de fórmulas

| Fórmula | Significado | Condiciones |
|---|---|---|
| $i_D = \epsilon \dfrac{d\Phi_E}{dt}$, $\quad j_D = \epsilon \dfrac{dE}{dt}$ | Corriente y densidad de corriente de desplazamiento | Flujo eléctrico variable en el tiempo |
| $\oint \vec{B} \cdot d\vec{l} = \mu_0 (i_C + i_D)_{\text{enc}}$ | Ley de Ampère-Maxwell (forma integral) | General, en el vacío ($\epsilon = \epsilon_0$) |
| $\nabla \cdot \vec{E} = \dfrac{\rho}{\epsilon_0}$, $\quad \nabla \cdot \vec{B} = 0$ | Leyes de Gauss eléctrica y magnética | En el vacío |
| $\nabla \times \vec{E} = -\dfrac{\partial \vec{B}}{\partial t}$, $\quad \nabla \times \vec{B} = \mu_0\vec{J} + \epsilon_0\mu_0\dfrac{\partial \vec{E}}{\partial t}$ | Leyes de Faraday y Ampère-Maxwell (diferencial) | En el vacío |
| $\nabla \cdot \vec{D} = \rho_f$, $\quad \nabla \times \vec{H} = \vec{J}_f + \dfrac{\partial \vec{D}}{\partial t}$ | Ecuaciones de Maxwell en la materia | $\vec{D}=\epsilon_0\vec{E}+\vec{P}$, $\;\vec{H}=\frac{1}{\mu_0}\vec{B}-\vec{M}$ |
| $\vec{D} = \epsilon \vec{E}$, $\quad \vec{H} = \dfrac{1}{\mu}\vec{B}$ | Relaciones constitutivas lineales | Medio lineal; $\epsilon=\epsilon_0(1+\chi_e)$, $\mu=\mu_0(1+\chi_m)$ |
| $u = \dfrac{1}{2}\left(\epsilon_0 E^2 + \dfrac{1}{\mu_0}B^2\right)$ | Densidad de energía electromagnética | En el vacío (en un medio: $\epsilon_0\to\epsilon$, $\mu_0\to\mu$) |
| $\vec{S} = \dfrac{1}{\mu_0}(\vec{E} \times \vec{B})$ | Vector de Poynting (flujo de energía) | En el vacío (en un medio: $\frac{1}{\mu}(\vec{E}\times\vec{B})$) |
| $\dfrac{dW}{dt} = -\dfrac{dU_{\text{em}}}{dt} - \oint_{\mathcal{S}} \vec{S} \cdot d\vec{a}$ | Teorema de Poynting (forma integral) | Conservación de energía en volumen $\mathcal{V}$ |
| $\dfrac{\partial}{\partial t}(u_{\text{mec}} + u_{\text{em}}) = -\nabla \cdot \vec{S}$ | Teorema de Poynting (forma diferencial) | Local, continuo |
| $\nabla^2 \vec{E} = \epsilon_0\mu_0 \dfrac{\partial^2 \vec{E}}{\partial t^2}$, $\quad \nabla^2 \vec{B} = \epsilon_0\mu_0 \dfrac{\partial^2 \vec{B}}{\partial t^2}$ | Ecuaciones de onda electromagnética | En el vacío sin fuentes ($\rho=0$, $\vec{J}=\vec{0}$) |
| $c = \dfrac{1}{\sqrt{\epsilon_0 \mu_0}} \approx 2.99792 \times 10^8\text{ m/s}$ | Rapidez de la luz en el vacío | Vacío |
| $k = \dfrac{2\pi}{\lambda} = \dfrac{\omega}{c}$, $\quad \omega = 2\pi f = \dfrac{2\pi c}{\lambda}$ | Número de onda y frecuencia angular *(del resumen)* | Onda monocromática en el vacío |
| $\vec{E}(\vec{r},t) = E_0 \cos(\vec{k}\cdot\vec{r} - \omega t + \delta)\hat{n}$ | Onda plana monocromática linealmente polarizada | $\hat{n}\cdot\hat{k}=0$ (onda transversal) |
| $\vec{B} = \dfrac{1}{c}(\hat{k} \times \vec{E})$, $\quad B_0 = \dfrac{E_0}{c}$ | Relación entre $\vec{E}$ y $\vec{B}$ en onda plana | Onda plana en el vacío |
| $\langle u \rangle = \dfrac{1}{2}\epsilon_0 E_0^2$, $\quad I = \langle S \rangle = \dfrac{1}{2}c\epsilon_0 E_0^2$ | Densidad de energía media e intensidad | Onda plana monocromática en el vacío |
| $v = \dfrac{1}{\sqrt{\epsilon\mu}} = \dfrac{c}{n}$, $\quad n = \sqrt{\dfrac{\epsilon\mu}{\epsilon_0\mu_0}}$ | Rapidez e índice de refracción en un medio | Medio lineal homogéneo sin cargas/corrientes libres |
| $\tilde{E}_{0_R} = \dfrac{1-\beta}{1+\beta}\tilde{E}_{0_I}$, $\quad \tilde{E}_{0_T} = \dfrac{2}{1+\beta}\tilde{E}_{0_I}$ | Amplitudes reflejada y transmitida | Incidencia normal; $\beta = \dfrac{\mu_1 v_1}{\mu_2 v_2} = \dfrac{\mu_1 n_2}{\mu_2 n_1}$ |
