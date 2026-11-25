---
title: "Ayudantia 04"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_04_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_04_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 04

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 4
#### Problema 1
Cuatro partículas, dos de las cuales poseen carga +q y las otras dos −q, están ubicadas como
indica la figura. Si cada una tiene una masa m y se suelta de los vértices del cuadrado a
partir del reposo, calcule la velocidad de las partículas cuando el largo del cuadrado vale ℓ.
Suponga que todas las cargas se mueven con la misma rapidez.

---

### Página 2

#### Problema 2
Considere un cilindro muy largo, de radio a, con densidad volumétrica de carga uniforme ρ0 ,
al que se le ha practicado una cavidad esférica de radio a como se ve en la figura. Calcule el
campo eléctrico y el potencial en todo el espacio exterior al cilindro.

#### Problema 3
Considere una región esférica de radio b, que tiene una distribución de carga uniforme ρ(r) =
ρ0 para la región determinada por a < r < b y densidad nula para r < a. Determine el
potencial eléctrico en todo el espacio.

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 4
#### Problema 1
Cuatro partículas, dos de las cuales poseen carga +q y las otras dos −q, están ubicadas como
indica la figura. Si cada una tiene una masa m y se suelta de los vértices del cuadrado a
partir del reposo, calcule la velocidad de las partículas cuando el largo del cuadrado vale ℓ.
Suponga que todas las cargas se mueven con la misma rapidez.

#### SOLUCION:
Por el principio de la conservación de energía, se cumple que
Einicial = Efinal
Si calculamos la energía inicial, notaremos que posee una contribución cinética y otra potencial, por lo que
Einicial = Kinicial + Uinicial

---

### Página 2

Como el sistema parte del reposo, se tiene que Kinicial = 0. La energía potencial inicial está
dada por:


qA qB qA qC qA qD qB qC qB q D q C q D
+
+
+
+
+
Uinicial =
4πϵ0 rA,B
rA,C
rA,D
rB,C
rB,D
rC,D


q2
q2
=
−4 ·
+2· √
4πϵ0
a
2a
!
√
q2
2−4
=
4πϵ0
a
Para la situación final, si cada una se mueve con velocidad v y poseen masa m, la energía
cinética final es:
X
mi 2
mv 2
Kfinal =
vi = 4
= 2mv 2
i=1
La energía potencial final se consigue cambiando a por ℓ, por lo que:
√
q2
2−4
Ufinal =
4πϵ0
ℓ
Así,
r
Uinicial = 2mv 2 + Ufinal

−→

v=

Uinicial − Ufinal
2m

Finalmente,
s
v=

q2 √
( 2 − 4)
8mπϵ0



1 1
−
a ℓ



---

### Página 3

#### Problema 2
Considere un cilindro muy largo, de radio a, con densidad volumétrica de carga uniforme ρ0 ,
al que se le ha practicado una cavidad esférica de radio a como se ve en la figura. Calcule el
campo eléctrico y el potencial en todo el espacio exterior al cilindro.

#### SOLUCION:
Para resolver este problema conviene usar le principio de superposición: el campo creado por
el cilindro con la cavidad es igual al campo creado por un cilindro uniforme de densidad
ρ0 menos el campo creado por una esfera también con densidad ρ0 . Ambos se calculan
fácilmente con ley de Gauss.
Para calcular el campo fuera del cilindro consideremos como superficie gaussiana un cilindro
de altura h, concéntrico con el cilindro original, con un radio r > a. Por simetría sabemos
⃗ c = Ec r̂, de modo que tenemos
que el campo sera de la forma E
Z
⃗ c · dA
⃗ = Ec 2πrh = πa hρ0
ϵ0
De modo que el campo eléctrico resulta en

⃗ c = a ρ0 r̂
2ϵ0 r
El potencial creado por el cilindro también tiene simetría cilíndrica y lo obtenemos integrando
Z
Z 2
a ρ0
a2 ρ 0
Vc = − E · dl = −
dr = −
ln r + C
2ϵ0 r
2ϵ0

---

### Página 4

Para la esfera, el campo eléctrico es
Z
⃗ c · dA
⃗ = Ec 4πρ2 = 3 πa ρ0
ϵ0
⃗ c = a ρ0 ρ̂
⇒ E
3ϵ0 ρ2
y el potencial es
Ve =

a3 ρ 0
+C
3ϵ0 ρ

No confundir la coordenada esférica ρ con la densidad de carga uniforme ρ0 .
Ahora, para obtener el resultado deseado, restamos estos campos. El problema tiene simetría
cilíndrica, por lo que debemos expresar el campo de la esfera en estas coordenadas. Tenemos
que ρ⃗ = ⃗r + ⃗z 1 , por lo que ρ2 = r2 + z 2 y el vector unitario ρ̂ es:
z
r
r̂ + √
ẑ
ρ̂ = √
r +z
r + z2
Ahora, expresamos todo en coordenadas cilíndricas
 2

a ρ0
ρ 0 a3 r
ρ 0 a3 z
E = Ec − Ee =
−
ẑ
r̂
−
2ϵ0 r 3ϵ0 (r2 + z 2 )3/2
3ϵ0 (r2 + z 2 )3/2
De la misma forma, el potencial resulta
V (r, z) = Vc − Ve = −

a2 ρ0
a3 ρ
√ 0
ln r −
+C
2ϵ0
3ϵ0 r2 + z 2

donde esta constante la podemos determinar eligiendo como referencia un punto de potencial
nulo.

Explicación en la última página.

---

### Página 5

#### Problema 3
Considere una región esférica de radio b, que tiene una distribución de carga uniforme ρ(r) =
ρ0 para la región determinada por a < r < b y densidad nula para r < a. Determine el
potencial eléctrico en todo el espacio.

#### SOLUCION:
Lo que haremos primero será calcular el campo eléctrico producido por esta distribución de
carga en todo el espacio y con este resultado obtendremos el potencial utilizando:
Z p
⃗ · d⃗ℓ
Vp = −
∞

Considerando el potencial igual a cero en el infinito. El problema tiene simetría esférica y
⃗ = E r̂. Consideraremos 3 regiones: I) r < a, II) a < r < b y III)
por lo tanto se tendrá que E
r > b.
I) r < a : Consideremos como superficie gaussiana un cascaron esférico de radio r < a. Se
tiene que el vector normal a esta superficie es paralelo a r̂. De esta manera se tendrá
⃗ es paralelo al vector normal n̂ de la superficie S por lo que E
⃗ · n̂ = E
que el campo E
y por lo tanto:
Z
Z
ϕ=
E · n̂dS = E dS = E · 4πr2
S

S

Por otro lado la carga en el interior de la superficie es nula ya que esta contenida en el
conductor: qint = 0. Aplicando la Ley de Gauss se tendrá que:
E · 4πr2 = 0
Y por lo tanto E = 0, si r < a.

---

### Página 6

II) a < r < b : Consideremos ahora como superficie gaussiana una cascara esférica de radio
⃗ · n̂ = E y por lo tanto
r. Al igual que en el caso anterior se tendrá que E
Z
⃗ · n̂dS = E4πr2
ϕ=
S

La carga interior qint se puede calcular fácilmente ya que la densidad de carga es
constante. Se tendrá que qint = ρ0 V , donde V es el volumen entre la esfera de radio r
y la esfera de radio a con lo que resulta

qint = ρ0 π r3 − a3
Aplicando la ley de Gauss:
E · 4πr2 = ρ0


π r 3 − a3
3ϵ0

Con lo que se obtiene:

⃗ = ρ0 (r − a ) r̂
3ϵ0 r2
donde la dirección viene dada nuevamente por la simetría esférica.
III) r > b : Procediendo de igual manera que en la región II) veremos que la carga almacenada en la distribución que rodea al conductor será:

qint = πρ0 b3 − a3
De esta manera aplicando la ley de Gauss tendremos que:
ρ0 (b3 − a3 )
3rϵ0
ρ0 (b − a3 )
E(r)
=
r̂
3ϵ0 r2

E · 4πr2 =

Resumiendo, el campo eléctrico en todo el espacio resulta

r<a


 ρ r3 −a3
)
0(
⃗ =
r̂ a < r < b
3ϵ0 r2

3 −a3

ρ
b
(
)

r̂ r > b
3ϵ0 r2

Ahora que tenemos el campo eléctrico en todo el espacio podemos calcular el potencial
eléctrico. Debemos elegir una trayectoria para tener una expresión para el vector d⃗ℓ. Elegimos

---

### Página 7

una línea recta que vaya desde el infinito hasta una distancia r > b Como podemos ver
⃗ · d⃗ℓ = E r̂ · d⃗ℓ = Edr. De esta manera el potencial eléctrico será:
Z r
Z r
Z r
ρ0 (b3 − a3 )
⃗ · d⃗ℓ = −
Edr = −
V (r) = −
dr
3ϵ0 r2
∞
∞
∞
Integrando se obtiene que:
V (r) =

ρ0 (b3 − a3 )
,
3ϵ0 r

si

r>b

Ahora queremos calcular el potencial a una distancia r, donde a < r < b. Por definición
tenemos que
Z r
⃗ · d⃗ℓ
V (r) = −
∞

Descomponemos esta integral de línea separando la trayectoria desde el infinito hasta r, en
las trayectorias desde infinito hasta b mas la trayectoria desde b hasta r.
Z b
Z r
⃗ · d⃗ℓ
V (r) = −
E · dℓ + −
∞

b

La primera integral resulta de evaluar el potencial anterior en r = b :
Z b
⃗ · d⃗ℓ = ρ0 (b − a )
V (b) = −
3ϵ0 b
∞
Por otro lado, para la otra integral tendremos
Z r
Z r
ρ0 (r3 − a3 )
dr
−
E · dℓ = −
3ϵ0 r2
b
b

Z b
Z r
ρ0
=−
·
rdr − a
dr
3ϵ0
∞
b r
 2 r 

r 
ρ0
r
=−
·
−a −
3ϵ0
2 b
r
 2
b
ρ0
b −r
(r − b)
=
·
+ a3
3ϵ0
rb
De esta manera, el potencial en r resulta ser


ρ 0 b 3 − a3 b 2 − r 2
3 (r − b)
V (r) =
+
+a
,
3ϵ0
b
rb

si

a<x<b

---

### Página 8

Para la región r < a descomponemos la trayectoria desde el infinito hasta r en 3 trayectorias.
Tendremos que el potencial es
Z r
Z a
Z b
Z r
⃗ · d⃗ℓ
E · d⃗r + −
E · dℓ + −
E · dℓ = −
V (r) = −
∞

∞

a

b

Al ser nulo el campo eléctrico para r < a tendremos que
Z r
⃗ · d⃗ℓ = 0
−
a

Y de esta manera el potencial resulta ser:


ρ 0 b 3 − a3 b 2 − a2
3 (a − b)
V (r) =
+
+a
,
3ϵ0
b
ab

si

r<a

---

### Página 9

Coordenadas esféricas a cilíndricas
Consideremos el siguiente enfoque geométrico: en una superficie esférica, un punto se ubica a
una distancia ρ del origen. Si proyectamos este punto sobre el plano xy, obtenemos un radio
r. Esto se ejemplifica en la siguiente imagen

Es directo notar que esta proyección corresponde al cateto opuesto del angulo polar θ (el cual
se mide desde el eje z, con 0 ≤ θ ≤ π), es decir
r = ρ sin θ

(1)

y la coordenada vertical es el cateto adyacente, por lo tanto
z = ρ cos θ

(2)

El angulo φ es compartido en ambos sistemas, pues mide la rotación alrededor del eje z.
Observemos que ρ̂ está en el plano generado por r̂ (horizontal, radial en el plano xy) y ẑ
(vertical). Por lo que podemos escribirlo como una combinación lineal
ρ̂ = ar̂ + bẑ,
con r̂ ⊥ ẑ y |ρ̂| = 1 ⇒ a2 + b2 = 1.
Como θ es el angulo entre ρ̂ y ẑ, notemos que
cos θ = ρ̂ · ẑ = (ar̂ + bẑ) · ẑ = a(r̂ · ẑ) + b(ẑ · ẑ) = 0 + b = b

---

### Página 10

Y como se debe cumplir que a2 + b2 = 1, entonces a = ± sin θ. Ahora, como la proyección
radial de ρ̂ apunta en la misma dirección de r̂, conservamos el signo positivo. Obtenemos
ρ̂ = sin θr̂ + cos θẑ
Multiplicando la expresión por un radio ρ, tenemos
ρρ̂ = ρ⃗ = ρ sin θr̂ + ρ cos θẑ
Reemplazando las ecuaciones (1) y (2), obtenemos finalmente
ρ⃗ = rr̂ + z ẑ
ρ⃗ = ⃗r + ⃗z
