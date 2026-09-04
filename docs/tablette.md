# La tableta

Alt T. Es el único sitio del juego donde algo se decide en lugar de accionarse —y lo que se decide ahí es lo que hace volar al avión.

Toda cabina tiene una hoy en día, y lo que sustituyó es la parte interesante. Calcular un despegue solía hacerse en el ordenador de gestión de vuelo, a través de una línea de anotación (scratchpad) y una tecla de página, y se hacía ahí por una razón que no tenía nada que ver con volar: el ordenador era el único con pantalla. El trabajo en sí —cuánto pesa, cuánto mide la pista, qué temperatura hace, por tanto cuánto motor hace falta— es aritmética sobre una hoja de carga.

## Las páginas

- **Plan de vuelo** — la salida, la llegada, y cada punto que queda por recorrer. Un punto se abre para dar su distancia, su rumbo y su aerovía, y para aceptar una restricción de altitud o velocidad, ser sustituido, o desaparecer. También se puede insertar un punto, o desviar.
- **Alternativos** — el aeródromo presentado en el plan de vuelo, calculado desde donde estás; un aeródromo por cada tramo de la ruta; y el que esté más cerca en este momento. Enter desvía.
- **Carga y combustible** — la hoja de carga, en qué estado está, y la acción que la acepta.
- **Rendimiento de despegue** — pista, temperatura, flaps, empuje, velocidades, la longitud requerida, y su envío al avión.
- **Rendimiento de aterrizaje** — velocidad de referencia y longitud de pista necesaria.

Cada línea de la página principal dice qué hay detrás en lugar de solo nombrarlo. El uso más habitual de una tableta en vuelo no es editar nada: es comprobar.

Las teclas son las del menú —flechas para moverse y para cambiar, mayús con las flechas para ir más rápido, Enter para tomar, Escape para volver una página. Todo lo demás pasa directamente al avión, y eso no es una cortesía: la tableta se abre en crucero con el piloto automático puesto, y una página que se tragara la palanca de gases sería una que nadie se atrevería a abrir en el aire.

## La hoja de carga, y en qué sentido corre la autoridad

Esta es la parte que se confunde con facilidad. Una tripulación no decide cuántos pasajeros van a bordo. El control de carga cuenta a quién se ha presentado de verdad, pesa lo que ha entrado de verdad en las bodegas, y emite una hoja de carga. La tripulación la lee, la comprueba contra lo que tiene, la acepta —el comandante la firma— y vuela el avión que esa hoja describe.

Por eso no puede llegar antes del embarque. Nadie conoce las cifras finales hasta que el último pasajero está sentado y las bodegas cerradas, así que la hoja llega al final de una rotación, unos minutos antes de la salida. Lo que existe antes es una estimación a partir de las reservas, y de ahí es de donde se calcula el rendimiento preliminar.

Así que la secuencia es:

1. Las cifras del plan de vuelo dan un rendimiento preliminar;
2. Se piden el embarque y el repostaje, y funcionan en paralelo;
3. Ambos terminan → llega la hoja de carga final, y tierra lo anuncia;
4. La tripulación la lee en la tableta y la acepta;
5. Las cifras de despegue, ya definitivas, se calculan y se envían al avión;
6. Puertas, empuje.

Hasta el paso 4, la página de despegue dice PRELIMINAR con esas mismas palabras. Después, "cifras definitivas, a partir de la hoja de carga aceptada." Aceptarla también invalida cualquier cosa ya enviada, porque unas cifras calculadas con una masa que nadie había firmado todavía son unas cifras que hay que calcular de nuevo —que es exactamente la comprobación cruzada que esta página existe para obligar a hacer.

## Cambios de última hora

La hoja definitiva se emite tan tarde que las cosas cambian después de ella. Una maleta que entra, un pasajero de última hora que embarca: en lugar de reemitirla, el cambio se escribe a mano sobre la hoja dentro de un margen —quinientos kilogramos aquí, unos seis pasajeros con su equipaje. La página dice "cambio de última hora de doscientos kilogramos", y las cifras dejan de ser definitivas hasta que se vuelve a aceptar.

Más allá de ese margen no es una hoja con una corrección encima: es la hoja equivocada. El control de carga la retira y envía otra, y la aceptación va con ella.

Y la asimetría es la honesta. Las adiciones después de terminar la carga ocurren ahí mismo; las reducciones no —volver a bajar a veinte personas no es algo que un plan pueda hacer. Recortar la carga planeada por debajo de lo que ya está a bordo, por tanto, no aligera el avión: hace que la hoja de carga no coincida con la cabina, y la página lo indica. No es un matiz de modelado. Un despegue calculado a partir de una masa sin combustible unas toneladas por debajo de la real da un flex demasiado alto y unas velocidades demasiado bajas, y el avión no acelera como prometía la hoja. Es una de las formas más comunes en que un cálculo de rendimiento real sale mal.

## Qué se bloquea, y cuándo

Las puertas son la línea —no los motores, y no los frenos.

- **Puertas abiertas, en un puesto:** la carga y el combustible se pueden editar, y aquí es donde se acepta la hoja. También las cifras de despegue y la ruta.
- **Puertas cerradas, en tierra:** la carga queda firmada. Las cifras de despegue y la ruta siguen siendo editables.
- **En el aire:** la carga está firmada, las cifras de despegue son de solo lectura, la ruta sigue siendo editable.

Una carga está en proceso de decidirse hasta que se cierran las puertas y queda firmada después; una tripulación que quiere una distinta está pidiendo que se vuelva a abrir el avión, no que se cambie una cifra. Un avión que nunca estuvo en un puesto se entregó ya cargado, así que está más allá de esa línea antes de empezar.

## Rendimiento de despegue

Esta es la página donde se concentra el oficio.

- **Pista** — cuál, y cuánta hay disponible.
- **Temperatura** — la de hoy, la real.
- **Flaps** — el escalón elegido.
- **Empuje** — flex y porcentaje. Las flechas lo recorren; Enter pide el mejor ajuste, que es la temperatura asumida más alta que todavía cabe en la pista.
- **Velocidades** — V1, rotación, V2.
- **Pista necesaria** — y cuánta sobra.
- **Enviar al avión.**

La temperatura asumida se calcula en grados enteros. Un avión al que se le dice que haga flex a 52,734 es uno que nadie podría briefear, y una temperatura de despegue se introduce, se repite y se briefea.

El ancla de todo el cálculo es esta: a la masa de referencia, empuje máximo y un día estándar a nivel del mar, la carrera en tierra calculada es la carrera en tierra publicada de la que se derivó. Todo lo demás es una desviación respecto a una cifra que un piloto puede reconocer.

El día cuenta doble, que es por qué "calor y altitud" es la trampa clásica y no simplemente "hace calor": un aire más enrarecido significa menos empuje y una velocidad verdadera mayor en la rotación, y las dos cosas se suman sobre una carrera que ya era la más larga del día.

## Rendimiento de aterrizaje

Velocidad de referencia, y la longitud de pista necesaria. Salen de la propia constante de frenado del modelo de vuelo y no de una tabla: una tableta que diera una distancia de aterrizaje sacada de una carta y después entregara el avión a un modelo que decelera a otro ritmo distinto le estaría diciendo al piloto una cifra que el avión no tiene ninguna intención de cumplir.

Desde la cabina, mayús 2 lee la carrera de aterrizaje sin abrir la tableta.

## Editando el plan en el aire

La ruta se puede editar hasta el final. Un replanteo toma los puntos desde aquí en adelante y reconstruye la ruta con los ya volados por delante de ellos —sin lo cual un plan reconstruido desde el principio giraría a un avión que va a medio camino de Bruselas de vuelta hacia el aeródromo del que salió. El controlador secuencia sobre el mismo navegador y recibe el nuevo plan, así que nunca se emite una autorización hacia un punto que ya no está en la ruta.

Alt D va directo a un punto sin abrir la tableta. Es una tecla propia porque una autorización directa llega cuando no hay tiempo de ir a buscar nada.

---

**Anterior:** [Los sistemas del avión](systemes.md) · **Siguiente:** [Glosario](glossaire.md)
