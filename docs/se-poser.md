# Aterrizando

Un piloto que no puede ver el aeródromo no puede volar un circuito visual. Lo que sí puede hacer es mantener un rumbo y una altitud —y eso es exactamente lo que pide un controlador de radar. Toda la llegada está construida sobre eso.

## Vectores: dos números cada vez

Pide vectores y el controlador te trae hacia el localizador tramo a tramo: un rumbo, una altitud, después el siguiente. Tu trabajo se reduce a dos números cada vez, hasta que te dicen que estás lo bastante cerca para interceptar.

Nada de esto es una secuencia que seguir en orden. En cada llamada el controlador mira dónde está realmente el avión y dice lo que es cierto en ese momento. Un piloto que ignora un vector, que se pasa o que llega desde una dirección inesperada simplemente recibe más vectores —no una máquina bloqueada. Un avión que ha sobrevolado el aeródromo se gira de vuelta hacia la puerta de entrada, no se pone en el rumbo de pista, que lo alejaría para siempre.

En el descenso y la aproximación, llega un vector nuevo cada dieciocho segundos si no pides nada: un tramo de aproximación dura uno o dos minutos, y un rumbo que llega después del giro no vale nada.

## El ILS

Pide la aproximación y te autorizan: "autorizado ILS pista tal, informe establecido."

Control 2 y después mayús I arma la aproximación. I lee las agujas. Una vez establecido, infórmalo, y te transfieren a la torre.

Y desde ese momento el controlador queda en silencio. Eso no es un descuido: interceptar y seguir el localizador es trabajo del piloto, no del radar. Es el único estado del vuelo en el que esa frecuencia deja de decir nada, y es la razón por la que un motor y al aire tiene que cancelar primero la autorización —sin lo cual un avión que hace motor y al aire ascendería alejándose de una pista que ya no está usando, en silencio, indefinidamente.

## La espera, cuando no estás listo

Una espera es una autorización para quedarte donde estás, y es lo único que dice un controlador que no te acerca a la pista. Se pide una cuando vas demasiado alto, demasiado rápido, o retrasado con una checklist. La alternativa es llegar al umbral en ese estado.

El patrón es un circuito hipódromo sobre un punto: un tramo hacia el punto, un giro de tasa uno —tres grados por segundo, así que ciento ochenta grados en un minuto—, un tramo de alejamiento, y un segundo giro. La anchura no es una cuestión de estilo: es lo que cuestan los dos giros, poco menos de cuatro kilómetros a velocidad de aproximación. Los tramos se vuelan a una distancia y no a un cronómetro, cinco millas desde el punto.

Una espera que has pedido no termina sola. Se sale de ella cuando pides la aproximación.

## La pila de espera (stack)

Una cuarta parte de las llegadas se encuentran a alguien por delante. El controlador entonces no te da vectores en círculos hasta que se abra un hueco: te apila. Cada avión entra mil pies por encima del anterior, y la pila se vacía desde abajo —el que está abajo del todo va a la aproximación, y todos los demás bajan un piso.

Aquí es un piso por vuelta del circuito: cada vez que pasas por el punto, un nivel menos, y el número de giros que te quedan es el número de aviones que tienes por delante. La autorización te dice las dos cosas que decide una tripulación —el retraso previsto y cuántos hay delante.

En el fondo de la pila te sacan; no tienes que pedirlo. La salida ocurre en el giro de alejamiento de vuelta hacia el tramo de aproximación en lugar de sobre el punto, lo cual te deja todo el tramo de aproximación para interceptar.

## El motor y al aire (go-around)

Tres cosas tienen que ser ciertas en orden, y el orden es el procedimiento.

1. **Asciende recto al frente primero.** El terreno delante de una pista está estudiado y el de al lado no. Esa es la única razón, y basta.
2. **Después sal del eje.** El eje de pista prolongado es donde está todo lo que viene detrás: un avión que asciende por él está cruzando toda la cola. El giro se hace hacia el viento en cola (downwind).
3. **Y solo entonces reincorpórate.** Una vez despejado y lo bastante lejos, los vectores normales se retoman solos y te traen de vuelta a la puerta.

Mayús Inicio da empuje máximo, cancelando cualquier flex. La torre te devuelve al radar en el mismo momento: el negocio de una torre es una pista, y un avión que no va a aterrizar en ella no tiene nada más que hacer ahí.

## La derrotación, y lo que sigue

Esta es la parte que el juego deja enteramente en tus manos, y merece la pena practicarla por sí misma: la situación de partida "en el punto de toma de contacto" te entrega un avión a trescientos metros pasado el umbral, a la velocidad de referencia, con el morro todavía alto y los aerofrenos desplegados.

La derrotación se vuela. El morro se queda donde lo dejó el flare; es Enter —que centra los mandos, no mayús Enter, que fija la actitud de vuelo nivelado— o la flecha arriba lo que lo baja.

El frenado depende del peso sobre las ruedas, y es lo menos intuitivo de todo el aterrizaje. Un ala a la velocidad de referencia con el morro alto todavía sostiene casi todo el avión: las ruedas no cargan nada, y los frenos no tienen de qué agarrarse. Morro a cinco grados sin aerofrenos, la carga es una cuarta parte de lo que sería; con los aerofrenos fuera, casi toda; morro a cero, toda. Veinte segundos de frenado son cincuenta kilómetros por hora de diferencia entre esos casos —en una pista, eso es una salida o la hierba.

Así que, en orden: baja el morro, después frena.

Corregir el derrape (decrabbing) no es automático, y se puede oír. En tierra el avión va adonde apunta: tomar contacto con cinco grados torcido significa salirse de lado a cinco grados. Nada lo corrige por ti. En la toma de contacto el avión anuncia el error en cuanto supera los tres grados —"tres grados a la derecha del eje"— porque un piloto que no puede ver hacia fuera no tiene otra forma de saberlo. Cinco segundos después, si el morro sigue alto, también lo dice.

V frena, mantenida. Control 6 y después R selecciona los inversores. Control 1 y después control S retrae los aerofrenos una vez detenido.

## Saliendo de la pista

El avión anuncia cada salida a medida que se vuelve tomable, una vez por salida, y de nuevo si una más cercana se vuelve tomable a medida que baja la velocidad. Tab toma la que se acaba de anunciar.

El ángulo decide la velocidad: cincuenta nudos para una salida a treinta grados, quince para una en ángulo recto. Es un máximo y no una instrucción —el frenado que te lleva hasta ahí ocurre en la pista, antes de la salida.

El detalle de rodar hasta el puesto, y la tecla que responde a "dónde estoy", están en *Rodando*.

## Después, la radio, y la checklist

Informa que has dejado libre la pista y te transfieren a tierra, que te da una ruta hasta el puesto. Informa que estás parado, y te desean buen vuelo.

Quedan dos checklists: después del aterrizaje y de estacionamiento. Alt C.

---

**Anterior:** [Volando y navegando](naviguer.md) · **Siguiente:** [La radio](radio.md)
