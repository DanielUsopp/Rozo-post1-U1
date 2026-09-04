# Post-contenido — Unidad 1: Fundamentos de Patrones de Diseño y Buenas Prácticas

## Descripción
Repositorio del post-contenido de la Unidad 1 de Patrones de Diseño de Software — Sexto Semestre. Contiene dos partes: refactorización SOLID de un God Object (`parte-1-refactorizacion-solid/`) y análisis de patrones GoF en Spring Framework (`parte-2-analisis-gof-spring/`).

## Parte 1 — Refactorización SOLID
Proyecto Maven que refactoriza `OrderProcessor` aplicando los principios SRP, OCP y DIP. Ver `parte-1-refactorizacion-solid/`.

## Parte 2 — Análisis de Patrones GoF en Spring
| # | Patrón | Categoría | Clase en Spring |
|---|--------|-----------|-----------------|
| 1 | Factory Method | Creacional | `org.springframework.beans.factory.BeanFactory` |
| 2 | Proxy | Estructural | `org.springframework.aop.framework.JdkDynamicAopProxy` |
| 3 | Template Method | Comportamiento | `org.springframework.jdbc.core.JdbcTemplate` |

Ver `parte-2-analisis-gof-spring/documento-analisis.md`.

## Herramientas utilizadas
- Java 17, Apache Maven, VS Code, Git, GitHub
- Código fuente de Spring Framework (investigación)

## Conclusiones
El desarrollo de este trabajo permitió comprender de forma práctica la importancia de alinear el código con los principios SOLID para evitar acoplamientos rígidos en aplicaciones monolíticas. Asimismo, el análisis del código fuente de Spring Framework demostró cómo los patrones de diseño GoF resuelven problemas complejos de infraestructura y extensibilidad de manera transparente para el desarrollador. La aplicación sistemática de estos conceptos garantiza la construcción de software empresarial altamente mantenible, modular y preparado para futuras evoluciones tecnológicas.