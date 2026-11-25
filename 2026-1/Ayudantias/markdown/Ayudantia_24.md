---
title: "Ayudantia 24"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_24.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_24_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 24

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 24
Repaso I2

#### Problema 1
Una esfera de radio R, con carga libre q, está sumergida en un medio dieléctrico homogéneo de
constante κ y de extensión teóricamente infinita. Calcular:
a) Los vectores de campo eléctrico y polarización a una distancia r > R.
b) La densidad de carga volumétrica de polarización.
#### Problema 2
Considere un cable coaxial compuesto por dos materiales dieléctricos lineales e isotrópicos, con
permitividades ε1 y ε2 , entre dos conductores de espesor despreciable, sobre los cuales se aplica
una diferencia de potencial V0 , como se muestra en la figura.

Determine:
(a) El vector desplazamiento en todo el espacio.

---

### Página 2

(b) El campo eléctrico en todo el espacio.
(c) El vector de polarización en todo el espacio.
(d) Las densidades de carga superficiales en cada interfaz, teniendo en cuenta que:
σp = P⃗ ¨ n̂
#### Problema 3
El circuito de la figura se usa para medir la rapidez de la flecha. En la práctica Vf = 24 V, C = 
20 pF, R1 = 2 MΩ, R2 = 3 MΩ, y d = 69 cm. En todos los cálculos numéricos mantenga 3 cifras
significativas.

a) Cuando se cierra el interruptor S el condensador está totalmente descargado y la flecha se
encuentra a la izquierda del circuito. Explique lo que sucede con el condensador. ¿Cuánto
tiempo debe transcurrir para que el condensador quede a 0,1 % de su carga máxima? Entregue
primero una fórmula algebraica para el tiempo, y luego evalúe con los valores indicados
antes. Considere la aproximación ln 1000 « 6,9.
b) En el instante t = 0 la flecha corta el circuito en la sección AC (asuma que el condensador
tiene en ese momento su carga máxima). Explique lo que sucede con el condensador. Calcule
su voltaje en función del tiempo.
c) En un instante posterior t > 0 la flecha corta la sección BD. Explique lo que sucede con
el condensador. Si el voltaje final del condensador es VCfin (voltaje en el momento del corte)
encuentre la rapidez de la flecha. Entregue primero una fórmula algebraica para la rapidez, y
luego evalúe con los valores indicados antes. Suponga que VCfin = VCmáx {2 (donde VCmáx es el
voltaje máximo del condensador), y use que ln 2 « 0,69.

---

### Página 3

#### Problema 4
Una corriente I circula por la espira cerrada de radios b y a pb > aq mostrada en la figura. Ambas
semicircunferencias tienen un origen común en P y θ = π{4.

Con esta información, calcule:
(a) El vector campo magnético en el punto P .
(b) El vector momento dipolar magnético de la espira.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 24
Repaso I2

#### Problema 1
Una esfera de radio R, con carga libre q, está sumergida en un medio dieléctrico homogéneo de
constante κ y de extensión teóricamente infinita. Calcular:
a) Los vectores de campo eléctrico y polarización a una distancia r > R.
b) La densidad de carga volumétrica de polarización.

#### Solución
Como se nos está pidiendo para r > R, cualquier superficie gaussiana que dibujemos encerrará a
la carga q que es nuestra carga libre, es decir,
ż
⃗ ¨ d⃗s = q ÝÑ D(r)
⃗
D
“

q
4πr2

Si el medio tiene permitividad relativa κ significa que podemos relacion desplazamiento electrico
con campo eléctrico como,
⃗ “ ϵE
⃗ = κϵ0 E
⃗ ÝÑ E(r)
⃗
D
“

q
r̂
4πϵ0 κr2

Además, de la definición de desplazamiento eléctrico podemos determinar la polarización,
qpκ ´ 1q
⃗ “ ϵ0 E
⃗ ` P⃗ ÝÑ P⃗ = pϵ - ϵ0 qE(r)
⃗
D
“
r̂
4πκr2
Calculamos la carga volumétrica de polariación como,
ρp = ´∇ ¨ P⃗

---

### Página 2

Dado que la polarización esférica P⃗ es de la forma:
qpκ ´ 1q
r̂
P⃗ (r) = 
4πκr2
la divergencia de P⃗ en coordenadas esféricas es:
˘
1 d ` 2
r P (r)
∇ ¨ P⃗ = 2
r dr
, obtenemos:
Sustituyendo P (r) = qpκ´1q
4πκr2
1 d
∇ ¨ P⃗ = 2
r dr

ˆ

1 d
∇ ¨ P⃗ = 2
r dr

ˆ

qpκ ´ 1q
r ¨
4πκr2

˙

Simplificando:
qpκ ´ 1q
4πκ

˙
“0

Por lo tanto, la densidad de carga de polarización volumétrica es:
ρp = 0
#### Problema 2
Considere un cable coaxial compuesto por dos materiales dieléctricos lineales e isotrópicos, con
permitividades ε1 y ε2 , entre dos conductores de espesor despreciable, sobre los cuales se aplica
una diferencia de potencial V0 , como se muestra en la figura.

Determine:
(a) El vector desplazamiento en todo el espacio.

---

### Página 3

(b) El campo eléctrico en todo el espacio.
(c) El vector de polarización en todo el espacio.
(d) Las densidades de carga superficiales en cada interfaz, teniendo en cuenta que:
σp = P⃗ ¨ n̂

#### Solución
#### Solución.
El sistema corresponde a un cable coaxial formado por dos regiones dieléctricas. El primer dieléctrico, de permitividad ε1 , ocupa la región
a < r < b,
mientras que el segundo dieléctrico, de permitividad ε2 , ocupa la región
b < r < c.
Los conductores se encuentran en r < a y r > c, y entre ellos se aplica una diferencia de potencial
V0 .
⃗
(a) Vector desplazamiento eléctrico D.
⃗ usamos la ley de Gauss en medios materiales:
Para encontrar D
¿
⃗ ¨ dA
⃗ = Qlibre .
D
S

Por simetría cilíndrica, el campo debe ser radial y solo puede depender de r, por lo que
escribimos
⃗
D(r)
“ Dr (r) r̂.
Tomamos como superficie gaussiana un cilindro coaxial de radio r y largo L. En la superficie
lateral,
⃗ = r dϕ dz r̂.
dA
Entonces,
ż L ż 2π

¿
⃗ ¨ dA
⃗“
D
S

Dr (r) r dϕ dz = Dr (r) 2πrL.

Igualando con la carga libre encerrada Q, se obtiene
Dr (r) 2πrL = Q,

---

### Página 4

y por tanto
⃗
D(r)
“

Q
r̂.
2πrL

En los conductores, el campo eléctrico es nulo en equilibrio electrostático, por lo que también
⃗ Así,
se anula D.
$
’
0,
r < a,
’
’
’
’
’
’ Q
’
’
r̂, a < r < b,
&
2πrL
⃗
D(r) = 
Q
’
’
’
r̂, b < r < c,
’
’
2πrL
’
’
’
’
%0,
r > c.
Para escribir el resultado en función de V0 , usamos que
⃗ = εE.
⃗
D
Por lo tanto, en cada dieléctrico:
⃗ 1 (r) = 
E

Q
r̂,
2πε1 rL

a < r < b,

⃗ 2 (r) = 
E

Q
r̂,
2πε2 rL

b < r < c.

y

Tomaremos:
V0 = V (c) - V (a),
según la polaridad indicada en la figura, la linea más larga (Terminal positivo) esta conectada
en r = c, es decir, este cascaron tiene mayor potencial. Si se escogiera la convención opuesta,
los campos cambiarían de signo, pero sus magnitudes serían las mismas.
La diferencia de potencial entre los conductores es
żc
⃗ ¨ d⃗r.
E

V0 = V (c) - V (a) = ´
a

Separando la integral en las dos regiones dieléctricas,
˙
ˆż b
żc
Q
Q
dr `
dr .
V0 = ´
b 2πε2 Lr
a 2πε1 Lr
Entonces,

„
ȷ
Q lnpb{aq lnpc{bq
V0 = ´
`
.
2πL
ε1
ε2

---

### Página 5

Despejando Q,
Q = ´

2πLV0 ε1 ε2
.
ε2 lnpb{aq ` ε1 lnpc{bq

⃗ resulta
Reemplazando en D,
$
’
0,
r < a,
’
’
’
’
&
V0 ε1 ε2
⃗
r̂, a < r < c,
D(r)
“ ´
ε2 lnpb{aq ` ε1 lnpc{bq r
’
’
’
’
’
%0,
r > c.
⃗
(b) Campo eléctrico E.
Usamos directamente la relación
⃗ = εE.
⃗
D
En la región a < r < b, la permitividad es ε1 , por lo que
⃗
⃗ 1 (r) = D(r) .
E
ε1
Así,
⃗ 1 (r) = ´
E

V0 ε2
r̂,
ε2 lnpb{aq ` ε1 lnpc{bq r

a < r < b.

En la región b < r < c, la permitividad es ε2 , entonces
⃗
⃗ 2 (r) = D(r) .
E
ε2
Por lo tanto,
⃗ 2 (r) = ´
E

V0 ε1
r̂,
ε2 lnpb{aq ` ε1 lnpc{bq r

b < r < c.

Finalmente,

⃗
E(r)
“

$
’
0,
r < a,
’
’
’
’
’
V0 ε2
’
’
’
&´ ε lnpb{aq ` ε lnpc{bq r r̂, a < r < b,

’
V0 ε1
’
’
´
r̂, b < r < c,
’
’
ε2 lnpb{aq ` ε1 lnpc{bq r
’
’
’
’
%
0,
r > c.

---

### Página 6

(c) Vector de polarización P⃗ .
Para un dieléctrico lineal e isotrópico,
⃗ ´ ε0 E.
⃗
P⃗ = D
⃗ = εE,
⃗ se obtiene
Como además D
⃗
P⃗ = pε - ε0 qE.
En los conductores no hay polarización, por lo tanto
P⃗ = 0

para r < a y r > c.

En el primer dieléctrico,
⃗ 1 (r),
P⃗1 (r) = pε1 - ε0 qE
de modo que
P⃗1 (r) = ´

V0 pε1 ´ ε0 qε2
r̂,
ε2 lnpb{aq ` ε1 lnpc{bq r

a < r < b.

En el segundo dieléctrico,
⃗ 2 (r),
P⃗2 (r) = pε2 - ε0 qE
por lo que
P⃗2 (r) = ´
En resumen,

P⃗ (r) = 

V0 pε2 ´ ε0 qε1
r̂,
ε2 lnpb{aq ` ε1 lnpc{bq r

$
’
0,
’
’
’
’
’
’
’
’
’
&´

b < r < c.

r < a,
V0 pε1 ´ ε0 qε2
r̂,
ε2 lnpb{aq ` ε1 lnpc{bq r

a < r < b,

’
V0 pε2 ´ ε0 qε1
’
’
r̂, b < r < c,
´
’
’
ε2 lnpb{aq ` ε1 lnpc{bq r
’
’
’
’
’
%0,
r > c.

(d) Densidades superficiales de carga de polarización.
La densidad superficial de carga ligada en una interfaz se calcula mediante
σp = P⃗ ¨ n̂,
donde n̂ es la normal saliente de la superficie del material considerado.
En este problema hay tres interfaces relevantes:
r = a,

r = b,

r = c.

---

### Página 7

Para simplificar la notación, definimos
D = ε2 lnpb{aq ` ε1 lnpc{bq.
Interfaz en r = a.
En r = a se tiene la interfaz entre el conductor interior y el dieléctrico de permitividad ε1 .
Como dentro del conductor P⃗ = 0, la carga superficial de polarización viene dada por el
valor de P⃗1 evaluado en r = a:
σp,a = P⃗1 (a) ¨ r̂.
Por lo tanto,
σp,a = ´

V0 pε1 ´ ε0 qε2 1
.
D
a

Interfaz en r = b.
En r = b se juntan los dos dieléctricos. La densidad superficial de polarización corresponde
al salto de la componente normal de P⃗ :
´
¯
σp,b = P⃗2 (b) - P⃗1 (b) ¨ r̂.
Evaluando,
V0 pε1 ´ ε0 qε2 1
r̂,
P⃗1 (b) = ´
D
b
y
V0 pε2 ´ ε0 qε1 1
P⃗2 (b) = ´
r̂.
D
b
Luego,
σp,b “

V0 1
rpε1 ´ ε0 qε2 ´ pε2 ´ ε0 qε1 s .
Db

Simplificando el término entre corchetes:
pε1 - ε0 qε2 - pε2 - ε0 qε1 = ε0 pε1 - ε2 q.
Por lo tanto,
σp,b “

V0 ε0 pε1 ´ ε2 q 1
.
D
b

Interfaz en r = c.
En r = c se tiene la interfaz entre el dieléctrico de permitividad ε2 y el conductor exterior.
En el conductor exterior no hay polarización, por lo que
´
¯
⃗
σp,c = 0 - P2 (c) ¨ r̂.

---

### Página 8

Como

V0 pε2 ´ ε0 qε1 1
r̂,
P⃗2 (c) = ´
D
c

obtenemos
σp,c “

V0 pε2 ´ ε0 qε1 1
.
D
c

Finalmente,
σp,a = ´

V0 pε1 ´ ε0 qε2
ε2 lnpb{aq ` ε1 lnpc{bq a

σp,b “

V0 ε0 pε1 ´ ε2 q
ε2 lnpb{aq ` ε1 lnpc{bq b

σp,c “

V0 pε2 ´ ε0 qε1
ε2 lnpb{aq ` ε1 lnpc{bq c

#### Problema 3
El circuito de la figura se usa para medir la rapidez de la flecha. En la práctica Vf = 24 V, C = 
20 pF, R1 = 2 MΩ, R2 = 3 MΩ, y d = 69 cm. En todos los cálculos numéricos mantenga 3 cifras
significativas.

a) Cuando se cierra el interruptor S el condensador está totalmente descargado y la flecha se
encuentra a la izquierda del circuito. Explique lo que sucede con el condensador. ¿Cuánto
tiempo debe transcurrir para que el condensador quede a 0,1 % de su carga máxima? Entregue
primero una fórmula algebraica para el tiempo, y luego evalúe con los valores indicados
antes. Considere la aproximación ln 1000 « 6,9.
b) En el instante t = 0 la flecha corta el circuito en la sección AC (asuma que el condensador
tiene en ese momento su carga máxima). Explique lo que sucede con el condensador. Calcule
su voltaje en función del tiempo.

---

### Página 9

c) En un instante posterior t > 0 la flecha corta la sección BD. Explique lo que sucede con
el condensador. Si el voltaje final del condensador es VCfin (voltaje en el momento del corte)
encuentre la rapidez de la flecha. Entregue primero una fórmula algebraica para la rapidez, y
luego evalúe con los valores indicados antes. Suponga que VCfin = VCmáx {2 (donde VCmáx es el
voltaje máximo del condensador), y use que ln 2 « 0,69.

#### Solución
Queremos resolver la ecuación para V del condensador, para esto podemos ignorar por completo
la rama que incluye R2 (ya que como están en paralelo, comparten voltaje), entonces aplicando
Kirchhoff a la malla grande,
Vf = VR1 ` Vc

(1)

reemplazamos solo VR1 ,
dVc
` Vc
dt

(2)

dVc
dt

(3)

Vf = R1 I ` Vc Ñ Vf = R1 C
El primer término el r.h.s sale de,
d{dt

Qc = CVc ÝÝÑ I = C

Resolvemos la ecuación por separación de variables para obtener,
Vc = Vf p1 - et{R1 C q

(4)

si queremos que Vc sea 0,999Vf , entonces,
e´T {R1 C = 0,001 Ñ T = R1 C ln 1000

(5)

T « 2,76 ˆ 10´4 s

(6)

Evaluando numéricamente,

En el momento que la flecha corta el primer segmento, la corriente no puede pasar por la parte
donde está la batería, por lo que el circuito pasa a ser,

---

### Página 10

Por ley de kirchhoff entonces,
VR1 ` VR ` Vc = 0 Ñ R1 I ` R2 I ` Vc = 0

(7)

y sabemos además que la corriente podemos escribirla como,
d{dt

Qc = CVc ÝÝÑ I = C

dVc
dt

(8)

Entonces la ecuación a resolver es,
dVc
` Vc = 0
dt
Esta ecuación la resolvemos fácilmente con separación de variables,
pR1 ` R2 qC

Vc = Vf e´t{pR1 `R2 qC

(9)

(10)

Como el voltaje inicial es su máximo, lo escribimos como Vf = Vcmax ,
Vc = Vcmax e´t{pR1 `R2 qC

(11)

Cuando la flecha corta la segunda parte, la corriente ya no puede circular porque el circuito no está
cerrado, por lo que se queda = congelado”.
Buscamos entonces el tiempo en que corta el segundo segmento (t = tv ), en donde sabemos el
voltaje del condensador será Vcmax = 2Vcf in
Vcmax
f in
“ Vcmax e´tv {pR1 `R2 qC Ñ tv = lnp2qpR1 ` R2 qC
Vc (tv ) = Vc = 

(12)
entonces la velocidad de la bala es simplemente la distancia recorrida sobre el tiempo que le toma
en cortar ambos segmentos,
v“

d
d
“
« 104 m/s
t
lnp2qpR1 ` R2 qC

(13)

---

### Página 11

#### Problema 4
Una corriente I circula por la espira cerrada de radios b y a pb > aq mostrada en la figura. Ambas
semicircunferencias tienen un origen común en P y θ = π{4.

Con esta información, calcule:
(a) El vector campo magnético en el punto P .
(b) El vector momento dipolar magnético de la espira.

#### Solución
La espira está formada por dos arcos circulares concéntricos, de radios a y b, unidos por dos segmentos radiales. Ambos arcos tienen centro en el punto P .
El ángulo que no forma parte de la espira es θ, por lo tanto el ángulo recorrido por cada arco es
α = 2π - θ.
Como en este problema
θ“
se tiene
α = 2π ´

π
,
π
7π
“
.

(a) Campo magnético en el punto P .
Para calcular el campo magnético usamos la ley de Biot-Savart:
⃗ “
dB

µ0 I d⃗ℓ ˆ r̂
.
4π r2

---

### Página 12

Primero calculemos el aporte de un arco circular genérico de radio R y ángulo α, cuyo centro
está en P .
En un arco circular, la distancia desde cada elemento de corriente hasta el centro es constante:
r = R.
Además, el elemento de largo es
dℓ = R dφ.
Como d⃗ℓ es tangente al arco y r̂ apunta radialmente hacia el punto P , ambos vectores son
perpendiculares. Por lo tanto,
|d⃗ℓ ˆ r̂| = dℓ.
Entonces, la magnitud del campo producido por el arco en el punto P es
dB “

µ0 I dℓ
.
4π R2

Reemplazando dℓ = R dφ:
dB “

µ0 I R dφ
.
4π R2

dB “

µ0 I
dφ.
4πR

Luego,

Integramos sobre todo el arco:
ż
B“

µ0 I
dB “
4πR

żα
dφ.

Por lo tanto,
Barco “

µ0 I
α.
4πR

Es decir,
⃗ arco “ µ0 I α k̂,
B
4πR
si la corriente circula en sentido antihorario, y
⃗ arco = - µ0 I α k̂,
B
4πR
si la corriente circula en sentido horario.
Ahora aplicamos este resultado a la espira.
El arco exterior tiene radio b. Según el sentido de la corriente mostrado en la figura, su
contribución apunta en dirección `k̂. Por lo tanto,
⃗ b “ µ0 I p2π ´ θq k̂.
B
4πb

---

### Página 13

El arco interior tiene radio a. Para que la espira sea cerrada, la corriente en el arco interior
circula en sentido contrario al arco exterior, por lo que su campo apunta en dirección ´k̂.
Así,
⃗ a = - µ0 I p2π - θq k̂.
B
4πa
Falta analizar los dos segmentos rectos que conectan ambos arcos. Estos segmentos son radiales, por lo que para cada elemento de corriente se cumple que d⃗ℓ es paralelo o antiparalelo
a r̂. Por lo tanto,
d⃗ℓ ˆ r̂ = 0.
Así, los segmentos radiales no aportan campo magnético en P .
Entonces, el campo magnético total en P es
⃗ q = B
⃗b ` B
⃗ a.
BpP
Reemplazando:
⃗ q “ µ0 I p2π ´ θq k̂ ´ µ0 I p2π ´ θq k̂.
BpP
4πb
4πa
Factorizando,
⃗ q “ µ0 I p2π ´ θq
BpP
4π

ˆ

1 1
´
b a

˙
k̂.

Como θ = π{4, se obtiene
⃗ q “ µ0 I
BpP
4π

ˆ

7π

˙ˆ

1 1
´
b a

˙
k̂.

Por lo tanto,
⃗ q = 7µ0 I
BpP

ˆ

1 1
´
b a

˙
k̂ .

Como b > a, se cumple que
1 1
´ < 0,
b a
por lo que el campo magnético neto apunta en dirección ´k̂.
Equivalentemente, se puede escribir como
⃗ q = - 7µ0 I
BpP

ˆ

1 1
´
a b

˙
k̂ .

---

### Página 14

(b) Momento dipolar magnético de la espira.
El momento dipolar magnético de una espira plana está dado por
m
⃗ = IA n̂,
donde A es el área encerrada por la espira y n̂ es el vector normal determinado por la regla
de la mano derecha.
En este caso, el área encerrada corresponde a un sector anular. Es decir, corresponde al área
de un sector circular de radio b menos el área de un sector circular de radio a, ambos con
ángulo
α = 2π - θ.
El área de un sector circular de radio R y ángulo α es
AR = R2 α.
Por lo tanto, el área encerrada por la espira es
A = b2 p2π - θq - a2 p2π - θq.
Factorizando,

A = p2π - θqpb2 - a2 q.

Usando θ = π{4:
A“

ˆ

Entonces,

7π

˙
pb2 ´ a2 q.

7π 2
pb ´ a2 q.

A“

Según el sentido de corriente indicado en la figura, el vector normal asociado a la espira
apunta en dirección `k̂. Por lo tanto,
m
⃗ = I

7π 2
pb ´ a2 q k̂.

Así,
m
⃗ “

7πI 2
pb ´ a2 q k̂ .
