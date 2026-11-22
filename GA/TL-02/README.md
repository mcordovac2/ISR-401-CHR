# GA-TL-02 - FORM

## Taller de entrevista estructurada y Design Thinking aplicados al PFC

**Universidad:** Universidad Técnica Estatal de Quevedo (UTEQ)  
**Facultad:** Ciencias de la Computación  
**Carrera:** Ingeniería de Software  
**Asignatura:** Ingeniería de Requerimientos (ISR-401)  
**Nivel:** Cuarto  
**Unidad:** Unidad 2 — Elicitación y Análisis de Requisitos  
**Modalidad:** Grupal · Actividad formativa, sin calificación numérica  
**Semana:** 4, del 16 al 22 de noviembre de 2026  
**Fecha límite:** sábado 21 de noviembre de 2026, 23:59  
**Docente:** Gleiston Cicerón Guerrero Ulloa, PhD

## 1. Integrantes

| Integrante | GitHub |
|---|---|
| Córdova Carreño Mayra Lucila | [mcordovaac2](https://github.com/mcordovaac2) |
| Herrera Morán Gilmar Javier | [GilmaR2006](https://github.com/GilmaR2006) |
| Rivas Bodero Jordy Fabián | [JordyR15](https://github.com/JordyR15) |

**Repositorio:** https://github.com/mcordovaac2/ISR-401-CHR  
**Directorio:** https://github.com/mcordovaac2/ISR-401-CHR/tree/main/GA/TL-02

El equipo de este taller está formado por los tres integrantes indicados. El proyecto seleccionado como caso de estudio procede de un PFC; utilizarlo en esta actividad no modifica la autoría ni la composición del equipo original de ese PFC.

## 2. Proyecto y propósito

**Caso de estudio:** Sistema de Gestión de Arriendos y Residencias Estudiantiles en los alrededores de la UTEQ.

Se estudia la administración de habitaciones y residencias destinadas a estudiantes, con atención a la disponibilidad, contratos, mensualidades, servicios básicos, comunicación y mantenimiento. Para este taller se seleccionó como parte interesada principal a una **propietaria de residencia estudiantil simulada**. Los perfiles de estudiante y personal de mantenimiento forman parte del contexto del proyecto, pero no fueron entrevistados en este ensayo.

El objetivo fue diseñar un guion de elicitación, ensayarlo mediante juego de roles, sintetizar la perspectiva del personaje mediante un mapa de empatía, formular un problema centrado en el usuario y revisar preguntas susceptibles de mejora. La actividad prepara **GA-SUM-03** y **TA-PFC-E2**.

## 3. Productos desarrollados

| Componente de la rúbrica | Contenido documentado en `main.tex` y `main.pdf` |
|---|---|
| Guion de entrevista | Apertura, cinco bloques temáticos, 15 preguntas (P1–P15) y cierre. |
| Consentimiento | Protocolo de consentimiento informado y autorización **verbal** incluida en la grabación. El formulario del anexo no se presenta como firmado. |
| Ensayo | Juego de roles grabado solo en audio, el 21/11/2026, con duración de **07:45**. |
| Mapa de empatía | Síntesis de Dice, Hace, Piensa, Siente, Dolores y Ganancias; las inferencias se distinguen de las respuestas simuladas. |
| Definición del problema | Necesidad del usuario y pregunta central «¿Cómo podríamos…?», con preguntas complementarias. |
| Revisión del guion | Identificación, reformulación y justificación de preguntas mejorables. |
| Evidencias | Manifiesto integrado en el documento, con metadatos del audio, ubicación institucional y huella SHA-256. |

**Alcance del ensayo:** la grabación se realizó **fuera de clase** entre Mayra Córdova, como entrevistadora, y una participante voluntaria, como propietaria simulada. **Gilmar Herrera y Jordy Rivas no participaron en esa grabación ni estuvieron presentes como observadores.** La guía oficial solicita un ensayo en clase con un compañero; el ejercicio externo se declara expresamente y no se hace pasar por una ejecución presencial en el aula. Las respuestas son parte de una simulación académica, no testimonios de una propietaria real.

## 4. Distribución del trabajo

| Integrante | Aportación documentada |
|---|---|
| **Mayra Córdova** | Elaboración del guion, protocolo de consentimiento, conducción y grabación del ensayo simulado; integración y revisión del documento. |
| **Gilmar Herrera** | Desarrollo del mapa de empatía y de la definición del problema centrada en el usuario a partir del registro del ensayo. |
| **Jordy Rivas** | Documentación y análisis posterior del ensayo, revisión de preguntas, registro de evidencias e instrucciones de compilación. |

La distribución de tareas documentales **no implica** que todos hayan intervenido en la grabación.

## 5. Archivos del directorio

La carpeta de la actividad contiene los siguientes archivos principales:

```text
GA/
└── TL-02/
    ├── README.md
    ├── main.tex
    └── main.pdf
```

| Archivo | Descripción |
|---|---|
| `main.tex` | Fuente LaTeX del informe: guion, consentimiento, ensayo, mapa de empatía, problema, ajustes, manifiesto y declaración de IA. |
| `main.pdf` | PDF generado a partir del código fuente. |
| `README.md` | Contexto, alcance, evidencias y procedimiento de compilación. |

El manifiesto está **dentro de `main.tex`/`main.pdf`**; no se requiere un `manifiesto.md` separado para describir el archivo existente. El mapa de empatía también está integrado en el documento, sin depender de un archivo gráfico externo.

## 6. Compilación reproducible

### 6.1. Herramientas y dependencias

- **Compilador:** pdfLaTeX (disponible en distribuciones como TeX Live o MiKTeX).
- **Archivo principal:** `GA/TL-02/main.tex`.
- **Paquetes utilizados:** `inputenc`, `fontenc`, `babel` (español), `lmodern`, `titlesec`, `tikz`, `lastpage`, `colortbl`, `geometry`, `setspace`, `array`, `tabularx`, `longtable`, `enumitem`, `needspace`, `amssymb`, `hyperref`, `fancyhdr`, `microtype`, `graphicx` y `xcolor`.
- **Bibliografía:** las referencias se encuentran directamente en `main.tex` mediante `thebibliography`; no se utiliza archivo `.bib` ni BibTeX.
- **Recursos externos:** el código actual no requiere una figura externa para compilar el mapa de empatía.

### 6.2. Procedimiento

Clonar el repositorio e ingresar a la carpeta:

```bash
git clone https://github.com/mcordovaac2/ISR-401-CHR.git
cd ISR-401-CHR/GA/TL-02
```

Ejecutar **tres pasadas** de pdfLaTeX para actualizar referencias cruzadas, numeración e índice:

```bash
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

El resultado debe ser `main.pdf` en el mismo directorio. Si se utiliza Overleaf, seleccionar **pdfLaTeX** como compilador y establecer `main.tex` como documento principal.

### 6.3. Comprobaciones de reproducibilidad

Después de compilar, verificar que:

- No existan errores de compilación ni referencias internas sin resolver.
- El índice incluya el apartado **Referencias**.
- Las tablas, los saltos de página y las referencias bibliográficas sean legibles.
- El PDF generado corresponda al `main.tex` publicado.
- La compilación funcione desde una copia recién clonada del repositorio.

El historial de compilación local no sustituye esta última prueba en un entorno limpio.

## 7. Manifiesto y protección de las evidencias

**Evidencia:** grabación de audio del juego de roles. El archivo **no se publica en GitHub**.

| Campo | Registro |
|---|---|
| Nombre | `GA-TL-02_Entrevista_Propietaria_2026-11-21.m4a` |
| Fecha | 21 de noviembre de 2026 |
| Duración | 07:45 |
| Formato | M4A |
| Tamaño | 10.798.192 bytes |
| SHA-256 | `69821E07DF5A38766E48A1672EC669FCF2ADFA8B4D9CD8BE13C2DC4CEA1AC799` |
| Almacenamiento | Google Drive de una cuenta institucional UTEQ, carpeta `GA-TL-02 - Evidencias Privadas` |
| Permiso informado | Lectura para miembros de la UTEQ que dispongan del enlace; **no está limitado exclusivamente al docente** |
| Consentimiento | Verbal, registrado al inicio del audio |

**Enlace institucional a la evidencia (requiere cuenta UTEQ autorizada):**  
https://drive.google.com/file/d/1loUDyv_cXjtktltbx32BDi9hD-7bvkpM/view?usp=sharing

La huella se obtuvo mediante PowerShell. Para calcularla nuevamente sobre una copia local del archivo:

```powershell
Get-FileHash -Path ".\GA-TL-02_Entrevista_Propietaria_2026-11-21.m4a" -Algorithm SHA256
```

El resultado debe compararse con el valor registrado; **no se afirma aquí haber verificado una segunda copia descargada**. La hora de creación del archivo no debe confundirse con la hora exacta de inicio de la entrevista.

**Privacidad:** la rúbrica solicita resguardar las evidencias personales en una carpeta institucional privada compartida con el docente. La configuración actual de lectura por dominio institucional es más amplia que el acceso exclusivo del docente y el equipo; se recomienda restringirla a las personas autorizadas y comprobar que el docente pueda abrir el archivo. No publicar en el repositorio audios, consentimientos firmados, cédulas, teléfonos ni otros datos personales de terceros.

## 8. Referencias y declaración de IA

Las referencias están numeradas en formato IEEE mediante `thebibliography` dentro de `main.tex`, y el documento incorpora citas `\cite{...}`. No se necesita `referencias.bib`. Deben comprobarse los datos bibliográficos y que cada cita respalde la afirmación correspondiente; la existencia de un enlace no garantiza su corrección.

El informe declara el uso de **ChatGPT (OpenAI, GPT-6)** como apoyo para redacción, revisión de preguntas, integración de aportaciones y ajustes de LaTeX. La revisión de fuentes, evidencias, afirmaciones y resultados corresponde al equipo. No se deben presentar respuestas simuladas como entrevistas reales ni atribuir participaciones que no ocurrieron.

## 9. Entrega y condiciones de validez

La guía oficial establece:

1. **Repositorio público:** los archivos principales `GA/TL-02/main.tex` y `GA/TL-02/main.pdf`, junto con el README y las dependencias necesarias, deben estar accesibles en GitHub.
2. **SGA:** subir **solo un PDF informativo de una página**, con los nombres de los integrantes, código y nombre de la actividad, fecha límite y URL completa del repositorio **en una sola línea**. **No subir el informe `main.pdf` de varias páginas como sustituto del PDF informativo.**
3. **Reproducibilidad:** el PDF debe poder regenerarse desde `main.tex` siguiendo este README.
4. **Plazo:** el contenido evaluable debía estar publicado antes del **21/11/2026 a las 23:59**; la fecha y la entrega se comprueban en GitHub y SGA.
5. **Integridad:** las fuentes y evidencias deben existir y ser explicables; el uso de IA debe declararse según la guía.

El incumplimiento de las condiciones de entrega válida puede impedir la presentación de **GA-SUM-03** y **TA-PFC-E2**. El README no demuestra por sí solo que el PDF informativo haya sido entregado ni que la fecha límite se haya cumplido.

## 10. Lista de cotejo y verificaciones finales

| Indicador de la rúbrica | Evidencia en el documento | Precaución |
|---|---|---|
| Guion estructurado y preguntas neutrales | Apertura, 15 preguntas en bloques y cierre | Comprobar claridad y neutralidad. |
| Ensayo con consentimiento y manifiesto | Audio, consentimiento verbal y metadatos | Fue fuera de clase, no en el aula como exige la guía. |
| Mapa de empatía coherente | Seis dimensiones vinculadas al ensayo | Son respuestas simuladas e inferencias, no hallazgos de campo real. |
| Problema centrado en el usuario | Planteamiento y «¿Cómo podríamos…?» | No confundir necesidad con solución predeterminada. |
| Preguntas defectuosas corregidas | Tabla de revisión y justificación | Mantener trazabilidad con las preguntas originales. |

**Pendiente de verificación externa antes de considerar la entrega conforme:** accesibilidad del enlace para el docente, exactitud de todas las referencias, compilación desde un clon limpio, historial de commits y entrega del PDF informativo de una página en el SGA. La decisión sobre el cumplimiento del requisito de ensayo en clase corresponde al docente.

## 11. Documento normativo de la actividad

Universidad Técnica Estatal de Quevedo, *Guía y rúbrica de evaluación: GA-TL-02 - FORM — Taller de entrevista estructurada y Design Thinking aplicados al PFC*, Ingeniería de Requerimientos (ISR-401), SPA 2026–2027, 5 páginas.
