---
title: "unidad4"
source_pdf: "Electro/2026-1/Clases/unidad4.pdf"
pages: 53
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# unidad4

### Página 1

FIS1533 – Electricidad y Magnetismo
Prof. Rodrigo López
Unidad 4

---

### Página 2

Unidad 4

-

Inductancia

-

Circuitos LRC

-

Corriente alterna

---

### Página 3

Inductancia mutua
Una corriente que circula por la bobina 1 produce un campo magnético B y, por lo tanto, un flujo magnético
a través de la bobina 2. Si la corriente en la bobina 1 cambia, el flujo a través de la bobina 2 también
cambia; de acuerdo con la ley de Faraday, esto induce una fem en la bobina 2. De este modo, un cambio
en la corriente de un circuito puede inducir otra corriente en un segundo circuito.

El flujo dependerá de la corriente variable. Introducimos la constante M21, llamada
inductancia mutua de las los bobinas

Ddonde Φ es el flujo a través de una sola espira de la bobina 2.
Entonces

---

### Página 4

Inductancia mutua
Podríamos analizar el caso opuesto, en el que una corriente cambiante en la bobina 2 induce un flujo
cambiante en la bobina 1.
La constante M12 es siempre igual a M21 aún cuando las dos bobinas sean diferentes. A este valor común lo
llamamos simplemente inductancia mutua M

Donde usamos

La unidad de medida en el SI de la inductancia mutua es el henry (H)

---

### Página 5

Autoinductancia
Incluso si consideramos un solo circuito aislado, podremos observar este efecto. Cuando en el circuito está
presente una corriente, se establece un campo magnético que crea un flujo magnético a través del mismo
circuito; este flujo cambia cuando la corriente cambia. Así, cualquier circuito que conduzca una corriente
variable tiene una fem inducida en él por la variación en su propio campo magnético. Esa clase de
fem se denomina fem autoinducida.

Cuando no hay riesgo de confusión con la inductancia mutua, la autoinductancia se
llama simplemente inductancia.
La fem autoinducida es

---

### Página 6

Inductores en circuitos
Un elemento de circuito diseñado para tener una inductancia particular se llama inductor, o bobina de
autoinducción. El símbolo habitual para un inductor en un circuito es

Un inductor en un circuito de corriente directa ayuda a mantener una corriente estable a pesar de las
fluctuaciones en la fem aplicada; en un circuito de corriente alterna, un inductor tiende a suprimir las
variaciones de la corriente que ocurran más rápido de lo deseado.
Pa estudiar estos circuitos es necesario desarrollar un principio general análogo a la ley de Kirchhoff de las
mallas. Pero en este caso, el campo eléctrico inducido magnéticamente dentro de las
bobinas del inductor no es conservativo.
Supongamos que el inductor tiene una resistencia insignificante. Para mover a las
cargas dentro a través de él se requiere un campo eléctrico muy pequeño, casi
despreciable.
Youtube

---

### Página 7

Inductores en circuitos
De acuerdo a la ley de Faraday, tenemos

El campo En es diferente de cero sólo dentro del inductor, por lo tanto la integral anterior es equivalente a

Lo que se puede escribir como

---

### Página 8

Inductores en circuitos
La fem autoinducida no se opone a la corriente I en sí, sino a cualquier cambio (dI/dt) en la corriente. Así,
el comportamiento de un inductor en un circuito es muy diferente del de un resistor.

---

### Página 9

Energía del campo magnético
El establecimiento de una corriente en un inductor requiere un suministro de energía, y un inductor que
conduce corriente contiene energía almacenada.
Si una corriente creciente pasa por el inductor, la fuente debe estar agregando energía al inductor, y la
potencia instantánea P (la tasa de transferencia de energía al inductor) es P = Vabi.
Si inicialmente la corriente es igual a cero, la entrada total de energía U necesaria para establecer una
corriente final I, se puede calcular a partir de

La energía dU suministrada al inductor durante un intervalo de tiempo dt es dU=Pdt
La energía total suministrada

---

### Página 10

Energía del campo magnético
La energía en un inductor en realidad se almacena en el campo magnético dentro de la bobina, al igual que
la energía de un capacitor lo hace en el campo eléctrico entre sus placas.
Supongamos un solenoide toroidal

Luego, la energía almacenada cuando la corriente es I

El campo magnético y, por tanto, la energía magnética se localizan en el volumen
V=2πrA encerrado por el devanado. La energía por unidad de volumen o densidad
de energía magnética

---

### Página 11

Energía del campo magnético
Usando la expresión para la magnitud del campo dentro del solenoide

Obtenemos una expresión general para la densidad de energía magnética en el vacío

---

### Página 12

Circuito RL
Crecimiento de la corriente en un circuito RL
Un inductor en un circuito hace difícil que ocurran cambios rápidos en la corriente, en virtud de los efectos
de la fem autoinducida. Vimos que cuanto más grande es la tasa de cambio de la corriente, dI/dt, mayor es
la fem autoinducida y mayor la diferencia de potencial entre las terminales del inductor.

Aplicando Kirchhoff

luego

---

### Página 13

Circuito RL
Crecimiento de la corriente en un circuito RL
En el instante en que el interruptor S1 se cierra por primera vez, i=0 y la caída del potencial a través de R es
igual a cero. La tasa de cambio inicial de la corriente es

Como se esperaba, cuanto mayor es la inductancia L, con más lentitud
aumenta la corriente.

La corriente final I no depende de la inductancia L.

---

### Página 14

Circuito RL
Crecimiento de la corriente en un circuito RL
La corriente en función del tiempo viene dada por

Luego,

definimos,
Constante de tiempo para
un circuito RL

---

### Página 15

Circuito RL
Crecimiento de la corriente en un circuito RL
Las consideraciones acerca de la energía brindan una perspectiva adicional sobre el comportamiento de un
circuito RL.
En cierto instante de
tiempo:

Potencia suministrada por la
fuente
Potencia almacenada
en inductor

Potencia disipada en
resistor

---

### Página 16

Circuito RL
Decaimiento de la corriente en un circuito RL
Ahora supongamos que el interruptor S1 en el circuito ha permanecido cerrado por un tiempo y la corriente
ha alcanzado el valor I0. Se reinicia el cronómetro para redefinir el tiempo inicial, se cierra el interruptor S 2
en el momento t = 0, con la batería puesta en derivación. (Al mismo tiempo se debe abrir S 1 para que no se
arruine la batería.)

Con I0 la corriente inicial en t = 0.

---

### Página 17

Circuito RL
Decaimiento de la corriente en un circuito RL
La energía necesaria para mantener la corriente durante este decaimiento proviene de la energía
almacenada en el campo magnético del inductor.

---

### Página 18

Circuito LC
Un circuito que contiene un inductor y un capacitor muestra un modo completamente nuevo de
comportamiento, caracterizado por una corriente y una carga oscilantes.

Youtube

---

### Página 19

Circuito LC

---

### Página 20

Circuito LC
Aplicando las leyes de Kirchhoff al circuito LC, partiendo desde la esquina inferior derecha del circuito,

Lo que se puede escribir como

Luego,

---

### Página 21

Circuito LC

---

### Página 22

Circuito LRC
En nuestro análisis del circuito LC se supuso que no hay resistencia en el circuito. Desde luego, ésta es una
idealización; todo inductor real tiene resistencia en sus devanados, y también puede haber resistencia en
los alambres de conexión. En virtud de la resistencia, la energía electromagnética en el circuito se disipa y
se convierte en otras formas, como energía interna de los materiales del circuito. La resistencia en un
circuito eléctrico es análoga a la fricción en un sistema mecánico.

Si la resistencia R es relativamente pequeña, el circuito aún oscila, pero con un movimiento
armónico amortiguado, y se dice que el circuito está subamortiguado. Si R se incrementa, las
oscilaciones cesan con más rapidez. Cuando R alcanza cierto valor, el circuito deja de oscilar;
está críticamente amortiguado. Para valores aún mayores de R, el circuito está
sobreamortiguado, y la carga del capacitor se acerca a cero aún más lentamente.

---

### Página 23

Circuito LRC
Aplicamos las leyes de Kirchhoff para determinar como varían q e i con el tiempo.

Usando la definición de corriente

Podemos escribir la solución de la forma

---

### Página 24

Circuito LRC
Podemos diferenciar los siguientes casos
●

R2 < 4L/C tenemos el caso subamortiguado.

●

R2 = 4L/C tenemos el caso de amortihuamiento crítico.

●

R2 > 4L/C tenemos el caso sobreamortiguado.

---

### Página 25

Corriente alterna
Cuando el voltaje y la corriente varían de forma sinusoidal hablaremos de corriente alterna.
Para suministrar una corriente alterna a un circuito se requiere una fuente de fem o voltaje alternos. Un
ejemplo de esto es una bobina de alambre que gira con velocidad angular constante en un campo
magnético. Esto crea una fem alterna sinusoidal y es el prototipo del generador comercial de corriente
alterna o alternador.
Frecuencia angular

Diferencia de potencial
instantánea
Amplitud del voltaje

---

### Página 26

Corriente alterna
Para representar voltajes y corrientes que varían en forma sinusoidal usaremos diagramas de vectores
giratorios:
●

el valor instantáneo de una cantidad que varía sinusoidalmente con respecto
al tiempo se representa mediante la proyección sobre un eje horizontal de un
vector con longitud igual a la amplitud de la cantidad

●

El vector gira en el sentido antihorario con rapidez angular constante ω.

●

Estos vectores giratorios reciben el nombre de fasores, y los diagramas que
los contienen se llaman diagramas de fasores.

¿cuál fasor corresponde a a) una corriente positiva que se está haciendo más positiva; b) una
corriente positiva que disminuye hacia cero; c) una corriente negativa que se está haciendo
más negativa; d ) una corriente negativa cuya magnitud disminuye hacia cero?

---

### Página 27

Corriente alterna
Podemos calcular el voltaje (o corriente) promedio en un ciclo, pero esto resulta no ser muy útil. En su lugar
utilizaremos el valor eficaz o valor cuadrático medio (rms).

Vrms = 220 V
El voltaje instantáneo
entre las terminales
varía de -311 V a 311 V

---

### Página 28

Corriente alterna
Representaremos a estas cantidades sinusoidales como la parte real del número complejo

Recordemos que un número complejo se puede escribir en su representación polar, según

Con la fórmula de Moivre

---

### Página 29

Corriente alterna
En adelante, usaremos las cantidades definidas como variables complejas, de la forma

Donde Q, I, V son constantes complejas. Al final del cálculo, las cantidades físicas se determinan tomando
la parte real de las cantidades complejas.

---

### Página 30

Resistencia y reactancia
Resistor en un circuito de CA
Definimos el sentido positivo de la corriente como antihorario alrededor del circuito. El potencial instantáneo
del punto a con respecto al punto b, es decir, la diferencia de potencial entre los extremos del resistor es

El voltaje máximo o la amplitud del voltaje es

---

### Página 31

Resistencia y reactancia
Inductor en un circuito de CA
Sustituimos el resistor por un inductor de inductancia L y resistencia nula. Aunque no hay resistencia, sí hay
una diferencia de potencial entre los terminales del inductor, ya que la corriente varía con el tiempo.

Ángulo de fase

Para un resistor ϕ=0
Para un inductor ϕ=π/2

---

### Página 32

Resistencia y reactancia
Inductor en un circuito de CA
Notamos que la relación entre la corriente y el voltaje se puede escribir de la forma

Donde ZL se define como la impedancia del circuito. La parte imaginaria de la impedancia recibe el nombre
de reactancia, en este caso reactancia inductiva

El hecho de que la impedancia sea compleja significa que la corriente no está en fase con el voltaje
aplicado.

---

### Página 33

Resistencia y reactancia
Inductor en un circuito de CA
La reactancia inductiva XL es una descripción de la fem autoinducida que se opone a cualquier cambio en la
corriente a través del inductor.
Para cierto voltaje aplicado, la reactancia inductiva aumenta cuando la frecuencia aumenta. Esta conclusión
es consistente con la ley de Faraday: cuanto mayor es la rapidez de cambio de la corriente en el inductor,
mayor es la fem inducida. La mayor fem inducida se traduce en un aumento en la reactancia y una
disminución en la corriente.
Los inductores se usan en ciertas aplicaciones de circuitos, tales como los sistemas de suministro de
energía eléctrica y los filtros de interferencias de radio, para bloquear altas frecuencias al mismo tiempo que
se permite el paso de frecuencias bajas o de cd. Un dispositivo de circuito que usa un inductor para este
propósito se llama filtro de paso bajo.

¿En qué frecuencias brilla más la lámpara?

---

### Página 34

Resistencia y reactancia
Capacitor en un circuito de CA
Al conectar una fuente de CA al capacitor, se producirá una corriente

Luego

El voltaje y la corriente del capacitor están fuera de fase por un cuarto de ciclo.

---

### Página 35

Resistencia y reactancia
Capacitor en un circuito de CA
El voltaje máximo es

Nuevamente tenemos la relación VC=ZCI, por tanto definimos la impedancia

Esto nos permite definir la cantidad XC como reactancia capacitiva,

---

### Página 36

Resistencia y reactancia
Capacitor en un circuito de CA
Cuando aumenta la frecuencia de la fuente de voltaje, disminuye la reactancia capacitiva y, por lo tanto,
aumenta la corriente máxima. De nuevo, la frecuencia de la corriente está determinada por la frecuencia de
la fuente de voltaje que activa al circuito. Cuando la frecuencia se aproxima a cero, la reactancia capacitiva
se aproxima al infinito y, por ende, la corriente se aproxima a cero. Esta conclusión tiene sentido porque el
circuito se aproxima a condiciones de corriente directa cuando ω se aproxima a cero y el capacitor
representa un circuito abierto.

Los capacitores tienden a pasar corriente de alta frecuencia y a bloquear las corrientes de baja frecuencia y
la cd; exactamente al contrario de los inductores. Un dispositivo que permite que pasen señales de alta
frecuencia en forma preferencial se llama filtro de paso alto.

¿En qué frecuencias brilla más la lámpara?

---

### Página 37

Circuito LRC en serie
Estudiaremos un circuito en serie que contiene un resistor, un inductor, un capacitor y una fuente de CA. En
este circuito, en virtud de la regla de Kirchhoff de las espiras, el voltaje total instantáneo vad entre las
terminales de los tres componentes es igual al voltaje de la fuente en ese instante.
Supongamos que la fuente suministra

Usando las reglas de Kirchhoff

Lo que se puede escribir como

Entonces podemos escribir

La impedancia total es la
suma de las impedancias de
cada elemento

---

### Página 38

Resistencia y reactancia
Comparación de los elementos en un circuito de CA

---

### Página 39

Circuito LRC en serie
Podemos escribir la impedancia en forma polar, según

Y la fase

Luego, la corriente se puede escribir como

---

### Página 40

Impedancias en serie
Si dos impedancias se conectan en serie, entonces fluye la misma corriente a través de cada una de ellas.
Los voltajes a través de las dos impedancias son V1=Z1I y V2=Z2I. El voltaje de la combinación
V1+V2=(Z1+Z2)I. Está claro, entonces, que en la conexión de impedancias en serie se suman las
impedancias; esto es

Esto es justamente lo que sucedió en el caso anterior, la conexión LRC en serie

Ojo que las impedancias
se deben sumar como
números complejos!

---

### Página 41

Impedancias en serie
Ojo que las impedancias se deben sumar como números complejos!
Sean

Luego, la suma es

Y en forma polar tenemos

---

### Página 42

Impedancias en paralelo
Cuando conectamos impedancias en paralelo, el mismo voltaje aparece a través de cada una de ellas y las
corrientes estarán dadas por I1=V/Z1 y I2=V/Z2, luego

Con lo cual queda claro que

---

### Página 43

Impedancias en serie y paralelo
Ejemplo:
Consideremos el circuito de la figura. La impedancia consiste en un resistor en serie con la combinación en
paralelo de un condensador y un inductor. Encuentre la corriente que circula por este circuito.

---

### Página 44

Impedancias en serie y paralelo
Ejemplo:
La figura muestra un circuito RLC en paralelo. Los voltajes instantáneos (y voltajes rms) en las terminales
de cada uno de los tres elementos de circuito son iguales, y cada uno está en fase con la corriente que
pasa por el resistor. a) Demuestre que la corriente rms entregada por la fuente es

b) Demuestre que el ángulo de fase entre el voltaje y la corriente es

---

### Página 45

Potencia en circuitos de CA
La potencia suministrada a un resistor puede determinarse multiplicando el voltaje a través de cada resistor
por la corriente que pasa a través de él. Sin embargo, para el caso más general, tal como la impedancia de
los casos anteriores, se necesita un enfoque más útil.
La potencia instantánea p entregada a un elemento de circuito se define como

La potencia media es una cantidad más importante, obtenida como el promedio durante un periodo
completo. Si las fases se escogen de tal modo que V sea real, entonces obtenemos

Lo que también se puede escribir como

Factor de potencia

---

### Página 46

Potencia en circuitos de CA
Potencia de un resistor
El producto entre el voltaje y la corriente es siempre positivo, porque ambos están en fase. De ahí que en
todo momento se suministre energía al resistor para ambos sentidos de la corriente, aunque la potencia no
sea constante.
La curva de potencia correspondiente a un resistor es simétrica con respecto a un valor igual a la mitad de
su valor máximo VI, así que la potencia media Pmed es

Y como Vrms=IrmsR, tenemos

---

### Página 47

Potencia en circuitos de CA
Potencia de un inductor
El voltaje en un inductor está desfasado en π/2 respecto a la corriente, por lo que el producto vi es negativo
durante la mitad del ciclo. La curva de potencia es simétrica con respecto al eje horizontal, por lo que la
potencia media es igual a cero.
Cuando p es positiva, la energía se suministra para establecer el campo magnético en el inductor; cuando p
es negativa, el campo desaparece y el inductor devuelve energía a la fuente. La transferencia neta de
energía en un ciclo es igual a cero.

---

### Página 48

Potencia en circuitos de CA
Potencia de un capacitor
El voltaje en un capacitor está desfasado en -π/2 respecto a la corriente, por lo que el producto vi es
negativo durante la mitad del ciclo. La curva de potencia es simétrica con respecto al eje horizontal, por lo
que la potencia media es igual a cero.
Se suministra energía para cargar el capacitor y se devuelve a la fuente cuando el capacitor se descarga.
La transferencia neta de energía en un ciclo es, una vez más, igual a cero.

---

### Página 49

Resonancia
Gran parte de la importancia práctica de los circuitos LRC en serie estriba en la forma en que tales
circuitos responden a las fuentes de diferente frecuencia angular ω.
En un circuito RLC la impedancia alcanza su valor mínimo, Z=R, en

A esta frecuencia el ángulo de fase es cero y la corriente es máxima de magnitud |V|/R.
Este crecimiento máximo de la amplitud de corriente a cierta frecuencia se llama resonancia.

---

### Página 50

Resonancia
El circuito en serie de la figura es similar a las configuraciones que en ocasiones se emplean en los
circuitos de sintonización de radios. Este circuito está conectado a las terminales de una fuente de CA con
voltaje terminal rms constante de 1.0 V y frecuencia variable. Calcule a) la frecuencia de resonancia; b) la
reactancia inductiva; la reactancia capacitiva, y la impedancia a la frecuencia de resonancia; c) la
corriente rms en la resonancia; y d ) el voltaje rms entre las terminales de cada elemento de circuito en la
resonancia.

---

### Página 51

Transformadores
Una de las grandes ventajas de la CA sobre la CD en la distribución de energía eléctrica es que es mucho
más fácil subir y bajar los voltajes con la CA que con la CD. Para la transmisión a grandes distancias es
deseable usar un voltaje tan elevado y una corriente tan pequeña como sea posible; esto reduce las
pérdidas de i2R en las líneas de transmisión, y permite utilizar alambres delgados, con lo cual se reducen
los costos de los materiales.
La conversión necesaria del voltaje se lleva a cabo por medio de transformadores.

El devanado al que se suministra energía se llama primario, y el devanado del que se
toma energía recibe el nombre de secundario.

---

### Página 52

Transformadores
El flujo por espira ΦB es el mismo tanto en el primario como en el secundario, por lo que las ecuaciones
indican que la fem inducida por espira es la misma en cada uno. La razón entre la fem secundaria Ɛ2 y la
fem primaria Ɛ1 es, por lo tanto, igual en cualquier instante a la razón entre las espiras del secundario y las
espiras del primario:

Como ambas fem oscilan con la misma frecuencia que la fuente de CA, tenemos

---

### Página 53

Transformadores
Si conectamos una resistencia al circuito secundario, encontramos que la potencia disipada en la
resistencia, iguala a la potencia provista por el circuito primario, dado que no hay resistencia en las
vueltas.
Entonces,

Luego,

Esto demuestra que, cuando se completa el circuito secundario a través de una resistencia R,
el resultado es el mismo que si se hubiera conectado la fuente directamente a una resistencia
igual a R dividida entre el cuadrado de la razón de espiras. En otras palabras, el transformador
“transforma” no sólo voltajes y corrientes, sino también resistencias. Desde un punto de vista
más general, se puede considerar que un transformador = transforma” la impedancia de la red a
la que está acoplado el circuito del secundario.
