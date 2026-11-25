---
title: "Examen 2025-2"
source_pdf: "Electro/pruebas-anteriores/Examen/Examen 2025-2.pdf"
pages: 8
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Examen 2025-2

### Página 1

FIS1533: Segundo semestre 2025

Examen

Examen
Fecha: 05 de diciembre de 2025

1. Problema
Tres placas conductoras paralelas de área A muy grande, se colocan separadas una distancia d y
de manera consecutiva, tal como se muestra en la figura. El espacio entre las placas esta lleno con
materiales dieléctricos de permitividad ε 1 y ε 2 , como se muestra en la figura. Las placas externas
están conectadas eléctricamente por medio de un cable conductor que tiene un extremo denotado
con la letra b. La placa central está conectada a un cable conductor eléctrico de extremo a. Las placas
están cargadas de tal forma que la carga de la placa central es + Q y los extremos a y b tienen una
diferencia de potencial Vab , ambas conocidas. Se pueden ignorar los efectos de los bordes.

a) (2 pto.) Calcular la capacitancia total, CT , entre los extremos a y b en términos de los parámetros
mostrados en la figura (A, ε 1 , ε 2 , d, Vab .).
b) (2 pto.) Calcular la densidad de carga libre, σ1 , en la superficie de contacto entre la placa conductora central y el material dieléctrico con permitividad ε 1 (En este punto puede considerar
conocida CT ).
c) (2 pto.) Calcular la densidad de carga ligada, σb , en la superficie de contacto entre la placa conductora central y el material dieléctrico con permitividad ε 1 (En este punto puede considerar
conocida CT y/o σ1 ).

Respuestas Forma 1

---

### Página 2

a) capacitancia total, CT
La placa central forma dos condensadores con el conductor exterior: uno a la izquierda (capacitancia C1 ) y otro
a la derecha (capacitancia C2 ). Como ambos conectan la misma placa central con el mismo conductor exterior,
estos dos condensadores están en paralelo; por tanto
C1 =
y

ε1 A
d

Ctotal = C1 + C2
es decir
Ctotal =

ε2 A
d

C2 =

0,5pts ,

0,5pts ,

0,5pts

(ε 1 + ε 2 ) A
d

0,5pts

b) Calcular la densidad de carga libre, σ1
La carga Q del conductor central se reparte entre las dos caras (izquierda y derecha) proporcionalmente a las
capacitancias. la capacitancia para el material ε 1 es
Q1 = C1 Vab

0,5pts

Q
Ctotal

0,5pts

donde
Vab =
por tanto

C1
Q
Ctotal
La densidad de carga libre σ1 por definición toma la forma
Q1 =

σ1 =

Q1
A

0,5pts

es decir

C1 Q
Ctotal A
Si se sustituyen las expresiones de Ctotal y C1 , se obtiene
σ1 =

σ1 =

0,5pts

ε1
Q
ε1 + ε2 A

---

### Página 3

c) Calcular la densidad de carga ligada, σb para el material ε 1
La densidad superficial de carga ligada para el material ε 1 esta dada por la expresión
σb1 = ⃗
P1 · n̂.

0,5pts

La polarización eléctrica para el material ε 1 está definida por

⃗P1 = ε 0 (ε r − 1)⃗E1 ,

0,5pts

con ε r1 = ε 1 /ε 0 . En la interfaz dieléctrico-conductor, donde el conductor está cargado positivamente, el vector
unitario n̂ apunta en el sentido contrario al del campo eléctrico, es decir

⃗E1 · n̂ = − E1 .
Por tanto

σb1 = ε 0 (ε r1 − 1)⃗E1 · n̂

es decir
σb1 = −ε 0 (ε r1 − 1) E1
El campo entre la placa central y cada placa exterior es uniforme (planas y grandes). La magnitud es la misma en
ambas regiones y viene dada por la expresión
E1 = E2 =

Vab
d

0,5pts

Sustituyendo esta expresión del campo se obtiene
σb1 = −ε 0 (ε r1 − 1)

Vab
d

0,5pts

En términos de Ctotal puede quedar dada como
σb1 = −ε 0 (ε r1 − 1)

Q
d Ctotal

---

### Página 4

2. Problema
Considere una espira cuadrada de lado a y masa m en el plano yz, colocada en un campo magnético
⃗B = ( B0 − αz) x̂, con α > 0. Considere que la espira, de resistencia R y autoinducción despreciable,
cae en la dirección vertical debido a la gravedad.

a) (1 pto.) Determine el flujo magnético a través de la espira.
b) (2 pto.) Encuentre la fuerza electromotriz y la corriente inducida en función de la velocidad v
de la espira
c) (1 pto.) Indique el sentido de la corriente inducida y justifique su respuesta según la ley de
Lenz.
d) (1 pto.) Determine la fuerza que experimenta la espira.
e) (1 pto.) ¿Cuál es la velocidad terminal de la espira?

---

### Página 5

#### Solución:
a) Empezamos calculando el flujo magnético a través de la espira. Para esto consideramos que el vector área será
⃗ = dydz x̂, luego:
dA
ΦB =
ΦB =

I

⃗
⃗B · d A

Z a Z z+ a
y =0

z=z

( B0 − αz)dydz =

Z a
y =0

dy

Z z+ a
z=z

( B0 − αz)dz

(0.5 pts.)


z+ a
αz2
Φ B = a B0 z −
2 z
Φ B = a2 B0 −

αa2 (2z + a)

(0.5 pts.)

b) Para calcular la fuerza electromotriz inducida, consideremos la Ley de Faraday:


dΦ B
d
αa2 (2z + a)
=−
ε=−
a2 B0 −
dt
dt
dz
ε = +αa2
dt
ε = +αa2 v

(0.25 pts.)
(0.25 pts.)
(0.5 pts.)

ε = −αa2 |v|
Note que la velocidad con la que cae es negativa, por lo que la fem inducida también lo es (0.5 pts.).
Luego, la corriente inducida será
|ε|
αa2 |v|
I=
=
.
R
R

(0.5 pts.)

c) Si la espira cae, el flujo aumenta, pues el campo magnético es inversamente proporcional a la altura, mientras
menor sea z, mayor será el campo (0.5 pts.). Luego, la corriente inducida debe generar un campo que se oponga a
este aumento. Con esto, la corriente debe tener el sentido horario (0.5 pts.).

---

### Página 6

d) Ya que tenemos un conductor con corriente inmerso en un campo magnético, podemos calcular la fuerza sobre
cada uno de los segmentos de la espira usando

⃗F = I

Z

d⃗ℓ × ⃗B

Para los segmentos verticales de la izquierda ⃗F1 y la derecha ⃗F2 , tenemos

⃗F1 = I

Z

d⃗ℓ1 × ⃗B = I

Z z+ a
z

dzẑ × ( B0 − αz) x̂


 z+ a
z2
dz( B0 − αz) ŷ = I B0 z − α
ŷ
2 z
z

i
h
⃗F1 = I B0 a − α (z + a)2 − z2 ŷ

⃗F1 = I

Z z+ a

(0.2 pts.)

Mientras que

⃗F2 = I

Z

d⃗ℓ2 × ⃗B = I

Z z
z+ a

dzẑ × ( B0 − αz) x̂

 z+ a

z2
ŷ
dz( B0 − αz) ŷ = − I B0 z − α
2 z
z
h

i
⃗F2 = − I B0 a − α (z + a)2 − z2 ŷ
Z z+ a

⃗F2 = − I

(0.2 pts.)

Por tanto, ⃗F1 + ⃗F2 = 0 (alternativamente usando argumentos de simetría 0.4 pts.). Por otra parte, los segmentos
horizontales superior ⃗F3 e inferior ⃗F4 , se encuentran a una altura fija, por lo que el campo no cambia a lo largo del
camino, así

⃗F3 = I⃗L3 × ⃗B = ILŷ × [ B0 − α(z + a)] x̂
⃗F3 = − IL [ B0 − α(z + a)] ẑ

(0.2 pts.)

Y para el segmento horizontal inferior,

⃗F4 = I⃗L4 × ⃗B = − ILŷ × [ B0 − αz] x̂
⃗F4 = IL ( B0 − αz) ẑ

(0.2 pts.)

Luego, la fuerza magnética sobre la espira, será

⃗FB = ⃗F3 + ⃗F4 = − IL [ B0 − α(z + a)] ẑ + IL ( B0 − αz) ẑ
Así

(0.1 pts.)

2 3

⃗FB = ILαaẑ = α a |v| L ẑ
R
Por último, la fuerza total sobre la espira, incluyendo la gravedad, será
 2 3

⃗FB = α a |v| L − mg ẑ
R

(0.1 pts.)

d) La velocidad terminal se alcanza una vez que la espira deja de acelerar mientras cae, por tanto ⃗F = 0 (0.3 pts.),
así
α2 a3 |vterm | L
0 =
− mg
(0.5 pts.)
R
Despejando tenemos
mgR
|vterm | = 2 3
(0.2 pts.)
α a L

---

### Página 7

3. Problema
Dado el circuito RLC en la figura

1. (2 pto.) ¿Cuál es la impedancia entre los terminales de conexión?
2. (2 pto.) Se aplica el voltaje alterno U (t) = U0 cos(ωt) a los terminales de conexión. Calcule la
amplitud de oscilación de la corriente alterna I (t) que entra al circuito.
3. (2 pto.) ¿Cuál es la potencia que se disipa en el circuito durante un período de oscilación del
voltaje alterno cuando la frecuencia angular del voltaje es ω = 1/( LC )?
#### Solución:
1. Resistencia R, inductancia L y capacitancia C en serie tienen la impedancia

 ω 2 
LC
R + iωL +
= R + iωL 1 −
iωC
ω
√
donde ω LC = 1/ LC es la frecuencia angular caracteristica del circuito LC.
Con la resistencia R en paralelo, la impedancia total resulta como:
 −1



h
i
Z =
+
ω 2
R
R + iωL 1 − LC
ω

h

=

R + iωL 1 −
h
R
2R + iωL 1 −

ω LC 2
ω

i

ω LC 2
ω

(2 pto.)

i

2. Amplitudes complejas de voltaje Ũ0 y corriente Ĩ0 :

U (t)

=





U0 cos(ωt) = ℜ 
U0 eiωt 
|{z}

=Ũ0


I (t)

=



 iφ iωt 
I0 cos(ωt + φ) = ℜ 
I0 e e 
|{z}

= Ĩ0

---

### Página 8

¨Ley de Ohm¨ para amplitudes complejas
Ũ0 = Z Ĩ0
por lo tanto la amplitud es:
I0

=

h
i
ω LC 2
U0 2R + iωL 1 − ω
i
h
R R + iωL 1 − ω LC 2

=

v
h
u
2 i2
u
(2R)2 + (ωL)2 1 − ωωLC
U0 u
u
h
i
R t
ω 2 2
R2 + (ωL)2 1 − ωLC

ω

(2 pto.)

√
3. Suponiendo correcta definición de frecuencia de resonancia ω LC = 1/ LC.
Sin cálculo: En resonancia voltajes de la capacitancia y de la inductancia de compensan (sin desfase), entonces es
como un circuito con dos resistencias en paralelo:
P=

U2
U0 I0
cos φ = 0
R

para ω = ω LC la fase es φ = 0 y la amplitud es I0 = 2U
R y resulta

P=

U2
U0 I0
cos φ = 0
R

(2 pto.)

En otro caso, usando valor dado (pero incorrecto) ω = 1/( LC ), aceptar cálculo que intenta calcular amplitud y
fase de la corriente para obtener potencia promediada.
