# La radio

La radio de AirBorne no es un menú de acciones disfrazado. Lo que puedes decir depende de dos cosas, en este orden, y el orden es todo el asunto.

- **Quién escucha** — la estación a la que está sintonizada la radio. Pedirle un push-back a la torre no se rechaza: es algo que no se dice, porque le estás hablando a la persona equivocada. Sintonizar la radio es cómo eliges con quién hablas.
- **En qué punto está el vuelo** — la fase. Un piloto en el puesto no pide aterrizar.

La fase se calcula primero a partir del avión —en tierra o no, motores, velocidad, altitud, velocidad vertical— y solo después a partir de hasta dónde ha llegado la radio.

## Las teclas

- **F1** abre el menú de radio: una lista corta de lo que tiene sentido en ese momento, y un dígito para elegir uno. Las flechas lo recorren, Enter lo toma, Escape lo cierra.
- **Mayús F1** repite la última instrucción.
- **Control F1** pide al controlador que la repita.
- **Espacio**, mantenido, es el botón de transmisión: se mantiene, se habla, se suelta.

Mientras el menú de radio está abierto, la fila de dígitos y las flechas le pertenecen a él —pero todo lo demás sigue funcionando. Un menú que se llevara consigo al avión sería un menú que nadie abriría en el aire.

El propio equipo es el panel de control 3:

- **F** lee el equipo; mayús F y control F sintonizan la caja de espera un canal cada vez. M hace lo mismo en megahertzios enteros.
- **S** avanza la espera a la siguiente estación, control S a la anterior. Eso es lo que hace que la radio sea usable sin un teclado numérico: cien pulsaciones para recorrer marcando toda la banda es un obstáculo, no un mando.
- **W** intercambia activa y espera. C selecciona COM 1 o COM 2. R lee ambos equipos.

La sintonización siempre se hace en la caja de espera. Un mando torpe nunca debe poder sacarte de la frecuencia en la que te dijeron que estuvieras.

## Las frecuencias son reales

La base de datos de aeródromos lleva veinte mil frecuencias reales —torres, tierra, entrega de autorizaciones, ATIS, aproximación, y a menudo el centro. Esas son las que se usan, y están marcadas como reales. Lo que nadie publica se asigna de forma determinista a partir del código OACI del aeródromo, en la banda que realmente ocupa ese servicio, con un espaciado de 25 kHz: un aeródromo sin torre publicada aun así tiene una, la misma en cada vuelo.

Cada frecuencia lleva de dónde viene, y la lista indica cuál es cuál. Una cifra que un piloto apunta y después descubre que está mal es peor que una que es obviamente inventada.

Un aeródromo que solo publica una frecuencia aire-aire la usa tanto para la torre como para tierra. Eso es lo que es un aeródromo no controlado: todo el mundo en la misma frecuencia.

## El ciclo completo

### El ATIS — en cualquier momento

Escucha la emisión: pista en uso, viento, QNH, nivel de transición. Nada que pedir; escuchas.

### Entrega de autorizaciones y tierra — antes de moverse

- pides la autorización → autorizado a tu destino, pista de salida, código de transpondedor, contacta con tierra
- pides push-back y arranque → aprobado, orientado hacia tal rumbo
- pides rodaje → la ruta por las calles de rodaje, espera antes de la pista
- repites la autorización de rodaje
- informas listo para salida → contacta con la torre

### La torre — en tierra

- informas listo para salida → alinéate y espera, o mantente
- pides alinearte → alinéate y espera
- pides despegar → autorizado para despegar, viento, contacta con salidas al estar en el aire

### La torre — recién en el aire

La transferencia a salidas se da sin que la pidas. Es la única llamada del vuelo que tiene que ocurrir tanto si lo piensas como si no, sin la cual el vuelo termina hablando con nadie.

### Salidas y aproximación — ascendiendo

- informas en el aire → contacto de radar, asciende al primer peldaño por encima del ascenso inicial
- informas nivelado → recibido, o la corrección si no es el que te dieron
- pides más alto → el siguiente peldaño, o el nivel que hayan nombrado si lo nombraron
- pides el crucero → contacta con el centro

### El centro — en crucero

- informas posición → recibido
- pides descenso → desciende al peldaño por debajo de ti

### Aproximación — descenso y llegada

- pides vectores → un rumbo, una altitud, después la autorización ILS
- pides la aproximación → autorizado ILS pista tal, informa establecido
- informas establecido → recibido, contacta con la torre

### La torre — llegando

- pides aterrizar → autorizado para aterrizar pista tal, viento
- informas pista despejada → contacta con tierra

### Tierra — después de aterrizar

- pides rodar al puesto → rueda al puesto por tal ruta
- informas parado → buen vuelo

## Por debajo del nivel de transición, ya no es un nivel

Es una altitud, con el QNH, dicho una vez en el momento en que te mandan por debajo de la transición —el único punto de un vuelo en el que la subescala viene de una persona, lo cual cuenta cuando no puedes leer un mando.

El QNH es el del aeródromo de llegada, no el de salida: son dos cifras distintas y has cruzado medio país entre una y otra. El nivel de transición va con esa autorización porque no se puede imprimir en una carta —depende de la altitud de transición publicada del aeródromo de llegada y de la presión del día.

## Lo que dice el controlador sin que se lo pidan

Un controlador real no espera indefinidamente a que el piloto piense en la siguiente llamada. Tras un momento de silencio, continúa:

- autorización dada, avión parado → "¿está listo para rodar?"
- rodaje dado, avión detenido → "informe listo para salida"
- listo para salida informado → el alineamiento, sin que se pida
- alineado → la autorización de despegue, sin que se pida
- en el aire → la transferencia a salidas, inmediata e incondicional
- descendiendo o en aproximación → un vector nuevo cada dieciocho segundos
- establecido en aproximación → la transferencia a la torre

Nada de esto te llega si no estás en su frecuencia. Perder una transferencia te deja de verdad inalcanzable, y eso lo enseña mejor que cualquier mensaje de aviso.

## El interfono, que no es la radio

Lo que se le dice al personal de tierra no pasa por ninguna frecuencia: es un cable entre la cabina de mando y un hombre de pie bajo el avión. Tiene su propia voz en los ajustes, deliberadamente separada de la de la radio —los dos dicen palabras parecidas sobre el mismo push-back, y solo uno de ellos es dueño de la calle de rodaje.

- **el push-back** — "confirme frenos puestos", "barra puesta, pasador puesto, confirme frenos sueltos", "empezando el push-back", "push-back completado, confirme frenos puestos", después el pasador retirado y el remolcador despejado.
- **"motores despejados"** — dicho sin que lo pidas, en cuanto el avión sale del puesto. La cabina no puede ver sus propios motores y el personal de tierra sí: hasta que se diga eso, arrancar significa arrancar sobre alguien.
- **el arranque** — "arrancando el número tal" desde la cabina, "autorizado a arrancar el número tal" de vuelta.

Todo eso se pide en el panel de control 4, no con F1.

## Hablando de verdad

Mantener espacio abre el micrófono. Lo que dices se transcribe y después se interpreta según lo que está pidiendo, entre las pocas cosas que tienen sentido en ese momento —y el intérprete se niega en lugar de adivinar cuando no está seguro, que es la propiedad que más importa. Tiene que citar las palabras que justifican su interpretación, y esas palabras tienen que venir de ti y no de la pregunta que se le hizo.

El menú F1 sigue disponible en todo momento y no necesita nada instalado. Es perfectamente suficiente para volar.

---

**Anterior:** [Aterrizando](se-poser.md) · **Siguiente:** [Las checklists](checklists.md)
