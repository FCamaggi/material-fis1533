---
title: "Ayudantia 16"
source_enunciado: "Electro/material-apoyo/ayudantias-jorge-matamala/Enunciados/Ayudantia 16.pdf"
source_solucion: "Electro/material-apoyo/ayudantias-jorge-matamala/Soluciones/solucion_ayudantia_16.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 16

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
Electricidad y magnetismo - FIS1533
Profesor: Marcelo Calderon
Ayudante: Jorge Matamala (jnmatamala@uc.cl)

Ayudantía 16
Circuito RC

1.

Resumen

El capacitor representa el fenómeno de almacenamiento de energía en forma de campo eléctrico, producto
de la acumulación de cargas de diferente signo entre las placas.
Como elemento circuital, posee la siguiente ecuación característica
i(t) = C

dv(t)
dt

que es obtenida derivando la ecuación que relaciona carga y capacitancia
Q(t) = Cv(t)
Considerando el siguiente circuito

Supongamos que el capacitor está descargado inicialmente, esto es
Q(0− ) = 0
La implicancia directa de esta condición es
vc (0− ) = 0
Es decir, antes de cerrar el interruptor el capacitor no es más que un cortocircuito.
Ahora, el interruptor se cierra en t = 0, obteniendo el siguiente circuito

Lo primero que se observa es que el nodo superior está directamente conectado a la fuente de voltaje, forzando
que
vc (0+ ) = V

—

1 de 3

—

---

### Página 2

Sin embargo, este cambio del voltaje en el capacitor ocurre muy abruptamente... casi de un instante a
otro. Se pasa de un voltaje cero a un voltaje V entre un tiempo t = 0− y t = 0+ , así que la ecuación de
corriente queda algo así
V −0
→∞
i(0+ ) = C +
0 −0
El denominador es extremadamente pequeño, ¡se tendrá una corriente gigantesca! Esto puede traer bastantes
problemas, así que para evitarlo siempre se agrega una resistencia entre la fuente y el capacitor. El objetivo
de esto es lograr limitar este peak de corriente y así evitar el salto de voltaje y posibles daños.
Agregando una resistencia, el circuito queda de la siguiente forma

Bajo la misma lógica de antes, justo después de cerrar el circuito, la corriente en la resistencia sigue la ley
de Ohm
V
i(0+ ) =
R
donde se ve que la resistencia pudo limitar la corriente peak y evitar que tomara un valor gigantesco.
A medida que pasa el tiempo, la corriente comienza a disminuir por el hecho de que el capacitor se carga. En
ese estado final, el capacitor se ve como un circuito abierto y su voltaje es igual al entregado por la fuente.
Si hacemos KVL podremos encontrar una expresión para el voltaje/corriente a medida que pasa el tiempo,
así
V − ic (t)R − vc (t) = 0
donde si reemplazamos la expresión de la corriente del capacitor se llega a
V = RC

dvc (t)
+ vc (t)

Lo anterior es una EDO de primer orden, donde su solución -¡demuéstrelo!- está dada por
t

vc (t) = (vc (0) − V )e− RC + V
ic (t) = (

V − vc (0) − t
)e RC
R

Para la descarga del capacitor se considera el siguiente circuito

2 de 3

---

### Página 3

Si se hace KVL justo después de cerrar el interruptor,
vc (t) = ic (t)R
vc (t) = −RC

dvc (t)

¿Por qué aparece un signo menos?
Lo anterior es una EDO con solución

t

vc (t) = Ke− RC
ic (t) = −

K − t
e RC
R

donde K es una constante que depende de las condiciones iniciales.

3 de 3

---

### Página 4

2.

Problemas

#### Problema 1
Sea el circuito de la figura, donde el interruptor S1 ha estado cerrado por un periodo muy largo y en
t = 0 se abre. Determine

1. El voltaje en el capacitor para t < 0
2. La corriente en R2 para t > 0
Nota: El elemento que tiene una flecha es una fuente de corriente, indica que en esa rama siempre se tiene
una corriente I1

#### Problema 2
En el circuito de la figura el interruptor está cerrado y el capacitor se encuentra cargado completamente.
Determine la corriente en cada resistencia y la carga del condensador. Ahora, en t = 0 se abre el interruptor
S. Encuentre la corriente que pasa por la resistencia R2 como función del tiempo. ¿Cuánto tiempo debe
transcurrir para que la carga en C disminuya hasta 4/5 del valor inicial?

#### Problema 3
Considere el circuito de la figura. En el instante t < 0 los interruptores están abiertos y el condensador
se encuentra descargado. En el instante t = 0 se cierra S1 , quedando abierto S2 . Luego, en un instante t = t0
se cierra S2 , por lo que para un tiempo t > t0 ambos interruptores están cerrados.

1. Encuentre la corriente a través de la batería en un instante 0 < t < t0
2. Considerando que qt=t0 = q0 (antes de cerrar S2 ), determine la corriente a través de la batería en un
instante t = t0 (instantáneamente después de cerrar el interruptor S2 )

4 de 3

---

### Página 5

#### Problema 4
Dos capacitores de capacitancias C1 y C2 están conectados a dos resistencias iguales R. En t = 0 el capacitor
C1 tiene una carga Q0 mientras que el C2 está descargado. Determine
1. Las cargas de los capacitores en función del tiempo
2. La energía disipada por las resistencias
3. La energía disipada total hasta que se alcance el equilibrio. ¿De qué depende dicha cantidad? Explique
el por qué de ello.

5 de 3

---

## Solución

### Página 1

I
A) VOLTA

>e

Como

ee

el CAPACITOR

Ny

Completamente

Albano

esta

TL 0

Fuente

[ (E) + I

Retaaommos

Corrientes

D- Solo

Que

se

hey

Con

er

:

-

Vc "

V,

'

=

-

É R

-

=

,

Cdd÷R

el

es

Pero

la

a

Para

TLO

ad

hurry
V.

=

(Antes )

)=p¥gV

I

,

+

Ii R.HR

capacitor

es

r§→

É =C%

EDO Separable

.

recon oar

Circuito

Corriere

✗

e-

=

Ec

-

¥

+

✗

Nooo Azul

0hm

Oe

""

KVL

en

UH

%

=

KCL

Ayu

es

Traba >A

v.

◦

Circuito

.

usamos

,

El

-

Olueoanoo d

Alone ,

se

,

Corriere

Ézlo )

Ii

+

se

VOLTA > es

Y

¥1k
S

=

,

d

s

-

PAM-M-cenevioeu-e.lt

y

,

:*

v.

Hagen

Corriere

É??jÉ÷
R

b) T ≥o

Chula

✗
,

ctennbrmnia

Asi

90C

---

### Página 2

Alli a- noo

C. I

Uco )

✗

p,R¥ V1

t

I,

R HRZ

Asi ,

Mct)

Y Por

hey

0hm

( p¥g Vit

I,

) C-

R.HR

[

ftp.t?z-nVitIiR.HRz) C-

---

### Página 3

?⃝

?⃝

[

On

el CAPACITOR

Totalmncre

TLO

CANSAOO

Se

lo

Tiene

Sisu / ente

rmRi

it

{

} ¥

Piz

Malla

Izquierda

se Tiene

E- É(RtRz)=0

=¥n

'

23=0

y

ROSADA

PARA LA

Pero 25-0

Sz

E

my

E.

Asi ,

Con

f)
KVL con la wallet Que

thermos

Carya

2in

ABIERTO

IR -1K

Se

Pero

mismo

→

causa

Canosa

Vc

? →

antes

I > Rs =D

C. =

Abin S

K

vi.

Tiene

C

%

Reconoanoo

Se

Ahora

que

r{¥{r

≤

.se
thee to

E- ÉR

É Como hav Alarcon la

. .

Fritt
{
÷ }
i

Capacitor

9- (5) = ( ( E- 2,10)Ri)

{

Al

'

-1¥

T ≥o

Corriere

Des Carya

capacitor

vc=÷=i
Se

Tiene

Net, i. a) Ra

_

la

Signore

eoo

Ide> R}

=)

=D

dot

qn÷

E-

hot)

9- a)

PARA LA

CTC

USAMA

la

÷

¥ =◦

A

Ae¥ñ+ⁿ

'

Carya

Nidal

9- a)

( (e- i. a)

I. (Rata)

eu

-1=0

éÉ+nD

YA

Calcutta

>

~

9-co)=Ae°= CCE ER )

A-

CCE -2in )

---

### Página 4

p

AH

Corriere

solo

Derive

9- ( T)

2i =%I÷é¥

↳

PAM

evcontmn

Tiempo

hasta

Inna

Que el coaction

MADO

Igoe la causa

9- (F)

Desousa

ewacién

Simple

CCE-i.R.IE#--4-gC(E-ir

459cg

¥"

e-

Ura

Se

É =h(¥)

)

F- ( (Rstrzlrl :)

---

### Página 5

Haaenoo

KUK

la math

exterior

t.T-1
T?n-ti7-min
Asi

Kero

k

Para

d¥ (nÉ{

eeaatm

9-

DCUUAMD Para

Cee

ER

i. Rio

9- a) = Be

CE

0949400

9-(-1--0)=0

E

◦

g)

B

Maal

ÉB=o

quean

Conoiaén

E- ÉR , Vc

a÷ri

9- H=BtCE=o

→

B.

CE

ce

Ici )

Ict)

b) Al Cernan Sz

¥ É¥

cerate

OLTLT,

Asi

Ue

r÷mi¥
Ri

%=L.±ñ÷7_
Notte

Por to

Eso

que

mismo,

Obere

ÉtÉz

Neos /To

Asi

Saber

antenna

la

to

Todo

A

reduce

causa

Find

obtain

Antes

a)

Para

É Que

calculate

Cernan

De

la

Pasa Por

Bacteria

Justo

Coamo

Conectamos

Donde

Por

Amado

Casa ,

es

I. R

M

Dear

( F- To)

(7-92)

Malla

exterior

(K

od

)

capacitor

E

I.

Malla

Sin

Capacitor

E- ÉzRz ÉR> =o

et capacitor

ÉR =o
>

=)

'q( E- ¥ ins)

É=

In,(E- Irs)

E- ÉR

¥ ÉR

>

es

FK't)=o

---

### Página 6

Reemeazasoo
Deseesanoo

É=Éz+É

i=::÷¥÷

# E-iryi-h-ye.ir )
E-

---

### Página 7

?⃝

ED Positive
COMO

Haaenoo

en

Circuito

C

Total

Qo

9-

ACTVA

O

¥,=0

%

'

Parque CSTÉ
BATENIA

Tir Vu ÉR=o

my

¥ -2in

/A Carda

UNA

9- a

Oes Pesnnoo

Y

Reemphasis

lo

Anterior

Q◦¥ˢ -22in ¥=o

Ahora

Asi

dd9

YA

Que

la Casa

oismnuye

C,

Pero

h- CADA

Cz

ee

Aumeeta

É=d-9÷

que

zrd

;÷

¥ 0%9-2=0

_

dd¥ +29¥
sfcs)
Como 9-267=0

Y

APIICANOO

fess

9-do)

1-

FI

Tomasso

ZRCO

Q%

☆ É=É+ci

EDO

Fcs>

%,=¥÷!§

Fracciones Parades

(5--1)/5

◦

Lance Para

Resolver .lt

(I

e- %)

'

St

9- it)

/

9¥

Laplace
◦

£{dd¥ }
"'

SFCS)

Ato)

°

Liat

§

;

Fraccioncs Parades lmaooo oebsresiaos
