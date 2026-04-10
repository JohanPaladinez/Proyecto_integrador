# Proyecto Integrador

Sistema embebido orientado a la automatización de un proceso de limpieza y monitoreo, implementado sobre ESP32 mediante módulos independientes para:

- Indicadores visuales con LED RGB
- Movimiento mecánico mediante polea y motor paso a paso
- Activación de transductor por relé
- Medición y registro de temperatura con sensor DS18B20

## Descripción general

Este proyecto busca integrar diferentes subsistemas electrónicos para ejecutar un ciclo automático de operación. La lógica actual está dividida en módulos separados, donde cada archivo controla una función específica del sistema:

- **LEDS**: indica visualmente el estado del sistema.
- **Polea**: mueve un mecanismo de subida y bajada del sensor.
- **RELE**: activa o desactiva el transductor durante el tiempo de limpieza.
- **Temperatura**: mide la temperatura y la envía a una base de datos MySQL por Wi-Fi.

## Objetivo

Desarrollar un prototipo funcional basado en ESP32 que permita automatizar tareas de limpieza y monitoreo, incorporando control de actuadores, señalización visual y registro de variables físicas.

## Estructura del repositorio

```bash
Proyecto_integrador/
│── Codigo_unificado
│── LEDS
│── RELE
│── Temperatura
└── README.md
