# Fase 1. Especificación de requisitos del sistema

## 1. Identificación de módulos funcionales

El sistema se organiza en los siguientes módulos funcionales:

1. **Gestión del tráfico** – monitoreo y análisis del flujo vehicular en tiempo real.
2. **Gestión de semáforos** – control y coordinación de semáforos inteligentes.
3. **Gestión de rutas** – cálculo y actualización de rutas óptimas para los usuarios.
4. **Gestión de sensores** – recolección y procesamiento de datos de sensores urbanos.
5. **Gestión de alertas** – generación y notificación de alertas de congestión o incidentes.
6. **Administración del sistema** – gestión de usuarios, configuración y monitoreo general de la plataforma.

## 2. Especificación de requisitos funcionales

### Módulo: Gestión del tráfico
- **RF01.** El sistema deberá monitorear el tráfico en tiempo real.
- **RF02.** El sistema deberá detectar congestiones vehiculares.
- **RF03.** El sistema deberá clasificar el nivel de congestión por zona (bajo, medio, alto).

### Módulo: Gestión de semáforos
- **RF04.** El sistema deberá ajustar automáticamente los tiempos de los semáforos según el flujo vehicular.
- **RF05.** El sistema deberá permitir la operación manual de semáforos desde el centro de control en caso de emergencia.

### Módulo: Gestión de rutas
- **RF06.** El sistema deberá calcular rutas óptimas para los usuarios.
- **RF07.** El sistema deberá actualizar las rutas en tiempo real ante cambios en el tráfico.
- **RF08.** El sistema deberá permitir a los usuarios consultar rutas desde una aplicación móvil.

### Módulo: Gestión de sensores
- **RF09.** El sistema deberá recolectar datos de sensores urbanos (cámaras, sensores de flujo, semáforos).
- **RF10.** El sistema deberá validar y filtrar los datos recibidos antes de procesarlos.

### Módulo: Gestión de alertas
- **RF11.** El sistema deberá generar alertas automáticas ante congestiones o incidentes detectados.
- **RF12.** El sistema deberá notificar las alertas a los usuarios a través de la aplicación móvil.

### Módulo: Administración del sistema
- **RF13.** El sistema deberá permitir la gestión de usuarios y roles (administrador, operador, usuario final).
- **RF14.** El sistema deberá registrar un histórico de eventos e incidentes para auditoría y análisis posterior.

## 3. Especificación de requisitos no funcionales

- **RNF01.** El sistema deberá tener una disponibilidad del 99,9 %.
- **RNF02.** El tiempo de respuesta no deberá superar los dos segundos.
- **RNF03.** Toda la comunicación deberá realizarse mediante protocolos seguros (HTTPS/TLS).
- **RNF04.** El sistema deberá permitir escalabilidad horizontal para soportar el crecimiento de sensores y usuarios conectados.
- **RNF05.** El sistema deberá garantizar tolerancia a fallos, evitando puntos únicos de falla en los componentes críticos.
- **RNF06.** El sistema deberá cumplir con normativas de protección de datos personales de los usuarios.
- **RNF07.** La interfaz de usuario de la aplicación móvil deberá ser accesible e intuitiva, permitiendo su uso sin capacitación previa.