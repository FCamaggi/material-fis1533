---
title: "Ayudantia 26"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_26.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_26_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 26

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 26
Ley de Faraday-Lenz

#### Problema 1
⃗ “
La espira rectangular de la figura se encuentra sumergida en un campo magnético uniforme B
B x̂. Si la espira gira con velocidad angular ω utilizando el eje z como eje de rotación, y asumiendo
que en t = 0 la espira se encuentra en el plano y-z, determine la fuerza electromotriz inducida y la
corriente inducida en la espira.

#### Problema 2
Una espira rectangular de dimensiones l y w se mueve con velocidad constante ⃗v alejándose de
un alambre recto infinitamente largo que lleva corriente I en el mismo plano de la espira. Sea la
resistencia total de la espira R. ¿Cuál es la corriente en la espira en el instante en que el lado más
cercano está a una distancia r del alambre?

---

### Página 2

Ahora imagine que la espira rectangular permanece estática con las medidas que aparecen en la
imagen, pero la corriente pasa a ser variable como I(t) = a ` bt. Calcule nuevamente la f.e.m
inducida y la dirección de la corriente.

#### Problema 3
Una espira circular de radio pequeño r está fija en el espacio. Una gran espira de radio R está
situada en un plano paralelo a la primera, es coaxial con ella y se le acerca con una velocidad constante ⃗v = vẑ. Las dos espiras son conductores óhmicos. Por la espira grande circula una corriente
constante I como se muestra en la figura, y en el instante t = 0 la distancia entre las dos espiras es z.

a) Calcular cómo cambia con el tiempo el flujo del campo magnético generado por la espira
grande a través de la espira pequeña. Se asume que r ! R de manera que el campo magnético
en el interior de la espira pequeña se puede considerar uniforme e igual a su valor a lo largo
del eje.
b) Calcular la f.e.m. inducida en la espira pequeña en un instante t cualquiera.

---

### Página 3

c) Argumentar en qué dirección fluye la corriente inducida en la espira pequeña en comparación
con el sentido de d⃗ℓ que se muestra en la figura cuando la espira grande se encuentra a la
izquierda y a la derecha de la espira pequeña. Calcular la corriente inducida en la espira
pequeña cuando las dos espiras están en el mismo plano y cuando t Ñ `8.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 26
Ley de Faraday-Lenz

#### Problema 1
⃗ “
La espira rectangular de la figura se encuentra sumergida en un campo magnético uniforme B
B x̂. Si la espira gira con velocidad angular ω utilizando el eje z como eje de rotación, y asumiendo
que en t = 0 la espira se encuentra en el plano y-z, determine la fuerza electromotriz inducida y la
corriente inducida en la espira.

#### Solución
Lo primero que debemos definir es nuestro vector normal, lo haremos en la dirección ´ϕ̂, recordando la definición de ϕ̂ (¡Del curso de dinámica!) obtenemos que,
n̂ = -psin θ x̂ ` cos θ ŷq
Podemos calcular el flujo de forma muy directa utilizando la definición,

---

### Página 2

ĳ
⃗ ¨B
⃗ = B
⃗ ¨S
⃗ = pB
⃗ ¨ n̂qS = BS sin ϕ = Bab sin ϕ
dS

Φ“
S

Para utilizar correctamente la la ley de Faraday, queremos dejar esta expresión en función del
tiempo de manera explícita, para utilizamos ω,
dϕ
“ ω Ñ ϕptq = ωt ` C
dt
Si la espira parte en el plano YZ como dice el enunciado, se tiene que cumplir que ϕp0q = π{2,
esto solo se logra si,
ϕptq = ωt `

π

Entonces nuestro flujo en función del tiempo queda así:
´
π¯
Φ = Bab sin ωt `
Para obtener la f.e.m. inducida utilizamos la ley de Faraday como,
´
d
π¯
dΦ
“ - Bab sin ωt `
ε = ´
dt
dt
Por tanto, la f.e.m inducida luce de la siguiente forma,
´
π¯
ε = -Babω cos ωt `
Solo falta conocer la corriente que circula por la espira, pero ya conocemos la resistencia y la f.e.m
(Voltaje), entonces la corriente que circula por la espira es,
I“

´
|ε|
Babω
π¯
“
cos ωt `
R
R

#### Problema 2
Una espira rectangular de dimensiones l y w se mueve con velocidad constante ⃗v alejándose de
un alambre recto infinitamente largo que lleva corriente I en el mismo plano de la espira. Sea la
resistencia total de la espira R. ¿Cuál es la corriente en la espira en el instante en que el lado más
cercano está a una distancia r del alambre?

---

### Página 3

Ahora imagine que la espira rectangular permanece estática con las medidas que aparecen en la
imagen, pero la corriente pasa a ser variable como I(t) = a ` bt. Calcule nuevamente la f.e.m
inducida y la dirección de la corriente.

#### Solución
Para ambas partes del ejercicio, el flujo magnético tendrá la misma expresión; el desarrollo cambiará recién cuando apliquemos la ley de Faraday, por lo que este primer cálculo sirve para ambas
partes.
Como el campo magnético entra en la hoja para nuestro caso, tomaremos que el vector normal
⃗ = -S k̂. Calculamos el flujo,
también lo hace, de tal forma que Φ > 0, es decir, S
ĳ
Φ“
S

⃗ ¨ dS
⃗ “ µ0 Il
B
2π

ż r`w
r

dr
µ0 Il ´
w¯
“
ln 1 `
r
2π
r

Ahora para sacar la corriente inducida debemos usar ley de Faraday,
ε = ´

dΦ
dt

Pero acá ya es distinto para cada uno de los dos casos, vamos por partes.
Para el PRIMER CASO, lo que se mueve es la espira, es decir, lo único que depende de t es r,
todo el resto se mantiene constante en el tiempo,
µ0 Il d ´
w ¯ µ0 Il
w
dr
ln 1 `
“
ε = ´
2π dt
r
2π rpw ` rq dt

---

### Página 4

Y como bien podemos inferir del enunciado, dr{dt corresponde nada más que a la velocidad con
la que va subiendo la espira, entonces la f.e.m inducida es,
ε“

w
µo Il
v
2π rpr ` wq

Y por tanto la corriente inducida,
I“

|ε|
µo Il
w
v
“
R
2π rpr ` wq R

Para determinar el sentido de la corriente basta con ver que pasa con el flujo que pasa por la espira a
medida que pasa el tiempo. ¿Disminuye o aumenta? En este caso disminuye, pensemos que el flujo
depende del área de la espira (Que no cambia) y el campo magnético que la atreviesa (Que disminuye a medida que se aleja del cable) entonces si a medida que pasa el tiempo el flujo magnético
disminuye, la corriente inducida tiene que ser tal que vaya aumentandolo, esto ocurre si la corriente
inducida genera un campo magnético que apunte en la misma dirección del que ya tenemos, es
decir, en sentido horario.
Para la SEGUNDA PARTE lo único que cambia es I en el tiempo, entonces,
ε = ´

µ0 l ´
w¯ d
ln 1 `
I
2π
r dt

Y como podemos notar de la ecuación de la corriente que se nos entrega, I(t) = a ` bt Ñ dI{dt = 
b, entonces nuestra f.e.m inducida es,
ε = ´

w¯
µ0 lb ´
ln 1 `
2π
r

Y la corriente,
I“

w¯
|ε|
µ0 lb ´
“´
ln 1 `
R
2πR
r

Para determinar el sentido de la corriente hacemos el mismo análisis anterior respecto al flujo ¿Aumenta o disminuye? El área de nuestra espira sigue sin cambiar, pero nuestro campo magnético
se va haciendo cada vez más intenso, entonces en este caso el flujo aumenta en el tiempo, caso
contrario a los de antes.
Para que se cumpla la ley de Lenz, la corriente tiene que ser tal que se oponga a este aumento de
flujo, generando un campo que apunte en sentido contrario al campo, es decir, saliendo de la hoja.
Esto se logra si la corriente va en sentido anti-horario.

---

### Página 5

#### Problema 3
Una espira circular de radio pequeño r está fija en el espacio. Una gran espira de radio R está
situada en un plano paralelo a la primera, es coaxial con ella y se le acerca con una velocidad constante ⃗v = vẑ. Las dos espiras son conductores óhmicos. Por la espira grande circula una corriente
constante I como se muestra en la figura, y en el instante t = 0 la distancia entre las dos espiras es z.

a) Calcular cómo cambia con el tiempo el flujo del campo magnético generado por la espira
grande a través de la espira pequeña. Se asume que r ! R de manera que el campo magnético
en el interior de la espira pequeña se puede considerar uniforme e igual a su valor a lo largo
del eje.
b) Calcular la f.e.m. inducida en la espira pequeña en un instante t cualquiera.
c) Argumentar en qué dirección fluye la corriente inducida en la espira pequeña en comparación
con el sentido de d⃗ℓ que se muestra en la figura cuando la espira grande se encuentra a la
izquierda y a la derecha de la espira pequeña. Calcular la corriente inducida en la espira
pequeña cuando las dos espiras están en el mismo plano y cuando t Ñ `8.

#### Solución
El cálculo del campo magnético generado por un anillo ya lo conocemos bastante bien, está dado
por,
⃗ 0, dq “
Bp0,

µ0 IR2
ẑ
2pR2 ` d2 q3{2

cuando calculemos la fem inducida necesitaremos derivar respecto al tiempo ¿Qué dependerá del
tiempo en el flujo? la distancia, porque como vemos esta se va acercando como d(t) = z - vt.
Procedemos a calcular el flujo como ya sabemos hacerlo,
ż
ΦB “

d⃗s ¨ B(0, 0, dptq) = 
S

µ0 IR2
πr2
2rR2 ` pz ´ vtq2 s3{2

---

### Página 6

Con esto ya podemos determinar la fem inducida utilizando la ley de Faraday,
E = ´

3µ0 IR2 vpz ´ vtq
dΦB
“´
πr2
dt
2rR2 ` pz ´ vtq2 s5{2

Ahora para la corriente inducida, cuando la grande se está acercando, el flujo magnético va aumentando, ya que el campo magnético se va haciendo más fuerte a medida que la distancia se acorta,
por lo que necesitamos un campo magnético inducido que se oponga a ese aumento de flujo, por lo
que la corriente inducida va en sentido contrario al d⃗l definido en la imagen.
Para el caso donde pasa de largo, la espira grande se va alejando y, por tanto, el flujo disminuye.
Siguiendo la misma lógica del análisis para el caso donde se acerca, la corriente va en el mismo
sentido del d⃗l definido en la imagen.
Cuando las dos espiras están en el mismo plano no habrá corriente inducida, el tiempo que ocurre
es en t = z{v, si reemplazamos esto en nuestra expresión para E obtendremos que la fem inducida
es 0.
Para el caso t Ñ 8 la fem igual será 0, al calcular el límite en la expresión para E obtendremos
dicho valor. Además, también es lo que se espera intuitivamente ya que a distancias muy grandes,
la espira chica sentirá un campo magnético cada vez más cercano a 0.
