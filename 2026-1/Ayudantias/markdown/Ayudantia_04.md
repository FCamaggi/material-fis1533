---
title: "Ayudantia 04"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_04.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_04_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 04

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 4
Campo Eléctrico: Distribuciones Continuas II

#### Problema 1
Un tubo cilíndrico de radio R y largo L posee una densidad de carga superficial σ. Determine el
campo eléctrico en un punto P ubicado en el mismo eje que el de simetría del cilindro, a una distancia a del extremo más cercano de este. Considere el origen del sistema en el centro del cilindro.

#### Problema 2
Un anillo de radio R0 tiene carga positiva Q, la cual esta distribuida uniformemente sobre su largo.
Considere una carga puntual de carga q negativa y masa m, la cual se ubica en reposo en el eje de
simetria del anillo, cerca del origen del sistema. Además, la carga está soldad a un resorte ideal de
constante elástica k0 y largo natural 0 con un extremo en el centro del anillo.

---

### Página 2

(a) Calcule el campo eléctrico en el eje de simetria del anillo.
(b) Calcule la fuerza total que siente la carga.
(c) Si la carga q se mueve exclusivamente en el eje de simetría del anillo, escriba las ecuaciones
que rigen su movimiento.
(d) Asuma que el radio del anillo es mucho más grande que las distancias que puede tomar
la carga puntual respecto al centro del anillo (z ! R0 ), estime la frecuencia de pequeñas
oscilaciones.
#### Problema 3
Se tiene un recipiente hemisférico de radio interior a, con una carga total Q repartida por su superficie. Calcule el campo eléctrico en su centro de curvatura.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 4
Campo Eléctrico: Distribuciones Continuas II

#### Problema 1
Un tubo cilíndrico de radio R y largo L posee una densidad de carga superficial σ. Determine el
campo eléctrico en un punto P ubicado en el mismo eje que el de simetría del cilindro, a una distancia a del extremo más cercano de este. Considere el origen del sistema en el centro del cilindro.

#### Solución
Para este problema imaginamos la siguiente situación, colocamos el eje z en el eje de simetría del
cilindro cuyo centro está en el origen del sistema.

---

### Página 2

Sin realizar ningún tipo de calculo sabemos algo sobre el campo eléctrico, por la simetría del problema, sabemos que las componentes en x e y van a ser 0.
Primero parametrizamos nuestro r1 , por conveniencia, utilizaremos coordenadas cilíndricas,

x1 = R cos ϕ x̂

Ñ

ϕ P p0, 2πq

y 1 = R sin ϕ ŷ

Ñ

ϕ P p0,2πq

Ñ

z P p´L{2, L{2q

z = z ẑ

Y el punto donde queremos medir el campo eléctrico, r, lo escribimos simplemente como,
ˆ
r“

˙
L
` a ẑ

De esta forma ya tenemos todo para definir nuestra integral para el campo eléctrico,
ˆ

r - r = -R cos ϕ x̂ - R sin ϕ ŷ `
|r - r1 |3 = pR2 ` p

˙
L
` a ´ z ẑ

L
` a ´ zq2 q3{2

El diferencial de carga lo definiremos nuevamente (Y como lo haremos el resto del curso) utilizando
la densidad de carga. Recuerden incluir los jacobianos cuando utlizamos coordenadas como
polares o esféricas!!!.
dq = σdA = σRdϕdz
Entonces para calcular el campo eléctrico escribimos la integral,

E“
4πε0

ȷ„
ȷ´3{2
ż 2π ż L{2 „
L
L
p ` a ´ zqẑ ´ R cos ϕx̂ ´ R sin ϕŷ R ` p ` a ´ zq
σRdϕdz
´L{2

Eliminamos directamente las contribuciones en x e y, porque sabemos que son 0, de todas formas
si deseas calcularas, rápidamente obtendrás que es 0.
La integral que nos queda es bastante simple utilizando sustituciones bastante evidentes (u = L2 `
a ´ z), obteniendo como resultado final,
⃗ = Rσ
E
2ε0

ˆ

´ 2
1{2
pR ` a q
pR ` pL2 ` a2 q1{2

˙

(1)

---

### Página 3

#### Problema 2
Un anillo de radio R0 tiene carga positiva Q, la cual esta distribuida uniformemente sobre su largo.
Considere una carga puntual de carga q negativa y masa m, la cual se ubica en reposo en el eje de
simetria del anillo, cerca del origen del sistema. Además, la carga está soldad a un resorte ideal de
constante elástica k0 y largo natural 0 con un extremo en el centro del anillo.

(a) Calcule el campo eléctrico en el eje de simetria del anillo.
(b) Calcule la fuerza total que siente la carga.
(c) Si la carga q se mueve exclusivamente en el eje de simetría del anillo, escriba las ecuaciones
que rigen su movimiento.
(d) Asuma que el radio del anillo es mucho más grande que las distancias que puede tomar
la carga puntual respecto al centro del anillo (z ! R0 ), estime la frecuencia de pequeñas
oscilaciones.

#### Solución
Primero necesitamos calcular el campo eléctrico del anillo respecto a su eje de simetría, para esto
utilizaremos la integral general para el campo eléctrico de una distribución,
E“
4πε0

ż

dq1 pr ´ r1 q
|r ´ r1 |3

Tenemos que definir nuestro r y r1 , recuerden r es donde estoy midiendo el campo (En este caso el
eje de simetría) y r1 es donde está ubicada nuestra carga, es decir, el anillo, Lo podemos definir de
la siguiente forma,

---

### Página 4

r = 0 x̂ ` 0 ŷ ` z ẑ
r1 = R0 cos ϕ x̂ ` R0 sin ϕ ŷ ` 0 ẑ
r - r1 = -R0 cos ϕ x̂ - R0 sin ϕ ` z ẑ
|r - r1 |2 = R02 ` z 2
Quedando solo por definir el diferencial de carga de la forma,
dq = λdl = λRdϕ
Como verán este procedimiento es bien estándar, siempre que calculemos campos eléctricos mediante integrales será así (Luego veremos otro forma de calcular campos eléctricos mucho más
fácil!). Volviendo al problema, reemplazando por lo que acabamos de obtener, la integral a resolver
sería la siguiente,
λ
E(z) = 
4πϵ0

ż 2π

p´R0 cos ϕ x̂ ´ R0 sin ϕ ` z ẑq
Rdϕ
pR02 ` z 2 q3{2

Ya sabemos que pasa con las integrales en los ejes x e y, se van por argumentos de simetría. Nos
queda por resolver,
R0 λ
E(z) = 
4πϵ0

ż 2π

z
pR02 ` z 2 q3{2

dϕ ẑ

La única variable que tenemos en esta integral es z, las otras son todas constantes. ¿Depende z de
ϕ? Claramente no, es decir, esta integral es completamente trivial de resolver, dando como resultado
el campo eléctrico generado por un anillo de distribución de carga uniforme, en su eje de simetría.
E(z) = 

z
R0 λ
2ϵ0 pR0 ` z 2 q3{2

Hasta acá el resultado es correcto, podrían pedirnos dejarnos el campo expresado en término de Q
en vez de λ es decir, utilizamos el hecho de que la carga está distribuida uniformemente,
λ“

Q
2πR0

Quedando como resultado el siguiente,
E(z) = 

Qz
4πϵ0 pR0 ` z 2 q3{2

---

### Página 5

Ambos resultados son igual de válidos, lo dejamos expresado así ya que Q era un dato entregado
en el problema y no λ, pero como sabemos ambos conceptos están relacionados.
Hasta acá hemos resuelto solamente el primer inciso, para calcular la fuerza que percibe la carga
puntual debemos considerar dos contribuciones, la fuerza de Coulomb y la fuerza elástica.
Para la fuerza de Coulomb necesitamos la carga eléctrica de la carga puntual, como se nos entrega
el dato de que esta carga es negativa, nos conviene escribirlo como ´|q|.
Felec = ´|q|E = ´

|q|Qz
4πϵ0 pR02 ` z 2 q3{2

Y para la fuerza elástica, debemos considerar el largo natural del resorte como 0,
Felastica = -zk0 ẑ
Sumando ambas contribuciones obtenemos la fuerza que percibe la carga puntual en función de su
posición en el eje z,
„
F = - k0 `

ȷ
|q|Q
z ẑ
4πϵ0 pR02 ` z 2 q3{2

Utilizando segunda ley de newton obtenemos la siguiente ecuación de movimiento,
„
ȷ
d2 z
|q|Q
m 2 = - k0 `
z
dt
4πϵ0 pR02 ` z 2 q3{2
Para encontrar la frecuencia de pequeñas oscilaciones debemos recordar materia de dinámica, la
forma general de un MAS es: ω 2 x ` x
: = 0, donde ω se refiere a la frecuencia del movimiento.
Pero si solo pasamo diviendo la masa m, nos estaría quedando una frecuencia dependiente de la
posición, lo que no puede ser!. Para esto utilizamos la relación que se nos entrega en el enunciado
para hacer la siguiente aproximación,
z
pR02 ` z 2 q3{2

«

z
R03

Utlizando esta aproximación, podemos escribir la ecuación de movimiento de la siguiente forma,
„
ȷ
d2 z
k0
1 |q|Q
`
`
z = 0
dt2
m 4πϵ0 mR03
Comparando al estructura de esta ecuación, con la forma general de un MAS, obtenemos que la
frecuencia de pequeñas oscilaciones para este caso es,
ω2 “

k0
|q|Q
`
m 4πϵ0 mR03

---

### Página 6

#### Problema 3
Se tiene un recipiente hemisférico de radio interior a, con una carga total Q repartida por su superficie. Calcule el campo eléctrico en su centro de curvatura.

#### Solución
La idea de este ejercicio es ya terminar de consolidar nuestras habilidades para calcular campos
eléctricos. Primero, como ya hemos hecho bastantes veces, definimos nuestros r y r1 , mismo cuento de siempre, r donde queremos medir el campo y r1 donde está nuestra carga. Claro que por
conveniencia elegimos el origen del sistema justo en el centro de curvatura, de tal manera que,

r = 0
r1 = a cos ϕ sin θ x̂ ` a sin ϕ sin θ ŷ ` a cos θ ẑ Ñ ϕ P r0, 2πs , θ P rπ{2, πs

Y definiendo el diferencial de carga como,
dq = σa2 sin θdθdϕ
Escribimos la integral como,
E = ´
4πϵ0

ż 2π ż π

a cos ϕ sin θ x̂ ` a sin ϕ sin θ ŷ ` a cos θ ẑ 2
σa sin θdθdϕ
a3
π{2

Nuevamente ¿Qué esperamos de las contribuciones en x e y? Que se anulen, nuevamente por argumentos de simetría, de todas maneras si no vemos eso directamente, al realizar la integral del
ángulo azimutal (ϕ), se harán 0 dichos términos. La integral que queda por calcular es,
σ
E = ´
4πϵ0

ż 2π ż π
cos θ sin θdθdϕ ẑ

π{2

---

### Página 7

Esta integral solo depende de θ, es decir, la integral en ϕ es trivial, para calcular la integral del
angulo polar basta con utilizar la identidad sin 2α = 2 cos α sin α.
Dando como reusltado final,
E“

σ
4ϵ0

Que también puede ser escrito como (Recuerden que esta densidad esta definida para la superficie
de una semi esfera),
E“

Q
8πϵ0 a2

(2)
