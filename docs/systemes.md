# Los sistemas del avión

Un avión de línea no se enciende sin más: se despierta siguiendo un orden, y cada paso existe porque el siguiente depende de él. Esta página explica por qué, sistema a sistema. Se aplica a la familia A320 —A318, A319, A320, A321 y sus variantes neo— cuya cabina está descrita panel por panel y cuyos procedimientos están escritos. Todos comparten la misma cabina de mando, que es la razón de ser de la familia y por qué una única habilitación de tipo los cubre a todos. El neo cambia los motores, no los interruptores.

Lo que se describe aquí es lo que modela el juego. Donde simplifica un panel real, se dice: aprender una dependencia inventada es tan fácil como aprender una real, y mucho más difícil de desaprender.

## La electricidad, que va antes que todo

Nada funciona sin alimentación, y hay cuatro formas de tenerla.

**Las baterías.** Dos, y duran unos minutos —no una rotación entera. Bastan para despertar la cabina y arrancar el APU, que es exactamente lo que se les pide. Control mayús 2 y después B lee la batería 1 y N la batería 2; cada una tiene dos posiciones, apagado y automático.

Solo con baterías y en tierra, es el inversor estático el que genera la corriente alterna, y necesita ambas: esa es la razón por la que hay dos que modelar.

**El grupo de tierra.** Un carro conectado al vientre del avión, que suministra electricidad y nada más. Control mayús 2 y después mayús E lo conecta. Hay que desconectarlo antes del push-back —un cable todavía enchufado a un avión que retrocede es un cable arrancado, y la checklist previa al arranque te lo dirá con esas palabras.

**El APU.** Ver más abajo. Es la respuesta cuando no hay grupo de tierra, que es a menudo.

**Los generadores de motor.** Una vez en marcha los motores alimentan el avión, y ese es el momento en que se apaga el APU. En el mismo panel, G lee el generador 1, H el generador 2 y A el generador del APU.

## El APU

Un tercer motor pequeño en la cola. No empuja nada: genera electricidad y aire comprimido.

Arranca solo con baterías y alimenta a todo el avión. Sobre todo, suministra el aire comprimido que hace girar los motores grandes al arrancar. Es ese zumbido agudo y continuo que se oye en cualquier vídeo de un avión estacionado.

Su panel es control mayús 3, y arrancarlo son dos acciones, como en el avión real: mayús M conecta el master, que abre la válvula de combustible de baja presión y la trampilla de admisión; mayús S ejecuta la secuencia, unos veinte segundos. M y S los leen, control M y control S los desconectan. Se niega si no hay alimentación o no hay combustible.

Y tiene un elemento aparte, en el mismo panel: el sangrado.

## El sangrado (bleed), y por qué se abre y después se cierra

Un "sangrado" es aire tomado de un compresor —caliente, y a presión. La misma tubería sirve para tres cosas completamente distintas: hacer girar un motor de arranque, alimentar los packs, y el antihielo.

En el panel del APU, B lee su sangrado, mayús B lo abre, control B lo cierra —y vuelve a aparecer en el panel de aire acondicionado, control mayús 4, en A, porque ahí es donde se compara con los sangrados de los motores.

El orden de las acciones se deriva enteramente de esto:

- **Antes del arranque**, el sangrado del APU tiene que estar abierto. Si no, nada manda aire al motor de arranque y el motor no girará. La checklist lo dice exactamente así: "el grupo auxiliar de potencia está en marcha pero su sangrado está cerrado. Nada hará girar el motor."
- **Después del arranque**, se cierra de nuevo. Los motores ya toman su propio aire, y no queda ninguna razón para hacer trabajar al APU.

También hay dos carros en tierra, y son máquinas distintas: el carro de climatización (control 4 y después mayús A) es de baja presión y mantiene habitable una cabina; el carro de arranque (control 4 y después mayús S) es de alta presión y hace girar un motor de arranque. Pedir el equivocado en un aeródromo caluroso y de altitud es un error real, y el avión te deja cometerlo.

## Los packs

Son las máquinas que acondicionan el aire: toman el aire caliente y a presión del sangrado y lo convierten en aire respirable a la temperatura correcta. Control mayús 4 y después P lee el pack 1 y L el pack 2; mayús los enciende, control los apaga. El mismo panel lleva los sangrados: E para el motor 1, R para el motor 2, A para el APU.

Algo que el juego modela bien: el caudal cae a cero durante un arranque de motor. Todo el aire disponible va al motor de arranque, y la cabina se queda sin él durante veinte segundos. Se puede oír, y es la razón real por la que un avión se queda de repente en silencio en el momento en que se arranca un motor.

El grupo de tierra solo suministra electricidad: los packs entonces no tienen nada que acondicionar hasta que algo les manda aire —el sangrado del APU, un carro, o un motor.

## Las bombas de combustible

Control mayús 7, y el panel es el del avión: seis bombas, dos por depósito —Q y W a la izquierda, E y R en el centro, T y Y a la derecha. X es el trasvase (crossfeed) entre las alas, y M el selector de modo, que decide si el depósito central se vacía por sí solo: mayús M fija automático, control M manual.

El combustible se cuenta en kilogramos, nunca en litros. Lo que hace volar a un avión es la masa de energía que lleva, y el volumen de un litro de queroseno cambia con la temperatura: el mismo repostaje, medido en litros, no es la misma energía a veinte bajo cero que a treinta y cinco grados. La masa es lo que le importa a todo el mundo a bordo de todos modos —entra en la velocidad de despegue, en la longitud de pista, en la altitud alcanzable. Los litros son cosa del camión.

## La hidráulica

Control mayús 6. Tres sistemas en el A320 —verde, azul y amarillo— y son los que accionan los mandos de vuelo, el tren y los frenos. E y R leen las bombas de los motores 1 y 2, B la bomba eléctrica azul, Y la amarilla, y P la unidad de transferencia de potencia: la máquina que permite que un sistema mueva a otro sin intercambiar nada de fluido entre ellos, y que ladra de forma muy reconocible durante un push-back.

La checklist de después del arranque comprueba que ningún sistema se ha caído y que no se ha dejado ninguna bomba apagada.

## Las centrales inerciales

Este es el sistema más interesante del avión, y el único cuya espera no se puede acortar.

El avión no sabe dónde está ni hacia dónde apunta, y nada de fuera se lo dice. Tres plataformas inmóviles sienten a la Tierra girar debajo de ellas y deducen el norte a partir de eso. Tarda unos minutos, no se puede acelerar, y cuanto más lejos del ecuador más tarda: lo que miden es la componente horizontal de la rotación terrestre, y esa componente se reduce con la latitud. Más allá de unos setenta y tres grados, simplemente se niegan —ya no hay suficiente señal.

Control mayús 1, y hay de verdad tres selectores, uno por central: U para la primera, I para la segunda, O para la tercera. Mayús mueve un selector un escalón hacia arriba, control hacia abajo, y cada uno tiene tres posiciones:

- **apagado**;
- **nav** — el modo normal, el que espera la checklist. La alineación empieza pasando por él, y nada puede saltarse la espera;
- **actitud** — lo que queda cuando se pierde una alineación en vuelo: el avión sabe cómo está orientado, pero ya no dónde está.

Es el primer punto de la primera checklist, y por eso es el primero: arranca la alineación en cuanto el avión tiene alimentación, y haz todo lo demás mientras funciona.

## La altimetría

Un altímetro es un barómetro. Pesa el aire que tiene encima y calcula una altura, lo cual significa que hay que decirle qué presión hay hoy al nivel del mar.

Ese ajuste —el QNH— viene del controlador, a la salida y a la llegada. Todo el mundo ajusta el mismo, así que todo el mundo mide desde la misma superficie, y eso es lo que hace que un avión notificado a tres mil pies pase realmente mil pies por encima de otro a dos mil.

Control 7 y después B lee la subescala, mayús B y control B la mueven un hectopascal cada vez, Q fija el estándar, 1013.

Un hectopascal son veintisiete pies. Un ajuste desviado en cuatro pone al instrumento a cien pies de la realidad, que es más que todo el margen de una aproximación —por eso la confirmación te dice cuánto te has desviado en cuanto merece la pena decirlo.

Por encima de la altitud de transición todo el mundo cambia a estándar y habla en niveles de vuelo: lo que importa ahí arriba no es la altura sobre el suelo, es la separación con el avión de al lado. La altitud de transición pertenece al aeródromo y es fija —tres mil pies en Schiphol, cinco mil en Francia, dieciocho mil en el Reino Unido. El nivel de transición depende además de la presión del día, por lo que no se puede imprimir en una carta: se te da por radio.

El avión te pide estándar al pasar la transición en el ascenso, y te devuelve la presión de llegada al pasarla en el descenso —pero solo si el ordenador de a bordo está encendido, porque esa cifra es la que nadie puede calcular solo.

## Los motores

Control 6 y después E lee cada motor, T las temperaturas de escape, y G le dice al personal de tierra que estás arrancando.

Un arranque son dos acciones porque son dos en el avión: mayús M sube el selector de modo a ignición/arranque, después mayús A conecta el master del motor uno o mayús Z el del motor dos. M, A y Z los leen; control los baja o los corta.

### Qué motor primero

Ningún avión impone un orden, y los órdenes publicados se contradicen entre sí: un 727 arranca 3-1-2 donde un MD-11 arranca 1-2-3. Lo que hace el piloto es elegir y después anunciarlo.

En lo que sí coinciden los órdenes publicados no es el avión: son las personas que están debajo. El interfono, la trampilla del tren de morro y la pasarela están a la izquierda —así que el lado derecho arranca primero, y el personal sigue trabajando a la izquierda de un avión que aún está en silencio.

En un ala que lleva dos motores, va antes el interior que el exterior, porque un bombero enviado al motor interior tendría que pasar por delante de uno exterior en marcha para llegar hasta él. Ambas reglas apuntan en el mismo sentido. Dos motores dan 2 y después 1; cuatro dan 3, 4, 2, 1.

### El sonido se construye, no se reproduce

Cada motor se sintetiza en tiempo real a partir de las cifras que publica su fabricante: el número de palas del fan y la velocidad del eje dan el tono que se reconoce como un reactor; el diámetro del fan decide cuándo las puntas se vuelven supersónicas y aparece el "buzzsaw"; la relación de derivación (bypass) decide si suena suave o áspero; y un motor de tres ejes lleva una línea grave que uno de dos ejes no tiene.

Eso significa tres cosas en la práctica: sin bucles ni costuras; un arranque que nunca termina antes que el motor; y un motor que nadie ha grabado jamás se puede volar igualmente. Es también la razón por la que la flota crece despacio —añadir un avión es medir una máquina, no soltar tres archivos de sonido en una carpeta.

Ve a escuchar desde el ala durante un arranque: mayús V. Lo que se come el mamparo de la cabina de mando es considerable.

## El empuje

Av Pág y Re Pág abren y cierran la palanca de gases, mayús con la tecla un diez por ciento, Inicio es máximo y Fin ralentí. Mayús Inicio da empuje máximo, cancelando cualquier reducción —eso es lo que se pulsa para un motor y al aire.

Un turbofán está "flat rated": por debajo de una temperatura de corte se contiene deliberadamente hasta el empuje certificado. Eso es lo que hace posible un despegue con empuje reducido, explicado en *Despegando*.

Control 6 y después R selecciona los inversores. El antihielo está aparte, en su propio panel —control mayús 5: W para el ala, E y R para los dos motores, P para la calefacción de sondas.

## El transpondedor

Responde a las interrogaciones del radar con un código de cuatro dígitos y tu altitud. Sin él no existes en la pantalla de un controlador —la checklist previa al despegue lo dice así: "el transpondedor está apagado. Nadie puede verte."

El controlador te da un código con tu autorización. Control 3 y después A lo pone directamente; G, H, J y K trabajan los cuatro dígitos uno a uno, en el orden en que se leen. Mayús X cambia entre espera y respondiendo.

## Lo que simplifica el juego, y por qué se dice

La cabina de la familia A320 está descrita panel por panel, con el número real de mandos: seis bombas de combustible y no una, dos packs y no uno, tres selectores inerciales de tres posiciones y no un botón, dos masters de motor detrás de un selector de modo. Eso es lo que permite que una página de ayuda nombre un interruptor por el nombre que lleva en el avión.

Todavía no es el panel completo —quedan pulsadores que solo importan en un fallo, y los selectores de temperatura. Donde el juego simplifica, se dice en lugar de ocultarlo, por una razón de fondo: lo que afirma un simulador se convierte en lo que cree el alumno. Un simulador puede permitirse una aproximación mientras nadie la ponga en palabras; una página de ayuda no. Cuando se abre un manual de A320, deberían encontrarse ahí las propias palabras y las propias acciones.

Y los aviones cuyas cabinas no se han descrito conservan la disposición genérica del juego, que es más sencilla y menos fiel —un solo control donde el avión tiene seis. Ver *Los paneles*.

---

**Anterior:** [Los paneles](panneaux.md) · **Siguiente:** [La tableta](tablette.md)
