# Índice del proyecto — Manual de SIGEVA-UNC (SeICyT, FFyH)

Punto de entrada. Dice en qué estado está el proyecto y dónde está cada cosa.

**Última actualización:** 2026-10-01.

## Estado

| | |
|---|---|
| Versión del manual | **0.1**, redactada, en revisión |
| Rama de trabajo | `borrador/v0.1` (`main` conserva solo el esqueleto inicial) |
| Sistema relevado | SIGEVA-UNC 13.2.16.2, rol de banco de datos, 30/09 y 01/10 de 2026 |
| Compila | Sí: `mkdocs build --strict` sin errores |
| Publicado | No. Falta resolver licencia, revisar capturas y validar sugerencias |

### Hecho

- Comparación de los tres manuales base (CONICET v4, UBA 7.ª ed., UNC 2011).
- Relevamiento del sistema real: estructura, todos los formularios de alta del banco de datos, buscadores de institución y revista.
- Manual 0.1: 21 páginas y 17 capturas, organizado según las solapas reales del sistema.

### Pendiente inmediato (del responsable)

1. Revisar las capturas de `docs/assets/`.
2. Validar las «Sugerencias de la SeICyT» incluidas en el manual.
3. Definir criterio sobre el catálogo de instituciones de la FFyH.
4. Consultas a la UNC: repositorio institucional y correo de alta de instituciones.
5. Licencia.

Detalle en [`investigacion/bitacora.md`](investigacion/bitacora.md), sección «Asuntos que requieren decisión o gestión del responsable».

### Pendiente de relevar en el sistema

Lista completa en [`docs/cambios.md`](docs/cambios.md) («No verificado todavía») y en [`investigacion/relevamiento-formularios.md`](investigacion/relevamiento-formularios.md), sección 11. En resumen: ingreso y registro, validaciones al guardar, edición y borrado, importar y compartir, trámite con código real, impresión del CV, buscador de autores y formularios que son variantes de otros ya vistos.

### Próxima etapa

- **Postulación a becas y otras solicitudes** (rol «Usuario presentación/solicitud»). No empezada.
- Subáreas de la clasificación para Humanidades y Ciencias Sociales (Experticia en CyT).
- Relevamiento de instructivos de otras facultades de la UNC y de otras universidades, solo si hace falta y abriendo cada documento.

## Documentos sobre el proyecto

| Documento | Para qué sirve |
|---|---|
| [`CLAUDE.md`](CLAUDE.md) | Objetivo, alcance, audiencia y **reglas de trabajo**. Leer primero. |
| [`INDICE.md`](INDICE.md) | Este archivo: estado y mapa. |
| [`HANDOFF.md`](HANDOFF.md) | Contexto de origen (traspaso desde el chat), hallazgos iniciales, backlog original y riesgos. Histórico: varias preguntas ya están resueltas. |
| [`investigacion/bitacora.md`](investigacion/bitacora.md) | Pedidos, decisiones y resultados por sesión; autorizaciones vigentes para navegar el sistema; asuntos pendientes del responsable. |
| [`investigacion/metodo-relevamiento.md`](investigacion/metodo-relevamiento.md) | Cómo se relevó el sistema y cómo se tomaron y recortaron las capturas. |

## Material de investigación (no se publica)

| Documento | Contenido |
|---|---|
| [`investigacion/fuentes.md`](investigacion/fuentes.md) | Fuentes consultadas y su estado de lectura. |
| [`investigacion/comparacion-manuales.md`](investigacion/comparacion-manuales.md) | Comparación CONICET / UBA / UNC. |
| [`investigacion/relevamiento-sistema.md`](investigacion/relevamiento-sistema.md) | Primera pasada: solapas, pantalla principal, mecánica de listas. |
| [`investigacion/relevamiento-formularios.md`](investigacion/relevamiento-formularios.md) | Campos de cada formulario, buscadores, rarezas y pendientes. **Es la base de datos del manual.** |
| [`investigacion/pistas-relevamiento-no-verificado.md`](investigacion/pistas-relevamiento-no-verificado.md) | Solo una lista de enlaces a comprobar. No citar. |
| `investigacion/fuentes-pdf/` | PDF de terceros. Fuera de git por licencias; las direcciones están en `fuentes.md`. |

## El manual (`docs/`)

| Sección | Páginas | Respaldo |
|---|---|---|
| Inicio | `index.md` | — |
| Aspectos generales | `primeros-pasos/que-es.md`, `usuario.md`, `roles.md` | `usuario.md` sale solo de documentos; el resto, mixto |
| Banco de datos: generalidades | `cv/navegacion.md`, `cv/mecanica.md`, `cv/campos-comunes.md` | Sistema real (edición y borrado, de manuales) |
| Banco de datos: secciones | `cv/datos-personales.md`, `cv/experticia.md`, `cv/formacion.md`, `cv/cargos.md`, `cv/antecedentes.md`, `cv/publicaciones.md`, `cv/desarrollos-servicios.md`, `cv/produccion-artistica.md`, `cv/otros.md`, `cv/adjunto-impresion.md` | Sistema real, sin guardar |
| Compartir e importar | `sincronizacion/index.md` | Pantalla de compartir vista; procedimiento, de la guía del CONICET |
| Trámite | `proyectos-y-tramites/index.md` | Pantalla vista; confirmación y desvinculación, del manual UBA |
| Apoyo | `faq.md`, `glosario.md`, `cambios.md` | — |
| Plantilla de página | `_plantilla.md` | No se publica |
| Capturas | `assets/*.png` | Propias, recortadas |

Cada página declara en su encabezado `fuente`, `verificado_contra`, `fecha_verificacion` y `estado`.

## Cómo trabajar

```bash
python -m venv .venv && .venv/bin/pip install -r requirements.txt   # una vez
.venv/bin/mkdocs serve            # vista previa en http://127.0.0.1:8000
.venv/bin/mkdocs build --strict   # comprobación antes de un commit
```

- Ramas: `main` (publicable) y `borrador/*` (en redacción).
- Al cerrar una versión, registrar en `docs/cambios.md` qué se verificó contra el sistema y cuándo.
- Al terminar una sesión de trabajo, agregar una entrada en `investigacion/bitacora.md` y actualizar la sección «Estado» de este índice.
