# Pauta Control 3 — Inducción electromagnética y fem de movimiento

> **Curso:** FIS1533 — Electricidad y Magnetismo (Segundo semestre 2025) · **Fecha:** 25 de noviembre de 2025 · **Forma:** 1

---

## Problema 1

Considere un riel conductor conectado a dos resistencias. Una barra conductora de largo $\ell$ desliza sin fricción sobre dos barras conductoras paralelas (separadas una distancia $\ell$) como muestra la figura. Dos resistencias, $R_1$ y $R_2$, se conectan a través de las barras. Existe un campo magnético uniforme en la región donde se encuentran las barras que apunta hacia el interior de la página ($-\hat{k}$). Suponga que un agente externo mueve la barra móvil hacia la izquierda a una velocidad constante $\vec{v}$.

- **a) (2.5 pts.)** Determine la FEM inducida entre los extremos de la barra en movimiento.
- **b) (2.5 pts.)** Determine la corriente a través de cada resistencia.
- **c) (1 pto.)** ¿Cuál es la fuerza que necesita aplicar para mantener la barra a velocidad constante?

> **[Figura]:** Dos rieles conductores horizontales paralelos separados por una distancia vertical $\ell$ (acotada a la derecha), conectados entre sí por la izquierda mediante una resistencia $R_1$ y por la derecha mediante una resistencia $R_2$. Apoyada perpendicularmente sobre ambos rieles se encuentra una barra conductora vertical móvil de largo $\ell$ que se desliza hacia la izquierda con velocidad constante $\vec{v}$ (flecha horizontal hacia la izquierda). En toda la región entre los rieles se dibujan cruces ($\times$) que representan un campo magnético uniforme $\vec{B}$ dirigido hacia el interior de la página ($-\hat{k}$ según el enunciado). Debajo del circuito aparece un sistema de ejes con $+x$ hacia la derecha, $+y$ hacia abajo y $\otimes$ etiquetado como $z$ (entrante a la página).

> **Nota:** Aunque la terna dibujada bajo la figura marca el símbolo entrante $\otimes$ como $z$, el enunciado especifica explícitamente que el campo magnético entrante apunta en $-\hat{k}$ (es decir, $+\hat{k}$ saliente de la página, correspondiente a $+x$ a la derecha y $+y$ hacia arriba). La solución oficial adopta la convención $\vec{B} = -B\hat{k}$ del enunciado.

### Solución

**Idea:** El desplazamiento de la barra móvil con velocidad constante $\vec{v}$ hacia la izquierda modifica el área —y con ello el flujo magnético— de las dos espiras cerradas formadas a izquierda y derecha de la barra. Aplicando la ley de Faraday-Lenz sobre la malla derecha $\Gamma$ (o directamente mediante la fem de movimiento $\mathcal{E} = \oint (\vec{v}\times\vec{B})\cdot d\vec{\ell}$) se obtiene la fem inducida entre los extremos de la barra. Como la barra se encuentra en paralelo con $R_1$ y $R_2$, cada resistencia queda sometida a la misma diferencia de potencial $|\mathcal{E}|$. Finalmente, la fuerza aplicada se halla igualando la potencia mecánica suministrada $P = Fv$ con la potencia eléctrica total disipada por efecto Joule en las dos resistencias.

---

#### Parte a) FEM inducida entre los extremos de la barra

Para obtener la fuerza electromotriz inducida en la barra, consideramos el circuito cerrado $\Gamma$ formado por la barra móvil y la resistencia $R_2$ (a la derecha). Sea $X$ la posición horizontal de la barra medida desde la rama de $R_2$ hacia la izquierda *(0.5 pts por la definición de la región)*.

> **[Figura — Región $\Gamma$ y corrientes inducidas]:** Esquema de la solución sobre el riel que indica la coordenada $X$ desde la resistencia $R_2$ hasta la barra móvil (con una cota horizontal apuntando hacia la izquierda). Se dibujan las corrientes inducidas: una flecha hacia abajo a lo largo de la barra móvil; la corriente $I_1$ circulando en sentido horario por la malla izquierda (subiendo por $R_1$); y la corriente $I_2$ circulando en sentido antihorario por la malla derecha $\Gamma$ (subiendo por $R_2$).

Para calcular el flujo magnético a través de la superficie plana encerrada por $\Gamma$, definimos el vector diferencial de área apuntando en la misma dirección que el campo magnético (entrante a la página):
$$d\vec{A} = -dA\,\hat{k} \qquad \text{(0.5 pts)}$$
donde $dA$ es el elemento diferencial de área. Entonces, el flujo magnético a través de $\Gamma$ toma la forma:
$$\Phi_2 = \int_\Gamma (-B\hat{k})\cdot(-dA\,\hat{k}) = \int_\Gamma B\,dA = B X \ell \qquad \text{(0.5 pts)}$$

> **Nota:** En la pauta oficial se imprime tipográficamente $(-d\vec{A}\hat{k})$ dentro del integrando, con un símbolo vectorial redundante sobre $dA$; el cálculo escalar siguiente $\int_\Gamma B\,dA = BX\ell$ es exacto.

Como la barra se mueve hacia la izquierda a rapidez constante $v = dX/dt > 0$, el área encerrada por $\Gamma$ aumenta y, en consecuencia, también aumenta el flujo entrante $\Phi_2$. Aplicando la ley de Lenz, la corriente inducida $I_2$ debe generar un campo magnético propio saliente ($+\hat{k}$) que se oponga a dicho aumento de flujo, por lo que $I_2$ circula en sentido antihorario en $\Gamma$ (atravesando la resistencia $R_2$ de abajo hacia arriba, como muestra la figura de solución). La fem inducida en la barra toma el mismo sentido que esta circulación (empujando portadores positivos de arriba hacia abajo dentro de la barra móvil), y su magnitud es:
$$|\mathcal{E}| = \left|\frac{d}{dt}\Phi_2\right| = \frac{d}{dt}(B\ell X) = B\ell \frac{dX}{dt} = B\ell v \qquad \text{(1.0 pto)}$$

$$\boxed{|\mathcal{E}| = B\ell v \quad (\text{con polaridad positiva en el riel inferior respecto al superior})}$$

---

#### Parte b) Corriente a través de cada resistencia

La barra móvil actúa como una fuente ideal de fem $|\mathcal{E}|$ conectada entre el riel superior y el riel inferior. Dado que ambas resistencias $R_1$ y $R_2$ conectan directamente esos mismos rieles (están en paralelo respecto a la barra), para cada resistencia se cumple $|\mathcal{E}| = I_i R_i$ *(0.5 pts)*:

$$I_1 = \frac{|\mathcal{E}|}{R_1} = \frac{B\ell v}{R_1} \qquad \text{(1.0 pto)}$$
$$I_2 = \frac{|\mathcal{E}|}{R_2} = \frac{B\ell v}{R_2} \qquad \text{(1.0 pto)}$$

En ambos casos, las corrientes circulan **de abajo hacia arriba** a través de cada resistencia (sentido horario en la malla izquierda para $I_1$ y sentido antihorario en la malla derecha para $I_2$), reuniéndose en la barra móvil hacia abajo.

$$\boxed{I_1 = \frac{B\ell v}{R_1}\ (\text{hacia arriba por } R_1), \qquad I_2 = \frac{B\ell v}{R_2}\ (\text{hacia arriba por } R_2)}$$

---

#### Parte c) Fuerza aplicada para mantener velocidad constante

La fuerza externa $F$ aplicada por el agente externo suministra potencia mecánica al sistema, la cual, al mantenerse constante la velocidad (energía cinética invariante), es igual a la potencia eléctrica disipada por efecto Joule en las resistencias.

En la parte mecánica, la potencia suministrada por la fuerza aplicada en la dirección de $\vec{v}$ es:
$$P = F v \qquad \text{(0.2 pts)}$$

En la parte eléctrica, la potencia disipada por $R_1$ y $R_2$ está dada por:
$$P = I_1^2 R_1 + I_2^2 R_2 = \left(\frac{B\ell v}{R_1}\right)^2 R_1 + \left(\frac{B\ell v}{R_2}\right)^2 R_2 = B^2 \ell^2 v^2 \left(\frac{1}{R_1} + \frac{1}{R_2}\right) \qquad \text{(0.3 pts)}$$

Igualando ambas expresiones de potencia:
$$F v = B^2 \ell^2 v^2 \left(\frac{1}{R_1} + \frac{1}{R_2}\right) \qquad \text{(0.2 pts)}$$

Por lo tanto, la magnitud de la fuerza externa necesaria (dirigida hacia la izquierda, en el sentido de $\vec{v}$) es:
$$F = B^2 \ell^2 v \left(\frac{1}{R_1} + \frac{1}{R_2}\right) \qquad \text{(0.3 pts)}$$

$$\boxed{\vec{F}_{\text{ext}} = B^2 \ell^2 v \left(\frac{1}{R_1} + \frac{1}{R_2}\right)\,\text{(hacia la izquierda)}}$$

**Verificación:**
- **Fuerza magnética directa:** Por la barra desciende una corriente total $I_{\text{barra}} = I_1 + I_2 = B\ell v\left(\frac{1}{R_1} + \frac{1}{R_2}\right)$. En presencia del campo entrante $\vec{B}$, la fuerza magnética sobre la barra es $\vec{F}_B = I_{\text{barra}}\vec{\ell}_{\text{barra}}\times\vec{B}$; por regla de la mano derecha (corriente hacia abajo, campo entrante), $\vec{F}_B$ apunta **hacia la derecha** (frenando el movimiento), con magnitud $F_B = I_{\text{barra}} \ell B = B^2 \ell^2 v\left(\frac{1}{R_1} + \frac{1}{R_2}\right)$. Para mantener $\vec{v}$ constante ($\vec{F}_{\text{neta}} = \vec{0}$), el agente externo debe ejercer $\vec{F}_{\text{ext}} = -\vec{F}_B$ hacia la izquierda con idéntica magnitud.
- **Malla izquierda como verificación de $|\mathcal{E}|$:** En la malla izquierda el ancho disminuye a razón $-v$, por lo que $\left|\frac{d\Phi_1}{dt}\right| = B\ell v$, y como el flujo entrante disminuye, Lenz exige una corriente horaria $I_1$ que refuerce el campo entrante, consistente con el sentido obtenido.
- **Unidades:** $[B^2 \ell^2 v / R] = (\text{T}^2\cdot\text{m}^2\cdot\text{m}/\text{s}) / (\text{V}/\text{A}) = \frac{(\text{N}/(\text{A}\cdot\text{m}))^2 \cdot \text{m}^3/\text{s}}{\text{J}/(\text{C}\cdot\text{A})} = \text{N}$, consistente.

---

## Resumen de resultados

| Problema | Parte | Cantidad | Resultado |
| :--- | :--- | :--- | :--- |
| **Problema 1** | a) | Magnitud de la FEM inducida | $|\mathcal{E}| = B\ell v$ |
| | b) | Corriente en $R_1$ | $I_1 = \dfrac{B\ell v}{R_1}$ (hacia arriba por $R_1$, sentido horario) |
| | b) | Corriente en $R_2$ | $I_2 = \dfrac{B\ell v}{R_2}$ (hacia arriba por $R_2$, sentido antihorario) |
| | c) | Fuerza externa aplicada | $F = B^2\ell^2 v \left(\dfrac{1}{R_1} + \dfrac{1}{R_2}\right)$ (hacia la izquierda) |
