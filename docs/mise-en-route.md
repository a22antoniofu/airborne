# Arrancando

Un avión de línea no se enciende sin más. Se despierta siguiendo un orden, y ese orden no es una convención: cada paso existe porque el siguiente depende de él.

La batería alimenta el avión. La batería arranca el APU. El APU suministra el aire que hace girar el primer motor. Y solo entonces los generadores de los motores toman el relevo, que es lo que permite apagar el APU.

Esa es toda la cadena. El resto de esta página es su detalle. Es lo que convierte el arranque en un procedimiento que merece la pena aprender, y no en un interruptor que se acciona.

Cuenta con unos veinte minutos. Eso es lo que dura de verdad una rotación, y es deliberado: no se embarca a ciento cincuenta personas en treinta segundos. Si solo quieres volar, la situación de partida "fuera del puesto, listo para rodar" te da exactamente el mismo avión con todo esto ya hecho.

Las teclas de abajo son las de la familia A320 —A318, A319, A320, A321 y sus variantes neo, que comparten una única cabina de mando. En un avión cuya cabina no se ha descrito, los paneles no llevan los mismos números; ver *Los paneles*, o preguntar con alt H.

## Lo que te encuentras al llegar

El avión está tal como lo dejó el vuelo anterior: cabina vacía, bodegas vacías, y solo las reservas en los depósitos. Ese es todo el sentido de empezar desde un puesto de estacionamiento. Una cifra de combustible de bloque y un factor de ocupación elegidos en un menú son decisiones que no cuestan nada, y una decisión que no cuesta nada no es una decisión. Aquí cuestan lo que realmente cuestan: minutos.

### 1. Alimentación

Nada funciona sin electricidad, y esta es la única acción que no tiene ninguna condición previa.

**Control mayús 2**, después **mayús B** y **mayús N**: las dos baterías a automático.

Dos, no una: en tierra y solo con baterías es el inversor estático el que genera la corriente alterna, y necesita ambas. Esa es la razón por la que hay dos que modelar.

Las baterías duran unos minutos —no una rotación entera. Están ahí para despertar la cabina y arrancar el APU, que es exactamente lo que se les pide. Si el aeródromo tiene grupo de tierra, mayús E lo conecta, y pasas a una fuente que no se agota.

El grupo de tierra da electricidad y nada más. No sustituye al APU al arrancar, porque lo que hace girar un motor no es corriente: es aire.

### 2. La alineación, desde el principio

Esta es la primera acción útil porque es la más larga, y porque nada puede acelerarla.

**Control mayús 1**, después **mayús U**, **mayús I** y **mayús O**: las tres centrales inerciales un paso, de apagado a navegación.

El avión no sabe dónde está ni hacia dónde apunta, y nada de fuera se lo dice. Tres plataformas inmóviles sienten a la Tierra girar debajo de ellas y deducen el norte a partir de eso. Tarda unos minutos, no se puede acortar, y cuanto más lejos estás del ecuador más tarda: lo que miden es la parte horizontal de la rotación terrestre, y esa parte se reduce con la latitud. Más allá de unos setenta y tres grados, se niegan — ya no hay suficiente señal.

Arráncala ahora y haz todo lo demás mientras funciona. Es también el primer punto de la primera checklist, y por eso es el primero.

### 3. El APU

**Control mayús 3**, y son dos acciones porque son dos en el avión:

- **Mayús M** — el master. Abre la válvula de combustible de baja presión y la trampilla de admisión.
- **Mayús S** — el arranque. Unos veinte segundos.

Pulsa el arranque sin el master y el avión te lo dice: "el interruptor master del APU está desconectado. No pasa nada."

El APU es un tercer motor pequeño en la cola. No empuja nada: genera electricidad y aire comprimido. Es ese zumbido agudo y continuo que se oye en cualquier vídeo de un avión estacionado, y es lo que va a hacer girar tus motores.

Después, en el mismo panel, mayús B abre su sangrado (bleed). Sin él el aire se queda en el APU y no llega nada al motor de arranque. La checklist lo dice con estas palabras: "el grupo auxiliar de potencia está en marcha pero su sangrado está cerrado. Nada hará girar el motor."

### 4. Combustible, en las tuberías

**Control mayús 7**: seis bombas, dos por depósito. Mayús Q y mayús W para el depósito izquierdo, mayús E y mayús R para el central, mayús T y mayús Y para el derecho.

Tener combustible en los depósitos y ninguna bomba en marcha es un caso distinto de no tener nada, y el avión los distingue: "hay combustible en los depósitos y ninguna bomba en marcha para llevarlo al motor."

### 5. La checklist de preparación de cabina

Alt C, después alt Enter para cada punto.

Comprueba lo que acabas de hacer, y se niega a avanzar hasta que sea cierto —diciendo qué falta en lugar de repetir la pregunta. "No hay alimentación eléctrica en el avión." "Solo con batería. Conecta el grupo de tierra o arranca el grupo auxiliar de potencia." "Las centrales inerciales todavía se están alineando." "El altímetro no tiene ajuste."

Este es el momento de fijar la subescala: control 7, después mayús B y control B hasta el valor que te acaba de dar el ATIS.

### 6. Combustible y pasajeros, en paralelo

**Control 4**, el panel de servicios de tierra. Dos servicios independientes, solicitados por separado, que funcionan al mismo tiempo porque así es como trabaja una rotación:

- **Mayús F** llama al camión de combustible. Tres minutos en llegar y minuto y medio en conectar, después bombea. Ocho toneladas tardan unos siete minutos.
- **Mayús B** llama a la pasarela y a los pasajeros. Dos minutos para la pasarela, después once pasajeros por minuto: ciento cincuenta personas son catorce minutos.

F y B leen cuánto ha avanzado cada uno, y T anuncia toda la rotación de una vez.

Un puesto remoto, atendido por autobús en lugar de pasarela, es más lento en ambos aspectos. Un fuselaje ancho, en cambio, no es diez veces más lento que uno estrecho: se reposta por varios puntos a la vez, y el caudal sigue el tamaño de los depósitos y no el número de asientos — lo que estás llenando son los depósitos.

El camión reposta según el indicador, no según un total. El APU consume mientras se bombea, y un servicio que contara su propio total te dejaría corto exactamente en lo que el APU hubiera quemado.

Y la masa se actualiza de forma continua — no la masa planeada, la que realmente está a bordo. Tus velocidades de despegue, tu velocidad de pérdida y tu equilibrado se mueven durante el embarque, exactamente como en la realidad.

### 7. La radio, mientras tanto

Nada de lo anterior necesita la radio, lo cual hace que este sea el momento adecuado para usarla.

Escucha el ATIS: pista en uso, viento, QNH, nivel de transición. Después F1, y pide a la entrega de autorizaciones tu clearance — obtienes la ruta a tu destino, la pista de salida, un código de transpondedor, e instrucciones para contactar con tierra.

Control 3 y después A pone el código de transpondedor que te acaban de dar.

Todo el ciclo de la radio tiene su propia página: *La radio*.

### 8. La hoja de carga

No puede llegar antes. Una tripulación no decide cuántos pasajeros van a bordo: el control de carga cuenta a quién se ha presentado, pesa lo que ha entrado en las bodegas, y emite la hoja. Nadie conoce las cifras finales hasta que el último pasajero está sentado y las bodegas cerradas.

Así que: terminados ambos servicios, llega la hoja, y tierra lo anuncia.

Alt T, la página de carga y combustible, la lees y la aceptas. Después la página de rendimiento de despegue recalcula tus velocidades y tu empuje —esta vez definitivos— y los envías al avión. Hasta que se acepta la hoja, esa página dice PRELIMINAR con esas mismas palabras.

Ver *La tableta* para lo que realmente se decide ahí.

### 9. La baliza, después las puertas

**Control mayús 8**, después **mayús B**: la baliza anticolisión.

Se enciende antes de que gire nada, y le dice una cosa a todo el que trabaja alrededor del avión: no te acerques, algo está a punto de arrancar. La checklist previa al arranque es explícita — "la baliza está apagada. Nadie fuera sabe que estás a punto de arrancar."

Después control 4 y control B cierra las puertas.

Cerrar antes de que termine el embarque deja fuera a quien todavía esté en el autobús, y el avión lo indica. Es la única forma de salir de un embarque que de otro modo tendrías que esperar hasta el final — una decisión del comandante, no un botón de cancelar.

Las puertas son la línea: una vez cerradas, la carga queda firmada. Una tripulación que quiera una distinta está pidiendo que se vuelva a abrir el avión.

Y desconecta el grupo de tierra si lo había: control mayús 2 después control E. Un cable todavía enchufado a un avión que está retrocediendo es un cable arrancado.

### 10. El push-back

Hacen falta dos autorizaciones, y eso no es burocracia. El control de tierra es dueño de la calle de rodaje detrás de tu puesto y no tiene ni idea de si la pasarela sigue puesta; el personal de tierra es dueño del avión y no puede ponerlo en una calle de rodaje para la que nadie lo ha autorizado.

- **F1** — pide al controlador el push-back y el arranque. Obtienes la aprobación y el rumbo con el que te dejarán orientado.
- **Control 4** después **mayús P** — llama al remolcador.

Después oirás al mecánico por el interfono, que no está en la frecuencia y tiene su propia voz: la barra puesta, el pasador, "confirme frenos sueltos", el empuje empezando, "push-back completado, confirme frenos puestos", el pasador retirado, el remolcador despejado.

Después, sin que lo pidas: "motores despejados." La cabina no puede ver sus propios motores y el personal de tierra sí. Hasta que se diga eso, arrancar significa arrancar sobre alguien.

Cuatro a cinco minutos, al paso del mecánico que camina a tu lado — que es lo que limita toda la operación.

### 11. Arrancando los motores

**Control 6**, y de nuevo dos acciones, porque son dos en el avión:

- **Mayús M** — el selector de modo de motor a ignición/arranque. Sin eso no pasa nada, y el avión te lo dice.
- **Mayús Z** — el master del motor dos. Después, una vez en marcha, mayús A para el motor uno.

G le dice al personal de tierra que estás arrancando; es la fraseología real, "arrancando el número dos", y obtienes una respuesta.

### Por qué el número dos primero

Ningún avión impone un orden, y los órdenes publicados se contradicen entre sí de un modelo a otro. En lo que coinciden no es el avión: son las personas que están debajo. El interfono, la trampilla del tren de morro y la pasarela están a la izquierda — así que el lado derecho arranca primero, y el personal sigue trabajando a la izquierda de un avión que aún está en silencio.

En un ala que lleva dos motores, va antes el interior que el exterior: un bombero enviado al motor interior tendría que caminar por delante de uno exterior en marcha para llegar hasta él. Ambas reglas apuntan en el mismo sentido. Dos motores dan 2 y después 1; cuatro dan 3, 4, 2, 1.

### Lo que oyes, y dónde oírlo

El arranque no es una muestra grabada: el sonido se construye en tiempo real a partir de las cifras propias del fabricante, así que nunca termina antes que el motor. El caudal de los packs cae a cero durante la secuencia —todo el aire va al motor de arranque—, que es la razón real por la que una cabina de pasajeros se queda de repente en silencio en ese momento.

Mayús V te lleva fuera, a la plataforma. Lo que se come el mamparo de la cabina de mando es considerable, y un arranque es lo que más merece la pena escuchar desde ahí fuera.

### 12. Después del arranque

Alt C: la checklist "después del arranque", que es la que cierra la cadena.

- El sangrado del APU se cierra — control mayús 3 después control B. Los motores ya toman su propio aire; no queda razón para hacer trabajar al APU.
- El APU se apaga — control M. Los generadores de los motores alimentan el avión.
- Los packs se conectan de nuevo — control mayús 4, mayús P y mayús L.
- Se comprueba la hidráulica — control mayús 6. Tres sistemas, y las dos bombas de motor que acaban de despertarse con ellos.
- El trim dentro de la banda de despegue — control 1, T para leerlo.
- Las tres centrales inerciales en navegación. Si no lo están, todavía se están alineando, y no queda más que esperar.

### 13. Listo para rodar

Pide rodaje: F1. Obtienes una ruta por las calles de rodaje e instrucciones de esperar antes de la pista.

A partir de ahí, todo está en *Rodando*.

## Si el motor se niega a arrancar

El avión nunca dice simplemente que no. Cada uno de estos rechazos nombra un paso que te has saltado, y todos están en esta página:

- "No hay alimentación eléctrica en el avión." — Paso 1.
- "El interruptor master del APU está desconectado. No pasa nada." — Paso 3, la primera de las dos acciones.
- "Nada puede hacer girar el motor." — No hay aire: el sangrado del APU está cerrado, o el APU está apagado, y no hay ningún otro motor en marcha del que sangrar aire.
- "Hay combustible en los depósitos y ninguna bomba en marcha para llevarlo al motor." — Paso 4.
- "Sin combustible." — Los depósitos están secos; llama al camión.
- "El selector de modo de motor no está en ignición/arranque." — Paso 11, la primera de las dos acciones.
- "Este avión no tiene grupo auxiliar de potencia." — No todos los modelos llevan uno. Entonces necesitas un carro de arranque: control 4 después mayús S.
- "Hay aire, y no el suficiente." — El caso de calor y altitud, que es un problema distinto de no tener ninguna fuente y tiene una respuesta distinta: un motor ya en marcha, o un carro de arranque. Está formulado de otra manera a propósito, porque un piloto que oye "sin aire" recurre al APU, y el APU ya está encendido.
- "El carro es un cable hasta el morro: el avión tiene que estar parado." — Un carro de arranque no es algo que se pida mientras se rueda.

---

**Anterior:** [Preguntando al avión](instruments.md) · **Siguiente:** [Rodando](rouler.md)
