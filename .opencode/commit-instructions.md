# Instrucciones para la Generación de Commits

Bajo ninguna circunstancia generarás un mensaje que no siga esta estructura exacta:
`<tipo>(<alcance opcional>): <descripción corta>`

## 1. Tipos Permitidos (`<tipo>`)
Utiliza únicamente los siguientes prefijos según la naturaleza del cambio:

* feat: Introduce una nueva característica, funcionalidad o un nuevo modelo fundamental en RUP (ej. nuevo caso de uso, nuevo diagrama).
* fix: Soluciona un error en el código o corrige una incongruencia detectada en la documentación o diagramas.
* docs: Cambios exclusivos en la documentación que no afectan a la ejecución (glosario, minutas, README, contexto del proyecto).
* refactor: Modificaciones en el código o reestructuración de directorios que no añaden funcionalidades ni corrigen errores (ej. organizar las carpetas RUP).
* style: Cambios de formato, indentación o convenciones que no afectan la lógica del sistema.
* test: Adición o modificación de pruebas automatizadas.
* chore: Actualizaciones de tareas de construcción, configuración de herramientas (como este mismo archivo) o dependencias.

## 2. Reglas Estrictas de Formato
1. Verbo en Imperativo: La descripción corta debe usar el modo imperativo (ej. "añade modelo de dominio", "corrige validación", "refactoriza directorios"). Nunca uses gerundios ("añadiendo") ni participios ("añadido").
2. Límites de Longitud: La primera línea (tipo + alcance + descripción) NUNCA debe superar los 72 caracteres.
3. Sin punto final: No termines la descripción corta con un punto.
4. Minúsculas: El `<tipo>` y el `<alcance>` deben ir siempre en minúsculas.

## 3. Trazabilidad RUP y Cuerpo del Commit
* Alcance RUP: Si el cambio pertenece a una fase específica de la metodología, indícalo en el alcance. Ejemplos: `(requisitos)`, `(analisis)`, `(diseno)`, `(bd)`.
* Cuerpo (Opcional): Si el cambio requiere explicación, deja una línea en blanco tras la descripción corta y detalla el *qué* y el *por qué* de la decisión arquitectónica o de código. No expliques el *cómo* (el código ya lo hace).

## Ejemplos de Commits Válidos:
* `feat(requisitos): añade especificación del caso de uso Iniciar Sesión`
* `fix(bd): corrige cardinalidad en la tabla de usuarios`
* `docs: actualiza minuta de la reunión de arranque`
* `refactor: elimina carpetas obsoletas de UML genérico`
