Portada

Nombre: [Tu Nombre / Apellido]

Código: [Tu Código de Estudiante]

Curso: Arquitectura de Software y Patrones de Diseño

Unidad: Unidad 1

Fecha: 2026-09-04

Introducción
El presente documento analiza la implementación práctica de patrones de diseño orientados a objetos (GoF) dentro del código fuente de Spring Framework, examinando cómo resuelven problemas complejos de desacoplamiento, gestión de recursos y extensibilidad en arquitecturas modernas con Spring Boot.

Análisis de Patrón 1: Factory Method (Creacional)

Nombre del Patrón: Factory Method

Categoría: Creacional

Clase / Componente en Spring: org.springframework.beans.factory.BeanFactory

Problema que resuelve: Desacopla la creación de instancias de objetos (beans) de la lógica de negocio que los consume, permitiendo que el contenedor IoC gestione dinámicamente el ciclo de vida, la configuración y el ámbito (scope) sin usar operadores new dispersos.

SOLID Asociado: Principio de Inversión de Dependencias (DIP).

Análisis de Patrón 2: Proxy (Estructural)

Nombre del Patrón: Proxy

Categoría: Estructural

Clase / Componente en Spring: org.springframework.aop.framework.JdkDynamicAopProxy

Problema que resuelve: Intercepta las llamadas a los métodos de los servicios de negocio para inyectar lógica transversal (cross-cutting concerns) como control de transacciones (@Transactional) o seguridad sin modificar el código fuente original.

SOLID Asociado: Principio Abierto/Cerrado (OCP).

Análisis de Patrón 3: Template Method (Comportamiento)

Nombre del Patrón: Template Method

Categoría: De Comportamiento

Clase / Componente en Spring: org.springframework.jdbc.core.JdbcTemplate

Problema que resuelve: Elimina el código repetitivo (boilerplate) asociado a la apertura y cierre de conexiones JDBC o manejo de excepciones, fijando el esqueleto del algoritmo de acceso a datos y delegando los pasos específicos a interfaces de callback.

SOLID Asociado: Principio de Responsabilidad Única (SRP).

Conclusiones
El diseño modular de Spring Framework demuestra cómo la aplicación sistemática de los patrones GoF facilita la creación de estructuras extensibles, desacopladas y altamente mantenibles, sirviendo como una referencia fundamental para el diseño de software empresarial.

Referencias

Gamma, E., Helm, R., Johnson, R., & Vlissides, J. (1994). Patrones de diseño: elementos de software orientado a objetos reutilizable . Addison-Wesley.

Documentación de Spring Framework. (2026). Referencia de tecnologías principales . Recuperado dehttps://docs.spring.io/spring-framework/reference/

Refactoring Guru. (2026). Catálogo de Patrones de Diseño. Recuperado de https://refactoring.guru/design-patterns/