---
layout: page
title: Política de privacidad de Aftervoice
---

Última actualización: 10 de septiembre de 2026.

Aftervoice es un instrumento para sesiones de escucha. Esta política dice qué pasa con los
datos que la aplicación produce. Lo que genera se queda en el teléfono, salvo un informe que
elijas enviar expresamente.

## En resumen

Aftervoice no tiene cuentas, publicidad ni estadísticas de uso. Las grabaciones, la pista del
micrófono, el diario, las notas, los marcadores y los datos de sensores no se suben a nuestros
servidores. La red se usa para los bancos de voces gestionados por Google Play y, solo cuando
tú lo pides, para un informe de texto.

## Qué se queda en el teléfono

- **Los ajustes**: idioma de la interfaz, idioma de la voz, temporizador, búsqueda automática,
  filtro de ruido.
- **El diario de sesiones**: fecha, tiempo de escucha, la sintonía usada, el título y las notas
  que escribes tú, y los marcadores con el nombre que les das.
- **Las grabaciones**, cuando pulsas Grabar. Escucha de la habitación guarda solo el
  micrófono, incluidas las voces cercanas, sin emitir audio. Sintonía guarda el audio de la
  aplicación y, con permiso, el micrófono. Este puede captar también el altavoz: las pistas
  no están aisladas acústicamente.

Son archivos privados de la aplicación, en su propio almacenamiento. Ninguna otra aplicación
del teléfono puede leerlos. La aplicación queda fuera tanto de la copia de seguridad en la nube
como de la transferencia a un teléfono nuevo: si cambias de dispositivo, el diario no te sigue.

## Qué se queda en el teléfono

Las grabaciones, el micrófono, el diario, los ajustes, las notas, los marcadores y los datos de
sensores se quedan en el teléfono. No hay análisis, recogida de fallos, publicidad ni SDK de
rastreo. La aplicación solo contacta con Altrove Labs cuando pulsas **Enviar informe**.

Los informes de fallos que ve el autor llegan de Google Play, agregados y anónimos, y describen
cómo se comportó la aplicación, nunca qué contenían tus sesiones.

## Informes y asistencia

Si pulsas **Informar** en una grabación, escribes el motivo dentro de Aftervoice. Solo al pulsar
**Enviar informe**, la aplicación envía a Altrove Labs mediante HTTPS el texto, la versión, el
idioma de la interfaz y los identificadores aleatorios de sesión y grabación. No envía audio,
pista de micrófono, notas, marcadores, identificadores del dispositivo ni dirección de correo.

El servidor ve necesariamente la dirección IP de la conexión. Solo la usa en memoria para
limitar abusos a cinco informes por hora, no la registra y la olvida en una hora o al reiniciar.
El informe se reenvía como correo a `support@altrovelabs.net` y se conserva solo el tiempo
necesario para evaluarlo. El proveedor del servicio de correo solo lo trata para entregarlo a
Altrove Labs. La aplicación muestra una referencia aleatoria con la que puedes pedir su
eliminación. Los datos no se usan para otros fines.

## El permiso de micrófono

Aftervoice pide un solo permiso, **el micrófono**, y lo usa en dos sitios:

- **Durante una grabación**, para guardar la habitación sola o junto a la pista sintética
  en Sintonía. El micrófono se abre al pulsar Grabar y se cierra al terminar, también cuando
  la aplicación pasa a segundo plano.
- **En el sónar**, donde el sonido recogido se filtra por encima de 17 kHz dentro de la
  aplicación antes de cualquier procesamiento, no se graba y no se conserva. El micrófono sigue
  abierto sólo mientras esa pantalla está abierta.

Si rechazas el permiso, Escucha de la habitación no graba y explica cómo permitir el acceso.
No activa la síntesis como alternativa. Sintonía puede grabar solo el audio de la aplicación
y lo indica explícitamente. El sonar requiere acceso al micrófono.

## Cuánto duran los datos y cómo se borran

Duran hasta que los borres. Puedes eliminar una grabación concreta o una sesión entera desde el
archivo, con confirmación. Desinstalar la aplicación lo elimina todo: ajustes, diario y
grabaciones.

## Menores

Aftervoice no está dirigida a menores de 13 años ni recoge deliberadamente datos sobre ellos.

## El audio que genera la aplicación

Los sonidos que hace Aftervoice los genera un modelo de voz que se ejecuta en el teléfono. No
son grabaciones de personas reales y no son prueba de nada.

El audio que produce la aplicación lleva una marca legible por una máquina que lo declara
sintético, como exige el artículo 50 del reglamento europeo de inteligencia artificial. La
marca está en el sonido mismo, no en una etiqueta del archivo: sobrevive a compartirlo, a
recomprimirlo y a un recorte, y sigue ahí en un archivo renombrado o reexportado. Cualquiera
puede verificarla, sin pedirnos nada, con el detector descrito en
[Verificar la marca](../detector.html).

La marca no contiene nada tuyo: no hay identificador del teléfono, ni de la sesión, ni de la
instalación. Dice una sola cosa, siempre la misma: este audio lo hizo una máquina. La pista de
micrófono de una grabación no está marcada, porque no es audio generado — es la habitación en
la que estabas.

## Contacto

Para preguntas sobre esta política: [support@altrovelabs.net](mailto:support@altrovelabs.net).

Responsable del tratamiento: **Altrove Labs**. Los datos del diario y las grabaciones permanecen
en tu poder y bajo tu control, en tu teléfono. Solo tratamos los informes y comunicaciones que
decides enviar; puedes ejercer tus derechos del RGPD escribiendo a la dirección anterior e
indicando, para un informe anónimo, su referencia.

## Cambios

Si esta política cambia, la fecha de arriba cambia con ella, y la versión anterior queda en el
historial público del repositorio del sitio.
