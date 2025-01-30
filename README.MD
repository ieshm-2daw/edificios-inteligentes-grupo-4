


# Control de Dispositivos con Home Assistant y TUYA

Este proyecto permite controlar dispositivos como televisores, aires acondicionados y corrientes eléctricas mediante un relé WiFi, utilizando Home Assistant y la integración de TUYA.

## Requisitos

- Home Assistant instalado y configurado.
- Cuenta en la aplicación de TUYA.
- Dispositivos compatibles con TUYA (relé WiFi, IR inteligente, etc.).

## Configuración

### Instalación de Home Assistant
Asegúrate de tener Home Assistant instalado y funcionando correctamente. Puedes consultar la [documentación oficial](https://www.home-assistant.io/) para más detalles.

### Integración de TUYA

1. Abre **Home Assistant**.
2. Descarga e instala la **extensión de TUYA**.
3. Introduce la **ID de usuario** para vincular todos tus dispositivos.

## Automatización de Dispositivos

Desde Home Assistant, puedes realizar algunas automatizaciones básicas. Sin embargo, la mayoría de las funciones avanzadas se gestionan desde la aplicación móvil de TUYA.

- **Relé WiFi**: Puede ser automatizado para encenderse o apagarse dependiendo de un actuador.
- **IR Inteligente**: No puede ser automatizado directamente en Home Assistant, ya que este no reconoce sus funciones específicas.

## Configuración en la Aplicación TUYA

Desde la aplicación de TUYA, es posible configurar automatizaciones avanzadas, como:

- Encender la televisión o el aire acondicionado cuando el sensor PIR detecte movimiento.
- Apagar los dispositivos después de un período sin movimiento.

Esto puede lograrse de dos formas:

1. **Automatizaciones Individuales**: Creando tres automatizaciones separadas para encender y apagar los dispositivos según el movimiento detectado.
2. **Escenas**: Una única configuración que, con un mismo detonante (movimiento), realice múltiples acciones, como:
   - Encender el aire acondicionado.
   - Encender la televisión.
   - Dar corriente al relé WiFi.



