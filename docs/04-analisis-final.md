# Fase 4. Análisis arquitectónico

## ¿Por qué son necesarias múltiples vistas?

Un sistema de software complejo, como el Smart Mobility System, no puede describirse completamente desde una sola perspectiva. Cada actor involucrado (usuarios, desarrolladores, arquitectos, gestores del proyecto) necesita entender el sistema desde un ángulo distinto: unos requieren ver la funcionalidad desde el punto de vista del usuario, otros la estructura interna del software, otros el comportamiento en tiempo de ejecución, y otros una visión general del negocio. Usar múltiples vistas arquitectónicas permite representar esta complejidad de forma organizada, evitando que un solo diagrama intente mostrar demasiada información a la vez, lo cual lo haría ilegible e inútil como herramienta de comunicación.

## ¿Qué representa cada vista?

- **Vista de casos de uso:** representa el comportamiento del sistema desde la perspectiva de los actores externos (usuarios, sensores, servicios externos), mostrando qué pueden hacer con el sistema.
- **Vista lógica:** representa la estructura interna del software, es decir, en qué componentes o módulos se organiza el sistema y cómo se relacionan entre sí.
- **Vista de procesos (diagrama de secuencia):** representa el comportamiento dinámico del sistema, mostrando cómo interactúan los componentes en el tiempo para resolver un caso concreto (en este trabajo, la detección de congestión y generación de alertas).
- **Vista conceptual:** representa una visión de muy alto nivel, mostrando los grandes dominios del sistema (usuarios, sensores, sistema central, servicios externos) sin entrar en detalles técnicos.

## ¿Cómo se complementan?

Las cuatro vistas se complementan porque cada una responde una pregunta distinta sobre el sistema. La vista conceptual ubica al lector en el panorama general; la vista de casos de uso detalla qué funcionalidades ofrece el sistema y a quién; la vista lógica explica cómo está construido internamente para ofrecer esas funcionalidades; y la vista de procesos muestra cómo esos componentes colaboran en tiempo real para cumplir un caso de uso específico. En conjunto, forman un recorrido que va de lo general a lo particular, y de lo estático a lo dinámico, dando una comprensión integral de la arquitectura del sistema.

## ¿Qué vista resultó más compleja y por qué?

La vista que resultó más compleja fue la **vista de procesos (diagrama de secuencia)**, ya que requiere pensar en el sistema no solo en términos de qué componentes existen, sino en el **orden temporal** exacto en que interactúan, incluyendo los distintos caminos posibles (por ejemplo, el caso en que se detecta congestión frente al caso en que no se detecta). Esto exige tener muy clara la lógica de negocio del escenario modelado antes de poder representarla correctamente, a diferencia de vistas como la conceptual o la de casos de uso, que son más descriptivas y menos dependientes de una secuencia lógica precisa.

# Conclusiones

- El uso de múltiples vistas arquitectónicas permitió representar el Smart Mobility System desde distintas perspectivas complementarias, facilitando su comprensión tanto a nivel funcional como técnico.
- La combinación de una vista conceptual de alto nivel con vistas más detalladas (casos de uso, lógica y de procesos) demuestra cómo la arquitectura de software debe equilibrar la visión general del sistema con el detalle necesario para su implementación.
- El modelado con UML resultó una herramienta efectiva para comunicar decisiones de diseño de forma clara y estandarizada, facilitando la trazabilidad entre los requisitos definidos en la Fase 1 y los componentes representados en las vistas arquitectónicas.
- Este ejercicio permitió comprender que un sistema de movilidad urbana inteligente, aunque conceptualmente simple de describir, involucra una arquitectura considerablemente compleja cuando se analiza a nivel de componentes, procesos e integración con servicios externos.