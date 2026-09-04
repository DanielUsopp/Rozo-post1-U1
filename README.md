# Rozo-post1-U1
"Post-contenido — Refactorización SOLID y análisis de patrones GoF en Spring

## Análisis de Violaciones SOLID

| Principio | Método/Sección afectada | Descripción de la violación |
|-----------|-------------------------|-----------------------------|
| SRP       | calculateTotal + applyDiscount + saveOrder + sendEmail + printReport | La clase asume múltiples responsabilidades no relacionadas (lógica de negocio, persistencia, notificaciones e impresión), lo que causa alta acoplamiento y baja cohesión. |
| OCP       | applyDiscount (if/else sobre customerType) | Modificar o agregar nuevos tipos de clientes requiere modificar directamente el código fuente existente en lugar de extenderlo mediante polimorfismo. |
| DIP       | Toda la clase (dependencias internas sin abstracciones) | La clase depende directamente de implementaciones concretas y de bajo nivel en lugar de depender de abstracciones o interfaces. |