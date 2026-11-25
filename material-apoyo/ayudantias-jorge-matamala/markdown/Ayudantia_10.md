---
title: "Ayudantia 10"
source_enunciado: "Electro/material-apoyo/ayudantias-jorge-matamala/Enunciados/Ayudantia 10.pdf"
source_solucion: "Electro/material-apoyo/ayudantias-jorge-matamala/Soluciones/solucion_ayudantia_10.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 10

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Instituto de Física
Electricidad y Magnetismo FIS1533-1, 2022-2
Profesor: Marcelo Calderón (marcelo.calderon@uc.cl).
Ayudante: Benjamin Wassermann (bewassermann@uc.cl).

Ayudantía 10
Electrostática: Capacitores y Dieléctricos

Resumen
Capacitores:
Podemos realizar conexiones entre capacitores. Donde la capacitancia se comporta de manera
ı̈nversa.a la resistencia.
Por lo tanto si tenemos capacitores en paralelo:

Ceq = C1 + C2

Para una conexión en serie:

=
+
Ceq
C1 C2

---

### Página 2

Por último, para capacitores de 2 cuerpos es importante conocer ciertos valores de capacitancia:
- C Placas paralelas: C = ε0 Ad
- C Cilíndrico: C = 4πε
ln b
a

- C Esférico: C = ( 4πε
− 1b )
a

- Dieléctrico:
En un material aislante las cargas se encuentran ”ligadas”, es decir no pueden moverse libremente. Por lo tanto al aplicar un campo eléctrico externo, los átomos del material se polarizan.De
esta forma el material se convierte en una distribución de dipolos. Esta redistribución produce
un nuevo campo eléctrico propio del material.
Para facilitarnos las cosas definimos un vector de polarización P~ como el momento dipolar
eléctrico por unidad de volumen en un material. También definimos nuestro vector de despla~ como:
zamiento D
~ = ε0 E
~ + P~
D
Tenemos densidades de carga inducidas en el dieléctrico debido al campo eléctrico externo
que produce un reordenamiento de las moléculas. Donde la densidad de carga superficial de
polarización es:
σp = P~ · n̂
Y la densidad de polarización volumétrica es:
ρp = −∇ · P~
Por otro lado tenemos que el vector de polarización es proporcional al campo externo aplicado:
~
P~ = ε0 χE
Donde ε0 es la permitividad del vacío y χ es la susceptibilidad eléctrica. La cual nos indica que
tan susceptible es el material a polarizarse.
(
ρl , Las cargas libres, que están a nuestra disposición
En general tenemos 2 tipos de cargas :
ρp , Cargas de polarización al interior del material
Escribiendo la Ley de Gauss en forma diferencial:
~ =
∇·E

ρ
ε0

Hay que recordar que en este caso ρ considera todas las cargas. Sean libres o de polarizaión.

---

### Página 3

Luego:
ρ = ρl + ρp
Reemplazando en la ecuación tenemos:
~ = ρl + ρp
ε0 E
Donde ρp = −∇ · P~ , entonces:
~ = ρl − ∇ · P~
ε0 E
Reordenando y agrupando obtenemos:
~ + P~ ) = ρl
∇ · (ε0 E
~ = ρl
∇·D
Por lo tanto:
I

~ · ds = Ql
D

s

Por último, algunas relaciones útiles son:
εr =

ε
= (1 + χ) ≥ 1
ε0

~ = εo (1 + χ)E
~ = εo εr E
~ = εE
~
D
Cosas importantes:
~ tanto cargas libres como de polarización son ”fuentes”
1. Para el cálculo de E
~ sólo actuan como fuentes las cargas libres.
2. Para el cálculo de D
3. εr suele llamarse constante dieléctrica que también se conoce como κ
4. Si ponemos un dieléctrico dentro de un capacitor su capacitancia aumenta: C 0 = C · εr

---

### Página 4

Problemas
#### Problema 1
Considere dos cilindros conductores coaxiales. El interior de radio a y el exterior de radio c. El espacio
a < r < b con b < c se llena con un dieléctrico de constante κ. Encuentre la capacitancia del dispositivo
por unidad de largo

#### Problema 2
En un condensador de placas cuadradas de área A = (2a)2 se introducen dos dieléctricos que llenan el
interior del condensador como se muestra en la figura. Si ε1 > ε2 , ¿Cuál es la magnitud de la fuerza que
debe aplicarse para mantener esta configuración?

#### Problema 3
Dos condensadores descargados de capacitancia C1 y C2 se conectan en paralelo a una batería que ofrece
un potencial V0 . Luego se desconectan y sin perder su carga, se conectan en serie. Calcule la nueva carga
en cada placa de los capacitores.

---

### Página 5

Respuestas
2πε0
1. C
L = 1 ln( b )+ln( c )
κ
a
b

2. F~ = − 12 CQ2 2a(ε1d−ε2 ) x̂
eq

1 −C2 )V0
3. Q01 = C1 (C
C1 +C2

1 −C2 )V0
Q02 = C2 (C
C1 +C2

---

## Solución

> **[SOLUCIÓN MANUSCRITA / ESCANEADA]:** El archivo original (`Electro/material-apoyo/ayudantias-jorge-matamala/Soluciones/solucion_ayudantia_10.pdf`, 6 págs) no posee capa de texto extraíble. Para leer el desarrollo completo, inspeccionar visualmente el PDF.
