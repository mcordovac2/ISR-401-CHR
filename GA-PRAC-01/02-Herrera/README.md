# 02 - Herrera

## Responsable
**Herrera Morán Gilmar Javier** (usuario de GitHub: [GilmaR2006](https://github.com/GilmaR2006))

## Actividad
GA-PRAC-01 - Comparación entre modelos de proceso de requisitos en escenarios reales.

## Apartado asignado

### C3. Actores del proceso y framework de IR (1,5 puntos)

- Identificar los actores de cada escenario y describir su rol en el proceso de requisitos.
- Ubicar las actividades centrales: elicitación, documentación y negociación.
- Ubicar las actividades transversales: validación y gestión de requisitos (incluye gestión de cambios y trazabilidad).
- Ubicar los artefactos del framework: metas, escenarios y requisitos orientados a la solución.
- Relacionar actividades y artefactos con las fases o iteraciones del escenario.

## Archivos

| Archivo | Contenido |
|---|---|
| `c3-actores-framework.tex` | Desarrollo completo de C3. Se incorpora a `../main.tex` con `\input{02-Herrera/c3-actores-framework.tex}`. |
| `main_C3.tex` | Documento mínimo para compilar solo el apartado C3 (vista previa). No es el documento oficial. |
| `main_C3.pdf` | PDF generado a partir de `main_C3.tex`. |

## Contenido de `c3-actores-framework.tex`

1. **Marco de referencia:** framework de IR de Pohl (actividades centrales, transversales y artefactos).
2. **Escenario 1 (Extractora Río Lindo):** actores y actividades del framework.
3. **Escenario 2 (Sabores de la Abuela Rosa):** actores y actividades del framework.
4. **Escenario 3 (Sistema de trámites municipales):** escenario elegido para la Plantilla 3. Incluye contexto del sistema, actores con su rol y su forma de participación, y las actividades y artefactos ubicados por fase o iteración.
5. **Escenario 4 (Cooperativa Frutos del Estero):** actores y actividades del framework.
6. **Síntesis.**

## Compilación

**Documento oficial:** `../main.tex`, que incorpora este apartado.

```bash
cd GA-PRAC-01
pdflatex main.tex
pdflatex main.tex
```

**Vista previa solo de C3:**

```bash
cd GA-PRAC-01/02-Herrera
pdflatex main_C3.tex
pdflatex main_C3.tex
```

Ambos requieren el paquete de español de `babel`, además de `array` y `longtable`. Más detalles en el README de `GA-PRAC-01`.

## Referencias utilizadas

Las referencias completas están en la bibliografía de `main.tex`. Este apartado cita:

- Pohl, K. (2025). *Requirements Engineering: Fundamentals, Principles, and Techniques* (2.ª ed.). Springer.
- IREB (2026). *CPRE Foundation Level Syllabus, versión 3.3.0*.
- Washizaki, H. (Ed.). (2024). *SWEBOK Guide, Version 4.0*. IEEE Computer Society.
- ISO/IEC/IEEE 29148:2018. *Requirements engineering*.

## Material de referencia
- Material complementario GA-PRAC-01 y rúbrica de la actividad.
- CLASE SEMANA 2 y MATERIAL PARA CLASE 2.
- Desarrollo del sílabo (páginas 31-48).

## Estado
**Completado.** Integrado en `main.tex`.
