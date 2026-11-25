---
title: "Ayudantia 06"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_06_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_06_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 06

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 6
#### Problema 1
Se desea diseñar un condensador esférico a partir de un casquete conductor esférico de radio
exterior a, que sea capaz de almacenar la mayor cantidad de energía posible, sujeto a la
restricción que el campo eléctrico en la superficie de la esfera conductora interior, concéntrica
con el casquete y de radio b < a, no pueda exceder un valor dado E0 . Calcule, en función de
E0 , a y constantes, el valor que debe tener el radio b y la magnitud de la energía que puede
almacenar el conductor.

---

### Página 2

#### Problema 2
Dos placas conductoras cuadradas, de longitud lateral d, están ubicadas radialmente, formando un ángulo α. Uno de los extremos de las placas se encuentra a distancia δ del punto de
intersección entre los planos que estas definen. La separación entre ambas en el otro extremo
es mucho menor que su longitud, como se muestra en la figura. Una de las placas se encuentra
a un potencial V = 0 y la otra a un potencial V = V0 .

Encuentre:
a) El campo eléctrico entre las placas.
b) La densidad superficial de carga σ sobre las placas.
c) El potencial entre las placas.
d) La capacidad del sistema.

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 6
#### Problema 1
Se desea diseñar un condensador esférico a partir de un casquete conductor esférico de radio
exterior a, que sea capaz de almacenar la mayor cantidad de energía posible, sujeto a la
restricción que el campo eléctrico en la superficie de la esfera conductora interior, concéntrica
con el casquete y de radio b < a, no pueda exceder un valor dado E0 . Calcule, en función de
E0 , a y constantes, el valor que debe tener el radio b y la magnitud de la energía que puede
almacenar el conductor.

#### SOLUCION:
Suponiendo una carga Q en la superficie conductora de radio b, entonces el campo eléctrico
a una distancia r del origen será de la forma:
Q
4πε0 r2


1 1
Q
⇒V =
−
4πε0 b a
E(r) =

---

### Página 2

Donde V es la diferencia de potencial entre la superficie de radio interior y exterior. De esta
manera, se obtiene la capacidad
4πε0 ab
Q
=
C=
V
a−b
Por otro lado, tomando el caso límite r = b en el cual el campo eléctrico alcanza su máximo
valor posible E(r = b) = E0 , se tiene:
σ
ε0
⇒ Q = 4πb σ = 4πb2 ε0 E0
b2 E0
⇒ E(r) = 2
r
E0 =

Luego se usan estos valores obtenidos para calcular la energía del sistema:
U=

Q2
2πε0 b3 E02 (a − b)
=
2C
a

Ahora para encontrar su máximo (o mínimo):

2πε0 E02
dU
=
3ab2 − 4b3 = 0
db
a
3a
⇒b=
Luego calculando la segunda derivada:

d2 U
2πε0 E02
2πε0 E02 18a2 − 27a2
3a
′′
=
6ab − 12b =⇒ U b =
=
<0
db2
a
a

Por lo tanto, U b = 3a
es máximo, con:
27πε0 E02 a3
3a
U b=
=

---

### Página 3

#### Problema 2
Dos placas conductoras cuadradas, de longitud lateral d, están ubicadas radialmente, formando un ángulo α. Uno de los extremos de las placas se encuentra a distancia δ del punto de
intersección entre los planos que estas definen. La separación entre ambas en el otro extremo
es mucho menor que su longitud, como se muestra en la figura. Una de las placas se encuentra
a un potencial V = 0 y la otra a un potencial V = V0 .

Encuentre:
a) El campo eléctrico entre las placas.
b) La densidad superficial de carga σ sobre las placas.
c) El potencial entre las placas.
d) La capacidad del sistema.
#### SOLUCION:
Sabemos que las lineas equipotenciales deben respetar la geometría del dispositivo. De esta
forma, las equipotenciales serán rectas radiales.

---

### Página 4

Por lo tanto, las lineas de campo, al ser perpendiculares a las equipotenciales, deben seguir
la dirección θ̂, es decir, son arcos concéntricos.

Entonces, despreciando los efectos del borde, podemos suponer que el potencial entre las
placas solo depende del ángulo polar.
Si usamos coordenadas cilíndricas, con el eje z coincidiendo con la intersección entre los
planos donde se encuentran las placas, y r y θ como coordenadas polares en el plano z = 0, la
afirmación anterior quiere decir que V solo depende de θ y no de r ni z. Esta aproximación es
razonable en la medida que la abertura α sea pequeña y la distancia d sea lo suficientemente
grande.
Como la función potencial V satisface la ecuación de Laplace entre los conductores, tenemos
que, usando la expresión del Laplaciano en cilíndricas:
∂V
1 ∂ 2V
∂ 2V
1 ∂
r
+ 2 2 +
=0
∇V =
r ∂r
∂r
r ∂θ
∂z 2
junto al hecho que V solo depende de θ, obtenemos
∂ 2V
=0
∂θ2
La solución de esta ecuación diferencial de segundo grado es de la forma
V (θ) = Aθ + B
en que A y B son constantes de integración. Si escogemos θ = 0 coincidiendo con la placa que
se encuentra a potencial cero y θ = α coincidiendo con la placa que se encuentra a potencial
V0 , tenemos que
V (0) = B = 0 → B = 0
V0
V (α) = Aα = V0 → A =
α
Con lo que obtenemos:
V (θ) = V0

θ
α

(1)

---

### Página 5

para 0 ≤ θ ≤ α.
De la ecuación (1) podemos obtener inmediatamente el campo eléctrico:
⃗ = −∇V
E
∂V
∂V
1 ∂V
r̂ −
θ̂ −
ẑ
=−
∂r
r ∂θ
∂z
Como habíamos deducido que el campo iba en dirección θ̂, nos queda
⃗ = − 1 ∂V θ̂ = − V0 θ̂
E
r ∂θ
αr

(2)

para 0 ≤ θ ≤ α.
A partir de la expresión para el campo eléctrico y utilizando el hecho que sobre un conductor
la densidad de carga es proporcional a la magnitud del campo, obtenemos la densidad de
carga sobre las placas.
⃗ · n̂ = σ
E
ϵ0
⇒ σ = ϵ0 E θ̂ · n̂
En la placa θ = 0, la normal n̂ y la dirección θ̂ son paralelos. Entonces θ̂ · n̂ = 1.
De la ecuación (2) obtenemos
ϵ0 V0
σ(θ = 0) = −
αr

(3)

En tanto que la placa superior, haciendo un calculo similar, pero esta vez usando que θ̂ y n̂
son anti-paralelos, obtenemos
ϵ0 V0
σ(θ = α) = +
(4)
αr
Integrando (3) y (4) obtenemos la carga total sobre cada una de las placas.
En la placa superior
Z d+δ
ϵ0 V0
d+δ
ϵ0 V0
dr =
ln
Q=
αr
α
δ
δ
Mientras la carga de la placa interior es −Q.
Finalmente, la capacidad del condensador es Q/∆V , donde ∆V = V0 − 0 = V0 , por lo tanto
ϵ0
d+δ
C = ln
.
α
δ

---

### Página 6

Gradiente y Laplaciano en distintas coordenadas1
Coordenadas Cartesianas

∂f
∂f
∂f
x̂ +
ŷ +
ẑ
∂x
∂y
∂z
∂ 2f
∂ 2f
∂ 2f
∇2 f =
+
+
∂x2
∂y 2
∂z 2
∇f =

Coordenadas Cilíndricas

∂f
1 ∂f
∂f
θ̂ +
r̂ +
ẑ
∂r
r ∂θ
∂z
1 ∂
∂ 2f
∂f
1 ∂ 2f
∇2 f =
r
+ 2 2 + 2
r ∂r
∂r
r ∂θ
∂z
∇f =

Coordenadas Esféricas

1 ∂f
1 ∂f
∂f
ρ̂ +
θ̂ +
ϕ̂
∇f =
∂ρ
ρ ∂θ
ρ sin θ ∂ϕ
1 ∂
∂
∂ 2f
∂f
2 ∂f
∇f= 2
ρ
+ 2
sin θ
+ 2 2
ρ ∂ρ
∂ρ
ρ sin θ ∂θ
∂θ
ρ sin θ ∂ϕ2

Notar que el gradiente de un campo escalar resulta en un vector, mientras que el Laplaciano es otro
escalar, ya que ∇2 f = ∇ · (∇f ).
