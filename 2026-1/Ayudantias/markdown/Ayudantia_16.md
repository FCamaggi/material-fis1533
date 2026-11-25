---
title: "Ayudantia 16"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_16.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_16_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 16

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 16
Circuitos y leyes de Kirchhoff

#### Problema 1
Una batería real puede modelarse por una f.e.m. ε ideal y una resistencia interna en serie R. Una
resistencia de carga R2 se conecta a los terminales de la batería.

a) Determine el valor de R2 tal que la diferencia de potencial aplicada a los terminales sea
máxima
b) Determine el valor de R2 para obtener una corriente máxima en el circuito
c) Determine el valor de R2 para que la potencia consumida por ésta sea la máxima posible
d) Determine el valor de R para que la potencia consumida por R2 sea la máxima posible
#### Problema 2
Considere la línea gráfica de l metros de largo y resistencia por unidad de largo r. Esta línea
tiene una falla de resistencia R en algún punto. Demuestre que la corriente mínima que leería un
amperímetro ideal depende de que la falla se encuentre en medio de la línea telegráfica.

---

### Página 2

#### Problema 3
Obtenga la resistencia equivalente del siguiente sistema, utilice leyes de Kirchhoff.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 16
Circuitos y leyes de Kirchhoff

#### Problema 1
Una batería real puede modelarse por una f.e.m. ε ideal y una resistencia interna en serie R. Una
resistencia de carga R2 se conecta a los terminales de la batería.

a) Determine el valor de R2 tal que la diferencia de potencial aplicada a los terminales sea
máxima
b) Determine el valor de R2 para obtener una corriente máxima en el circuito
c) Determine el valor de R2 para que la potencia consumida por ésta sea la máxima posible
d) Determine el valor de R para que la potencia consumida por R2 sea la máxima posible

#### Solución
Para esto tenemos que usar ley de mallas, la idea de esta ley es que todo el potencial que entregue
la batería debe ser utilizado por los componentes (Esta es una primera idea que sirve para entender
la ley) de esta forma,

---

### Página 2

Vbateria - VR - VR2 = 0
ε - IR - IR2 = 0
Despejando la corriente,
I“

ε
R ` R2

Como esta corriente es igual para todos los componentes del circuito (Están todos conectados en
serie) podemos calcular la diferencia de potencial entre los extremos de la batería (Recordar que la
resistencia R es parte de la batería),
V = IR2 = 

R2 ε
ε
“
R ` R2
1 ` R{R2

Como podemos ver, este potencial es máximo cuando R2 Ñ 8
Teníamos que la intensidad de corriente era,
I“

ε
R ` R2

La cual es máxima cuando R2 = 0, es decir, provocando un cortocircuito en los terminales de la
batería.
La potencia de una resistencia se puede calcular de forma directa,
P = IV = 

R2 ε
ε
R 2 ε2
“
R ` R2 R ` R2
pR ` R2 q2

Recordando como maximizamos una función,
dP
ε2 pR ` R2 q2 ´ 2pR ` R2 qR2 ε2
“
“0
dR2
pR ` R2 q4
Resolviendo la ecuación para R2 encontramos que para que la potencia disipada sea máxima, debe
cumplirse que,
R2 = R
La existencia de la resistencia R hace que se pierda voltaje en la resistencia R2 , y como la potencia
es directamente proporcional al voltaje, necesitamos que R = 0 para que la potencia disipada por
R2 sea máxima.

---

### Página 3

#### Problema 2
Considere la línea gráfica de l metros de largo y resistencia por unidad de largo r. Esta línea
tiene una falla de resistencia R en algún punto. Demuestre que la corriente mínima que leería un
amperímetro ideal depende de que la falla se encuentre en medio de la línea telegráfica.

#### Solución
Si llamamos I a la corriente que pasa por R y de igual forma I1 pI2 q a la que pasa por R1 pR2 q, la
ley de nodos nos dice que se cumple la siguiente relación,

I1 = I ` I2
I = I1 - I2
Siguiendo con el típico análisis de circuitos, escribimos la ley de mallas para los dos caminos que
vemos en la imagen del enunciado, dando como resultado,

V - rxI1 - RpI1 - I2 q = 0
I2 rpℓ - xq ` RpI2 - I1 q = 0
De la primera ecuación obtenemos que,
I1 “

V ` RI2
R ` rx

reemplazando esta cantidad en la segunda ecuación, obtenemos la expresión final para la corriente
que pasa por el amperímetro,
I2 “

RV
Rrl ` r2 xpl ´ xq

Como queremos que sea mínima, queremos buscar que el denominador sea máximo,

(1)

---

### Página 4

d
pRrl ` r2 xl - r2 x2 q = r2 l - 2r2 x = 0
dx

(2)

lo que da como resultado final,
x“

l

#### Problema 3
Obtenga la resistencia equivalente del siguiente sistema, utilice leyes de Kirchhoff.

#### Solución
Queremos encontrar la resistencia equivalente entre los terminales a y b. Para ello usaremos las
leyes de Kirchhoff.
Supongamos que conectamos una fuente de voltaje V entre los terminales a y b, de modo que
Va = V,

Vb = 0.

Definimos dos nodos internos:
V1 : nodo entre las dos resistencias centrales,
V2 : nodo entre la resistencia central derecha y la resistencia hacia b.
El circuito tiene cinco resistencias, todas de valor R. Las conexiones son:
Entre Va y V1 hay una resistencia R.

---

### Página 5

Entre V1 y V2 hay una resistencia R.
Entre V2 y Vb hay una resistencia R.
Entre Va y V2 hay una resistencia R, correspondiente a la rama superior.
Entre V1 y Vb hay una resistencia R, correspondiente a la rama inferior.
Aplicamos la ley de corrientes de Kirchhoff en el nodo V1 . La suma de corrientes que salen del
nodo debe ser cero:
V1 ´ Va V1 ´ V2 V1 ´ Vb
`
`
“ 0.
R
R
R
Como Va = V y Vb = 0, tenemos
V1 ´ V
V1 ´ V2 V1
`
`
“ 0.
R
R
R
Multiplicando toda la ecuación por R, queda
V1 - V ` V1 - V2 ` V1 = 0.
Agrupando términos,
3V1 - V2 = V.
Ahora aplicamos la ley de corrientes de Kirchhoff en el nodo V2 :
V2 ´ V1 V2 ´ Vb V2 ´ Va
`
`
“ 0.
R
R
R
Usando nuevamente Va = V y Vb = 0, queda
V2 ´ V1 V2 V2 ´ V
`
`
“ 0.
R
R
R
Multiplicando por R,
V2 - V1 ` V2 ` V2 - V = 0.
Por lo tanto,
3V2 - V1 = V.
Así, obtenemos el siguiente sistema de ecuaciones:

---

### Página 6

#
3V1 - V2 = V,
´V1 ` 3V2 = V.
Restamos ambas ecuaciones:
p3V1 - V2 q - p´V1 ` 3V2 q = V - V.
Entonces,
4V1 - 4V2 = 0.
De aquí se obtiene
V1 = V2 .
Reemplazando esto en la primera ecuación,
3V1 - V1 = V,
2V1 = V,
y por lo tanto
V1 “

V
.

Como V1 = V2 , también se tiene
V
.
Ahora calculamos la corriente total I que entrega la fuente desde el terminal a. Desde el nodo a, la
corriente puede salir por dos resistencias:
V2 “

I“

Va ´ V1 Va ´ V2
`
.
R
R

Como Va = V , V1 = V {2 y V2 = V {2, entonces
V ´ V2
V ´ V2
I“
`
.
R
R
Por lo tanto,
I“

V

R

`

V

R

.

---

### Página 7

I“

V
V
`
.
2R 2R
I“

V
.
R

La resistencia equivalente se define como
Req “

V
.
I

Luego,
V
Req = V .
R

Finalmente,
Req = R .
Comentario: Si eliminamos la resistencia central obtenemos un circuito mucho más simple de
resolver, pero con el mismo resultado. ¿Por qué pareciera que podemos ignorar la resistencia
central?
