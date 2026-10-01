# HANDOFF — Contexto, hallazgos y plan

Fecha del traspaso: 2026-09-30.
Origen: conversación en Claude (chat) que se continúa en un repositorio con Claude Code.

> **Actualización 2026-09-30 (Claude Code).** Decidido: tratamiento *vos*; alcance v1 = CV + sincronización + trámites FFyH; verificación navegando el sistema real en solo lectura. Las pp. 246–257 del manual UBA ya se leyeron. Los archivos de investigación se movieron a `investigacion/`. Estado vigente: `CLAUDE.md` e `investigacion/fuentes.md`.

## 1. Objetivo
Un manual de SIGEVA-UNC para investigadores, en formato tipo MkDocs, que permita consulta ágil y versionado. Debe actualizar el manual UNC (2011) al menos al estado del manual UBA (7.ª ed.) y sumar sugerencias propias que se definirán durante el proyecto.

## 2. Qué se hizo en la conversación, y qué quedó descartado

### 2.1 Relevamiento general de manuales de universidades nacionales: DESCARTADO
En un primer paso se pidió relevar manuales de SIGEVA de todas las universidades nacionales. La herramienta de búsqueda extendida devolvió solo un identificador de tarea, sin resultados. A pesar de eso se redactó y presentó un informe extenso (tabla de ~30 universidades, enlaces, afirmaciones de "verifiqué tres fuentes") que **no estaba respaldado por resultados leídos**. Ese informe fue un error y **no debe usarse**. El relevamiento sigue pendiente y habría que rehacerlo abriendo cada documento (ver backlog).

### 2.2 Comparación de tres manuales: VÁLIDA (con límites)
Se leyeron directamente los PDF de: guía CONICET v4 (2017), manual UBA 7.ª ed., manual UNC (2011). Resultado completo en `comparacion-manuales.md`. Límites:
- UBA: el texto extraído se cortó en la p. 248 de 257. No se leyó postulación (4.3.5–4.3.6), integrantes (5) ni material de referencia (6).
- Las capturas de pantalla no se extraen; la lista de campos por solapa de CONICET v4 está en una imagen.
- Para la estructura de CV de CONICET se usó la descripción del módulo en https://sigeva.conicet.gov.ar/.

## 3. Hallazgos verificados (resumen)
1. **El manual UNC deriva del de la UBA.** Su propio apartado final lo declara (desarrollado por TIC de la UBA, adaptado por la Prosecretaría de Informática de la UNC, con aporte de CONICET). Texto y mecánicas casi idénticos; conserva referencias cruzadas con numeración UBA que no existen en el UNC.
2. **El manual UBA tiene errores de referencias cruzadas** (off-by-one en secciones de autores e instituciones; "3.9.4" en lugar de 3.11.1 para financiamiento).
3. **Cobertura UNC 2011 mucho menor que UBA 7.ª ed.** (brecha detallada en sección 4).
4. **La guía CONICET v4 aporta funciones que ni UBA ni UNC documentan**: precarga de artículos por DOI/ISSN, asignación de colaborador, impresión del CV con selección de secciones y rango de fechas, FAQ de errores comunes, y la regla de que el nombre de autor debe coincidir con el nombre registrado.
5. **Solo el manual UBA documenta el efecto "foto"**: al asociarse a un proyecto o presentar, el sistema copia el banco de datos; los cambios posteriores no se reflejan salvo desasociarse y reasociarse.
6. **Ninguno de los tres es un manual para docentes** ni cubre evaluación/carrera docente. La carga de docencia en UBA es mucho más rica que en UNC.
7. **Sincronización:** tanto UBA como UNC la describen (compartir en origen con contraseña; importar formulario por formulario en destino). Restricciones distintas: UBA no comparte identificación, domicilio ni lugar de trabajo; UNC (2011) lista 8 secciones habilitadas y no incluye Formación académica ni Carrera de investigador.

## 4. Brecha: qué tiene UBA 7.ª ed. y no el manual UNC 2011
(El manual UNC es de 2011; es posible que el sistema actual de la UNC ya tenga varios de estos formularios. **Hay que verificarlo con una cuenta real** antes de documentarlos.)

- Datos personales: separación en identificación / domicilio / lugar de trabajo; reglas de campos mínimos.
- Formación complementaria (especialidades de salud, posdoctorado, cursos, idiomas); niveles académicos completos (básico a doctorado).
- Cargos: docencia con actividades curriculares dictadas, cargos de I+D (incluye categoría del Programa de Incentivos), gestión institucional.
- Antecedentes: extensión, evaluación, becas, otras actividades CyT, áreas de actuación.
- Producción: tesis, "demás producciones", trabajos en eventos no publicados, producción artística (9 subtipos).
- Otros antecedentes: premios, participación/organización de eventos, membresías.
- Trámites: vincularse a un proyecto con código, efecto "foto".
- Postulación de proyectos como director e integrante (el alcance es decisión del proyecto; ver preguntas abiertas).
- Impresión del CV; navegación general; reglas de contraseña ya presentes en UNC.

## 5. Sugerencias propias candidatas (a validar contra el sistema real)
Marcadas como ideas, no como hechos:
- Página de "Antes de empezar": qué datos tener a mano, orden de carga recomendado.
- Guía de sincronización UNC ↔ CONICET ↔ CVar como flujo único, con diagrama (la guía oficial de sincronización de CONICET es v2).
- Sección de errores comunes tomada de casos reales (nombre de autor no reconocido, institución o revista no encontrada, usuario bloqueado).
- Aclarar el efecto "foto" con un ejemplo.
- Mapa de equivalencias entre formularios SIGEVA y CVar.
- Plantillas de buenas prácticas de carga (consistencia de nombres de autor, palabras clave, archivos a texto completo).
- Contenido específico para docentes-investigadores (cargos docentes, categoría de Incentivos).
- Metadatos por página: fecha de verificación y versión del sistema, para detectar obsolescencia.

## 6. Propuesta de navegación (`mkdocs.yml`, borrador)
```yaml
site_name: SIGEVA-UNC — Guía para investigadores
theme:
  name: material
  language: es
nav:
  - Inicio: index.md
  - Primeros pasos:
      - Qué es SIGEVA y cómo se relaciona con CONICET y CVar: primeros-pasos/que-es.md
      - Crear usuario e ingresar: primeros-pasos/usuario.md
      - Roles: primeros-pasos/roles.md
  - Cargar tu CV:
      - Cómo funcionan las tablas y los formularios: cv/mecanica.md
      - Autores, palabras clave e instituciones: cv/campos-comunes.md
      - Datos personales: cv/datos-personales.md
      - Formación: cv/formacion.md
      - Cargos (docencia, I+D, gestión): cv/cargos.md
      - Antecedentes: cv/antecedentes.md
      - Producción científica: cv/produccion-cientifica.md
      - Producción tecnológica: cv/produccion-tecnologica.md
      - Producción artística: cv/produccion-artistica.md
      - Otros antecedentes: cv/otros.md
      - CV adjunto e impresión: cv/adjunto-impresion.md
  - Sincronizar datos: sincronizacion/index.md
  - Proyectos y trámites: proyectos-y-tramites/index.md
  - Preguntas frecuentes: faq.md
  - Glosario: glosario.md
  - Registro de cambios: cambios.md
```

## 7. Backlog sugerido para Claude Code (en orden)
1. Inicializar repo, `mkdocs.yml`, tema Material, CI de build (GitHub Actions) y despliegue.
2. Definir plantilla de página con front matter (`fuente`, `verificado_contra`, `fecha_verificacion`, `estado`).
3. **Obtener acceso al SIGEVA-UNC real** (cuenta del usuario) y relevar qué formularios existen hoy; sin esto, la brecha de la sección 4 es solo hipótesis.
4. Leer las páginas 248–257 del manual UBA (no leídas) y los demás documentos necesarios.
5. Redactar primero: Primeros pasos, mecánica de tablas, campos comunes, CV adjunto/impresión, sincronización.
6. Redactar secciones del CV en orden de uso docente-investigador: cargos, formación, producción científica.
7. Rehacer el relevamiento de otras universidades **solo si hace falta** y abriendo cada documento.
8. Relevar instructivos de facultades de la UNC (no verificados; ver sección 8).
9. Resolver licencias y publicar.

## 8. Preguntas abiertas
- ¿Tratamiento vos o usted?
- ¿El alcance incluye postulación a convocatorias (UBA lo incluye) o solo carga de CV (banco de datos)?
- ¿Se cubrirán los usos docentes de SIGEVA en la UNC (evaluación/carrera docente)? **No está verificado que la UNC lo use así**: el manual 2011 no lo trata y el relevamiento previo no es confiable. Hay que buscar instructivos de facultades y confirmarlo.
- ¿Qué convocatorias de la UNC se canalizan hoy por SIGEVA?
- Licencia del nuevo manual y resolución de la discrepancia de licencias de CONICET.
- ¿Quién valida el contenido (Prosecretaría de Informática, SeCyT-UNC)? Conviene contactarles para evitar duplicar y para posible adopción oficial.

## 9. Riesgos
- Documentar formularios que ya no existen o cambiaron (manual UNC de 2011).
- Reproducir contenido con licencia restrictiva.
- Datos personales en capturas.
