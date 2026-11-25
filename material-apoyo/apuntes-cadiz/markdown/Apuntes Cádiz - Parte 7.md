---
title: "Parte 7"
source_pdf: "Electro/material-apoyo/apuntes-cadiz/Apuntes Cádiz - Parte 7.pdf"
pages: 55
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Parte 7

### Página 1

Parte VII
Ecuaciones de Maxwell y sus bases
empíricas

---

### Página 2

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 3

#### Capítulo 14
Ecuaciones de Maxwell
14.1.

Corriente de Desplazamiento

Habíamos visto anteriormente que si un conductor con corriente posee cierta simetría favorable, el campo magnético se podía obtener fácilmente mediante la ley de Ampère
˛
~ x) = µ0 Ienc
d~x · B(~
Γ

Esta ecuación indica que la circulación del campo magnético sobre cualquier curva cerrada
es siempre µ0 Ienc , donde Ienc es la corriente que atraviesa una superficie cuyo contorno es la
curva de integración.
Ahora, en un medio material la ley de Ampère es
˛
~ x) = I
d~x · H(~
Γ

Esta ley se puede llevar a su forma diferencial mediante el teorema de Stokes
~ × H(~
~ x) = J(~x)
∇
Sin embargo, esta ley es inconsistente en algunas ocasiones y encontraremos entonces una
generalización válida, que fue propuesta por Maxwell. Consideremos el circuito eléctrico de
la figura, que consiste de un condensador de placas paralelas, que se está cargando con una
corriente de magnitud constante I

Utilizando la ley de Ampère al contorno C y a la superficie S1
˛
¨
~ x) =
~ x) · J(~
~ x) = I
dS(~
d~x · H(~
C

S1

---

### Página 4

Si, por otra parte, se utiliza la ley de Ampère al contorno C y a la superficie S2 , entonces
J(~x) es cero para todo ~x ∈ S2
˛

C

~ x) =
d~x · H(~

¨

S2

~ x) · J(~
~ x) = 0
dS(~

Vemos que existe entonces una ambiguedad fundamental en la ley de Ampère al escoger dos
superficies de integración distintas. El error es fácil de ver al mirar su forma diferencial
~ × H(~
~ x) = J(~
~ x)
∇
Utilizamos ahora el hecho de que la divergencia de un rotor es nulo
~ ·∇
~ × H(~
~ x) = ∇
~ · J(~
~ x) = 0
∇
~ · J~ = 0 es inconsistente con la conservación de la carga en la presente
Es inmediato que ∇
situación, por que de hecho, en el volumen encerrado por ambas superficies, hay un ∂ρ/∂t
distinto de cero ( se está acumulando carga en el condensador).
Maxwell corrigió la ley de Ampère al agregar un término tal que de ella se desprenda
~ · J(~
~ x) = − ∂ρ(~x)
∇
∂t
De la primera ecuación de Maxwell
~ · D(~
~ x) = ρ(~x)
∇
y sustituyendo en la ecuación de continuidad
~
~ · J(~
~ x) + ∂ ∇
~ · D(~
~ x) = ∇
~ · (J(~
~ x) + ∂ D(~x) ) = 0
∇
∂t
∂t
~

de manera que la corrección de Maxwell está en agregar el término ∂∂tD a la forma diferencial
de la ley de Ampère, y entonces se obtiene la ley de Ampère-Maxwell
~
~ × H(~
~ x) = J(~
~ x) + ∂ D(~x)
∇
∂t
es evidente que en el caso de campos que no dependen del tiempo, esta ley es igual a la ley de
Ampère. La introducción del segundo término , llamado densidad de corriente de desplazamiento, representa una de las más grandes contribuciones de Maxwell a la teoría electromagnética.
Veremos que al modificar ésta ley, las ecuaciones de Maxwell predicen la propagación de ondas
electromagnéticas.
Por último, la forma integral de la ley de Ampère-Maxwell queda de la forma
˛

Γ

~ x) =
d~x · H(~

~ x) · J(~
~ x) + d
dS(~
dt
S(Γ)

¨

¨

S(Γ)

~ x) · D(~
~ x)
dS(~

En el ejemplo, al integrar en la superficie S2 , el segundo término no es nulo, debido a que
~ a través de S2 que está variando en el tiempo, de hecho la magnitud
hay un flujo del campo D
del campo crece cuando se acumula carga en el condensador.

---

### Página 5

14.2.

Ecuaciones de Maxwell

Las ecuaciones de Maxwell resumen toda la teoría electromagnética. Éstas establecen la
~ ~x)) con los
relación entre las fuentes (densidad de carga ρ(t, ~x), y densidad de corriente J(t,
~
~
~
~
campos E(t, ~x), B(t, ~x), D(t, ~x), H(t, ~x))
~ · D(t,
~ ~x) = ρ(~x)
∇
~
~ × E(t,
~ ~x) = − ∂ B(t, ~x)
∇
∂t
~ · B(t,
~ ~x) = 0
∇
~
~ × H(~
~ x) = J(~
~ x) + ∂ D(~x)
∇
∂t
~ ·D
~ = ρ es la ley de Gauss, cuya forma integral es
La primera ecuación ∇
ˆˆ
˚
 ~
~
x) · D(t, ~x) =
d3 xρ(t, ~x)
 dS(~
S

V (S)

~ ×E
~ = − ∂ B~ es la forma diferencial de la ley de inducción de Faraday, ésta
La ecuación ∇
∂t
dice que un campo magnético variable en el tiempo induce un campo eléctrico, en su forma
integral
ˆˆ
˛
d 
~
~ x) · B(t,
~ ~x)
d~x · E(t, ~x) = −
  dS(~
dt
Γ
S(Γ)
~ ·B
~ = 0 es la ley de Gauss magnética, y representa el hecho de que los
La ecuación ∇
monopolos magnéticos nunca han sido observados. Es decir, las líneas de campo magnético son
cerradas, consecuencia de esto es que el flujo magnético sobre una superficie cerrada es siempre
cero. En su forma integral
ˆˆ
 ~
~ ~x) = 0
x) · B(t,
 dS(~
S

~ ×H
~ = J~ + ∂ D~ es una extensión de la ley de Ampère, mencionada
Por último, la ecuación ∇
∂t
anteriormente. Hay que notar que ésta implica la ecuación de continuidad.
Es claro que las ecuaciones de Maxwell representan expresiones matemáticas de ciertos resultados experimentales. Resulta evidente entonces que no pueden demostrarse, sin embargo,
la aplicabilidad para cualquier situación puede verificarse.
~ + ~v × B),
~ que describe la acción de
Junto con la ecuación de la fuerza de Lorentz, F~ = q(E
los campos sobre partículas cargadas, este conjunto de leyes nos da una descripción clásica
completa de las partículas que actúan electromagnéticamente.

---

### Página 6

14.2.1.

Vector de Poynting- Conservación de la Energía

Las ecuaciones de Maxwell son consistentes con la ley de conservación de la carga eléctrica
~ · J(t,
~ ~x) + ∂ρ(t, ~x) = 0
∇
∂t
o, en su forma integral
~ x) · J(~
~ x) = − d
dS(~
dt
S(V )

ˆˆ




˚

d3 xρ(~x)

V

intentemos establecer una ley equivalente para la Conservación de la energía. Podemos
comenzar el análisis definiendo una densidad de energía electromagnética (t, ~x). Del mismo
~ ~x), donde
modo, definimos el vector de Poynting S(t,
~ ~x) · dS(~
~ x)
S(t,

~ x) por unidad de tiemes la energía electromagnética de campo cruzando una superficie dS(~
~ ~x) están claramente inspiradas en ρ(t, ~x)
po. Notar que nuestras definiciones de (t, ~x) y S(t,
~ ~x). Uno podría pensar entonces que la ley de conservación de la energía se escribe en la
y J(t,
forma
ˆˆ
˚
d

~ x) · S(t,
~ ~x)
−
d x(t, ~x) =   dS(~
dt
V
S(V )
Sin embargo, esto no está correcto, pues falta incluir un término que involucre el trabajo
realizado por los campos sobre las cargas presentes en la región V (por unidad de tiempo). La
fuerza neta que actúa sobre un elemento de carga por unidad de volumen es (de acuerdo a la
fuerza de Lorentz)
~ + J~ × B
~ = ρ(E
~ + ~v × B)
~
f~ = ρE
de forma que el trabajo realizado sobre las cargas por unidad de tiempo es
˚
˚

 ˚
3 ~
~
~ x) · E(~
~ x)
W =
d xf · ~v =
d xρ(~x) E(~x) · ~v (~x) =
d3 x0 J(~
V

V

V

Luego, la ley de conservación de la energía debe ser como sigue
ˆˆ
˚
˚
d

~
~
~ x) · E(~
~ x)
−
d x(t, ~x) =   dS(~x) · S(t, ~x) +
d3 xJ(~
dt
V
S(V )
V
La interpretación es bien clara: la disminución de energía por unidad de tiempo en un
volumen V es igual al flujo de energía electromagnética por unidad de tiempo a través del
contorno de V más el trabajo reaizado sobre las cargas en V por unidad de tiempo. En su
forma diferencial
∂(t, ~x) ~ ~
~ ~x) · E(t,
~ ~x)
+ ∇ · S(t, ~x) = −J(t,
∂t
Veamos que una expresión de este tipo se obtiene a partir de las ecuaciones de Maxwell
~
1 ~
~ ~x) − 0 ∂ E(t, ~x)
J~ = ∇
× B(t,
µ0
∂t

---

### Página 7

~ ~x) · E(t,
~ ~x) = −
−J(t,
Además
y



~
1 ~
~ ~x) · ∂ E(t, ~x)
~ × B(t,
~ ~x) + 0 E(t,
E(t, ~x) · ∇
µ0
∂t

~
~ × E(t,
~ ~x) = − ∂ B(t, ~x)
∇
∂t






~
~
~
~
~
~
~
~
~
E(t, ~x) · ∇ × B(t, ~x) = B(t, ~x) · ∇ × E(t, ~x) − ∇ · E(t, ~x) × B(t, ~x)






~
~ ~x) · ∇
~ × E(t,
~ ~x) − ∇
~ · E(t,
~ ~x) × B(t,
~ ~x) +0 E(t,
~ ~x) ∂ E(t, ~x)
~ ~x)·E(t,
~ ~x) = − 1 B(t,
−J(t,
µ0
∂t
~
~
~ ~x) · E(t,
~ ~x) = 1 B(t,
~ ~x) · ∂ B(t, ~x) + 0 E(t,
~ ~x) ∂ E(t, ~x) + ∇
~ ·
−J(t,
µ0
∂t
∂t

~ ~x) · E(t,
~ ~x) = ∂
−J(t,
∂t




1 ~2
1 ~2
~ ·
B (t, ~x) + ∇
0 E (t, ~x) +
2µ0

~
~ ~x) × B(t, ~x)
E(t,
µ0

~
~ ~x) × B(t, ~x)
E(t,
µ0

!

!

~
Comparando con nuestra expresión anterior, obtenemos fórmulas explícitas para  y S
1 ~2
1 ~2
(t, ~x) +
B (t, ~x)
(t, ~x) = 0 E
2µ0
~ ~x) = 1 E(t,
~ ~x) × B(t,
~ ~x)
S(t,
µ0

---

### Página 8

14.3.

Ecuaciones de Maxwell en un Medio Lineal, Homogéneo e Isotrópico

~ yE
~ en general está dada por
Es bien sabido que la relación entre los campos D


~
~ ~x)
~
D(t, ~x) = 0 P + E(t,

Sin embargo, en ciertos medios, la polarización depende linealmente del campo eléctrico
(medios lineales), de forma que
~ ~x) = E(t,
~ ~x)
D(t,
donde  es la permitividad del medio, y no depende de ~x para medios homogéneos e isotrópicos.
~ está relacionado con B
~
Del mismo modo, en este tipo de medios simples, el campo H
mediante
~ ~x) = 1 B(t,
~ ~x)
H(t,
µ
donde µ es la permeabilidad del medio. De esta forma las ecuaciones de Maxwell se pueden
escribir como
~ · E(t,
~ ~x) = ρ(t, ~x)
∇

~ ~x)
~ × E(t,
~ ~x) = − ∂ B(t,
∇
∂t
~ · B(t,
~ ~x) = 0
∇

~ ~x)
~ × B(t,
~ ~x) = µJ(t,
~ ~x) + µ ∂ E(t,
∇
∂t
~ y B,
~ donde propiedades del medio
Es un sistema de ecuaciones diferenciales acoplado para E
se incluyen en  y µ

---

### Página 9

Problema
Un cable coaxial consiste de dos conductores cilíndricos concéntricos , el interior de radio a y
el exterior de radio b (ambos con resistencia nula). La longitud de ambos cables l es tal que
l >> b. El cable transmite energía en DC desde una batería a una carga. La batería provee
una fem ε entre ambos conductores en un extremo del cable , y la carga es una resistencia R
conectada entre los conductores al otro extremo del cable. Una corriente I fluye a través del
conductor interior y regresa por el conductor exterior. La batería carga el conductor interno
con carga −Q y el externo con +Q

a) Encuentre el campo eléctrico en todas partes
~ en todas partes
b) Encuentre la dirección y magnitud de B
c) Calcule el vector de Poynting al interior del cable
~ sobre una superficie apropiada, encuentre la potencia que fluye en el cable
d) Al integrar S
coaxial
#### Solución
a) Despreciando efectos de borde, se puede calcular el campo eléctrico mediante la ley de Gauss,
utilizando como superficie de integración un cilindro de largo h y radio r, con a < r < b, como
se muestra en la figura

ˆˆ

ˆˆ

ˆˆ



 ~ 0
~ x0 ) = 
~ x0 ) = 
x ) · E(~
x0 )n̂(~x0 ) · E(~
 dS(~
 dS(ϕ, z)r̂ · E(r)r̂
 dS(~
S

S

ˆˆ

S

ˆˆ

 ~ 0

~ x0 ) = E(r) 
x ) · E(~
 dS(~
 dS(r, ϕ, z) = E(r)2πrh
S

S

la carga encerrada por S es
qint = 2πahσ

---

### Página 10

donde σ es la densidad de carga (homogénea) en el conductor interno
σ=

−Q
2πaL

con esto
2πah
E(r)2πrh =
0
E(r) =



−Q
2πaL



−Q
2πrL0

de forma que el campo eléctrico entre ambos conductores está dado por
~
E(r)
=

−Q
r̂
2πrL0

Además, se sabe
ε = φ(b) − φ(a) = −

ˆ b
a

~ x0 )
d~x0 · E(~

tomando una curva parametrizada por ~x = rr̂, con r̂ alguna dirección radial fija, y a < r < b,
se obtiene

ˆ b

ˆ b

−Q
Q
drE(r) = −
dr
=
ε=−
2πrL0
2πL0
a
a
ε=

ˆ b

dr
a r

Q
ln(b/a)
2πL0

luego
Q = ε2πL0 ln(a/b)
y
−ε ln (a/b)
~
r̂
E(r)
=
r
por supuesto, que el campo eléctrico para r < a es nulo (interior de un conductor), y lo
mismo ocurre para r > b, pues el cable coaxial es eléctricamente neutro.
b) El campo magnético para a < r < b puede se obtenido mediante la ley de Ampère,
utilizando como contorno una curva circular Γ concéntrica al conductor interno y de radio r.

---

### Página 11

Notar que el sentido de la corriente por el conductor interno es según ẑ. Por simetría, el
campo magnético sólo dependerá de la variable r, y será tangente a la curva Γ en todos sus
puntos
˛
ˆ 2π
~
~ ϕ̂ = 2πrB(r)
d~x · B(~x) =
dϕrϕ̂ · B(r)

Γ

la corriente encerrada por Γ es simplemente I, luego
˛
~ x) = µ0 I
d~x · B(~
Γ

2πrB(r) = µ0 I
µ0 I
~
B(r)
=
ϕ̂
2πr
El campo magnético es nulo para r > a (Cualquier curva encierra una corriente nula, pues
ambos conductores llevan I en sentidos opuestos).
c) El vector de Poynting al interior del cable (a < r < b) está dado por



1 −ε ln (a/b)
1 ~
µ0 I
~
~
S(r) = E(r) × B(r) =
r̂ × ϕ̂
µ0
µ0
r
2πr
−Iε ln (a/b)
~
ẑ
S(r)
=
2πr2
El vector de Poynting representa un flujo de energía por unidad de tiempo y área en dirección
−ẑ (es decir, desde la fem hacia la resistencia). Para calcular la potencia que se transmite a
través de la línea se debe calcular el flujo del vector Poynting sobre una sección transversal
entre ambos conductores, esto es

P =

¨

S

~ x) · S(~
~ x) =
dS(~

ˆ 2π

ˆ b

−Iε ln (a/b)
dϕ
drr(−ẑ) ·
ẑ = Iε ln (a/b)
2πr2
a

ˆ b
a

dr

r

P = εI
que es efectivamente la potencia que se disipa en la resistencia. Con este ejemplo se ilustra
como los campos realmente son los que transportan la energía desde la fuente a la carga

---

### Página 12

Problema
Un condensador de placas paralelas circulares se está cargando de modo que entre las placas
~
existe un campo eléctrico E(t)
aproximadamente uniforme. Obtenga el campo magnético entre
las placas del condensador en función de la distancia r al eje del mismo.

#### Solución
De la cuarta ecuación de Maxwell, tenemos que
~
~ ×H
~ = J~ + ∂ D
∇
∂t
en este caso, para la región entre placas
J~ = ~0
~ = 0 E,
~ yH
~ = B/µ
~ 0 , con lo que
Además, en el vacío se tiene D
~
~
~ ×B
~ =  0 µ0 ∂ E = 1 ∂ E
∇
∂t
c ∂t
Ahora, integrando sobre una circunferencia a distancia r del eje de las placas, y utilizando
el teorema de Stokes
˛

C


 ¨
~
~
~ x) · 1 ∂ E(~x)
~
~
dS(~x) · ∇ × B(~x) =
dS(~
c2 ∂t
S
S
¨
˛
1 d
~
~ x) · E(~
~ x) = 1 d (Eπr2 )
d~x · B = 2
dS(~
c dt S
c2 dt
C

~ =
d~x · B

¨

˛

C

~ = B2πr =
d~x · B

Finalmente
B=

r dE
2c2 dt

πr2 dE
c2 dt

---

### Página 13

Parte VIII
Ondas Electromagnéticas

---

### Página 14

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 15

#### Capítulo 15
Ondas Planas Monocromáticas
Una de las consecuencias importantes de las ecuaciones de Maxwell, es la predicción de la
existencia de ondas electromagnéticas que se propagan a la velocidad de la luz (La luz es, en
efecto, una onda electromagnética)
c= √
µ
La razón es que un campo eléctrico variable en el tiempo produce un campo magnético y vice
versa. El acoplamiento entre estos dos campos lleva a la generación de ondas electromagnéticas.
Esta predicción fue confirmada por Hertz en 1887

Fig. 15.1: Heinrich Hertz
Heinrich Hertz (1857-1894) Físico Alemán. Clarificó y expandió la teoría electromagnética
de la luz que fue propuesta por Maxwell. Fue el primero en demostrar de forma satisfactoria la
existencia de ondas electromagnéticas al construír un aparato para producir y detectar ondas
de radio.

15.1.

Ondas electromagnéticas planas en medios no conductores y libres de fuentes

Sabemos que cargas y corrientes son fuentes de campos electromagnéticos. Más adelante
veremos exactamente como son creados estos campos a partir de cierta distribución de fuentes.
Por el momento, mostraremos algunas soluciones particulares a las ecuaciones de Maxwell, en
primer lugar, las ondas planas. Supongamos que se quiere estudiar el comportamiento de los
campos en una región del espacio libre de fuentes (Es evidente que para que existan campos,
deben existir fuentes en algun lugar del espacio). Lo que quiero decir con esto es que encontraremos un tipo de solución para regiones que están lejos de las fuentes (es decir ρ(t, ~x) = 0 en
la zona de interés). También asumiremos que el medio en el cual se propagan las ondas no es

---

### Página 16

~ ~x) en respuesta
buen conductor, en ese caso tampoco existirá una densidad de corriente J(t,
al campo eléctrico. En este caso las ecuaciones de Maxwell son
~ · E(t,
~ ~x) = 0
∇

~ × E(t,
~ ~x) = − ∂ B(t,
~ ~x)
∇
∂t
~ · B(t,
~ ~x) = 0
∇

~ × B(t,
~ ~x) = µ ∂ E(t,
~ ~x)
∇
∂t
Utilizaremos ahora la conocida identidad

De esta forma



~
~
~
~ 2 f~
~
~
~
∇×∇×f =∇ ∇·f −∇


~ ~x)
~ ×∇
~ × E(t,
~ ~x) = ∇
~ ∇
~ · E(t,
~ ~x) − ∇
~ 2 E(t,
∇

pero en regiones libre de fuentes

~ · E(t,
~ ~x) = 0
∇
como indica la primera ecuación de Maxwell. Así
~ ×∇
~ × E(t,
~ ~x) = −∇
~ 2 E(t,
~ ~x)
∇
por otro lado

de forma que



~ ×∇
~ × E(t,
~ ~x) = −∇
~ × ∂ B(t,
~ ~x) = − ∂ ∇
~ × B(t,
~ ~x)
∇
∂t
∂t


∂2 ~
∂ ~
∂
~
~
~
µ E(t, ~x) = −µ 2 E(t,
~x)
∇ × ∇ × E(t, ~x) = −
∂t
∂t
∂t
~ ~x) − µ ∂ E(t,
~ ~x) = 0
~ 2 E(t,
∇
∂t2

definiendo

c= √
µ

~ 2 E(t,
~ ~x) − 1 ∂ E(t,
~ ~x) = 0
∇
c2 ∂t2
Esta es la conocida Ecuación de Onda. Es decir, hemos llegado a que en un medio libre
de cargas y no conductor, el campo eléctrico satisface la ecuación de onda. Las soluciones
son ondas que se propagan a velocidad c. Es fácil verificar que el campo magnético satisface
exactamente la misma ecuación, en efecto


~ ~x) = −∇
~ 2 B(t,
~ ~x)
~ ×∇
~ × B(t,
~ ~x) = ∇
~ ∇
~ · B(t,
~ ~x) − ∇
~ 2 B(t,
∇

---

### Página 17

por otro lado



∂
~ ×∇
~ × B(t,
~ ~x) = ∇
~ × µ E(t,
~ ~x)
∇
∂t

~ ~x)
~ ×∇
~ × B(t,
~ ~x) = µ ∂ ∇
~ × E(t,
~ ~x) = −µ ∂ B(t,
∇
∂t
∂t2
En resumen

~ 2 E(t,
~ ~x) − 1 ∂ E(t,
~ ~x) = 0
∇
c2 ∂t2

~ ~x) − 1 ∂ B(t,
~ ~x) = 0
~ 2 B(t,
∇
c2 ∂t2
~ ~x) y B(t,
~ ~x).
son las ecuaciones desacopladas para los campos E(t,
Ecuación de Onda en una dimensión
La forma general de la ecuación de onda en una dimensión es
 2

∂
1 ∂2
ψ(x, t) = 0
−
∂x2 c2 ∂t2
Resulta inmediato verificar que cualquier función de la forma ψ(x ± ct) satisface la ecuación
de onda en una dimensión. La demostración es la siguiente: Sea x0 = x ± ct, con esto ∂x
=1y
∂x
∂x0
= ±c. Usando la regla de la cadena
∂t
∂ψ(x0 ) ∂x0
∂ψ(x0 )
∂ψ(x0 )
=
=
∂x
∂x0 ∂x
∂x0


∂ 2 ψ(x0 ) ∂x
∂ 2 ψ(x0 )
∂ ∂ψ(x0 )
∂ 2 ψ(x0 )
=
=
=
∂ 2 x0
∂x
∂x0
∂x02 ∂x0
∂x02

Similarmente, las derivadas parciales con respecto a t son
∂ψ
∂ψ ∂x0
∂ψ
=
= ±c 0
∂t
∂x ∂t
∂x
∂
∂2ψ
=
∂t
∂t
Luego



∂ψ
± 0
∂x



=±

∂ 2 ψ ∂x0
2∂ ψ
=
c
∂x02 ∂t
∂x02

∂2ψ
∂2ψ
2∂ ψ
=
=
c
∂x02
∂x2
∂t2
lo cual muestra que ψ(x ± ct) es solución de la ecuación de onda en una dimensión. La
ecuación de onda es un ecuación diferencial lineal, lo que impica que si ψ1 (x, t) y ψ2 (x, t) son
soluciones de la ecuación de onda, entonces ψ1 (x, t) ± ψ2 (x, t) también es solución .vLas ondas
electromagnéticas obedecen entonces el principio de superposición

---

### Página 18

Solución a la ecuación de Onda
Para resolver la ecuación de onda que satisfacen los campos electromagnéticos, supondremos que
la variación temporal de éstos es de la forma eiwt ( es decir, tienen una dependencia oscilatoria
en el tiempo a una frecuencia bien determinada, w). A este tipo de ondas las llamaremos
monocromáticas
~ ~x) = E(~
~ x)eiwt
E(t,
~ ~x) = B(~
~ x)eiwt
B(t,
de forma que
∂2 ~
~ x)
E(t, ~x) = −w2 E(~
∂t2
~ x) satisface
Entonces la parte espacial E(~

~ 2 E(~
~ x) + w E(t,
~ ~x) = 0
∇
c2
busquemos una solución de la forma
~ x) = E
~ 0 e−i~k·~x
E(~
~ 0 es un vector constante
donde ~k =| ~k | k̂ y E
~ 2 E(~
~ x) = ∇
~ 2E
~ 0 e−i(kx x+ky y+kz z) = −k 2 E
~ 0 ei~k·~x
∇
donde k =| ~k |, de forma que
~

~ 0 e−ik·~x +
−k 2 E

w2 ~ −i~k·~x
=0
E0 e
c2

En efecto, es solución si
k=

r

w
c

Finalmente, hemos encontrado que una solución de la ecuación de onda en medios no conductores y libres de cargas son campos de la forma
~ ~x) = E
~ 0 ei(wt−~k·~x)
E(t,
~ ~x) = B
~ 0 ei(wt−~k·~x)
B(t,
con | ~k |= wc . Sin embargo, los campos deben tener divergencia nula, de forma que
del mismo modo

~ · E(t,
~ ~x) = 0 → ~k · E
~0 = 0
∇
~ · B(t,
~ ~x) = 0 → ~k · B
~0 = 0
∇

Ambos campos deben ser transversales (perpendiculares a la dirección de propagación)
Propagación en el eje z
Supongamos ahora que la dirección de propagación de los campos es en la dirección del eje z,
es decir
~k = β k̂ = w k̂
c

---

### Página 19

y

~k · ~x = βz
entonces

~ z) = E
~ 0 ei(wt−βz)
E(t,
~ z) = B
~ 0 ei(wt−βz)
B(t,

además, ambos campos deben ser perpendiculares al eje z. Por ejemplo, si escogemos
~ z) = E0 ei(wt−βz) î
E(t,
de la ecuación
se obtiene

~ × E(t,
~ z) = − ∂ B(t,
~ z)
∇
∂t
∂
~ 0 ei(wt−βz)
E0 ei(wt−βz) ĵ = −iβE0 ei(wt−βz) ĵ = −iwB
∂z

entonces
y se desprende que

~ 0 ei(wt−βz)
iβE0 ei(wt−βz) ĵ = iwB
~ 0 = E0 ĵ
B
c

Finalmente
~ z) = E0 ei(wt−βz) î
E(t,
~ z) = B0 ei(wt−βz) ĵ
B(t,
B0
=
E0
c
w
β=
c

~ yB
~ están siempre en fase, es decir, alcanzan sus máximos y mínimos al mismo
Vemos que E
tiempo.
Nota
Por supuesto que los campos físicos se obtienen al tomar la parte real de las soluciones encontradas
~ z) = E0 cos (wt − βz) î
E(t,
~ z) = E0 cos (wt − βz) ĵ
B(t,
c

---

### Página 20

Resumen
~ y B
~ son perpendiculares a la dirección de
1. Las ondas son transversales ya que tanto E
~ ×B
~
propagación, que coincide con la dirección del producto E
~
~
~
~ =0
2. Los campos E y B son perpendiculares entre sí. Es decir E · B
3. La razón entre las magnitudes de los campos es
E0
w
= =c= √
B0
β
µ0  0
4. La velocidad de propagación es igual a la velocidad de la luz en el medio c = √1µ
5. Las ondas electromagnéticas obedecen el principio de superposición
Vector Poynting
En general, el flujo de Energía por unidad de área (y tiempo) está descrito por el vector de
Poynting
~ ~x) = 1 E(t,
~ ~x) × B(t,
~ ~x) = E(t,
~ ~x) × H(t,
~ ~x)
S(t,
µ
Debido a que los campos son perpendiculares
~ ~x) |=
| S(t,

1 ~
~ ~x) |= 1 | E(t,
~ ~x) || B(t,
~ ~x) |
| E(t, ~x) × B(t,
µ
µ

En el caso de las ondas planas monocromáticas recién visto
~ ~x) = 1 E0 B0 cos2 (wt − βx) k̂
S(t,
µ c
Como es de esperar, el vector de Poynting apunta en la dirección de propagación

~ | es
La intensidad de la onda I, definida como el promedio temporal de | S
I=

E0 B0
E2
cB02
E0 B0
cos2 (wt − βx) =
= 0 =
µ
2µ
2cµ
2µ

donde hemos usado
cos2 (wt − βx) = 1/2
Notar que la magnitud de la intensidad es constante. Por supuesto que esto no es muy realista, pues es bien sabido de la vida diaria que la energía de la radiación decae con la distancia.
Veremos más adelante que los campos electromagnéticos tienen en general la forma de ondas
esféricas, cuya amplitud decae como el inverso de la distancia 1/r, de forma que la magnitud
del vector poynting decae como 1/r2 . Por supuesto que las ondas planas, si bien son soluciones

---

### Página 21

de las ecuaciones de Maxwell, constituyen sólo un estudio aproximado de los campos electromagnéticos muy distantes de las fuentes. (Por ejemplo, de la radiación producida por el Sol en
la tierra, se puede suponer que la magnitud de los campos es constante). Veremos también que
es posible generar ondas planas teóricamente, pero en la práctica no

---

### Página 22

Ejemplo
En la superficie de la atmósfera terrestre, la magnitud del vector Poynting (en promedio temporal) es hSi = 1,35 × 103 (W/m2 ).
a) Asumiendo que la radiación solar en la superficie de la atmósfera consiste en una onda sinusoidal plana, ¿Cuáles son las magnitudes del campo eléctrico y magnético ?
b) ¿Cual es el promedio temporal de la potencial radiada por el Sol? La distancia media entre
el Sol y la Tierra es R = 1,5 × 1011 m
#### Solución
a) El promedio temporal del vector Poynting esta relacionado con la magnitud del campo
eléctrico según
0 cE02
hSi =
La amplitud del campo eléctrico es entonces
s
s
2 hSi
2 (1,35 × 103 W/m2 )
E0 =
=
= 1,01 × 103 V /m
c0
(3 × 108 m/s) (8,85 × 10−12 C 2 /N m2 )
La magnitud del campo magnético es
B0 =

E0
1,01 × 103 V /m
=
= 3,4 × 10−6 T = 3,4µT
c
3 × 108 m/s

Notar que este campo magnético es menor que el campo magnético terrestre, que varía entre
30 y 60 µ T
b) La potencia total irradiada por el Sol a una distancia R es (en promedio)

2
hP i = hSi 4πR2 = 1,35 × 103 W/m2 4π 1,5 × 1011 m = 3,8 × 1026 W

Por supuesto que aquí hemos supuesto que la radiación emitida por el sol corresponde a
ondas esféricas. La intensidad a una distancia r del Sol es
I = hSi =

hP i
4πr2

la cual decrece como 1/r2

Fig. 15.2: Como veremos más adelante, los campos de radiación en general son ondas esféricas

---

### Página 23

15.2.

Ondas Planas en medios conductores

Veremos que las soluciones para las ondas electromagnéticas planas en medios conductores
difieren bastante en su comportamiento con respecto al caso de un medio dieléctrico perfecto (no
conductor) que vimos anteriormente. Aceptaremos ahora que el medio tenga una conductividad
σ, de forma que existirá una corriente eléctrica en el medio en respuesta al campo eléctrico. Si
el medio es ohmico
~ ~x) = σ E(t,
~ ~x)
J(t,
Claramente seguiremos suponiendo que el medio es lineal, homogéneo e isotrópico, de forma
que las ecuaciones de Maxwell quedan
~ · E(t,
~ ~x) = 0
∇
~
~ × E(t,
~ ~x) = − ∂ B(t, ~x)
∇
∂t
~ · B(t,
~ ~x) = 0
∇
~ × B(t,
~ ~x) = µσ E(t,
~ ~x) + µ ∂ E(t,
~ ~x)
∇
∂t

Al igual que antes, evaluamos

Además



~ · E(t,
~ ~x) − ∇
~ 2 E(t,
~ ~x) = −∇
~ 2 E(t,
~ ~x)
~ ×∇
~ × E(t,
~ ~x) = ∇
~ ∇
∇
~ ×∇
~ × E(t,
~ ~x) = −∇
~ × ∂ B(t,
~ ~x) = − ∂ ∇
~ × B(t,
~ ~x)
∇
∂t
∂t

~ ×∇
~ × E(t,
~ ~x) = − ∂
∇
∂t




∂ ~
∂ ~
∂2 ~
~
~x)
µσ E(t, ~x) + µ E(t, ~x) = −µσ E(t,
~x) − µ 2 E(t,
∂t
∂t
∂t

con esto,la ecuación para el campo eléctrico es
~ ~x) − µ ∂ E(t,
~ ~x) − µσ ∂ E(t,
~ ~x) = 0
~ 2 E(t,
∇
∂t
∂t

Es fácil verificar, siguiendo los mismos pasos, que el campo magnético satisface la misma
ecuación
~ 2 B(t,
~ ~x) = 0
~ ~x) − µ ∂ B(t,
~ ~x) − µσ ∂ B(t,
∇
∂t
∂t
La única diferencia con el caso anterior (propagación en medios dieléctricos perfectos) la
∂ ~
constituye el término µσ ∂t
E(t, ~x). Veremos que la conductividad del medio tendrá como efecto
una atenuación de las ondas a medida que penetra en el material. Nuevamente supondremos
que los campos son de la forma

~ ~x) = E(~
~ x)eiwt
E(t,

---

### Página 24

luego
Definimos




~
~ x)eiwt = 0
∇ + µw − iµσw E(~
k 2 = w2 µ − iµσw

y la ecuación queda de la forma



~ 2 + k 2 E(~
~ x) = 0
∇

Si la propagación es en el eje z, entonces la ecuación a resolver es

 2
∂
~ x) = 0
+ k E(~
∂z 2
cuya solución es, por supuesto
~ x) = E
~ 0 e−ikz
E(~
y entonces la solución completa queda
~ ~x) = E
~ 0 ei(wt−kz)
E(t,
Así

Hay que recordar que k es un número complejo, que escribiremos en la forma k = β − iα.
k 2 = µw2 − iµσw = β 2 − α2 − 2iαβ
se debe resolver
2αβ = µσw → α =
β 2 − α2 = µw2 → β 2 −
β2 −

β =

µ2 σ 2 w 2
= w2 µ
4β

µ2 σ 2 w 2
= w2 µ
4β

β 4 − β 2 w2 µ −

µσw
2β

µ2 σ 2 w 2
=0

p
w 4 µ2  2 + µ2 σ 2 w 2
q
w µ ± w µ 1 + wσ2 2

w2 µ ±

β2 =

Obviamente la solución correcta es con el signo positivo, pues β es real
!
r
 σ 2
µ
β 2 = w2
1+
+1
w
v
!
r
u
 σ 2
u µ
1+
+1
β = wt
w

---

### Página 25

y como
α2 = β 2 − w2 µ
µ
α2 = w 2

r

1+

µ
α2 = w 2
v
u
u µ
α = wt

r

 σ 2
w

!

+1

1+

 σ 2

r

 σ 2

1+

w

− w2 µ
!

−1

w

!

−1

#### Solución
Se concluye que las ondas planas monocromáticas en un medio con conductividad σ son de la
forma
~ z) = E
~ 0 e−αz ei(wt−βz)
E(t,
~ 0 debe
donde hemos asumido que la propagación es en la dirección z, y al igual que antes E
ser un vector perpendicular a z. Notar que la amplitud de la onda es atenuada por un factor
exponencial e−iαz , por lo que α es llamada Constante de atenuación
v
!
r
u
 σ 2
u µ
β = wt
1+
+1
w
v
u
u µ
α = wt

r

1+

 σ 2
w

!

−1

Ésta es la solución exacta para ondas planas monocromáticas en un medio lineal y de conductividad σ. Notar que para un dieléctrico perfecto, la constante de atenuación es cero y se
recupera el caso visto anteriormente
Observación
Este factor exponencial atenuante es el que explica que en ciertos materiales las ondas no se
propaguen correctamente. Por ejemplo, para el agua de mar (que constituye un medio conductor), dentro de un gran rango de frecuencias el factor α es grande, de forma que las ondas
decaen bastante rápido. (Esto explica en parte por qué los submarinos no se comunican mediante ondas electromagnéticas)
La razón física de este factor atenuante radica en la naturaleza misma del medio. Por ser
conductor, existe una gran cantidad de cargas libres que son aceleradas por la prescencia del
campo eléctrico (principalmente, pues ya es sabido que su magnitud es muchísimo mayor a
la del campo magnético). De esta forma, parte de la energía electromagnética que se propaga
es utilizada en trabajo para mover las cargas libres presentes en el medio. Con esto, resulta
natural que la onda electromagnética pierda energía a medida que avanza en el material

---

### Página 26

~ 0 = E0 î. Nuevamente, de la ley de Faraday podemos determinar
Supongamos ahora que E
la relación entre las magnitudes de los campos
~ × E(t,
~ ~x) = − ∂ B(t,
~ ~x)
∇
∂t
∂
~ 0 e−αz ei(wt−βz)
k̂ × E0 e−αz ei(wt−βz) î = −iwB
∂z
~ 0 e−αz ei(wt−βz)
(iβ + α) × E0 e−αz ei(wt−βz) ĵ = iwB

~ 0 = B0 ĵ con
Se obtiene B

B0 =

iβ + α
E0
iw

β − iα
k
E0 = E0
w
w
p
k = w2 µ − iµσw

B0 =
con

B0 =
y entonces

r

iµσ
E0 =
µ −
w
E0
=
B0

o
E0
=
H0

s

r

r

µσ + iwµ
E0
iw

iw
σµ + iwµ

iwµ
=η
σ + iw

Esta razón, que depende de las características del medio (µ, , σ) y de la frecuencia w, se
conoce como impedancia característica del medio. Notar que en general (σ 6= 0) es un
número complejo, esto quiere decir que para medios con conductividad, el campo eléctrico y
magnético no están en fase
La impedancia característica en representación polar es
η =| η | eiϑ
donde
| η |=
y

w
µ

p

(σ 2 + w2 2 )

!1/2

ϑ=

=

µ/
p σ
( w )2 + 1)

!1/2

(π/2 − Arctan(w/σ))
σ
tan 2ϑ =
w

p
µ/
=
 1/4
σ 2
1 + w

---

### Página 27

Con esto, la solución general para ondas planas que se propagan en dirección z queda
~ t) = E0 e−αz ei(wt−βz) ê1
E(z,
E0 −αz i(wt−βz−ϑ)
~
ê2
H(z,
t) =
e e
|η|
e1 × e2 = k̂

La velocidad de propagación es

w
=s
β


q

µ
σ 2
1 + w + 1

2π
=
β

2π
q
µ
1+

c=

y la longitud de onda
λ=

w

15.3.

s




σ 2
+1
w

Solución para buenos conductores

Si la conductividad es grande en el sentido σ >> w, entonces
v
!!
r
u
r
 σ 2
u µ
µσ
β = wt
1+
+1
≈w
w
2w
v
u
u µ
α = wt

r

1+

 σ 2

!!

w

−1

r

wµσ

≈w

r

µσ
2w

Es decir, aproximadamente se tiene
α=β=

w
En términos de la frecuencia en Hertz f = 2π

α=β=

p
πf σ

En este caso los campos son atenuados rápidamente. Se define la profundidad de penetración como la distancia dentro del material a la cual los campos han decaido en un factor
1/e (aproximadamente al 30 % de su valor original)
δ=

=√
α
πf σ

Además, en este caso la impedancia característica queda
r
wµ iπ/4
E0
η=
=
e
σ
H0

Es decir, los campos se encuentran en un desfase de ϑ = π/4

---

### Página 28

~ t) = E0 e−αz ei(wt−βz) ê1
E(z,
E0 −αz i(wt−βz−π/4)
~
e e
ê2
H(z,
t) =
|η|
e1 × e2 = k̂

La velocidad de propagación es

w
c= =
β
y la longitud de onda
λ=

r

2w
= wδ
σµ

2π
2π
= 2πδ
=√
β
πf µσ

Nota: Notar que aquí, la definición de un buen conductor no es una propiedad única del
material, puesto que debe tenerse σ >> w. Es decir, un material se considera buen conductor
en determinado rango de frecuencias.

15.4.

Resumen sobre las ondas planas monocromáticas

Hemos visto que las ecuaciones de Maxwell aceptan como solución campos electromagnéticos
que están descritos matemáticamente por ondas planas. Para una propagación según el eje z,
los campos son de la forma
~ t) = E0 e−αz ei(wt−βz) ê1
E(z,
E0 −αz i(wt−βz−ϑ)
~
ê2
H(z,
t) =
e e
|η|
e1 × e2 = k̂
1. En un dieléctrico perfecto (conductividad nula), la constante de atenuación es cero, y la
impedancia intrínseca es un número real puro
r
E0
E0
µ
η=
=
= √ =c
→
H0

B0
µ
En el espacio vacío, la impedancia intrínseca es
r
µ0
≈ 120π
η=
0
En este caso

~ t) = E0 ei(wt−βz) ê1
E(z,
~ t) = E0 ei(wt−βz) ê2
B(z,
c
e1 × e2 = k̂

---

### Página 29

Con
β=

w
√
= w µ
c

2. En un buen conductor (σ >> w), los campos son fuertemente atenuados a medida que
se propagan en el medio. Aquí, en un análisis aproximado
r
wµσ p
α=β=
= πf σ
la impedancia intrínseca es un complejo con fase π/4 y su magnitud es
r
wµ
| η |=
σ

Los campos son atenuados por un factor 1/e al ingresar una distancia igual a la profundidad
de penetración
δ= = =√
α
β
πf µσ

---

### Página 30

Problema
~ ~x) = Em sin (wt − βz) ĵ en el espacio libre, encuentre D(t,
~ ~x), B(t,
~ ~x) y H(t,
~ ~x). DibuDado E(t,
~ yH
~ en t = 0
je E
#### Solución
Se tiene

~ ~x) = Em sin (wt − βz) ĵ
E(t,

de aquí es inmediato que
~ ~x) = 0 E(t,
~ ~x) = 0 Em sin (wt − βz) ĵ
D(t,
Además, de la ecuación de Maxwell
~
~ × E(t,
~ ~x) = − ∂ B(t, ~x)
∇
∂t
como la propagación es en z, la única derivada parcial espacial para el campo eléctrico que
no es nula es la que involucra z, es decir
~
∂
~ ~x) = − ∂ B(t, ~x)
k̂ × E(t,
∂z
∂t
~
∂
~ ~x) = − ∂ Em sin (wt − βz) î = βEm cos (wt − βz) î = − ∂ B(t, ~x)
k̂ × E(t,
∂z
∂z
∂t
Luego

~ ~x) = − β Em sin (wt − βz) î = − Em sin (wt − βz) î
B(t,
w
c
~ ~x) es, simplemente
Por último, el campo H(t,
~ ~x) = − Em sin (wt − βz) î
~ ~x) = 1 B(t,
H(t,
µ0
µ0 c

~ yH
~ están dados por
En t = 0, los campos E
~ ~x) = −Em sin (βz) ĵ
E(0,
Em
~
H(0,
~x) =
sin (βz) î
µ0 c

---

### Página 31

Problema
~ = Hm ei(wt+βz) î en el espacio libre, encuentre E
~
Dado H
#### Solución
~ representa una onda plana que se
Una forma de resolver este problema es notando que H
propaga en dirección −ẑ. Luego, debe tenerse que el vector poynting tenga esta dirección, lo
cual se logra con un campo eléctrico polarizado según ĵ, en efecto
~=E
~ ×H
~ = E ĵ × H î = −EH k̂
S
Además, se cumple que

E
=√
B
µ0  0

o, equivalentemente
E
=
H
y entonces

r

µ0
βµ0
=
0
w

~ = wµ0 Hm ei(wt+βz) ĵ
E
β

Otra forma, es recordando que el espacio vacío tiene conductividad nula y entonces
~
~ × H = ∂D
∇
∂t
~ × H = ∂ k̂ × H
~ = βHm ei(wt+βz) ĵ
∇
∂z
entonces

~
∂D
= βHm ei(wt+βz) ĵ
∂t
~ = β Hm ei(wt+βz) ĵ
D
w

~ = β Hm ei(wt+βz) ĵ
E
w0
En efecto, es el mismo resultado anterior
√
~ = µ0 0 Hm ei(wt+βz) ĵ = √µ0 Hm ei(wt+βz) ĵ
E
0
µ0  0
~ = wµ0 Hm ei(wt+βz) ĵ
E
β

---

### Página 32

Problema
Dados

~ = 30πei(108 t+βz) î, H
~ = Hm ei(108 t+βz) ĵ
E

en el espacio libre, encontrar Hm y β (β > 0)
#### Solución
Estas son ondas planas que satisfacen las ecuaciones de Maxwell en el vacío, de forma que
w
=√
= 3 × 108 (m/s)
β
µ0  0
Luego
β=
Además

Luego

w
=
=
c
3 × 108

|E|
|E|
=c→
=
|B|
|H|
| Hm |=

r

µ0
= 120π
0

30π
=
120π

Además, las ondas se propagan en la dirección −k̂, por lo que
~ ×H
~ = −k̂
E
entonces
Hm = −

y
~ = 30πei(108 t+ 13 z) î
E
~ = − 1 ei(108 t+ 13 ) ĵ
H

---

### Página 33

Problema
En un medio homogéneo no conductor donde µr = 1, encuentre r y w si
~ = 30πei(wt−(4/3)y) ẑ, H
~ = 1,0πei(wt−(4/3)y) î
E
¿Cuál es la velocidad de la luz en esta región?
#### Solución
Se trata de ondas planas con β = 4/3. Luego
3 × 108
w
= √
=√ =√
β
µ
µ0  r  0
r
Además

E
= 30π =
H

r

Así

Resolviendo

µ
=


r

µ0
= 120π
r 0

r

3 × 108
w
= √
4/3
r
r
30π = 120π
r
r = 16
w = 108 (rad/s)

la velocidad de la luz en este medio es
3 × 108
c= √ = √
=
µ
µ0 160
es un cuarto de la velocidad de la luz en el vacío

r

---

### Página 34

Problema
~ = e−αz ei(wt−βz) î (V /m) con f = 100 Mhz, en la superficie de un conductor de cobre,
Suponga E
σ = 58 M S/m, localizado en z > 0 . Examine la atenuación a medida que la onda se propaga
en el interior del conductor

#### Solución
A una profundidad z, la magnitud del campo eléctrico es
~ |= e−αz = e−z/δ
|E
donde δ = 1/α es la profundidad de penetración
δ=√

= 6,61µm
πf µσ

Es decir, después de 6,61 micrómetros dentro del conductor, el campo es atenuado en 1e , a
un 36,8 % de su valor inicial. A 5δ o 33 micrómetros, la magnitud es 0,67 % de su valor inicial

---

### Página 35

Problema
Para agua de mar con µ = µ0 y conductividad σ ≈ 4,3 (S/m), ¿a qué frecuencia la profundidad
de penetración es de un metro?
#### Solución
Supongamos un rango de frecuencias en el que el agua de mar es considerado un buen conductor,
es decir
σ >> w
(notar que la permitividad del vacío es del orden de 10−12 , y la constante dieléctrica r en
general no es muy grande). La profundidad de penetración está dada por
r
r
=
δ=
µwσ
µ0 wσ
δ2 =

→w=
µ0 wσ
σµ0 δ 2

Se desea δ = 1 (m), entonces
w=
o, en Hertz

= 3,7 × 105
4,3 × 4π × 10−7 12
f=

w
= 58,6 × 103
2π

o sea, una frecuencia de aproximadamente 60 kHz para una profundidad de un metro. Si un
submarino está equipado con un receptor de muy alta sensibilidad y si se utiliza un transmisor
de muy alta potencia, es posible comunicarse con otro submarino sumergido. Sin embargo, debe
utilizarse una frecuencia muy baja, y aún en este caso se produce una atenuación muy fuerte
de la señal. En efecto, a 5 profundidades de penetración (5 metros), la magnitud de los campos
se reduce al 1 % del valor original, y por consiguiente la potencia se reduce al 0,01 % de la
potencia incidente

---

### Página 36

Problema
Una onda plana uniforme que se propaga en un medio determinado, tiene un campo eléctrico
~ z) = 5e−γz ei108 t ĵ
E(t,
Si el medio se caracteriza por
σ = 3,5S/m
r = 1
µr = 18
~ , η y la profundidad de penetración para el medio. ¿Después de recorrer
Determine γ, H
qué distancia la onda se atenúa al 10 % de su valor inicial? ¿Cuál es la velocidad de propagación
en este medio?
#### Solución
Las ondas planas que son solución de las ecuaciones de Maxwell son de la forma
~ z) = E
~ 0 e−ikz eiwt
E(t,
donde
k = β − iα
~ z) = E
~ 0 e−iβz−αz eiwt
E(t,
comparando con
~ z) = 5e−γz ei108 t ĵ
E(t,
se aprecia que se trata de una onda plana a frecuencia w = 108 Hertz, polarizada según ĵ y
con
γ = α + iβ
Notemos que

Se aprecia que

σ
3,5
3,5
=
= 3953,02
=
w
0 × 10
8,854 × 10−12 × 108
σ >> w

de forma que el medio se puede considerar un buen conductor. En este caso
r
108 × 18 ∗ 4π × 10−7 × 3,5
wµσ
α≈β≈
=
= 62,9159
Con esto
γ = 62,9159 + i62,9159 =

62,9159 iπ/4
√
e

La profundidad de penetración es
δ=

= 0,0158942
α

---

### Página 37

La impedancia característica del medio es (en una muy buena aproximación)
s
r
wµ iπ/4
108 × 18 × 4π10−7 iπ/4
η=
e
e
=
= 25,4219eiπ/4
σ
3,5
~ z) está dado por
El campo H(t,
H(t, z) = −

5 −αz i(108 t−βz −π/4)
5 −γz i108 t −iπ/4
î = −
î
e e
e e
e
|η|
|η|

H(t, z) = −0,196681e−62,9159z ei(10 t−62,9159z −π/4) î

La velocidad de propagación está relacionada con la constante de propagación β
β=

w
→c=
= 1, 5895 × 108
c
62,9159

un poco más de la mitad de la velocidad de la luz en el vacío. Por último, para determinar
a que distancia dentro del material la onda se ha atenuado hasta un 10 % de su valor original,
se debe resolver
0,1 = e−αx = e−62,9159x
−2,30258 = −62,9159x
x = 3,65978 × 10−2 = 3,65978cm

---

### Página 38

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 39

#### Capítulo 16
Condiciones de borde en la frontera
Las condiciones que deben satisfacer los campos electromagnéticos en una zona interfacial
que separa dos madios se deducen, por supuesto, de las ecuaciones de Maxwell. La más simple
de obtener es la que cumple la componente normal del campo magnético, y se obtiene a partir
de la ecuación
~ · B(t,
~ ~x) = 0
∇
En cualquier zona interfacial entre dos medios se puede construír una superficie cilíndrica
como se muestra en la figura

Integrando la ecuación de Maxwell sobre el volumen limitado por el cilindro se obtiene
ˆˆ
˚

3 ~
~
~
~ ~x) = 0
d x∇ · B(t, ~x) =   dS(x̂)
· B(t,
V

¨

S1

S(V )

~ ~x) +
dS1 n̂1 · B(t,

¨

S2

~ ~x) +
dS2 n̂2 · B(t,

¨

S3

~ ~x) = 0
dS3 n̂3 · B(t,

~ ~x) es finito, el último
donde S3 es el manto del cilindro, mientras S1 y S2 las tapas. Si B(t,
término se puede anular si h → 0. Además, en este límite (h → 0) las superficies S1 y S2 son
prácticamente las mismas, S1 → S2 , con n̂1 = −n̂2 y entonces
¨
ˆˆ



~
~
~
~
dS
d
S(x̂)
·
B(t,
~
x
)
=
·
B(t,
~
x
)
−
n̂
·
B(t,
~
x
)
=0
n̂

S(V )

S1

~ ~x) − n̂1 · B(t,
~ ~x) = 0
n̂1 · B(t,
Es decir, la componente normal del campo magnético es continua al atravesar un medio

---

### Página 40

B1n = B2n
Ahora veremos que la componente tangencial del campo eléctrico es continua. A partir de
la ecuación
~
~ × E(t,
~ ~x) + ∂ B(t, ~x) = 0
∇
∂t
Integremos esta ecuación sobre una superficie plana rectangular como la de la figura

El contorno de S es el camino Γ indicado en la figura. Utilizando el teorema de Stokes
ˆˆ

 ~
 dS(x̂) ·
S



ˆˆ
 ˛
~ ~x)
∂ B(t,
 ~
~ ~x) = − 
~ × E(t,
~ ~x) = d~x · E(t,
x) ·
∇
 dS(~
∂t
Γ
S

En el caso en que h1 → 0, h2 →

lE1t − lE2t = 0
la integral de superficie por supuesto es nula ya que la superficie total tiende a cero
S →(suponemos que la derivada temporal del campo magnético es finita). De aquí se deduce
~ ~x) debe ser continua al atravesar una interfaz entre dos
que la componente tangencial de E(t,
medios
lE1t = lE2t
Utilizando ahora la primera ecuación de Maxwell
~ · D(t,
~ ~x) = ρ(t, ~x)
∇
y utilizando la misma superficie para el caso del campo magnético (cilindro de altura h) se
obtiene
˚
˚
3 ~
~
d x∇ · D(t, ~x) =
d3 xρ(~x)
V

V




¨

ˆˆ

V (S)

~ x) · D(t,
~ ~x) =
dS(~

d3 xρ(~x)

V

si h → 0, entonces
(D1n − D2n ) A = σA
donde A es la superficie de las tapas, y σ es la densidad superficial de carga en la frontera
~ ~x) es discontinua al
que divide a los dos medios. Así, la componente normal del campo D(t,
atravesar una superficie cargada

---

### Página 41

D1n − D2n = σ
o, equivalentemente para medios lineales
1 E1n − 2 E2n = σ
Por último, de la ecuación
~ × H(t, ~x) = J(t,
~ ~x) + ∂D(t, ~x)
∇
∂t
y utilizando la misma superficie de integración que el caso del campo eléctrico, se obtiene
ˆˆ
ˆˆ

 ˆˆ
∂D(t, ~x)
 ~
 ~
 ~
~
x) · ∇ × H(t, ~x) =  dS(~x) · J(t, ~x) +  dS(~
x) ·
 dS(~
∂t
S
S
S
ˆˆ
ˆˆ
˛
∂D(t, ~x)
 ~
 ~
d~x · ×H(t, ~x) =  dS(~x) · J(t, ~x) +  dS(~
x) ·
∂t
Γ
S
S
~ es finita
Si nuevamente h1 y h2 tienden a cero, y la derivada temporal del campo D
~ ~x) · n̂
H1t − H2t = J(t,

~ ~x)
donde n es la perpendicular a la superficie S. Es decir, la componente tangencial de H(t,
es discontinua al atravesar un medio con densidad de carga superficial en la interfaz.
Resumen
Al atravesar una interfaz entre dos medios (1 y 2), los campos electromagnéticos satisfacen
B1n = B2n
E1t = E2t
D1n − D2n = σ
H1n − H2n = J~ · n̂

---

### Página 42

16.1.

Condiciones de Borde para incidencia normal

Las ondas electromagnéticas que se propagan en materiales generalmente entran en el material a través de una frontera entre éste y otro medio, que puede ser aire o vacío. Aquí utilizaremos
las condiciones de borde que satisfacen los campos para el caso de ondas que inciden normalmente sobre una interfaz. (Esto significa que la dirección de propagación es perpendicular a
la frontera). Veremos que la onda incidente será acompañada por una onda reflejada y una
transmitida. Consideremos el caso que se muestra en la figura

~ i (x, z), H
~ i (y, z)) que se desplaza en el sentido positivo de z,
Se aprecia una onda incidente (E
~ r (y, z) describen la onda reflejada que se desplaza en el sentido negativo
~ r (x, z), H
los campos E
~ t (x, z), H
~ t (y, z) describen la onda transmitida. La interfaz es el plano z = 0, con el
de z, y E
medio 1 a la izquierda y el medio 2 a la derecha. Más concretamente
~ i (t, z) = E i e−ikz eiwt î
E
~ r (t, z) = E r eikz eiwt î
E
~ t (t, z) = E t e−ikz eiwt î
E
~ i (t, z) = H i e−ikz eiwt ĵ
H
~ r (t, z) = −H r eikz eiwt ĵ
H
~ t (t, z) = H t e−ikz eiwt ĵ
H

Estas son ondas planas que se propagan en dirección z. Son soluciones a las Ecuaciones de
Maxwell si
k = β − iα
Con α y β encontrados anteriormente (Son propiedad de la frecuencia y del medio en el cual
se propagan las ondas). Interesa determinar que relación se cumple entre las magnitudes de
los campos incidentes, reflejados y transmitidos. Para ello, usaremos el hecho de que el campo
eléctrico debe ser continuo en z = 0 (es completamente transversal a la interfaz). Esto significa
~ r (t, 0) = E
~ t (t, 0)
~ i (t, 0) + E
E
o bien
Ei + Er = Et
~ z) es también
Además, si no hay una corriente superficial en la interfaz, el campo H(t,
continuo en z = 0
~ r (t, 0) = H
~ t (t, 0)
~ i (t, 0) + H
H

---

### Página 43

o bien
Hi − Hr = Ht
~ y H
~ están dadas por las impedancias
Además, para cada onda las magnitudes entre E
intrínsecas del medio. En resumen, se debe resolver lo siguiente
Ei + Er = Et
Hi − Hr = Ht
Ei
Er
=
η
=
Hi
Hr
Et
= η2
Ht

Utilizando la última junto a las dos primeras se obtiene lo siguiente
Ei + Er
Et
=
η
=
Ht
Hi − Hr
Ei + Er
(E i − E r )
η1

η2 = 1
η2 = η 1

Ei + Er
→ E i (η2 − η1 ) = E r (η1 + η2 )
Ei − Er

Finalmente
r

E =E

i



η2 − η 1
η1 + η 2




2η2
E =E
η 1 + η2


η 2 − η1
r
i
H =H
η 1 + η2


2η1
t
i
H =H
η1 + η 2
t

i



~ r = 0, H
~ r = 0, lo cual es evidente pues en este caso
Es inmediato que si η1 = η2 , entonces E
no existe ninguna interfaz. Recordar que la impedancia de un medio está dada en general por
r
iwµ
η=
σ + iw0
Para un buen conductor
r
wµ iπ/4
η≈
e
σ
Para un medio dieléctrico perfecto (conductividad nula)
r
µ
η=


---

### Página 44

Para el espacio vacío
η=

16.1.1.

r

µ0
= 120π
0

Incidencia Normal en un conductor perfecto: Ondas estacionarias

Un caso particular interesante de la ley de reflexión y transmisión en una interfaz para
ondas que inciden normalmente es cuando el medio 2 es un conductor perfecto. En este medio,
la impedancia intrínseca tiende a cero
r
iwµ
lím η2 = lím
=0
σ→∞
σ→∞
σ + iw0
Luego, se cumple
r

E =E

i



−η1
η1



= −E i

Et = 0


−η1
r
i
= −H i
H =H
η1
Ht = 0

Es decir, la onda es completamente reflejada. Veremos que esta condición da origen a la
creación de una onda estacionaria. El campo eléctrico total queda
~ r (t, z)
~ z) = E
~ i (t, z) + E
E(t,
~ z) = E i e−ikz eiwt î − E i eikz eiwt î
E(t,
~ z) = E i eiwt î e−ikz − eikz
E(t,



Si el medio 1 es un dieléctrico perfecto, entonces k = β (α = 0)

~ z) = E i eiwt î e−iβz − eiβz = −2i sin(βz)E i eiwt î
E(t,

Tomando la parte real

~ z) = 2E i sin(βz) sin(wt)î
E(t,

Esta es una onda que se anula para valores determinados de z (∀t), dados por
z=

wnπ
fn
nπ
=
=
β
c
2λf

n
, n = 0, ±1, ±2, ...
2λ
donde λ es la longitud de onda en el medio 1. Por otra parte, el campo eléctrico se anula
para todo t tal que
z=

---

### Página 45

nπ
, n = 0, ±1, ±2, ...
w
Esta onda es llamada estacionaria puesto que no se propaga, sino que simplemente oscila
en el espacio y el tiempo.
sin wt = 0 → t =

Para el campo magnético se tiene
~ r (t, z)
~ z) = H
~ i (t, z) + H
H(t,
~ z) = H i e−iβz eiwt ĵ + H i eiβz eiwt ĵ
H(t,

~ z) = H i eiwt ĵ e−iβz + eiβz = 2H i eiwt cos(βz)ĵ
H(t,

tomando la parte real

~ z) = 2H i cos(βz) cos wtĵ
H(t,
Se anula para


π
1 π
βz = + nπ → z = n +
2 β


n 1
λ, n = 0, ±1, ±2, ...
z=
+
2 4
Además, se aprecia que se anula para todo t tal que
cos wt = 0
Se aprecia que para ondas estacionarias, el campo eléctrico y magnético están en un desfase
de π/2

Fig. 16.1: Ondas estacionarias se pueden lograr al confinar ondas electromagnéticas entre dos
planos perfectamente conductores

---

### Página 46

Problema
~ 1 = 1,2î + 0,8ĵ + 0,4k̂ (T). Encuentre H
~ 2 (H
~ en z = +0) y los
En la región 1 de la figura, B
ángulos entre los campos y una tangente a la superficie

#### Solución
Se tiene

~ 1 = 1,2î + 0,8ĵ + 0,4k̂
B

la componente normal del campo magnético a una superficie es siempre continua, es decir
~ 2 · ẑ
~ 1 · ẑ = B
B
se desprende que el campo magnético en z = 0+ es de la forma
~ 2 = B2x î + B2y ĵ + 0,4k̂
B
Además, en la regiòn 1 la permeabilidad está dada por
µ1 = µr1 µ0 = 15µ0
~ en z = 0− es
de forma que el campo H
~1 =
H


1 ~
1 
1,2î + 0,8ĵ + 0,4k̂
B1 =
15µ0
15µ0

~ es continua al atravesar una superficie sin densidad de
La componente tangencial de H
~ en z = 0+ es de la forma
carga superficial. Suponiendo que éste es el caso, el campo H

1 
~
1,2î + 0,8ĵ + H2z k̂
H2 =
15µ0
En resumen

Además

~ 2 = B2x î + B2y ĵ + 0,4k̂
B


~2 = 1
H
1,2î + 0,8ĵ + H2z k̂
15µ0
~2 = 1 B
~2
~2 = 1 B
H
µ2
µ0

luego
B2x = µ0 H2x =

1,2

---

### Página 47

B2y = µ0 H2y =

0,8

B2z = µ0 H2z = 0,4 → H2z =
Finalmente
~2 =
H

0,4
µ0

 0,4
1 
k̂
1,2î + 0,8ĵ +
15µ0
µ0

---

### Página 48

Problema
~ de 500 Mhz viaja por el espacio libre e incide perpendicularmente sobre un medio
Un campo E
parcialmente conductor como se ilustra en la figura. Si la amplitud del campo incidente es
~ i0 = 100 V /m, determine
E
a) Las amplitudes de las ondas una vez atravesado completamente el medio (Et0 , Ht0 )
b) La potencia temporal que porta la onda incidente
c) La potencia temporal que porta la onda transmitida nuevamente al espacio

#### Solución
Definimos el eje ẑ como se indica en la figura, donde el origen coincide con el extremo izquierdo
del medio parcialmente conductor

La onda incidente está descrita por
~ i = Ei0 ei(5×108 t−βz) î, z < 0
E
donde la constante de propagación en el vacío está dada por
β=

w
√
= 5 × 108 µ0 0
c

Al incidir normalmente sobre el medio conductor, parte de la onda se refleja, y otra es
transmitida hacia el medio. Si Em0 es la amplitud de la onda transmitida en la interfaz (z = 0),
entonces se cumple


2ηm
Em0 = Ei0
η0 + η m

---

### Página 49

donde ηm es la impedancia intrínseca del medio conductor
s
r
iwµ
i5 × 108 µ0
η2 =
=
σ + iw
1 + i5 × 108 550
η2 = 44,5594 + i13,2865
El que sea un número complejo implica que existirá un desfase entre la onda incidente y la
onda transmitida al medio. η0 es la impedancia intrínseca del vacío
r
µ0
η0 =
= 120π
0
Así, para Ei0 = 100
Em0 = 21,3182 + i5,63173i = 22,0495ei0,258274
Con esto, la onda transmitida al medio parcialmente conductor está descrita por
~ m (t, z) = Em0 e−αm z ei(wt−βm z) , 0 < z < 30 × 10−3
E
~ m (t, z) = 22,0495e−αm z ei(5×108 t−βm z+0,258274) , 0 < z < 30 × 10−3
E
donde la constante de atenuación (αm ) en este medio está dada por
v
!
r
u
 σ 2
u µ
1+
−1
αm = wt
w

Así

v

s
u

2
u
u µ0 550 
1+
− 1 = 24,26005
αm = 5 × 108 t
5 × 108 550

~ m (t, z) = 22,0495e−24,26005z ei(5×108 t−βm z+0,258274) , 0 < z < 30 × 10−3
E

La magnitud del campo en z = 30 × 10−3 es
Emt = 22,0495e−24,26005×30×10

−3

= 10,6491

Si Et0 es la amplitud del campo eléctrico transmitido nuevamente al vacío, se cumple


2η0
Et0 = Emt |
|= 19,0375
η0 + η m

~ se relaciona con la del campo eléctrico según
la amplitud del campo H
Et0
= η0
Ht0
Ht0 =

η0
= 0,0504984
Et0

---

### Página 50

b) El promedio temporal del vector Poynting de la onda incidente es
D E
~i = Ei0 k̂ = 13,2629k̂(W/m2 )
S
2cµ0
c) Para la onda transmitida nuevamente al vacío
D E
~t = Et0 k̂ = 0,480681k̂(W/m2 )
S
2cµ0

---

### Página 51

Problema
Se requiere que Ud. haga una estimación de la intensidad de campo eléctrico, en V /m, que
requerirría generar un radar de 2 Ghz de penetración de suelo, con el objeto de detectar piezas
metálicas de gran tamaño, enterradas a una profundidad de hasta 2 metros. Dependiendo de
la composición y la humedad del terreno, este puede tener el siguiente rango de parámetros
10−4 ≤ σ ≤ 10−2
3 ≤ rt ≤ 8
µrt = 1
Por otra parte se estima que las piezas enterradas tienen el siguiente rango de parámetros
107 ≤ σm ≤ 6 × 107
1 ≤ µrm ≤ 7000
rm = 1
Se requiere saber que intensidad de campo eléctrico en V /m se requiere en el aire, sobre
la superficie del terreno, para detectar en el aire sobre la superficie del terreno, un rebote del
objeto metálico que tenga una amplitud de 1V /m, asumiendo incidencia normal
#### Solución
Para estimar la intensidad mínima de campo eléctrico que debe generar el radar, debemos
suponer la peor situación posible. Supondremos que hay una pieza metálica situada a 2 m de
profundidad en la tierra. El caso menos favorable para la propagación en la tierra es cuando ésta
presenta su máxima conductividad (mayor atenuación). Más aún, para que ésta se comporte
como un buen conductor (atenuante) debe tenerse σt >> wt , de forma que consideramos el
caso de mayor conductividad y menor constante dieléctrica.
La reflexión en la placa metálica será buena en la medida que ηm (impedancia intrínseca del
metal) sea lo más pequeña posible. De esta forma, el peor de los casos para la reflexión en la
pieza metálica ocurre cuando ηm toma su máximo valor posible, y entonces cuando posee la
menor conductividad y la mayor permeabilidad magnética.

~ i (campo emitido por el radar en la
En la figura de arriba se aprecia una onda incidente E
~ ti , que se propaga en dirección −z, esta onda
superficie), y una onda transmitida en la tierra E
será reflejada por la pieza metálica en z = 0

---

### Página 52

En esta figura se muestra el campo que se ha reflejado en el metal y se propaga hacia la
~ rm , y la onda recibida finalmente en la superficie, llamada E
~ t.
superficie, que llamaremos E
Sabemos que esta última tiene una magnitud de Et = 1 (V /m). La magnitud de la onda
reflejada en el metal se describe por
Erm (z) = Er0 e−αz
donde α es el coeficiente de atenuación en la tierra
v
s

u
2

u
σt
u µt  t 
α = wt
1+
− 1
wt

con w = 2 × 109 Hz, σt = 10−2 (S/m), µt = 4π10−7 = µ0 , t = rt 0 = 3 × 8,854 × 10−12 .
Reemplazando estos valores
α = 1,08742
Debido a las condiciones de contorno en la interfaz (z = 2), se cumple
Et = 1 = E |

2η0
|
η0 + ηt

~ rm en z = 2, y η0 es la impedancia intrínseca del aire,
donde E es la magnitud del campo E
considerada igual a la del vacío.
r
µ0
η0 =
= 120π
0
y la impedancia intrínseca de la tierra
r
iwµ0
= 217,434 + i3,2564
ηt =
σt + iw0 rt
con esto se obtiene
E=|

η0 + η t
|= 0,788393V /m
2η0

Además
E = Erm (z = 2) = Er0 e−α2 = Er0 e−1,08742×2
de donde la magnitud de la onda reflejada en el metal en z = 0 es
Er0 = Ee1,08742×2 = 6,93842V /m

---

### Página 53

~ ti que fue transmitida a la
Ahora, esta onda reflejada en el metal proviene de la onda E
tierra. La magnitud de esta última se puede expresar como
Eti = E0 eαz
donde E0 (magnitud en z = 0) está relacionada con Er0 mediante
Er0 = E0 |

ηm − ηt
|
η m + ηt

donde la impedancia intrínseca de la pieza de metal es
r
iwµ0 µm
ηm =
σm + iw0 m
con w = 2 × 109 Hz, σm = 107 (S/m), µm = 700, m = 1 resulta
ηm = 2,35095 + i2,35095
Notar que es un complejo con fase π/4, que es lo que se obtiene para un buen conductor.
Con todo esto
E0 = Er0 |

ηm + ηt
|= 7,09235
ηm − ηt

Justo en z = 2, la magnitud de la onda transmitida a la tierra es
Eti (2) = E0 eαz = 7,09235e1,08742×2 = 62,4177V /m
Si Ei es la magnitud de la onda que emite el radar en la superficie, entonces se cumple
Eti (2) = Ei |

2ηt
|
ηt + η0

Ei = 62,4177 |

ηt + η 0
|
2ηt

Ei = 85,3109
Es decir, se requiere emitir un campo de magnitud aproximadamente Ei = 85, 3 (V /m)

---

### Página 54

16.2.

Reflexión y Refracción en la frontera de dos medios
dieléctricos. Incidencia Oblicua

Un caso más general que el discutido en la sección de incidencia normal es el de la reflexión
y refracción de una onda plana que incide oblicuamente por el plano de una zona interfacial de
un dieléctrico. La situación está descrita por la siguiente figura

El sistema de coordenadas que utilizaremos se ilustra en la figura. Los medios sobre y bajo
el plano z = 0 están caracterizados por permitividades y permeabilidades {1 , µ1 } y {2 , µ2 }
respectivamente. Una onda plana con vector de onda ~ki y frecuencia w incide desde el medio
1. La onda refractada y reflejada tienen vectores de onda ~kt y ~kr , respectivamente, y ûn es
un vector unitario normal dirigo desde el medio 1 al medio 2. (En el dibujo, concide con la
dirección z). La onda incidente está descrita por
~ i (t, ~x) = E
~ 0 ei(wt−~ki ·~x)
E
!
~ki × E
~i
~ i (t, ~x) =
H
η1
β1
donde ~ki es la dirección de propagación de la onda incidente, cuya magnitud es ki = β1 =
√
w
~ 0 debe tener una dirección perpendicular a ~ki (las ondas electro= µ1 1 w. Además E
c1
magnéticas son transversales). Para la onda refractada

con kt = β2 = cw2 =

√

~ t (t, ~x) = E
~ t ei(wt−~kt ·~x)
E
!
~kt × E
~t
~ t (t, ~x) =
H
η2
β2
2 µ2 w. Por último, la onda reflejada está descrita por
~ 0 ei(wt−~kr ·~x)
~ r (t, ~x) = E
E
!
~kr × E
~r
~ r (t, ~x) =
H
η1
β1

notar que la magnitud del vector de onda reflejada es igual al de la incidente, kr = β1 .
La existencia de condiciones de borde en la interfaz z = 0, que se deben satisfacer para
todos los puntos en el plano en todo instante, implica que la variación espacial (y temporal) de

---

### Página 55

los campos debe ser la misma en z = 0. De esta forma, las ondas reflejadas y refractadas deben
tener la misma frecuencia w que la incidente si las condiciones en la frontera se satisfacen para
todo t. Además, debe tenerse que las 3 ondas deben tener la misma fase en z = 0






~ki · ~x
~
~
= kt · ~x
= kr · ~x
z=0

z=0

z=0

De aquí se aprecia que los tres vectores de onda deben permanecer en un plano, llamado
plano de incidencia. En la figura, corresponde al plano x − z. Esta condición se puede
reescribir en términos de los ángulos de incidencia ϑi , de reflexión ϑr y de refracción ϑt . Notar
que ningún vector de onda tiene componente según j, luego


~ki · ~x = (kix x + kiz z)
= kix x = ki sin ϑi x
z=0

análogo para el resto, así

ki sin ϑi x = kr sin ϑr x = kt sin ϑt x
ki sin ϑi = kr sin ϑr = kt sin ϑt
Como ki = kr , se obtiene que el ángulo de incidencia es igual al ángulo de reflexión
sin ϑi = sin ϑr
Además, se obtiene la ley de Snell
ki sin ϑi = kt sin ϑt
r
sin ϑi
 2 µ2
kt
=
=
sin ϑt
ki
 1 µ1
r
sin ϑi
 2 µ2
c1
=
=
sin ϑt
 1 µ1
c2

16.2.1.

Polarización paralela y perpendicular
ϑi , ϑr , ϑt
~ki , ~kr , ~kt
~ i, E
~ r, H
~ r, E
~ t, H
~t
~ i, H
E
