# Fase 2. Análisis del sistema

## 1. Identificación de actores

| Actor | Descripción |
|---|---|
| **Usuario (conductor o peatón)** | Persona que utiliza la aplicación móvil para consultar rutas, recibir alertas de tráfico o incidentes. |
| **Sistema de sensores** | Conjunto de dispositivos IoT (cámaras, sensores de flujo vehicular, sensores en semáforos) que capturan datos en tiempo real del entorno urbano. |
| **Centro de control** | Área/rol encargado de supervisar el sistema, gestionar semáforos de forma manual en emergencias y tomar decisiones operativas. |
| **Aplicación móvil** | Interfaz mediante la cual los usuarios interactúan con el sistema: consultan rutas y reciben notificaciones. |
| **Servicios externos (mapas, clima)** | Sistemas de terceros que proveen información complementaria, como cartografía y condiciones climáticas, para mejorar el cálculo de rutas y la generación de alertas. |

## 2. Funcionalidades principales

- Monitoreo del tráfico en tiempo real a partir de datos de sensores urbanos.
- Gestión inteligente y automatizada de semáforos según el flujo vehicular.
- Cálculo y actualización de rutas óptimas para los usuarios.
- Generación y notificación de alertas de congestión o incidentes.
- Integración con aplicaciones móviles para la interacción con los usuarios finales.
- Integración con servicios externos (mapas, clima) para enriquecer la información entregada.

## 3. Problemas que resuelve el sistema

- Congestión vehicular no gestionada, que genera pérdidas de tiempo y aumento de emisiones contaminantes.
- Falta de información en tiempo real para que los usuarios tomen decisiones de movilidad.
- Semáforos con tiempos fijos que no responden a las condiciones reales del tráfico.
- Demora en la detección y respuesta ante incidentes o congestiones en la vía pública.
- Ausencia de un canal centralizado que integre datos de sensores, rutas y alertas para la ciudad.

## 4. Restricciones del sistema

- **Restricción de tiempo real:** el sistema debe procesar datos de sensores y responder a los usuarios en tiempos muy bajos (segundos), dado que la información de tráfico pierde valor rápidamente.
- **Restricción de disponibilidad:** el sistema debe operar de forma continua (24/7), ya que la movilidad urbana no se detiene.
- **Restricción de escalabilidad:** debe soportar el crecimiento en el número de sensores, usuarios y zonas urbanas cubiertas sin degradar su rendimiento.
- **Restricción de interoperabilidad:** debe integrarse con servicios externos (mapas, clima) y con aplicaciones móviles de terceros mediante APIs estandarizadas.
- **Restricción de seguridad:** los datos transmitidos (ubicación de usuarios, datos de sensores) deben protegerse mediante protocolos seguros y control de acceso.