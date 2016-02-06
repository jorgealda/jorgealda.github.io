---
layout: post
title:  "Lagrange y Hamilton: reescribiendo las leyes"
date:   2014-10-25 12:50:56 +0100
categories: bosoneando
permalink: /bosoneando/:year/:month/:day/:title/
--- 

![](http://www.mlahanas.de/Stamps/Data/PHPerson/thumbnails/Lagrange001.jpg) ![](http://www.mlahanas.de/Stamps/Data/PHPerson/thumbnails/Hamilton001.jpg)

La mecánica es la rama de la física que estudia el movimiento y sus causas. Aunque haya sido estudiada desde los albores de la humanidad ( al menos desde que a un intrépido homínido se le ocurrió lanzarle un proyectil al desdichado animal que se convertiría en su cena), empezó a ser una ciencia rigurosa con los trabajos de Galileo y Newton, que culminaron con sus tres leyes en 1687:

1. En ausencia de fuerzas, un cuerpo permanece en su estado de reposo o de movimiento rectilíneo uniforme. $$ \vec{F}=0 \Leftrightarrow \ddot{\vec{r}}=0 $$
2. Las fuerzas producen aceleraciones sobre los cuerpos. La magnitud que relaciona fuerzas y aceleraciones es la masa $$\vec{F} =\dot{\vec{p} }= m \ddot{\vec{r}}$$
3. Ley de acción y reacción: si un cuerpo ejerce una fuerza sobre otro, el segundo ejerce una fuerza sobre el primero de igual magnitud y sentido contrario $$ \vec{F}_{2\to 1} = - \vec{F}_{1\to 2}$$

[Notación: ponemos un punto sobre una variable para indicar que la estamos derivando parcialmente respecto al tiempo - si la variable depende de varias magnitudes, entre ellas el tiempo, indica cómo varia al cambiar el tiempo SIN cambiar el resto de dependencias -. $$\vec{r}$$ es el vector de posición y $$\vec{p}$$ el momento lineal $$\vec{p} =m \dot{\vec{r}}$$ ]


Hasta aquí todo parece muy fácil, ¿no?

En primer lugar, la notación vectorial, aunque resulte muy cómoda, puede llevar a engaños porque lo que estamos escribiendo con una sola ecuación son en realidad tres. Y son siempre tres, aunque el movimiento de la partícula esté restringido (tenga menos grados de libertad), a no ser que la restricción sea a un movimiento plano o rectilíneo. Además, la fuerza en general depende de la posición y velocidad, con lo cual hay que resolver un sistema de tres ecuaciones diferenciales de segundo orden acopladas, lo cual no siempre es fácil. Los problemas se multiplican si se consideran varios cuerpos.

Entrando en acción
------------------

Aunque este post trate sobre mecánica, voy a hacer una pequeña disgresión a la óptica. Para explicar la reflexión y refracción de la luz, el abogado y aficionado a las matemáticas y la física Pierre Fermat (famoso por quedarse sin papel a la hora de escribir la demostración de un famoso teorema en teoría de números) propuso el principio de mínimo tiempo en 1662, 16 años antes que las leyes de Newton (aunque Herón de Alejandría y Alhacén habían hecho propuestas similares algunos siglos antes). El principio de Fermat asegura que la trayectoria que sigue un rayo de luz es aquélla que hace el tiempo de propagación mínimo (en realidad vale con que sea un extremal: máximos y puntos de inflexión están permitidos). En jerga matemática, si denotamos con $$s$$ la longitud recorrida por el rayo hasta llegar a un punto de su trayectoria, y $$n(s)$$ al índice de refracción en ese punto, el tiempo de propagación está dado por 

$$\begin{equation} t = \frac{1}{c } \int_{s_i}^{s_f} n(s) ds \end{equation}$$

[la velocidad de la luz en un medio es $$v=c /n$$, donde $$c$$ es la velocidad de la luz en el vacío y $$n \geq 1$$. En una porción del recorrido suficientemente pequeña, $$ds$$, la velocidad es aproximadamente constante y se recorre en un tiempo $$ dt = ds/v$$. El símbolo de integral suma los tiempos de todos los cachitos]

La condición de que el tiempo total sea un extremal se expresa de la siguiente manera: imaginemos que hacemos un cambio pequeño en la trayectoria $$\delta s$$. Esto provoca un cambio en el tiempo de propagación $$\delta t$$. El extremal se produce cuando $$\delta t =0$$


¡Basta ya de óptica! Volvamos a la mecánica. Maupertuis propuso un principio de mínimo, inspirado por el de la luz, para las partículas. Para ello definió una magnitud, la acción (acción abreviada, para no confundirla con la acción de verdad): $$ S_M = \int p ds$$

Esta magnitud debía ser extremal. Al resolver la ecuación ( empleando el cálculo de variaciones) se obtiene la forma de la trayectoria, pero no la posición en función del tiempo.


La solución la propuso Hamilton. La magnitud que hay que hace extremal es la acción (ésta sí es la buena):

$$S = \int_{t_1}^{t_2} L dt$$

La magnitud $$L$$ es el lagrangiano, definido como la energía cinética menos la energía potencial $$L=T-V$$

El principio de Hamilton asevera que la acción a lo largo de la trayectoria es extremal. Éste es el axioma en el que se basa la formulación actual de la mecánica clásica, y básicamente del resto de la física (y hasta ahora funciona de maravilla).


**Atención: A partir de aquí puede haber matemáticas peligrosas. Avance bajo su propio riesgo.**


Dadme un lagrangiano y moveré el mundo
----------------------------------

De momento no es evidente cuál es la ventaja de usar el principio de Hamilton en vez de las ecuaciones de Newton de toda la vida. La clave está en el sistema de coordenadas: las ecuaciones de Newton solamente funcionan con un sistema de coordenadas cartesianas, mientras que el principio de Hamilton es mucho menos exigente: se puede aplicar con cualquier sistema de coordenadas generalizado. Las coordenadas generalizadas son un conjunto de números $$q_\alpha $$ que describen la posición del sistema mecánico, y hay tantas como grados de libertad tenga. Por ejemplo, si tenemos una cuenta insertada en un alambre retorcido, en las coordenadas cartesianas se necesitan tres números para describir su posición, aunque esta se pueda determinar con una única coordenada generalizada: la distancia desde la cuenta hasta el extremo del alambre, medida sobre el propio alambre.

Una vez que se han definido las coordenadas generalizadas, hay que expresar la energía cinética y potencial en términos de estas coordenadas. Ahora solo hay que hacer la acción extremal, pero ¿cómo? El cálculo de variaciones nos ofrece la solución, la conocida como ecuación de Euler-Lagrange (si el lagrangiano solo depende de las coordenadas generalizadas y sus primeras derivadas): 

$$\frac{d L}{d q_\alpha} = \frac{d}{d t}\left( \frac{\partial L}{\partial \dot{q}_\alpha}\right) $$

Como un ejemplo básico, vamos a comprobar cómo utilizando las coordenadas cartesianas y una energía potencial independiente de la velocidad se recupera la segunda ley de Newton: 

$$L = \frac{1}{2} m \dot{x}^2 - V(x)$$

$$\frac{d L}{d x} = - \frac{d V(x)}{d x} = \frac{d}{d t}\left( \frac{\partial L}{\partial \dot{x}}\right) = \frac{d}{d t}\left( m \dot{x}\right) = m \ddot{x}$$

Efectivamente, esta es la expresión para una fuerza conservativa $$F_x = - \frac{d V(x)}{d x}$$.

Pero la potencia de la formulación lagrangiana no se acaba en la mecánica clásica. La manera de definir una teoría es proporcionando su lagrangiano (más habitualmente la densidad del lagrangiano, $$\mathcal{L}$$, especialmente para teorías consistentes con la relatividad especial). Por ejemplo, para el electromagnetismo, si $$F_{\mu\nu}$$ es el tensor del campo electromagnético 

$$\mathcal{L} = \frac{1}{4} F^{\mu\nu}F_{\mu\nu}$$

O para el modelo estándar de la física de partículas

![](http://www.quantumdiaries.org/wp-content/uploads/2012/09/sm_lagrangian_UCDavis.png)

El mérito de escribir esta fórmula corresponde a [T. D. Gutiérrez](http://nuclear.ucdavis.edu/~tgutierr/files/stmL1.html)
	


	


Hamilton: el regreso
---------------------

Hemos conseguido reducir el número de ecuaciones diferenciales que hay que resolver al elegir sabiamente las coordenadas en las que vamos a trabajar, pero siguen siendo ecuaciones diferenciales de segundo orden. ¿Podemos convertirlas en ecuaciones de primer orden?

Volvamos un momento a la ecuación de Euler-Lagrange para las coordenadas cartesianas. Hay un término que resulta familiar... Es nuestro amigo el momento lineal! (si no es tu amigo aún, espera a conocerlo bien)
 
$$\frac{d L}{d x}  = \frac{d}{d t}\left( m \dot{x}\right)$$

Empleando otro sistema de coordenadas, el término análogo se conoce como momento generalizado $$p_\alpha$$ 

$$p_\alpha = \frac{\partial L}{\partial \dot{q}_\alpha}$$

Puede resultar conveniente expresar la información que tenemos condensada sobre nuestro sistema en términos de las posiciones y momentos, y que no aparezca ninguna derivada. El mecanismo matemático para hacerlo es la transformada de Legendre: 

$$H(q_\alpha, p_\alpha) = \sum_\alpha p_\alpha \dot{q}_\alpha - L$$

La magnitud que resulta de hacer la transformada de Legendre del lagrangiano es nuestro nuevo protagonista, el hamiltoniano. Si la energía cinética depende solo de los cuadrados de las velocidades y la potencial solo de las posiciones, entonces el hamiltoniano coincide con la energía total. El hamiltoniano es muchas veces más útil que la energía, ya que si el sistema está forzado (se le está aplicando una fuerza externa) la energía no se conserva pero el hamiltoniano sí.

La dinámica de un sistema en términos del hamiltoniano se expresa en forma de ecuaciones diferenciales de primer orden (eso sí, el doble que grados de libertad. Aquí nada es gratis), las ecuaciones de Hamilton-Jacobi 

$$\frac{d H}{d p_\alpha} = \dot{q}_\alpha \qquad \frac{d H}{d q_\alpha} = - \dot{p}_\alpha$$

De nuevo, usando las coordenadas cartesianas volvemos a la segunda ley de Newton

$$H = \frac{p^2}{2 m} + V(x)$$

$$\frac{p}{m} = \dot{x} \qquad \frac{d V(x)}{d x} = - \dot{p}_x$$


El teorema más bello de la física
---------------------------------

Ahora supongamos que tenemos una magnitud física que depende de las posiciones y los momentos, pero no _explícitamente_ del tiempo $$A(q_\alpha, p_\alpha)$$. Vamos a calcular su derivada respecto al tiempo, usando la regla de la cadena:

$$\frac{d A}{d t} = \sum_\alpha \left( \frac{d A}{d q_\alpha} \dot{q}_\alpha+\frac{d A}{d p_\alpha} \dot{p}_\alpha\right)$$

Pero estas cantidades ya las conocemos, gracias a Hamilton y Jacobi

$$\frac{d A}{d t} = \sum_\alpha \left(\frac{d A}{d q_\alpha}\frac{d H}{d p_\alpha} - \frac{d A}{d p_\alpha}\frac{d H}{d q_\alpha}\right)$$

Se define el corchete de Poisson de dos magnitudes como 

$$\{A, B\} = \sum_\alpha \left( \frac{d A}{d q_\alpha}\frac{d B}{d p_\alpha} - \frac{d A}{d p_\alpha}\frac{d B}{d q_\alpha} \right) $$

Por lo tanto, la evolución temporal de la magnitud es

$$\frac{d A}{d t} = \{A, H\}$$


Hagamos más probaturas con los corchetes de Poisson. Por ejemplo, vamos a calcular el corchete de una magnitud con el momento generalizado

$$\{A, p_\alpha\} = \sum_\alpha \frac{d A}{d q_\alpha}\frac{d p_\alpha}{d p_\alpha} - \frac{d A}{d p_\alpha}\frac{d p_\alpha}{d q_\alpha} = \frac{d A}{d q_\alpha} $$

Esto no son más que dos casos particulares de una propiedad más general. Supongamos que tenemos una función $$G(q_\alpha, p_\alpha)$$, a la que llamaremos generador infinitesimal de la transformación -¡vaya nombrecito!-, tal que al realizar una transformación (pequeña) de nuestro sistema, sus nuevas coordenadas son

$$\delta q_\alpha = \frac{\partial G}{\partial p_\alpha}\delta \lambda \qquad \delta p_\alpha = -\frac{\partial G}{\partial q_\alpha} \delta \lambda$$

Vamos a ver cómo cambia una magnitud $$A$$ bajo esta transformación

$$\delta A = \sum \frac{\partial A}{\partial q_\alpha}\delta q_\alpha + \frac{\partial A}{\partial p_\alpha}\delta p_\alpha = \left(\sum \frac{\partial A}{\partial q_\alpha}\frac{\partial G}{\partial p_\alpha} - \frac{\partial A}{\partial p_\alpha}\frac{\partial G}{\partial q_\alpha} \right) \delta \lambda = \{ A, G\} \delta \lambda $$

Ahora vamos a suponer que la magnitud que queremos ver cómo se transforma es el propio hamiltoniano, y que hemos dado con una transformación que lo deja invariante (este tipo de transformaciones se llaman simetrías):

$$\delta H = 0 = \{H, G\} = - \frac{d G}{d t} $$

Esto quiere decir que si tenemos una simetría del hamiltoniano, entonces hay una magnitud que se conserva en el tiempo. Esto es precisamente lo que enuncia el teorema de Nöther. ¿Bonito, no?

Los ejemplos típicos de simetrías en el hamiltoniano son las traslaciones espaciales, la traslación temporal y las rotaciones; las cantidades conservadas correspondientes son el momento lineal, el hamiltoniano y el momento angular. En física de partículas aparecen nuevas simetrías (simetrías gauge), entre las que destaca la simetría del potencial vector electromagnético que implica la conservación de la carga eléctrica.


Para más información...
-----------------------

* Tom W. B. Kibble, Frank H. Berkshire: Classical Mechanics. Imperial College Press, 5th edition 2004.

* Enrique F. Borja: [Mecánica Lagrangiana](http://cuentos-cuanticos.com/2011/10/02/mecanica-lagrangiana/), [La acción 1](http://cuentos-cuanticos.com/2011/10/06/la-accion-1/) y [2](http://cuentos-cuanticos.com/2011/10/07/la-accion-2/), [Simetrías y cantidades conservadas. El teorema Nöther](http://cuentos-cuanticos.com/2011/10/20/simetrias-cantidades-conservadas-teorema-noether/), [Esto no era tan complicado: Las aventuras del Hamiltoniano](http://cuentos-cuanticos.com/2011/07/31/hamiltoniano/). Cuentos cuánticos.



