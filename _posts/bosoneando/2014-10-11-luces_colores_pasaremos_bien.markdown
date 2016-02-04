---
layout: post
title:  "Luces de colores, lo pasaremos bien"
date:   2014-10-11 14:39:56 +0100
categories: bosoneando
permalink: /bosoneando/:year/:month/:day/:title/
---

![Isamu Akasaki, Hiroshi Amano y Shuji Nakamura](http://www.nobelprize.org/nobel_prizes/physics/laureates/2014/)
Isamu Akasaki, Hiroshi Amano y Shuji Nakamura, © Nobel Media 2014


Recientemente, la Fundación Nobel ha comunicado [la decisión](http://www.nobelprize.org/nobel_prizes/physics/laureates/2014/) de otorgar el Nobel de Física de 2014 a los físicos japoneses Isamu Akasaki, Hiroshi Amano y Shuji Nakamura "por la invención de diodos emisores de luz azul eficientes que han permitido fuentes de luz blanca brillantes y de bajo consumo". El premio no está exento de polémica, ya que el inventor del LED rojo, Nick Holonyak, se siente "decepcionado e irritado" por no haber sido reconocido.



##¡Únete a la banda!

La mecánica cuántica predice que los electrones que forman parte de un átomo no pueden tener cualquier valor de energía. sino unos valores concretos correspondientes a los niveles del átomo. Estos niveles están caracterizados por cuatro números cuánticos ($$n$$ número cuántico principal, $$\ell$$ número cuántico azimutal, $$m_\ell$$ número cuántico magnético y $$m_s$$ número cuántico de espín). 

Al tratar con partículas idénticas, la cuántica debe hacer uso del postulado de simetrización, que dicta que la función de ondas que describe a las partículas debe ser invariante (bosones) o cambiar de signo (fermiones) al intercambiar dos partículas. El hecho de que los electrones sean fermiones y ganen un signo menos bajo intercambio implica que no puede haber dos electrones con los mismos números cuánticos (principio de exclusión de Pauli).

Si ahora aproximamos un gran número de átomos idénticos para formar una red cristalina, el principio de exclusión de Pauli nos indica que la estructura de niveles de los átomos no puede permanecer inalterada, ya que esto supondría un gran número de electrones en los mismos niveles. En su lugar, se produce una modificación de las energías de los estados, formándose un continuo de niveles: nace así la estructura de bandas.  Hay bandas de energía permitidas, en las que puede haber electrones, separadas por bandas de energía prohibidas. Para determinar la energía de un electrón en una banda es necesario un nuevo número cuántico, $$k$$ el cuasimomento cristalino.


Dependiendo de la estructura de bandas, los sólidos cristalinos se clasifican en tres tipos:

    Conductores: A 0K, cuando los electrones ocupan las posiciones de mínima energía, hay una banda parcialmente ocupada (las bandas inferiores están totalmente ocupadas y las superiores totalmente vacías).
    Aislantes: A 0K, hay capas totalmente llenas y totalmente vacías. La última capa llena es la capa de valencia, y la primera vacía la capa de conducción, y están separadas por el gap. La anchura del gap es muy elevada, impidiendo los fenómenos de conducción a las temperaturas y corrientes habituales.
    Semiconductores: La estructura de bandas es similar a los aislantes, pero la energía del gap es mucho menor, del orden de la energía térmica. Son los que ofrecen mayor variedad de comportamiento eléctrico.

En los semiconductores, a las temperaturas convencionales, un electrón puede ganar energía y pasar de los niveles superiores de la banda de valencia a los inferiores de la banda de conducción. Ahora, el material puede conducir la corriente eléctrica por dos motivos: en primer lugar, en la capa de conducción el electrón tiene libertad de movimiento por la red, y en la capa de valencia, porque el nivel que ha quedado vacío puede ser ocupado por los electrones vecinos, produciendo un movimiento de cargas. Para caracterizar este segundo proceso, en vez de tener que estudiar el movimiento de todos los electrones de la capa, es matemáticamente equivalente sustituirlo por una "partícula" que representa al nivel vacío, el hueco, de características físicas iguales al electrón original excepto su carga, que es positiva.

Por motivo de la temperatura, se producen y aniquilan continuamente pares de electrón-hueco. Si el cristal se encuentra en equilibrio (no hay corriente eléctrica u otros aportes externos de energía), la concentración de los portadores de carga se estabiliza en unos valores característicos de cada material y temperatura.
Dopaje

Estas concentraciones se pueden modificar de forma externa durante el proceso de fabricación del material, añadiendo impurezas a la red. Estos átomos extraños aportan nuevos niveles (discretos) de energía a la estructura de bandas:

    Impurezas donadoras: estos átomos poseen niveles ocupados en el gap próximos al borde inferior de la capa de conducción. Sus electrones pasan fácilmente a conducción sin generar huecos.
    Impurezas aceptoras: los átomos poseen niveles vacíos en el gap próximos al borde superior de la capa de valencia. Los electrones de valencia pueden ocuparlos fácilmente, creando huecos pero no electrones de conducción.

Los semiconductores en los que predominan las impurezas donadoras se denominan extrínsecos tipo N, y aquéllos en los que dominan las impurezas aceptoras son extrínsecos tipo P.

En los semiconductores extrínsecos (en el rango habitual de temperaturas) la cantidad de portadores mayoritarios (electrones en los N y huecos en los P) está determinado exclusivamente por la concentración de las impureza, y es varios órdenes de magnitud superior a la que tendría el semiconductor intrínseco (sin impurificar), mientras que la concentración de portadores minoritarios desciende.


##Uniendo las piezas

Una vez que se tienen distintos tipos de semiconductores, podemos proceder a realizar uniones. El dispositivo más simple es la unión PN. Como su propio nombre indica, está formado por un semiconductor tipo P y uno tipo N (en realidad no se unen dos semiconductores, sino que se crecen simultáneamente los dos cristales para que no haya imperfecciones en la unión).

En la zona de unión hay un proceso de difusión: los electrones pasan de la zona N a la P y los huecos a la inversa - no les gustan las multitudes, y están "más anchos" en el otro lado. Así, en la zona e transición en el material N hay un exceso de cargas positivas y en la zona P un exceso de cargas negativas. Esto crea una diferencia de potencial y un campo eléctrico. El campo atrae a los electrones hacia la región N y los huecos hacia la región P. En equilibrio, las tendencias de difusión y arrastre se compensan.



Ahora vamos a conectar nuestra unión a una batería:

    Polarización directa: se conecta el borne positivo al tipo P y el borne negativo al N. El potencial de la batería atrae a los electrones a la región N y los huecos a la región P: estos portadores llegan hasta la zona de transición, donde se aniquilan. En todo el material hay una corriente que va en semtido P $$\to$$ N. (La corriente puede ser tan elevada que puede incluso quemar el dispositivo. Para evitarlo hay que poner una resistencia en serie que regule la corriente).
    Polarización inversa: se conecta el borne positivo al tipo N y el borne negativo al tipo P. Ahora el potencial de la batería atrae a los electrones de la región N y los huecos de la región P alejándolos de la zona de transición. La diferencia de potencial en la unión crece y se hace mayor que el potencial de alimentación: no circula la corriente.

El dispositivo fabricado tiene un comportamiento fuertemente asimétrico en función del sentido de la corriente: hemos creado un diodo.

##¡Hágase la luz!

Hemos visto que en una unión PN trabajando con polarización directa hay procesos de recombinación en la zona de unión, es decir, que los electrones pasan de la banda de conducción a la banda de valencia, perdiendo para ello energía. Pero ¿adónde va esa energía? La respuesta depende del tipo de material.


Volvamos con nuestro viejo amigo el cuasimomento cristalino $$k$$: es una cantidad conservada. Si el electrón en el borde superior de la capa de valencia y en el borde inferior de la capa de conducción tienen el mismo cuasimomento, lo que se conoce como semiconductor de gap directo, el electrón puede pasar de un nivel a otro por la absorción o emisión de un fotón (que no transporta cuasimomento).


Por el contrario, si los cuasimomentos en ambos extremos de las bandas no coinciden (gap indireto), la transición se hace acoplada a las vibraciones de la red - lo que es lo mismo, disipación como calor - que aporta la diferencia de cuasimomento. En principio, podría ir parte de la energía a la red y e a un fotón, pero es un proceso muy poco probable por involucrar más partículas, y el fotón no estaría en el rango visible.



Por lo tanto, una unión PN de semiconductores de gap directo con polarización directa es capaz de producir luz. Esto es lo que se conoce como LED, diodo emisor de luz. El color - frecuencia - de la luz producida (que es bastante monocromática) depende de la diferencia de energías entre la banda de valencia y de conducción: cuanto más próximas estén, más rojiza.


##Colorín colorado...


El primer LED operativo fue construido en 1961 por Biard y Pittman usando  arseniuro de galio, y emitía en infrarrojo. Holonyak inventó el primer LED visible, el rojo, tan solo un año después. En poco tiempo también estuvieron disponibles otros colores, como el amarillo y el verde. Pero el LED azul se hizo de rogar.

El LED azul fue desarrollado en 1994 por el equipo receptor del Nobel. Está formado por distintas capas de nitruro de galio y nitruro de indio-galio. En nitruro de galio tiene una banda prohibida de 3.4 eV, correspondiente al ultravioleta próximo, y ya fue propuesto en los años 60 como el material idóneo para los diodos azules. Sin embargo, en aquella época no se contaba con la tecnología necesaria para fabricar cristales suficientemente grandes y para introducir impurezas aceptoras. Además, para aumentar la eficiencia de la emisión se usaron heterouniones, en las que el material P y el N tienen distinta composición química.

Estructura del LED azul con doble heterounión: Nakamura, Mukai & Senoh. Appl. Phys. Lett. 64, 1687 (1994)


Actualmente se construyen diodos láser azules que se emplean para la grabación y lectura de discos de alta densidad de almacenamiento (Blu-ray), y se están desarrollando diodos ultravioletas para emplearlos para desinfección, disociando el DNA de los microorganismos.


La disponibilidad del LED azul permite la creación de LED blancos, de dos formas distintas: o bien, como en los monitores LED se puede crear el blanco (y el resto de colores) a partir de los tres colores primarios, o bien, como en las lámparas LED, por fosforescencia. El diodo emite luz azul, o incluso ultravioleta, que llega a una capa fosforescente, que absorbe la luz, y por efecto Stokes, la reemite con un espectro más ancho (luz blanca) y a menor frecuencia. El fundamento es similar a los clásicos fluorescentes, donde la luz ultravioleta inicial procede de la desexcitación de los átomos del vapor de mercurio tras haber sido ionizados por el cebador. La principal diferencia es que el LED es significativamente más eficaz (los LED proporcionan 300 lm/W, frente a los 70 lm/W de los fluorescentes o los 16 lm/W de una bombilla de filamento), siendo la fuente de iluminación - sin contar al Sol - más eficiente de la que disponemos. Y eso bien vale un Nobel.


###Para más información:

The Royal Swedish Academy of Sciences: The Nobel Prize in Physics 2014 - Advanced Information

Francis R. Villatoro: Nobel Física 2014: Akasaki, Amano y Nakamura por el diodo azul

Enrique F. Borja: Un Nobel pintado de azul 


Esta entrada partcipa en el LVII carnaval de la Física, celebrado en octubre de 2014 y albergado por el blog Divulgación, y con el tema "Física y divulgación". 
