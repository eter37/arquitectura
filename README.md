# Sistema Inteligente de Movilidad Urbana (Smart Mobility System)

**Arquitectura del Software – Taller: Modelado y representación arquitectónica del sistema**

> Estudiante: Santiago Rodriguez Ospina


## Contenido

- [Introducción](#introducción)
- [Descripción del sistema](#descripción-del-sistema)
- [Fase 1. Especificación de requisitos](docs/01-requisitos.md)
- [Fase 2. Análisis del sistema](docs/02-analisis.md)
- [Fase 3. Vistas arquitectónicas](docs/03-vistas.md)
- [Fase 4. Análisis arquitectónico y conclusiones](docs/04-analisis-final.md)

## Introducción

## Introducción

La movilidad urbana es uno de los mayores desafíos de las ciudades actuales, donde el crecimiento del parque automotor genera problemas de congestión, tiempos de desplazamiento elevados y un impacto negativo en la calidad de vida de los ciudadanos. Este trabajo presenta el diseño arquitectónico de un **Sistema Inteligente de Movilidad Urbana (Smart Mobility System)**, cuyo propósito es monitorear el tráfico en tiempo real, gestionar semáforos de forma inteligente, calcular rutas óptimas, integrarse con aplicaciones móviles y servicios externos, y generar alertas ante congestiones o incidentes.

A lo largo de este documento se desarrolla la especificación de requisitos del sistema, el análisis de sus actores y restricciones, y su representación arquitectónica mediante cuatro vistas complementarias (casos de uso, lógica, de procesos y conceptual), aplicando los conceptos estudiados en la Unidad 2 de Arquitectura del Software.

## Descripción del sistema

El **Smart Mobility System** es un sistema inteligente de movilidad urbana orientado a monitorear el tráfico en tiempo real, gestionar semáforos inteligentes, permitir a los usuarios consultar rutas óptimas, integrarse con aplicaciones móviles, procesar datos de sensores urbanos y generar alertas de congestión o incidentes.

### Importancia del sistema

El crecimiento acelerado de las ciudades y del parque automotor ha convertido la congestión vehicular en uno de los principales problemas de la movilidad urbana actual, generando pérdidas de tiempo, mayor consumo de combustible, aumento de emisiones contaminantes y afectaciones en la calidad de vida de los ciudadanos. Frente a esto, los sistemas inteligentes de movilidad urbana cobran especial relevancia porque permiten pasar de una gestión reactiva del tráfico —donde se actúa una vez el problema ya ocurrió— a una gestión **proactiva y basada en datos**, capaz de anticipar congestiones, optimizar el uso de la infraestructura vial existente (sin necesidad de grandes obras físicas) y ofrecer información oportuna a los ciudadanos para que tomen mejores decisiones de desplazamiento. En este sentido, el sistema no solo busca mejorar la eficiencia del tráfico, sino también contribuir a ciudades más sostenibles y seguras.

### Elementos principales del sistema

El sistema está compuesto por los siguientes elementos:

- **Sensores urbanos:** cámaras de tráfico, sensores de flujo vehicular y sensores integrados en los semáforos, encargados de capturar información del entorno en tiempo real.
- **Centro de procesamiento y análisis de datos:** componente encargado de validar, filtrar y analizar la información recolectada, incluyendo un módulo de análisis predictivo para anticipar congestiones.
- **Módulo de gestión de tráfico y semáforos:** ajusta de forma automática (o manual, en caso de emergencias) los tiempos de los semáforos según las condiciones reales de tráfico.
- **Módulo de gestión de rutas y alertas:** calcula rutas óptimas para los usuarios y genera notificaciones ante congestiones o incidentes detectados.
- **Aplicación móvil:** interfaz mediante la cual los usuarios (conductores y peatones) consultan rutas y reciben alertas en tiempo real.
- **Integración con servicios externos:** conexión con proveedores de mapas y servicios meteorológicos, que enriquecen el cálculo de rutas y la generación de alertas.
- **Centro de control:** encargado de la supervisión general del sistema y de la intervención manual sobre los semáforos cuando la situación lo requiere.

Estos elementos trabajan de forma integrada para ofrecer una plataforma capaz de responder en tiempo real a las condiciones de tráfico de la ciudad, tal como se detalla en las secciones de requisitos, análisis y vistas arquitectónicas de este documento.