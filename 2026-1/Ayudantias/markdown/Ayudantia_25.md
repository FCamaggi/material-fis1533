---
title: "Ayudantia 25"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_25.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_25_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 25

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 25
Ley de Ampere

#### Problema 1
Imagine un cilindro macizo de radio a por el que = baja” una corriente estacionaria I, calcule el
campo magnético dentro y fuera de esta configuración en los dos siguientes casos:
La corriente está uniformemente distribuida a lo largo del manto del cilindro.
La corriente está distribuida de tal manera que J es proporcional a s, la distancia al eje del
cilindro.
#### Problema 2
Calcule el campo magnético dentro de un solenoide de N vueltas, largo l, que conduce una corriente estacionaria I.
Para simplificar el cálculo asumimos que l debe ser muy grande comparado al radio del solenoide.
¿Por qué necesitamos esto? Imagine la situación para un l cualquiera, piense cómo se ve el campo
fuera del solenoide en este caso, luego piense qué sucede si l es muy grande.

#### Problema 3
Se tienen dos corrientes, ambas con igual sentido (en el dibujo, saliendo de la hoja). Una de ellas
circula por el plano infinito y tiene magnitud Js , y la otra es una corriente cilíndrica infinitamente
larga cuya densidad es
´
r¯
J = J0 1 ´
.
R

---

### Página 2

Se define al punto P como el punto ubicado a distancia R{2 del centro del cilindro, por el eje de
simetría que es perpendicular al plano:

a) Encuentre el campo magnético, en P , generado por Js .
b) Encuentre el campo magnético, en P , generado por J.
c) Encuentre el valor de J0 pJs q, que hace que el campo magnético resultante en el punto P sea
nulo.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 25
Ley de Ampere

#### Problema 1
Imagine un cilindro macizo de radio a por el que = baja” una corriente estacionaria I, calcule el
campo magnético dentro y fuera de esta configuración en los dos siguientes casos:
La corriente está uniformemente distribuida a lo largo del manto del cilindro.
La corriente está distribuida de tal manera que J es proporcional a s, la distancia al eje del
cilindro.

#### Solución
Usaremos la ley de Ampère:
¿
⃗ ¨ d⃗l “ µ0 Ienc ,
B
donde Ienc es la corriente encerrada por el camino de integración.
Caso 1: Corriente distribuida en el manto (superficie)
Como la corriente I⃗ está solo en la superficie (manto), no hay corriente dentro del cilindro. Por lo
tanto:
Ienc = 0,

para s < a.

Por la ley de Ampère, el campo magnético dentro del cilindro es
⃗
Bpsq
“ ⃗0,

s < a.

---

### Página 2

Para s ě a, toda la corriente está encerrada, entonces
⃗ ¨ d⃗l = B(s) ¨ 2πs = µ0 I,
lo que da
µ0 I
⃗
ϕ̂,
Bpsq
“
2πs

s ě a,

donde ϕ̂ es el vector unitario tangencial (en dirección azimutal).
Caso 2: Densidad de corriente proporcional a s
La densidad de corriente es
⃗ = ksẑ,
Jpsq
donde k es una constante y la corriente está en dirección axial ẑ.
La corriente total es
ża
I“

ża
s2 ds = 2πk

J(s) ¨ 2πs ds = 2πk

a3
,

de donde
k“

3I
.
2πa3

Para s < a, la corriente encerrada es
żs

s3
s3
Ienc = 2πk s ds = 2πk = I 3 .
a

Aplicando la ley de Ampère,
µ0 I 2
s3
⃗
Bpsq ¨ 2πs “ µ0 Ienc “ µ0 I 3 ùñ Bpsq
“
s ϕ̂,
a
2πa3
Para s ě a,
µ0 I
⃗
Bpsq
“
ϕ̂.
2πs

s < a.

---

### Página 3

Resumen final

⃗
Bpsq
“

$
⃗0,
’
’
’
’
’
’
’
’
µ0 I
’
’
’
& 2πs ϕ̂,

corriente en el manto, s < a,
corriente en el manto, s ě a,

’
µ0 I 2
’
’
s ϕ̂,
’
’
’
2πa3
’
’
’
’
’
% µ0 I ϕ̂,
2πs

densidad proporcional a s, s < a,
densidad proporcional a s, s ě a.

#### Problema 2
Calcule el campo magnético dentro de un solenoide de N vueltas, largo l, que conduce una corriente estacionaria I.
Para simplificar el cálculo asumimos que l debe ser muy grande comparado al radio del solenoide.
¿Por qué necesitamos esto? Imagine la situación para un l cualquiera, piense cómo se ve el campo
fuera del solenoide en este caso, luego piense qué sucede si l es muy grande.

#### Solución
Para determinar el campo magnético dentro de un solenoide, utilizamos la ley de Ampère:
⃗ ¨ d⃗l “ µ0 Ienc ,
donde Ienc es la corriente encerrada por el camino de integración.
Para aprovechar la simetría, elegimos un camino rectangular para la integral de Ampère:
Un lado dentro del solenoide, paralelo a su eje, de longitud h.
Un lado fuera del solenoide, también paralelo al eje, de longitud h.
Dos lados perpendiculares al eje, que se suponen con contribución nula al integral por simetría.

---

### Página 4

Dentro del solenoide, el campo magnético es aproximadamente uniforme y paralelo al eje del
⃗ = B ẑ.
solenoide, denotado como B
El lado dentro del solenoide contribuye
ż
⃗ ¨ d⃗l = Bh,
interior

donde h es la longitud del lado elegido.
El lado fuera del solenoide tiene un campo magnético despreciable (asumiendo solenoide muy largo), por lo que su contribución es aproximadamente cero.
El número de vueltas que atraviesan el camino de integración es
N
h.
l
Cada vuelta transporta corriente I, por lo que la corriente encerrada es
nh “

Ienc = nhI = 

N
hI.
l

Por la ley,
Bh “ µ0 Ienc “ µ0

N
hI,
l

y cancelando h,
N
I.
l
- El campo magnético dentro del solenoide es uniforme y está dado por
B “ µ0

⃗ “ µ0 N I ẑ.
l
- El supuesto de l " r asegura que los extremos del solenoide no contribuyan significativamente al
campo magnético dentro, haciendo válida esta aproximación.

---

### Página 5

#### Problema 3
Se tienen dos corrientes, ambas con igual sentido (en el dibujo, saliendo de la hoja). Una de ellas
circula por el plano infinito y tiene magnitud Js , y la otra es una corriente cilíndrica infinitamente
larga cuya densidad es
´
r¯
.
J = J0 1 ´
R
Se define al punto P como el punto ubicado a distancia R{2 del centro del cilindro, por el eje de
simetría que es perpendicular al plano:

a) Encuentre el campo magnético, en P , generado por Js .
b) Encuentre el campo magnético, en P , generado por J.
c) Encuentre el valor de J0 pJs q, que hace que el campo magnético resultante en el punto P sea
nulo.

#### Solución
Para el campo generado por Js utilizamos el mismo método que para la espira,

---

### Página 6

la corriente encerrada corresponde a,
I = Js bl
y la integral sobre el camino amperiano se traduce en,
⃗ ⃗l = B ˚ 2l
Bd
finalmente, mediante la ley de Ampère,
⃗ = - µ0 Js b ŷ
B ˚ 2l “ µ0 Js bl Ñ B
Para el cálculo del campo debido al cilindro utilizamos la misma idea, comenzamos con la corriente
encerrada, solo nos centraremos en la región r < R ya que el punto P (lo que nos interesa) se
encuentra ahí. La corriente encerrada es entonces,
ż 2π
I“

żr

ˆ 2
˙
´
r¯
r3
r
dθ rdrJ0 1 ´
“ 2πJ0
´
R
3R
o

y la integral de camino del campo magnético sería,
⃗ ⃗l = B2πr
Bd
utilizando la ley de Ampère llegamos al resultado que esperábamos buscar,
ˆ 2
˙
ˆ
˙
r
r3
r
r
⃗ “ µ0 J0
B ˚ 2πr = 2πJ0 µ0
´
ÑB
´
θ̂
3R
2 3R
Para el cálculo final en el punto P no hace falta evaluar nada para nuestro primer campo, como
vemos no depende de la distancia a la que se encuentre de la región con corriente.
En el segundo caso, debemos reemplazar por r = R{2 y además vemos que como este punto está
en el mismo eje que une el centro del cilindro con la placa, justo en el punto P , el campo magnético
apunta en `ŷ; siendo entonces el resultado,
ˆ
⃗ “ µ0 J0

R
R2
´
12R

˙

µ0 Js b
µ0
ŷ ´
ŷ “

ˆ

˙
J0 R
´ µ0 Js b ŷ

y si queremos que este campo se anule en P , el valor de J0 debe ser tal que,
J0 R
3bJs
´ µ0 Js b = 0 Ñ J0 = 
R
