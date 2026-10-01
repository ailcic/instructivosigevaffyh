# Relevamiento del sistema real (SIGEVA-UNC)

- **Fecha:** 2026-09-30.
- **Sistema:** https://sigeva.unc.edu.ar — versión que muestra el pie de página: **13.2.16.2**.
- **Rol usado:** usuario banco de datos de actividades CyT.
- **Método:** navegación en solo lectura con la sesión del usuario (no se guardó, modificó, borró, compartió ni importó nada). No se registran datos personales: de las tablas solo se anotaron rótulos, encabezados y botones.
- **Alcance de esta pasada:** pantalla principal, pantalla de entrada de cada solapa, y las tres opciones de "Principal". **No** se abrieron todavía los submenús restantes ni los formularios de alta ("Nuevo"), así que los campos de cada formulario siguen sin relevar (salvo Identificación).

> **Nota del 2026-10-01.** Esta es la primera pasada. Los puntos 1, 2 (en su mayoría), 5, 6 y 8 de la sección 6 se relevaron después: ver `relevamiento-formularios.md`. «Experticia en CyT» resultó ser el equivalente de las «Áreas de actuación» del manual UBA.

## 1. Navegación general

Barra superior (solapas): **Principal · Datos personales · Formación · Cargos · Antecedentes · Producciones y servicios · Otros anteced. · Trámite**, más el botón **Cerrar sesión**. Debajo, una segunda barra con los submenús de la solapa activa.

| Solapa | Submenús (segunda barra) |
|---|---|
| Principal | Instructivos · Compartir forms. · Asignar colaborador |
| Datos personales | Identificación · Dirección residencial · Lugar de trabajo · Experticia en CyT |
| Formación | Formación académica · Formación complementaria |
| Cargos | Docencia · Cargos I+D · Cargos en gestión institucional · Otros cargos |
| Antecedentes | Formación de recursos humanos · Financiamiento CyT · Extensión · Evaluación · Otras actividades CyT |
| Producciones y servicios | Publicaciones · Des. tecnol., organizacionales y socio comunitarios · Prod. artística · Servicios · Prod. de bienes intensivos en conoc. |
| Otros anteced. | Redes, gestión editorial y eventos · Premios · Currículum |
| Trámite | (sin submenú) |

En varias solapas la segunda barra incluye además un ítem "Más ..." (no explorado).

## 2. Pantalla principal: inventario de secciones

La pantalla principal lista todas las secciones del banco de datos agrupadas, con una columna "Estado" (Con datos / …) o "Cant." (cantidad de registros) y enlace a cada una.

**Datos personales** (Estado): Identificación · Dirección residencial · Lugar de trabajo · Experticia en CyT.

**Formación**
- Formación académica: Nivel universitario de posgrado/doctorado · posgrado/maestría · posgrado/especialización · Nivel universitario de grado · Nivel terciario no universitario · Nivel medio · Nivel básico.
- Formación complementaria: Especialidad certificada por organismo/s de salud · Posdoctorado · Cursos de posgrado y/o capacitaciones extracurriculares · Idiomas · Estancias y pasantías.

**Cargos**
- Docencia: Nivel superior universitario y/o posgrado · Nivel terciario no universitario · Nivel básico y/o medio · Cursos de posgrado y capacitaciones extracurriculares.
- Cargos I+D: Cargos en organismos científico-tecnológicos · Categorización del programa de incentivos · Cargos de I+D en otro tipo de instituciones.
- Cargos en gestión institucional.
- Otros cargos.

**Antecedentes**
- Formación de recursos humanos en CyT: Becarios · Tesistas · Investigadores · Pasantes de I+D y/o formación académica · Personal técnico y de apoyo a la I+D.
- Evaluación: Evaluación de personal CyT y jurado de tesis y/o premios · Evaluación de programas/proyectos de I+D y/o extensión · Evaluación de trabajos en revistas CyT · Evaluación institucional · Otro tipo de evaluación.
- Financiamiento CyT: Proyectos de I+D · Proyectos de extensión, vinculación y transferencia · Proyectos de comunicación pública de CyT · Subsidios para eventos CyT · Subsidios para infraestructura y equipamiento · Becas recibidas.
- Otras actividades CyT: Operación y mantenimiento de sistemas de alta complejidad · Normalización · Ejercicio de la profesión en el ámbito no académico · Otra actividad CyT.
- Extensión: Comunicación pública de la ciencia y la tecnología · Extensión rural o industrial · Prestación de servicios sociales y/o comunitarios · Producción y/o divulgación artística o cultural · Otro tipo de actividad de extensión.

**Producciones y servicios**
- Publicaciones: Artículos publicados en revistas · Libros · Partes de libros · Trabajos en eventos C-T publicados · Tesis · Demás producciones C-T publicados · Informes técnicos.
- Producción artística: Musical-sonora · Visual · Audiovisual multimedial · Corporal teatral · Género literario narrativo · Género literario dramático, poético o ensayo · Género literario guión · Otro tipo de género literario.
- Desarrollos tecnológicos, organizacionales y socio-comunitarios: Desarrollo de productos, procesos productivos y sistemas tecnológicos · Desarrollo de procesos socio-comunitarios · Desarrollo de procesos de gestión empresarial · Desarrollo de procesos de gestión pública.
- Servicios.
- Producción de bienes intensivos en conocimiento.

**Otros antecedentes**
- Redes, gestión editorial y eventos: Participación u organización de eventos CyT · Trabajos en eventos C-T no publicados · Participación en redes temáticas o institucionales · Membresías en asociaciones C-T y/o profesionales · Coordinación de proyectos de cooperación académica o C-T · Gestión editorial.
- Premios y/o distinciones.
- Otros antecedentes: Curriculum vitae (Estado).

Al pie de la pantalla principal: **Compartir formularios** e **Imprimir currículum** ("Imprimir CV"; no se abrió).

## 3. Mecánica observada en las pantallas de lista

- Cada solapa abre una página con una tabla por tipo de registro (por ejemplo, en Docencia: una tabla por nivel).
- Cada tabla tiene un enlace **Nuevo** en el encabezado, acciones **Editar | Borrar** por fila y un botón **Importar** propio. Al pie de la página, **Salir**.
- Tabla vacía: muestra un mensaje de que no hay registros.
- Columnas vistas (encabezados):
  - Docencia: Fecha inicio · Fecha fin · Institución.
  - Formación académica: Fecha ingreso · Fecha egreso · Institución · Carrera.
  - Formación de RRHH: Año inicio · Año fin · Apellido y nombre · y, según la tabla, Tipo de beca · Institución del dirigido · Función · Tipo de tesis · Carrera · Ámbito institucional · Institución.
  - Publicaciones: Año · Título · y, según la tabla, Revista · Editorial · ISBN · Libro · Tipo de parte · Tipo evento · Evento científico · Fecha defensa/aprobación · Tesis · Institución · ISSN · Fecha inicio · Fecha fin · Disciplina. Hay una columna/acción **Precarga** (a ver en qué tabla y cómo funciona: candidata a ser la precarga por DOI/ISSN que documenta CONICET v4).
  - Redes, gestión editorial y eventos: Año · Evento · Tipo de evento · País · Título · Evento científico · Año inicio · Año fin · Alcance geográfico · Red · Asociación · Proyecto · Título de la revista.

## 4. Formularios vistos

**Identificación** (formulario único, botones Guardar / Salir). Campos, por nombre interno: nombre, apellido, apellido de casada, sexo (tres opciones), estado civil, cantidad de hijos, país de nacionalidad, condición de nacionalidad, tipo de documento, país de emisión del pasaporte, número de documento, CUIT/CUIL, país / provincia / partido de nacimiento (y "otro partido"), fecha de nacimiento, información adicional. Faltan relevar los rótulos visibles, cuáles son obligatorios y cuáles vienen bloqueados.

**Trámite** — título "Participación en una convocatoria". Un único campo **Código del trámite** (obligatorio), botones Aceptar / Salir y una nota con tres pasos (no transcripta). Coincide con el "vincularse a un proyecto con código" del manual UBA.

**Compartir formularios** — campos: Institución (obligatorio; **la única opción del desplegable es CONICET**), Contraseña y Confirmar contraseña (obligatorios); botones Compartir / Salir. El texto de la pantalla advierte que la operación autoriza de forma permanente la importación de los formularios con los datos cargados al momento en que se soliciten, y enlaza al instructivo de sincronización.

**Asignar colaborador** — tabla con columnas Rol · Apellido y nombre · Cuil · Fecha alta; enlace Nuevo; acciones Ver | Borrar por fila. El rol que figura es "Colaborador banco de datos de actividades CyT".

**Instructivos** — tres enlaces: Manual del Banco de Datos de Actividades CyT · Instructivo Navegación · Instructivo de sincronización. (No se abrieron: falta ver a qué documentos apuntan.)

## 5. Qué confirma respecto de la brecha (HANDOFF, sección 4)

Existen hoy en SIGEVA-UNC, aunque el manual UNC 2011 no los documenta:
- Datos personales separados en identificación / dirección residencial / lugar de trabajo, más **Experticia en CyT**.
- Formación complementaria (salud, posdoctorado, cursos, idiomas, estancias y pasantías) y niveles académicos de básico a doctorado.
- Cargos: docencia por nivel, cargos I+D (con Categorización del programa de incentivos), gestión institucional, otros cargos.
- Antecedentes: extensión, evaluación, becas recibidas (dentro de Financiamiento CyT), otras actividades CyT.
- Producción: tesis, demás producciones, informes técnicos, producción artística (8 subtipos listados), desarrollos tecnológicos/organizacionales/socio-comunitarios, servicios, bienes intensivos en conocimiento.
- Otros antecedentes: premios, eventos, trabajos en eventos no publicados, redes, membresías, cooperación, gestión editorial, CV adjunto.
- Trámite por código, asignación de colaborador, impresión del CV, sincronización (compartir e importar).

Diferencias con lo anotado de los manuales:
- "Áreas de actuación" (UBA) no aparece con ese nombre; lo más parecido es "Experticia en CyT" (a confirmar abriéndola).
- La estructura coincide más con la del portal SIGEVA-CONICET que con la del manual UBA: conviene reorganizar `mkdocs.yml` siguiendo las solapas reales (por ejemplo, "Producciones y servicios" como un solo bloque con cinco submenús, en lugar de científica / tecnológica / artística).
- El compartir desde la UNC solo ofrece CONICET como destino (consistente con la guía de sincronización de CONICET v2: entre dos instituciones que no son CONICET hay que pasar por SIGEVA-CONICET).

## 6. Pendiente de relevar

1. Formularios de alta ("Nuevo") de cada tabla: campos, obligatorios, desplegables, buscadores de instituciones/autores/revistas. Se puede abrir cada uno y salir sin guardar.
2. Submenús no abiertos: Dirección residencial, Lugar de trabajo, Experticia en CyT, Formación complementaria, Cargos I+D, Gestión institucional, Otros cargos, Financiamiento CyT, Extensión, Evaluación, Otras actividades CyT, los cuatro restantes de Producciones, Premios, Currículum.
3. "Más ..." de la segunda barra.
4. Pantalla de **Importar** (qué pide y qué instituciones ofrece) — mirar sin ejecutar.
5. **Imprimir CV**: opciones de selección de secciones y fechas.
6. Destino de los tres enlaces de Instructivos.
7. Pantalla de selección de rol tras el login y roles disponibles ("Usuario presentación/solicitud"), y pantallas previas al login (registro, recuperación de contraseña).
8. Columna "Precarga" de Publicaciones.
