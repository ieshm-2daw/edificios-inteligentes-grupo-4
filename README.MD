# Control de Dispositivos con Home Assistant y TUYA

## Lo que hemos conseguido:

Este proyecto permite integrar y automatizar dispositivos inteligentes utilizando **Home Assistant** y **TUYA**. Con esta configuración, se logra:
- Controlar la televisión, el aire acondicionado y la corriente eléctrica mediante un relé WiFi.
- Vincular dispositivos a Home Assistant a través de la integración de TUYA.
- Configurar automatizaciones para encender y apagar dispositivos según la detección de movimiento.
- Crear escenas en la aplicación TUYA para realizar múltiples acciones con un solo evento.

## Instalación y Configuración Inicial

En primer lugar, debemos descargar la aplicación **Smart Life**, mediante la cual controlaremos los distintos dispositivos asociados. Luego, crearemos una cuenta y emparejaremos los dispositivos con la aplicación.

El emparejamiento es sencillo:
1. Pulsar durante **5 segundos** el botón de los sensores a emparejar (en este caso, un sensor PIR de movimiento y un control remoto IR universal).
2. Activar el **Bluetooth** del dispositivo móvil.
3. Esperar a que la aplicación detecte los dispositivos y agregarlos para configurar la **red WiFi**.

Una vez completado el emparejamiento, los dispositivos estarán listos para su uso. En el caso del control remoto IR, puede ser necesario replicar manualmente los comandos del aire acondicionado si no se encuentra en la base de datos de Smart Life. En cambio, con la televisión, este proceso suele ser automático.

## Integración con Home Assistant

1. Abrir **Home Assistant**.
2. Descargar e instalar la **extensión de TUYA**.
3. Introducir la **ID de usuario** para vincular todos los dispositivos.

Desde Home Assistant, se pueden realizar automatizaciones básicas, aunque la mayoría de las configuraciones avanzadas se gestionan desde la aplicación móvil.

## Automatización de Dispositivos

### Automatización desde la Aplicación TUYA

La aplicación TUYA permite realizar automatizaciones avanzadas, como:

- Encender la televisión o el aire acondicionado cuando el sensor PIR detecte movimiento.
- Apagar los dispositivos después de un período sin movimiento.

Esto puede implementarse mediante:

1. **Automatizaciones Individuales**: Configuraciones separadas para cada acción (encender o apagar dispositivos).
2. **Escenas**: Permiten ejecutar varias acciones con un mismo evento. Por ejemplo:
   - Encender el aire acondicionado.
   - Encender la televisión.
   - Activar el relé WiFi.

## Conclusión

Con esta configuración, se logra un control eficiente de los dispositivos inteligentes mediante Home Assistant y TUYA, optimizando la automatización del hogar.

Para más información, consulta la [documentación oficial de TUYA](https://developer.tuya.com/) o la [comunidad de Home Assistant](https://community.home-assistant.io/).


