# Bitácora del proyecto

Registro cronológico de pedidos, decisiones y resultados de las sesiones de trabajo con Claude Code. Sirve para retomar el proyecto sin depender del historial de la consola.

- Los pedidos del responsable del proyecto se citan textualmente («…»).
- No se registran datos personales ni contenido del CV usado para relevar el sistema.
- El estado vigente está en [`../INDICE.md`](../INDICE.md); acá queda el camino recorrido.

---

## Etapa previa (chat, antes del repositorio)

Resumida en [`../HANDOFF.md`](../HANDOFF.md): comparación de los tres manuales base (válida) y un relevamiento de ~30 universidades que quedó **descartado** por no estar respaldado en documentos leídos.

## 2026-09-30 — Arranque en Claude Code

Antes de esta bitácora (commit `040f94f`, «Estructura inicial del manual de SIGEVA-UNC»):

- Decidido: tratamiento *vos*; alcance v1 = CV + sincronización + trámites FFyH; verificación navegando el sistema real en solo lectura.
- Se leyeron y registraron en `fuentes.md` el instructivo de concursos de la UNC, las dos guías de sincronización del CONICET, el instructivo de ficha docente de la FCM y la guía funcional de evaluación docente.
- Se creó el esqueleto MkDocs con páginas en blanco.

---

## 2026-09-30 — Sesión de relevamiento del sistema

### 1. Acceso al sistema

> «ya deberías poder acceder con mi sesión iniciada en https://sigeva.unc.edu.ar/eva//indexBancoDatos.do»

- Se accedió con la sesión del usuario mediante la extensión de Chrome, rol «Usuario banco de datos de actividades de CyT». Versión del sistema: 13.2.16.2.
- Primera pasada, solo lectura: pantalla principal, entrada de cada solapa y las tres opciones de **Principal**.
- Resultado: [`relevamiento-sistema.md`](relevamiento-sistema.md).
- Hallazgos: la brecha del HANDOFF (sección 4) se confirma casi entera; la estructura real difiere del `mkdocs.yml` borrador; **Compartir formularios** solo ofrece CONICET; **Trámite** es un campo de código; «Áreas de actuación» (UBA) no existe con ese nombre.

### 2. Formularios de alta

> «sí, abrí cada "Nuevo" y salí sin guardar, el campo de "Expercitica en CyT" es muy importante para el proyecto de visibilización de investigaciones de la SEICyT-FFyH.»

- **Autorización ampliada:** abrir formularios «Nuevo» vacíos y salir sin guardar.
- **Prioridad declarada:** el formulario **Experticia en CyT** es clave para el proyecto de visibilización de investigaciones de la SeICyT-FFyH. Debe tener tratamiento destacado en el manual.
- Se abrieron los formularios de alta de todas las solapas (uno por grupo cuando varias tablas comparten formulario) y se anotaron campos, obligatorios, opciones de listas y notas.
- Resultado: [`relevamiento-formularios.md`](relevamiento-formularios.md), secciones 1 a 11.
- Hallazgos: bloque OPT-OUT / repositorio institucional (Ley 26.899) en todas las producciones; precarga de artículos por DOI/ISSN; Imprimir CV con selección de secciones, fechas y salida PDF o DOC; los instructivos del sistema enlazan a documentos del CONICET, no al manual UNC 2011; «Jurado de concursos docentes» está en Evaluación de personal CyT; varias rarezas del sistema.
- No se pulsó **Importar** (queda fuera de la regla de solo lectura).

### 3. Buscadores

> «sí, hacé la búsqueda de prueba sin guardar»

- **Autorización ampliada:** escribir un texto de prueba en los buscadores y ejecutar la búsqueda, sin seleccionar ni guardar.
- Se probaron el buscador de instituciones («filosofia y humanidades», 96 resultados) y el de revistas («filosofia», 36 resultados).
- Resultado: `relevamiento-formularios.md`, sección 12.
- Hallazgo para la SeICyT: bajo UNC \ Facultad de Filosofía y Humanidades el catálogo lista 17 dependencias y parece desactualizado.

### 4. ¿Alcanza para una primera versión?

> «tenemos suficiente por ahora para una primera versión del instructivo que replique en la medida de lo posible el manual de la UBA pero con los detalles aprendidos del sistema UNC? En otra ocasión seguiremos con el módulo de postulación a BECAS y otros solicitudes.»

- Respuesta: sí para la carga del CV; sincronización, ingreso y trámites solo parcialmente, marcados como pendientes.
- **Decisión de alcance:** la postulación a becas y otras solicitudes (rol de presentación) queda para una etapa posterior.

---

## 2026-10-01 — Redacción de la versión 0.1

> «tomá capturas de los formularios vacíos mientras redactás, luego las modificaré si veo que tienen datos personales, sigamos las solapas reales del sistema. Sigamos la estructera y cobertura del manual de la UBA pero con redacción propia, de manera similar a lo que fue el manual de 2011 de la universidad.»

**Decisiones:**

- Las capturas son de formularios vacíos; el responsable las revisa y modifica si encuentra datos personales.
- La navegación del manual sigue las solapas reales del sistema.
- Estructura y cobertura del manual de la UBA, redacción propia, en la línea del manual UNC 2011.

**Hecho:**

- Rama `borrador/v0.1`.
- Relectura de las secciones generales del manual UBA (1–3.7, 3.14, 3.15, 5) y del manual UNC 2011 (índice, introducción, compartir/importar) desde los PDF locales.
- 17 capturas en `docs/assets/`.
- 21 páginas redactadas; `mkdocs.yml` reorganizado; `produccion-cientifica.md` → `publicaciones.md`, `produccion-tecnologica.md` → `desarrollos-servicios.md`; páginas nuevas `cv/navegacion.md` y `cv/experticia.md`.
- `mkdocs build --strict` sin errores; anclas internas comprobadas contra el sitio generado.
- Hallazgo nuevo: la pantalla **Trámite** de la UNC declara en sus notas el efecto «foto».

> «verifica que no haya contenido importante para continuar el proyecto que esté sólo en la consola y no en los .md del proyecto; de paso puedes crear un índice como lugar de entrada para saber el estado del proyecto, los documentos acerca del proyecto (como la bitacora que tiene los mensajes que estén acá). Luego de esto creamos con gh cli el remoto en ailcic/intstructivosigevaffyh, commit y push.»

- Se crearon esta bitácora, [`../INDICE.md`](../INDICE.md) y [`metodo-relevamiento.md`](metodo-relevamiento.md) con lo que estaba solo en la consola.
- Se actualizaron `HANDOFF.md`, `fuentes.md` y `relevamiento-sistema.md` para que no contradigan el estado actual.

---

## Autorizaciones vigentes para navegar el sistema

Acumuladas a lo largo de las sesiones. Cualquier cosa fuera de esta lista requiere pedir permiso de nuevo.

| Permitido | No permitido |
|---|---|
| Navegar todas las pantallas con la sesión del usuario | Guardar, modificar o borrar registros |
| Abrir formularios «Nuevo» vacíos y salir sin guardar | Pulsar **Importar** o **Compartir** |
| Ejecutar búsquedas de prueba en los buscadores, sin seleccionar | Usar «Ingresar otra» en los buscadores |
| Poner campos en blanco en pantalla (sin guardar) para capturar | Ingresar un código en **Trámite** |
| Capturar formularios vacíos | Registrar datos personales en notas o capturas |

## Asuntos que requieren decisión o gestión del responsable

1. **Revisar las capturas** de `docs/assets/` por si quedó algún dato personal.
2. **Validar las «Sugerencias de la SeICyT»** del manual: las redactó Claude como propuesta y se van a leer como criterio de la Secretaría (nivel institucional a elegir, un registro por cargo, uso de «Consejero», orden de carga, etc.).
3. **Catálogo de instituciones de la FFyH:** revisar las 17 dependencias que lista el sistema, definir qué nivel recomendar y si corresponde pedir altas o correcciones.
4. **Repositorio institucional:** averiguar con la UNC cómo opera el envío de textos completos (bloque OPT-OUT) antes de recomendar qué versión subir.
5. **Correo `lugardetrabajo@sigeva.unc.edu.ar`:** confirmar que sigue vigente antes de publicarlo en el manual.
6. **Licencia** del manual y discrepancia de licencias del CONICET (ver `CLAUDE.md`).
7. **Validación institucional:** contacto con la Prosecretaría de Informática y la SeCyT-UNC (pregunta abierta del HANDOFF).
