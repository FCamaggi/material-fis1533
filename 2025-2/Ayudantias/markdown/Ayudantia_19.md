---
title: "Ayudantia 19"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_19_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_19_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 19

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Enunciado Ayudantía 19
21 de Octubre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Magnetostática

1.1

Campo Magnético - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Determinar el campo magnético generado por una corriente mediante su definición.
□
✓ Aplicar el principio de superposición para campos magnéticos en un sistema compuesto
□
por dos o más cuerpos.
□ Evaluar cualitativamente el campo magnético en un punto del espacio, considerando su
sentido y dirección, mediante la regla de la mano derecha.

✓ Identificar y utilizar un sistema de coordenadas pertinente al contexto.
□
✓ Identificar y diferenciar los tipos de densidades de corriente según el contexto.
□
□ Utilizar conceptos de cinemática circunferencial, tales como velocidad angular y tangencial.
□ Conocer e identificar las líneas de campo magnético correspondientes a un dipolo magnético.

✓ Conocer la unidad de medida para el campo magnético.
□
✓ Conocer el valor y la unidad de medida de la constante de permeabilidad del vacío.
□

---

### Página 2

1.2

Campo Magnético - Ley de Biot-Savart

El campo magnético que genera una carga = q” en movimiento puede ser expresado como:
B=

µ0 q v × r̂ ′
4π r2

(1)

Donde = v” es su velocidad y = µ0 ” la constante de permeabilidad del vacío:

µ0 = 4π × 10−7

Tm
A

(2)

Por otra parte, la unidad para campo magnético en el S.I es el = Tesla”:

1T=1

N
C · m/s

(3)

Otra unidad de medida relacionada es el = Gauss”:

1 G = 10−4 T
(4)
Asimismo, el campo magnético que genera una corriente estará dado por la Ley de Biot-Savart:
Densidad

Relación Densidad Corriente

Integral Campo Magnética

Lineal

—

Superficial

K(x ′ ) = σv

B(x) = 4π

RR

Volumétrica

⃗J(x ′ ) = ρv

B(x) = 4π

RRR

B(x) = 4π

R
L

S

V

Idl×(x−x ′ )
|x−x ′ |3

K(x ′ )×(x−x ′ )
dS
|x−x ′ |3
⃗
J(x ′ )×(x−x ′ )
dV
|x−x ′ |3

En ocasiones la corriente se producirá al rotar un cuerpo con carga,
por lo que puede ser útil recordar que:

v=w×r ′

(5)

Donde = w” es la velocidad angular con la que rota la superficie o volumen.
Es posible utilizar la regla de la mano derecha para determinar su sentido y dirección.

De esta manera, se puede llegar a la Tercera Ecuación de Maxwell:
∇·B=0

(6)

Lo anterior implica que no existen monopolos magnéticos.
Luego, las líneas de campo magnético se cierran sobre sí mismas,
es decir, salen del polo norte y entran por el polo sur (ver Figura 1).

1.3

Campo Magnético - Cómo Utilizarlo Correctamente

Los pasos a seguir para aplicar el campo magnético por definición son:
1. Reconocer el tipo de densidad de corriente asociado al cuerpo en estudio, según la dimensión en la que vive. Por ejemplo, un disco es bidimensional y, por lo tanto, su
densidad sería superficial.

---

### Página 3

2. Luego, cambiar el diferencial según el tipo de densidad y calcular el valor de la densidad
de corriente si es que no la entregan de manera explícita. En este paso se deberá utilizar
el tipo de coordenada pertinente al problema y las relaciones entre los diferenciales, las
cuales se pueden encontrar en la tabla del Anexo ??.
3. Después, y respetando el tipo de coordenadas en uso, se tendrá que construir = x”, el cual
es un vector que se extiende desde el origen hasta el punto deseado. Siempre recuerden
agregar el sentido y dirección de un vector.
4. Por último, y respetando el tipo de coordenadas en uso, se tendrá que construir = x ′ ”, el
cual es un vector que recorre desde el origen todo el cuerpo por el cual circula corriente.
Siempre recuerden agregar el sentido y dirección de un vector.
5. Realizar el producto cruz entre la densidad de corriente y la diferencia de los vectores de
posición. Para una resolución más sencilla de esta operación, revisar Anexo ??.
6. No hay que olvidar los límites de integración, los cuales dependerán netamente del ejercicio en cuestión, en especial del sentido de la corriente. Será más fácil guiarse por la
figura que generalmente se encontrará a disposición.
7. Por último, solo quedaría integrar la expresión cuidadosamente. Recuerden que el campo
magnético es un vector (por lo que también posee sentido y dirección) y que no es posible
mezclar términos que pertenezcan a distintas coordenadas a la hora de integrar.

Figura 1. Líneas de campo magnético correspondientes a un imán.

---

### Página 4

1.3.1

“Ejercicios Teoría Electromagnética ”, 12.5.6, Fabián Cádiz

Considere un disco muy delgado que tiene una densidad de carga superficial σ uniformemente distribuida. El disco se pone a girar a velocidad angular w en torno a su eje.
Encuentre el campo magnético en el eje del disco.

Figura 2. Disco cargado girando en torno a su eje.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo magnético en el eje del disco. Como la figura no posee ninguna
simetría apta para la Ley de Ampére, se aplicará la definición de campo magnético:
ZZ
K(x ′ ) × (x − x ′ )
B(x) =
dS
4π
|x − x ′ |3
S
Se nota que se usa la doble integral debido a la naturaleza del problema,
puesto que el disco vive en dos dimensiones.

Además, y como el disco está en revolución, se producirá una corriente que vendrá dada por:
K = σv
Como no se conoce la velocidad, se deberá determinar de la siguiente forma:

v=w×r ′

---

### Página 5

1.3.2

“Ejercicios Teoría Electromagnética ”, 12.5.14, Fabián Cádiz

Considere la espira de corriente formada por segmentos radiales y arcos de circunferencia
como se muestra en la figura. Obtenga el campo magnético B en el punto P .

Figura 3. Espira de Corriente.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo magnético en el punto = P ”, el cual puede ser expresado como
la suma de los campos generados por los 5 segmentos . Como las figuras no poseen ninguna
simetría apta para la Ley de Ampére, se aplicará la definición de campo magnético:
Z
Idl × (x − x ′ )
B(x) =
4π L
|x − x ′ |3
Se nota que se usa la integral simple debido a la naturaleza del problema,
puesto que la espira vive en una dimensión.

Figura 4. Espira de Corriente (Segmentos).

---

## Solución

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Ayudantía 19
21 de Octubre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Magnetostática

1.1

Campo Magnético - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Determinar el campo magnético generado por una corriente mediante su definición.
□
✓ Aplicar el principio de superposición para campos magnéticos en un sistema compuesto
□
por dos o más cuerpos.
□ Evaluar cualitativamente el campo magnético en un punto del espacio, considerando su
sentido y dirección, mediante la regla de la mano derecha.

✓ Identificar y utilizar un sistema de coordenadas pertinente al contexto.
□
✓ Identificar y diferenciar los tipos de densidades de corriente según el contexto.
□
□ Utilizar conceptos de cinemática circunferencial, tales como velocidad angular y tangencial.
□ Conocer e identificar las líneas de campo magnético correspondientes a un dipolo magnético.

✓ Conocer la unidad de medida para el campo magnético.
□
✓ Conocer el valor y la unidad de medida de la constante de permeabilidad del vacío.
□

---

### Página 2

1.2

Campo Magnético - Ley de Biot-Savart

El campo magnético que genera una carga = q” en movimiento puede ser expresado como:
B=

µ0 q v × r̂ ′
4π r2

(1)

Donde = v” es su velocidad y = µ0 ” la constante de permeabilidad del vacío:

µ0 = 4π × 10−7

Tm
A

(2)

Por otra parte, la unidad para campo magnético en el S.I es el = Tesla”:

1T=1

N
C · m/s

(3)

Otra unidad de medida relacionada es el = Gauss”:

1 G = 10−4 T
(4)
Asimismo, el campo magnético que genera una corriente estará dado por la Ley de Biot-Savart:
Densidad

Relación Densidad Corriente

Integral Campo Magnética

Lineal

—

Superficial

K(x ′ ) = σv

B(x) = 4π

RR

Volumétrica

⃗J(x ′ ) = ρv

B(x) = 4π

RRR

B(x) = 4π

R
L

S

V

Idl×(x−x ′ )
|x−x ′ |3

K(x ′ )×(x−x ′ )
dS
|x−x ′ |3
⃗
J(x ′ )×(x−x ′ )
dV
|x−x ′ |3

En ocasiones la corriente se producirá al rotar un cuerpo con carga,
por lo que puede ser útil recordar que:

v=w×r ′

(5)

Donde = w” es la velocidad angular con la que rota la superficie o volumen.
Es posible utilizar la regla de la mano derecha para determinar su sentido y dirección.

De esta manera, se puede llegar a la Tercera Ecuación de Maxwell:
∇·B=0

(6)

Lo anterior implica que no existen monopolos magnéticos.
Luego, las líneas de campo magnético se cierran sobre sí mismas,
es decir, salen del polo norte y entran por el polo sur (ver Figura 1).

1.3

Campo Magnético - Cómo Utilizarlo Correctamente

Los pasos a seguir para aplicar el campo magnético por definición son:
1. Reconocer el tipo de densidad de corriente asociado al cuerpo en estudio, según la dimensión en la que vive. Por ejemplo, un disco es bidimensional y, por lo tanto, su
densidad sería superficial.

---

### Página 3

2. Luego, cambiar el diferencial según el tipo de densidad y calcular el valor de la densidad
de corriente si es que no la entregan de manera explícita. En este paso se deberá utilizar
el tipo de coordenada pertinente al problema y las relaciones entre los diferenciales, las
cuales se pueden encontrar en la tabla del Anexo ??.
3. Después, y respetando el tipo de coordenadas en uso, se tendrá que construir = x”, el cual
es un vector que se extiende desde el origen hasta el punto deseado. Siempre recuerden
agregar el sentido y dirección de un vector.
4. Por último, y respetando el tipo de coordenadas en uso, se tendrá que construir = x ′ ”, el
cual es un vector que recorre desde el origen todo el cuerpo por el cual circula corriente.
Siempre recuerden agregar el sentido y dirección de un vector.
5. Realizar el producto cruz entre la densidad de corriente y la diferencia de los vectores de
posición. Para una resolución más sencilla de esta operación, revisar Anexo ??.
6. No hay que olvidar los límites de integración, los cuales dependerán netamente del ejercicio en cuestión, en especial del sentido de la corriente. Será más fácil guiarse por la
figura que generalmente se encontrará a disposición.
7. Por último, solo quedaría integrar la expresión cuidadosamente. Recuerden que el campo
magnético es un vector (por lo que también posee sentido y dirección) y que no es posible
mezclar términos que pertenezcan a distintas coordenadas a la hora de integrar.

Figura 1. Líneas de campo magnético correspondientes a un imán.

---

### Página 4

1.3.1

“Ejercicios Teoría Electromagnética ”, 12.5.6, Fabián Cádiz

Considere un disco muy delgado que tiene una densidad de carga superficial σ uniformemente distribuida. El disco se pone a girar a velocidad angular w en torno a su eje.
Encuentre el campo magnético en el eje del disco.

Figura 2. Disco cargado girando en torno a su eje.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo magnético en el eje del disco. Como la figura no posee ninguna
simetría apta para la Ley de Ampére, se aplicará la definición de campo magnético:
ZZ
K(x ′ ) × (x − x ′ )
B(x) =
dS
4π
S
Se nota que se usa la doble integral debido a la naturaleza del problema,
puesto que el disco vive en dos dimensiones.

Además, y como el disco está en revolución, se producirá una corriente que vendrá dada por:
K = σv
Como no se conoce la velocidad, se deberá determinar de la siguiente forma:

v=w×r ′
Paso 1: Componentes Campo Magnético - r
Desde ahora en adelante, nuestro sistema de referencia será el centro del disco y se utilizarán
coordenadas cilíndricas por la geometría del ejercicio. Se recuerda que el vector r parte en el
origen y se extiende hasta el punto en donde se quiere calcular el campo:
r = zẑ,

z ∈ ] − ∞, ∞[

Donde = z” se refiere a cualquier punto del eje = z”.

---

### Página 5

Paso 2: Componentes Campo Magnético - r ′
Luego, el vector r ′ inicia en el origen y recorre todo el cuerpo con carga:
r ′ = rr̂,

r ∈ [0, R[,

θ ∈ [0, 2π[

Donde = r” es el radio del disco y = r̂” la componente radial en coordenadas cilíndricas.

Paso 3: Componentes Campo Magnético - r − r ′
Con lo anterior, también se construyen las demás componentes de la integral:
r − r ′ = zẑ − rr̂
Calculando el módulo del vector anterior:

|r − r ′ | =

p
z 2 + r2

Paso 4: Densidad de Corriente - K
Utilizando la fórmula respectiva se tiene que:
K = σv
= σ(w × r ′ )
= σ(wẑ × rr̂)
= σwrθ̂
Para realizar este producto cruz de manera sencilla se recuerda que estamos en la base “(r, θ, z)”
en coordenadas cilíndricas, por lo que ẑ × r̂ = θ̂. Al avanzar hacia adelante el signo es positivo.

Paso 5: Componentes Campo Magnético - K × (r − r ′ )
Usando los resultados anteriores:
K × (r − r ′ ) = σwrθ̂ × (zẑ − rr̂)
= σwr(θ̂ × zẑ − θ̂ × rr̂)
= σwr(zr̂ + rẑ)
Para realizar estos productos cruz de manera sencilla se recuerda que estamos en la base “(r, θ, z)”
en coordenadas cilíndricas, por lo que θ̂ × ẑ = r̂ y θ̂ × r̂ = −ẑ. Al avanzar hacia adelante el signo
es positivo, mientras que al ir hacia atrás es negativo, respectivamente.

Paso 6: Componentes Campo Magnético - dS
Considerando que la densidad de corriente es superficial y que la única componente constante
para el cascarón es z:
ds = r drdθ
Para llegar a lo anterior se utilizó el diferencial de superficie para cilíndricas,
observando la componente constante y omitiendo el sentido vectorial.

---

### Página 6

Paso 7: Campo Magnético - B
Finalmente, se utiliza la definición de campo magnético considerando los límites de integración
propuestos con anterioridad:
ZZ
K(x ′ ) × (x − x ′ )
B=
dS
4π
S
µ0 2π R σwr(zr̂ + rẑ)
=
r drdθ
4π 0
(z 2 + r2 )3/2
Para simplificar los cálculos, y por temas de simetría, se puede
obviar la parte asociada a la componente radial. De esta manera:

B=
4π

Z 2π Z R

σwr3 ẑ
drdθ
(z 2 + r2 )3/2

Z R
r3 ẑ
=
dr
· 2πσw
2 3/2
4π
0 (z + r )
µ0 σw R
r3 ẑ
=
dr
2 3/2
0 (z + r )
√
Z z 2 +R2
µ0 σw
α(α2 − z 2 )ẑ
=
dα
√
α3
z2
Z √z 2 +R2
µ0 σw
z2
=
(1 − 2 )ẑ dα
√
α
z2
√

z 2 +R2

µ0 σw
z2
=
(α + ) √
ẑ
α
z2
√
z2
z2
µ0 σw p 2
− z 2 − √ ) ẑ
=
( z + R2 + √
z 2 + R2
z2
µ0 σw z + R + z
|z|
=
( √
− |z| −
) ẑ
|z|
z +R
µ0 σw 2z 2 + R2
(√
− 2|z|) ẑ
=
z 2 + R2
Notar que se realizó un cambio de variable α2 = z 2 + r2√ → 2α dα = 2r dr.
También, y como z > 0, se puede considerar que z 2 = |z| = z.

(7)

---

### Página 7

1.3.2

“Ejercicios Teoría Electromagnética ”, 12.5.14, Fabián Cádiz

Considere la espira de corriente formada por segmentos radiales y arcos de circunferencia
como se muestra en la figura. Obtenga el campo magnético B en el punto P .

Figura 3. Espira de Corriente.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo magnético en el punto = P ”, el cual puede ser expresado como
la suma de los campos generados por los 5 segmentos . Como las figuras no poseen ninguna
simetría apta para la Ley de Ampére, se aplicará la definición de campo magnético:
Idl × (x − x ′ )
B(x) =
4π L
Se nota que se usa la integral simple debido a la naturaleza del problema,
puesto que la espira vive en una dimensión.

Figura 4. Espira de Corriente (Segmentos).

---

### Página 8

Paso 1: Campo Magnético Segmento 1 - B1
Desde ahora en adelante, nuestro sistema de referencia será el punto = P ” y se utilizarán
coordenadas cilíndricas por la geometría del ejercicio. Se recuerda que el vector r inicia en el
origen y se extiende hasta el punto en donde se quiere calcular el campo:
r=0
Como el centro de referencia coincide con el punto a calcular el vector es nulo.

Luego, el vector r ′ inicia en el origen y recorre todo el cuerpo con corriente:
r ′ = rr̂,

r ∈ ]∞, b],

θ=0

Donde = r” es el largo del segmento y = r̂” la componente radial en coordenadas cilíndricas.

Con lo anterior, también se construyen las demás componentes de la integral:
r − r ′ = 0 − rr̂
Calculando el módulo del vector anterior:

|r − r ′ | = r
Usando los resultados anteriores:
Idl × (r − r ′ ) = Idrr̂ × −rr̂
=0
Como es un producto cruz entre dos componentes iguales, el resultado es 0.
Para determinar = dl” se debe observar cómo es el movimiento de la corriente (en este
caso es de forma radial), las coordenadas en uso (cilíndricas) y el tipo de diferencial (lineal).

Finalmente, se utiliza la definición de campo magnético considerando los límites de integración
propuestos con anterioridad para el segmento 1:
Idl × (x − x ′ )
B1 =
(8)
4π L
=0
Paso 2: Campo Segmento 2 - B2
Se recuerda que el vector r inicia en el origen y se extiende hasta el punto en donde se quiere
calcular el campo:
r=0
Como el centro de referencia coincide con el punto a calcular el vector es nulo.

Luego, el vector r ′ inicia en el origen y recorre todo el cuerpo con corriente:
r ′ = br̂,

θ ∈ [0, ϕ]

Donde = b” es el radio de la circunferencia mayor y = r̂” la componente radial en
coordenadas cilíndricas. Se debe hacer énfasis en cómo es el sentido de la corriente.

Se siguen determinando componentes de la integral:
r − r ′ = 0 − br̂
Calculando el módulo del vector anterior:

---

### Página 9

|r − r ′ | = b
Usando los resultados anteriores:
Idl × (r − r ′ ) = Ibdθθ̂ × −br̂
= Ib2 dθ ẑ
Para realizar este producto cruz de manera sencilla se recuerda que estamos en la base “(r, θ, z)”
en coordenadas cilíndricas, por lo que θ̂ × r̂ = −ẑ. Al avanzar hacia atrás el signo es negativo.
Para determinar = dl” se debe observar cómo es el movimiento de la corriente (en este caso
es de forma angular), las coordenadas en uso (cilíndricas) y el tipo de diferencial (lineal).

Finalmente, se utiliza la definición de campo magnético considerando los límites de integración
propuestos con anterioridad para el segmento 2:
Idl × (x − x ′ )
B2 =
4π L
Z ϕ 2
Ib dθ ẑ
=
4π 0
b3
(9)
Z ϕ
Idθ ẑ
=
4π 0
b
µ0 Iϕ
ẑ
=
4πb
Paso 3: Campo Segmento 3 - B3
Se recuerda que el vector r inicia en el origen y se extiende hasta el punto en donde se quiere
calcular el campo:
r=0
Como el centro de referencia coincide con el punto a calcular el vector es nulo.

Luego, el vector r ′ inicia en el origen y recorre todo el cuerpo con corriente:
r ′ = rr̂,

r ∈ [b, a],

θ=ϕ

Donde = r” es el largo del segmento y = r̂” la componente radial en coordenadas cilíndricas.

Con lo anterior, también se construyen las demás componentes de la integral:
r − r ′ = 0 − rr̂
Calculando el módulo del vector anterior:

|r − r ′ | = r
Usando los resultados anteriores:
Idl × (r − r ′ ) = Idrr̂ × −rr̂
=0
Como es un producto cruz entre dos componentes iguales, el resultado es 0.
Para determinar = dl” se debe observar cómo es el movimiento de la corriente (en este
caso es de forma radial), las coordenadas en uso (cilíndricas) y el tipo de diferencial (lineal).

---

### Página 10

Finalmente, se utiliza la definición de campo magnético considerando los límites de integración
propuestos con anterioridad para el segmento 3:
Idl × (x − x ′ )
B3 =
(10)
4π L
=0
Paso 4: Campo Segmento 4 - B4
Se recuerda que el vector r inica en el origen y se extiende hasta el punto en donde se quiere
calcular el campo:
r=0
Como el centro de referencia coincide con el punto a calcular el vector es nulo.

Luego, el vector r ′ inicia en el origen y recorre todo el cuerpo con corriente:
r ′ = ar̂,

θ ∈ [ϕ, 0]

Donde = a” es el radio de la circunferencia mayor y = r̂” la componente radial en
coordenadas cilíndricas. Se debe hacer énfasis en cómo es el sentido de la corriente.

Con lo anterior, también se construyen las demás componentes de la integral:
r − r ′ = 0 − ar̂
Calculando el módulo del vector anterior:

|r − r ′ | = a
Usando los resultados anteriores:
Idl × (r − r ′ ) = Iadθθ̂ × −ar̂
= Ia2 dθ ẑ
Para realizar este producto cruz de manera sencilla se recuerda que estamos en la base “(r, θ, z)”
en coordenadas cilíndricas, por lo que θ̂ × r̂ = −ẑ. Al avanzar hacia atrás el signo es negativo.
Para determinar = dl” se debe observar cómo es el movimiento de la corriente (en este caso
es de forma angular), las coordenadas en uso (cilíndricas) y el tipo de diferencial (lineal).

Finalmente, se utiliza la definición de campo magnético considerando los límites de integración
propuestos con anterioridad para el segmento 4:
Idl × (x − x ′ )
B4 =
4π L
Z 0 2
Ia dθ ẑ
=
4π ϕ
a3
(11)
Z 0
Idθ ẑ
=
4π ϕ
a
µ0 Iϕ
=−
ẑ
4πa

---

### Página 11

Paso 5: Campo Segmento 5 - B5
Se recuerda que el vector r inicia en el origen y se extiende hasta el punto en donde se quiere
calcular el campo:
r=0
Luego, el vector r ′ inicia en el origen y recorre todo el cuerpo con corriente:
r ′ = rr̂,

r ∈ [b, ∞[,

θ=0

Donde = r” es el largo del segmento y = r̂” la componente radial en coordenadas cilíndricas.

Con lo anterior, también se construyen las demás componentes de la integral:
r − r ′ = 0 − rr̂
Calculando el módulo del vector anterior:

|r − r ′ | = r
Usando los resultados anteriores:
Idl × (r − r ′ ) = Idrr̂ × −rr̂
=0
Como es un producto cruz entre dos componentes iguales, el resultado es 0.
Para determinar = dl” se debe observar cómo es el movimiento de la corriente (en este
caso es de forma radial), las coordenadas en uso (cilíndricas) y el tipo de diferencial (lineal).

Finalmente, se utiliza la definición de campo magnético considerando los límites de integración
propuestos con anterioridad para el segmento 5:
Idl × (x − x ′ )
B5 =
(12)
4π L
=0
Paso 6: Principio de Superposición - B
Finalmente, y mediante el principio de superposición, el campo magnético en el punto P será
la suma de los campos generados por los 5 subtramos:
B = B1 + B2 + B3 + B4 + B5
µ0 Iϕ
µ0 Iϕ
=
ẑ −
ẑ
4πb
4πa
µ0 Iϕ 1 1
=
( − ) ẑ
4π b a

(13)
