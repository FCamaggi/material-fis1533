---
title: "Resumen Electricidad y Magnetismo"
source_enunciado: "Electro/material-apoyo/ayudantias-jorge-matamala/Enunciados/Resumen_Electricidad_y_Magnetismo.pdf"
source_solucion: "N/A"
extraction_mode: "pdftotext_cleaned"
---

# Resumen Electricidad y Magnetismo

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Instituto de Física
Electricidad y Magnetismo FIS1533-5
Benjamin Wassermann.

Resumen
Electricidad y Magnetismo

Ley de Coulomb:
Existe una fuerza, parecida a la gravedad, que se produce entre dos partículas con carga. La ley de
Coulomb nos dice que la fuerza que ejerce una partícula con carga q1 (en posición r1 ) sobre otra
con carga q2 (en r2 ) es:
F=

q1 q2 r 2 − r 1
.
4πε0 |r2 − r1 |3

Notamos que la fuerza es proporcional al producto de las cargas. Si hay dos cargas de igual signo,
se repelen, mientras que si tienen signo opuesto, se atraen. Además, es inversamente proporcional
al cuadrado de la distancia entre las cargas.
Normalmente en vez de preocuparnos por esta fuerza, nos abstraemos un poco y pensamos en el
concepto de Campo Eléctrico

Campo Eléctrico:
El campo eléctrico E en un punto r, producido por una carga puntual q que se encuentra en
un punto r ′ es:

E(r) =

q
r − r′
.
4πε0 |r − r ′ |3

Luego, si E1 es el campo producido por q1 , entonces la fuerza que ejerce q1 sobre q2 es F12 = q2 ·E1 (r2 )

Superposición:
El principio de superposición dice que si tenemos una carga que produce un campo E1 , y otra
que produce un campo E2 , el campo eléctrico total será E1 + E2. Con este principio podemos calcular el campo que producen muchas cargas puntuales como:

E(r) =

1 X r − r′
q
.
4πε0 q |r − r ′ |3

---

### Página 2

Trabajo y Energía:
Para mover una carga q debemos contrarestar la fuerza que existe sobre ella, luego el trabajo
necesario para mover la carga es:
Z
F · dr

Wa→b = −
c

Usando el teorema trabajo energía W = ∆U podemos definir energía almacenada por una configuración de cargas como:
U=

X
i<j

qi qj
4πε0 |ri − rj |

1. La energía almacenda por una configuración de cargas es equivalente al trabajo que cuesta
armar dicha configuración.
2. El principio de superposición aplica para todos los conceptos anteriromente mencionados.
3. ”Donde menos de donde”
Distribución de Cargas:
En la realidad, lo más común es encontrar cuerpos mucho más grandes que el tamaño del electrón,
cargados electricamente. Mejor conocidos como distribuciones continuas de carga.
Luego definimos el concepto de densidad de carga para 3 casos posibles:
1. Lineal:

∆q
∆l→ 0 ∆l

λ = lím
2. Superficial:

∆q
∆S→ 0 ∆S

σ = lím
3. Volumétrica:

∆q
∆V → 0 ∆V

ρ = lím

Aplicando el principio de superposición pero en medios continuos, obtenemos una expresión para el
campo eléctrico:
E(r) =
4πε0

Z
dq

r − r′
|r − r ′ |3

Donde dq depende del tipo de distribución. Para distribuciones lineales dq = λdl para superficies
dq = σdS y para volúmenes dq = ρdV .

---

### Página 3

Ley de Gauss:
La forma integral nos dice que para una carga puntual q ubicada en un punto fijo del espacio
y una superficie S que la encierra. El flujo del campo eléctrico que atraviesa S viene dado por:
I

⃗ · ds = q
E
ε0
S

Por otro lado la forma diferencial nos dice que la divergencia del campo en un punto (es decir,
cuanto = se separa” el campo en un punto) es proporcional a la densidad de carga en ese punto:
∇·E=

ρ
ε0

1. La Ley de Gauss siempre es verdad, pero no siempre es útil, pues necesitamos simetría.
2. La clave es que haya mucha simetría, pues en estos casos podemos tener un campo elétrico
constante sobre la superficie, y así sacarlo de la integral. De otra forma, no podríamos calcular
la integral.
3. El campo eléctrico no es necesariamente continuo. Las discontinuidades del campo son provocadas generalmente por cargas puntuales o superficies cargadas
4. Existen 3 tipos de simetrías: plana, cilíndrica y esférica.
Potencial Eléctrico:
El campo eléctrico producido por una carga Q a una distancia r viene dado por:
⃗ =
E

1 Q
r̂
4πε0 r2

Ahora, usando la identidad vectorial:
r̂
= −∇
r
r
Podemos escribir:
⃗ = −∇ϕ
E
Donde ϕ es un campo escalar que llamaremos ”Potencial Electrostático”
Para satisfacer la condición de arriba lo habitual es usar un punto de referencia r0 , donde el potencial
lo definimos como cero, de modo que:
Z r
ϕ(r) = −

E · dl
r0

---

### Página 4

Usualmente r0 = ∞.
Entonces el potencial producido por una carga Q en R, tomando el infinito como punto de referencia
es:
ϕ(r) =

Q
4πε0 |r − R|

⃗ debemos ejercer una fuerza que
Por otra parte, si tenemos una carga q sometida a un campo E
contrarreste la acción del campo sobre ella. Luego el trabajo necesario es:
Z
Wa→b = −

F · dr
c

⃗ = −q∇ϕ, reemplazando:
Pero F⃗ = q E

Z
∇ϕ · dr = q[ϕ(b) − ϕ(a)]

Wa→b = q
c

⃗ es conservativo.
Lo que nos recuerda que E
Por lo tanto:
W = q · ∆ϕ
1. ϕ es un escalar.
2. El potencial cumple con el principio de superposición.
3. Podemos interpretar el potencial como el trabajo por unidad de carga.
Conductores:
En un conductor, la última capa de elecrones, puede desplazarse libremente en presencia de un
campo eléctrico. Sin embargo, los electrones no pueden salir.
Si acercamos una carga Q a un conductor los electrones de este se reacomodan llegando a una
posición de equilibrio despues de un tiempo llamado ”tiempo de relajación”.Transcurrido ese tiempo
el campo eléctrico en el interior del conductor es cero. Pues si no lo fuera los electrones libres seguirían
moviéndose.
Sin embargo es en la superficie donde el campo no necesariamente es nulo. Por lo que aparece una
densidad de carga superficial σ.

---

### Página 5

Para calcular el campo en la superficie usamos la ley de Gauss de forma local tomando un cilindro
recto de área δa y altura h
Y obtenemos que el campo en la superficie de un conductor es:
⃗ = σ n̂
E
ε0

Resumiendo, algunas propiedades importantes de los conductores son:
⃗ int = 0
- E
⃗ no tiene componente tangencial.
- E
⃗ es siempre normal a la superficie.
- E
- En el borde existe una densidad de carga σ
⃗ = σ n̂
- E
ε0
- ϕ es constante dentro del conductor, pues no hay campo.
Capacitores:
Un capacitor es un dispositivo el cual tiene la capacidad de almacenar carga. Puede estar compuesto por uno o dos conductores de forma arbitraria.

Luego si sometemos un capacitor a una diferencia de potencial tenemos que nuestras principales
ecuaciones son:
Q = CV
Donde Q es la carga almacenada, V el voltaje y C la capacitancia del capacitor en Farads [F].

Y la energía almacenada es:
U = CV 2
Por otro lado podemos realizar conexiones entre capacitores. Donde la capacitancia se comporta de
manera inversa a la resistencia.

---

### Página 6

Por lo tanto si tenemos capacitores en paralelo:
Ceq = C1 + C2
Para una conexión en serie:
=
+
Ceq
C1 C2
Por último, para capacitores de 2 cuerpos es importante conocer ciertos valores de capacitancia:
- C Placas paralelas: C = ε0 Ad
- C Cilíndrico: C = 4πε
ln b
a

- C Esférico: C = ( 4πε
− 1b )
a

⃗ int = 0
1. En un conductor E
2. Existe una fuerza entere conductores que viene dada por F⃗ = −∇U
3. La capacitancia depende exclusivamente de la geometría.
4. Efecto punta: Menor radio de curvatura, mayor campo Eléctrico.
Dieléctrico:
En un material aislante las cargas se encuentran ”ligadas”, es decir no pueden moverse libremente.
Por lo tanto al aplicar un campo eléctrico externo, los átomos del material se polarizan.De esta
forma el material se convierte en una distribución de dipolos. Esta redistribución produce un nuevo
campo eléctrico propio del material.
Para facilitarnos las cosas definimos un vector de polarización P⃗ como el momento dipolar eléctrico
⃗
por unidad de volumen en un material. También definimos nuestro vector de desplazamiento D
como:
⃗ = ε0 E
⃗ + P⃗
D
Tenemos densidades de carga inducidas en el dieléctrico debido al campo eléctrico externo que
produce un reordenamiento de las moléculas. Donde la densidad de carga superficial de polarización
es:
σp = P⃗ · n̂
Y la densidad de polarización volumétrica es:
ρp = −∇ · P⃗

---

### Página 7

Por otro lado tenemos que el vector de polarización es proporcional al campo externo aplicado:
⃗
P⃗ = ε0 χE
Donde ε0 es la permitividad del vacío y χ es la susceptibilidad eléctrica. La cual nos indica que tan
susceptible es el material a polarizarse.
(
ρl , Las cargas libres, que están a nuestra disposición
En general tenemos 2 tipos de cargas :
ρp , Cargas de polarización al interior del material
Escribiendo la Ley de Gauss en forma diferencial:
⃗ = ρ
∇·E
ε0
Hay que recordar que en este caso ρ considera todas las cargas. Sean libres o de polarizaión.
Luego:
ρ = ρl + ρp
Reemplazando en la ecuación tenemos:
⃗ = ρl + ρp
ε0 E
Donde ρp = −∇ · P⃗ , entonces:
⃗ = ρl − ∇ · P⃗
ε0 E
Reordenando y agrupando obtenemos:
⃗ + P⃗ ) = ρl
∇ · (ε0 E
⃗ = ρl
∇·D
Por lo tanto:
I

⃗ · ds = Ql
D

s

Por último, algunas relaciones útiles son:
εr =

ε
= (1 + χ) ≥ 1
ε0

⃗ = εo (1 + χ)E
⃗ = εo εr E
⃗ = εE
⃗
D

---

### Página 8

Corriente Eléctrica:

Se entiende corriente eléctrica como el flujo de cargas en un determinado tiempo. Es decir:
I=

dq
dt

Ahora si nos concentramos en una sección transversal S, podemos definir la densidad de corriente
J⃗ como la carga que pasa por esa sección en un determinado tiempo:
I
I=

J⃗ · ds

s

De manera alternativa:
J⃗ = N q⃗v
Donde N es número de portadores por unidad de volumen, q es la carga y v la velocidad que llevan.
Tenemos nuestra ecuación de continuidad:
∂ρ
+ ∇J⃗ = 0
∂t
Por último la ley de Ohm en forma local sería:
⃗
J⃗ = g E
Donde g es la conductividad eléctrica, que corresponde al inverso de la resistividad.
⃗ tanto cargas libres como de polarización son ”fuentes”
1. Para el cálculo de E
⃗ sólo actuan como fuentes las cargas libres.
2. Para el cálculo de D
3. εr suele llamarse constante dieléctrica que también se conoce como κ
4. Si ponemos un dieléctrico dentro de un capacitor su capacitancia aumenta: C ′ = C · εr
Ley de Ohm:
Se entiende corriente eléctrica como el flujo de cargas en un determinado tiempo. Es decir:
I=

dq
dt

Definimos la ley de Ohm en forma local como:
⃗
J⃗ = g E

---

### Página 9

En forma global, la Ley de Ohm relaciona la diferencia de potencial V entre dos puntos en un
circuito, con la corriente I que fluye entre los puntos:
V = IR
Donde R es la constante de proporcionalidad entre voltaje y corriente. Conocida como resistencia,
donde:
R=

ρl
A

Con l el largo, A la sección transversal y ρ resistividad. Que corresponde al inverso de la conductividad g.
Por último las perdidas de potencia en forma de calor que provocan las resistencias pueden ser
calculadas como:

P = V I = RI 2 =

V2
R

Resistencias:
Existen principalmente 2 tipos de arreglos de resistencias.
i) Serie:
Si tenemos n resistencias en serie podemos condensarlas en una sola resistencia equivalente Req
donde
Req = R1 + R2 + ... + Rn
ii) Paralelo
Lo mismo ocurre para el arreglo en paralelo, donde:
=
+
+ ... +
Req
R1 R2
Rn
Por otro lado resulta muy util definir el operador paralelo como:
R1 //R2 =

R1 R2
R1 + R2

---

### Página 10

Leyes de Kirchhoff :
i) Ley de nodos: La suma de todas las corrientes que entran a un nodo debe ser igual a la suma de las corrientes que salen del mismo.
X

Iin =

X

Iout

ii) Ley de mallas: La suma de todos los voltajes correspondientes a cada uno de los elementos que
forman un circuito o una parte de él es nula cuando se recorre un camino cerrado (malla).
n
X

Vi = 0

i=1

1. Para resistencias en serie tenemos que la corriente es constante
2. Para resistencias en paralelo tenemos que el voltaje es constante
3. El voltaje puede ser interpretado como trabajo por unidad de carga [ CJ ]
4. Un nodo es una zona del circuito que tiene igual voltaje en todos sus puntos.
5. Una malla es un camino cerrado dentro del circuito.
Ley de Biot-Savart:
El campo magnético que genera una corriente I en un circuito puede ser determinado como:

Z

⃗ r ) = µ0
B(⃗
4π

⃗ × (⃗r − R)
⃗
I dl
⃗ 3
|⃗r − R|

⃗ es
⃗ es el lugar donde se encuentra la corriente, dl
Con ⃗r el lugar donde se desea conocer el campo, R
el elemento vectorial que parametriza la dirección de la corriente y µ0 la permeabilidad magnética
del vacío.
Por otro lado, la fuerza magnética que ejerce el circuito a sobre el circuito b es:
F⃗ =

Z

⃗ b × B⃗a
Ib dl

b

⃗ a viene dado por la
Notar que si la corriente es constante puede salir de la integral. Por otra parte B
expresión para el campo magnético, nuestra primera ecuación. Luego resulta evidente que conviene
calcular primero el campo magnético y luego la fuerza.
1. El campo magnético cumple con el principio de superposición.

---

### Página 11

2. ”Donde quiero medir, menos de donde proviene”
3. Los campos magnéticos siempre rotan en torno a la corriente según la regla de la mano derecha.
⃗ se mide en tesla, donde 1T = 1N/(A · m)
4. B
Fuerza de Lorentz:
La fuerza de Lorentz indica que una carga q con una velocidad ⃗v bajo la influencia de un cam⃗ siente una fuerza dada por:
po magnético B
⃗
F⃗ = q⃗v × B
⃗ la fuerza cambia a:
Adicionalmente, en presencia de un campo eléctrico E
⃗ + ⃗v × B)
⃗
F⃗ = q (E
⃗ son dos vectores que forman un plano. Perpendicular a éste, aparece la fuerza
1. Nótese que ⃗v y B
de Lorentz.
2. Debido a la naturaleza de la fuerza de Lorentz, la energía cinética de la carga es siempre
constante, pues la fuerza de Lorentz no realiza trabajo sobre la carga. Debido a lo anterior, el
módulo de la velocidad es siempre constante.
3. En problemas de cargas puntales en zonas de campo magnético constante, siempre tenga en
cuenta que esta se moverá en una circunferencia o en una espiral.
4. Carga positiva → Mano Izquierda, Carga negativa → Mano Derecha.
Ley de Ampere:

La ley de Ampere en su forma diferencial plantea que:
⃗ ×B
⃗ = µ0 J⃗
∇
Para todo campo magnético se cunple que:
⃗ =0
∇·B
En otras palabras, no existen monopolos magnéticos.
Usando el teorema de Stokes, la ley de Ampere en su forma integral propone que para cualquier
camino cerrado Γ se cumple que:
I

⃗ = µ0 I
⃗ · dl
B

Γ

---

### Página 12

Donde I es la corriente encerrada que atraviesa la superficie definida por Γ.
⃗ son dos vectores que forman un plano. Perpendicular a éste, aparece la fuerza
1. Nótese que ⃗v y B
de Lorentz.
2. Debido a la naturaleza de la fuerza de Lorentz, la energía cinética de la carga es siempre
constante, pues la fuerza de Lorentz no realiza trabajo sobre la carga. Debido a lo anterior, el
módulo de la velocidad es siempre constante.
3. Carga positiva → Mano Izquierda, Carga negativa → Mano Derecha.
4. Algunos casos para las cuales es util la ley de Ampere son: cilíndros, planos, bobinas y toroides.
5. Recordar que la corriente es la integral de J⃗ en dS
Magnetización:
⃗ como la densidad de momento magnético por unidad
Definimos el vector de magnetización M
de volumen dentro de un medio material.
Para incluir el efecto del campo magnético que generan las corrientes de magnetización definimos
⃗ como:
el vector intensidad de campo magnético H
⃗ = 1B
⃗ −M
⃗
H
µ0
Luego, podemos escribir la ley de Ampere en forma generalizada:
I

⃗ · dl = Il
H

Donde Il son las corrientes libres que circulan por el material.
⃗ y H:
⃗
Para gran cantidad de materiales se cumple una relación lineal entre M
⃗ = χm · H
⃗
M
Donde χm es la susceptibilidad magnética del material. Conocido el valor de este parámetro podemos clasificar a los materiales:
- Paramagnético χm > 0 ; Crean un campo magnético que se alinea con el externo
- Diamagnético χm < 0 ; Crean un campo magnético que se opone al externo
- Ferromagnético χm ≫ 1 ; Curva de Histéresis
Por último definimos la permeabilidad magnética relativa como:
µ r = 1 + χm

---

### Página 13

Por lo tanto es util tener presente todas las siguientes relaciones:
⃗ = µ0 ( H
⃗ +M
⃗ ) = µ0 (1 + χm )H
⃗ = µH
⃗
B
1. Recordar que la corriente es la integral de J⃗ en dS.
2. Algunos casos para las cuales es util la ley de Ampere son: cilíndros, planos, bobinas y toroides.
Ya sea para el vacío o medios magnéticos.
3. En histéresis tenemos distinto camino de ida y vuelta, quedamos con un remanente.
Flujo:
Definiremos ϕ como el flujo de campo magnético que atraviesa una superficie, es decir:
Z
ϕ=

⃗
⃗ · dS
B

s

Inducción:
La ley de Faraday indica que la fem inducida en un circuito cerrado está dado por:

ε=−

∂ϕ
∂t

Por lo tanto en presencia de campo magnéticos que dependen del tiempo se cumple que:
⃗
⃗ = − ∂B
∇×E
∂t
Lo que vendría a ser la Ley de Faraday en su forma diferencial.
Ley de Lenz:
La corriente inducida en un circuito debido a la variación temporal del flujo del campo magnético
siempre es opuesta al crecimiento o decrecimiento del mismo.
1. No habrá una fem inducida si no hay un cambio del flujo en el tiempo.
2. Existen 3 formas de variar el flujo: Variar el campo magnético, la sección o la orientación.
3. El sentido de la corriente queda definido por la Ley de Lenz.
4. Recordemos que la fem es el agente responsable de empujar la corriente a través del circuito.

---

### Página 14

Onda Sinusoidal:
g(t) = A · cos(ωt + ϕ)
i) A es la amplitud
ii) √A2 es el valor RMS
iii) ω = 2πf

Régimen permanente:
En la repuesta de un circuito de orden mayor a cero se distinguen dos regímenes: el transitorio
y el permanente.
El régimen transitorio se asocia a la superposición de la respuesta homogénea y la respuesta forzada
del sistema.
El régimen permanente se asocia a lo que queda una vez que la respuesta homogénea ha desaparecido,
es decir, sólo la respuesta forzada
Cuando la función g(t) que exita el circuito es una sinusoide, la respuesta forzada corresponde a
una sinusoide de la misma frecuencia con cierta amplitud y desfase.
Fasores:
Dado que tenemos 2 grados de libertad, amplitud y fase, una forma muy conveniente de representar las señales es por medio de un fasor.
a + jb =

p
b
a2 + b2 < tan−1 ( )
a

Impedancia:
La impedancia Z es un concepto equivalente al de resistencia. Indica cuánto se opone al flujo de
corriente un componente o circuito en régimen sinusoidal permanente.
Z=

V
I

En particular:
Elemento

Z

ϕ

ω→
− ∞

ω→
− 0

R
C
L

R

-90

CC
CA

CA
CC

jωc

jωL

1. En un circuito en régimen sinusoidal permanente sólo nos interesa la amplitud y el desfase de
cada señal, dado que la frecuencia es igual para todas.
2. El desfase por convención indica como está el voltaje respecto de la corriente.

---

### Página 15

3. La magnitud de un fasor representa la amplitud de la sinusoide, mientras que la fase representa
el desfase que tiene la señal con respecto a una señal de referencia.
4. Resulta muy conveniente analizar circuitos en régimen permanente en el dominio de la frecuencia, usando la transformada Fourier o Laplace.
5. Operamos con las impedancias de igual manera que con las resistencias.
6. La frecuencia de resonancia ω0 de un circuito eléctrico es aquella frecuencia la cual anula la
parte imaginaria de la impendancia equivalente. Para esta frecuencia tenemos máxima corriente
y potencia promedio.

---

## Solución

> *(Solución oficial no disponible en el repositorio)*
