# Relevamiento de formularios de alta (SIGEVA-UNC)

- **Fecha:** 2026-09-30. **Versión del sistema:** 13.2.16.2. **Rol:** usuario banco de datos de actividades CyT.
- **Método:** se abrió cada formulario "Nuevo" vacío y se salió sin guardar. Solo lectura; sin datos personales.
- Complementa `relevamiento-sistema.md` (estructura general).

**Convenciones de estas notas**
- `*` = campo marcado como obligatorio en pantalla.
- "→ opciones" = valores del desplegable tal como aparecen.
- **Buscador de institución**: bloque que se repite en casi todos los formularios. Tiene un campo de texto "Institución" con botón **Buscar**, y un campo "Institución seleccionada" (obligatorio) con botón **Limpiar**. Falta relevar cómo se ve el resultado de la búsqueda y qué pasa si la institución no existe.
- **Áreas de conocimiento**: bloque con dos desplegables encadenados (área y subárea) más un campo "Especialidad". Usa la misma clasificación de 6 grandes áreas que Experticia en CyT (ver sección 1).
- Las notas al pie numeradas de cada formulario están resumidas, no transcriptas.

---

## 1. Datos personales → Experticia en CyT

**Clave para el proyecto de visibilización de investigaciones de la SeICyT-FFyH.** Es un formulario único (no una tabla de registros), con botones Guardar / Salir y tres bloques:

1. **Resumen** `*` — texto libre. La ayuda en pantalla pide una descripción breve, en palabras propias, de la experticia del desarrollo profesional (técnicas que se dominan, campos de aplicación, etc.), de **hasta 1100 caracteres**.
2. **Áreas de actuación y líneas de investigación** `*` — tabla con botón Nuevo y Borrar por fila. Cada fila tiene:
   - **Área de actuación**: dos desplegables encadenados (área de 2 dígitos → subárea de 3 dígitos).
   - **Línea**: texto libre, máximo 150 caracteres.
   - La ayuda en pantalla indica: hasta **4 áreas de actuación**, en orden de relevancia, y hasta **3 líneas de investigación** por área.
3. **Palabras clave** — dos tablas con Nuevo / Borrar por fila: **Palabra clave en español** `*` y **Palabra clave en inglés** `*`. La ayuda pide un **mínimo de 3** en cada idioma, una por renglón.

**Clasificación de áreas** (primer desplegable, 48 opciones; coincide en estructura con la clasificación de campos de CyT de la OCDE — a confirmar la fuente oficial):
- 1 Ciencias Naturales y Exactas: 1.1 Matemáticas · 1.2 Ciencias de la Computación e Información · 1.3 Ciencias Físicas · 1.4 Ciencias Químicas · 1.5 Ciencias de la Tierra y relacionadas con el Medio Ambiente · 1.6 Ciencias Biológicas · 1.7 Otras Ciencias Naturales y Exactas
- 2 Ingenierías y Tecnologías: 2.1 Civil · 2.2 Eléctrica, Electrónica e Ingeniería de la Información · 2.3 Mecánica · 2.4 Química · 2.5 de los Materiales · 2.6 Médica · 2.7 del Medio Ambiente · 2.8 Biotecnología del Medio Ambiente · 2.9 Biotecnología Industrial · 2.10 Nanotecnología · 2.11 Otras Ingenierías y Tecnologías
- 3 Ciencias Médicas y de la Salud: 3.1 Medicina Básica · 3.2 Medicina Clínica · 3.3 Ciencias de la Salud · 3.4 Biotecnología de la Salud · 3.5 Otras Ciencias Médicas
- 4 Ciencias Agrícolas: 4.1 Agricultura, Silvicultura y Pesca · 4.2 Producción Animal y Lechería · 4.3 Ciencias Veterinarias · 4.4 Biotecnología Agropecuaria · 4.5 Otras Ciencias Agrícolas
- 5 Ciencias Sociales: 5.1 Psicología · 5.2 Economía y Negocios · 5.3 Ciencias de la Educación · 5.4 Sociología · 5.5 Derecho · 5.6 Ciencia Política · 5.7 Geografía Económica y Social · 5.8 Comunicación y Medios · 5.9 Otras Ciencias Sociales
- 6 Humanidades: 6.1 Historia y Arqueología · 6.2 Lengua y Literatura · 6.3 Filosofía, Ética y Religión · 6.4 Arte · 6.5 Otras Humanidades

**Subáreas vistas** (el segundo desplegable se carga según el primero; solo se vieron tres, sin modificar nada):
- 6.3 → 6.3.1 Filosofía, Historia y Filosofía de la Ciencia y la Tecnología · 6.3.2 Ética (excepto ética relacionada con subáreas específicas) · 6.3.3 Teología · 6.3.4 Estudios Religiosos · 6.3.5 Otras Filosofía, Étnica y Religión [sic]
- 5.3 → 5.3.1 Educación General (incluye capacitación, pedagogía y didáctica) · 5.3.2 Educación Especial · 5.3.3 Otras Ciencias de la Educación
- 6.5 → 6.5.1 Otras Humanidades

**Pendiente para Experticia:** listar las subáreas de 6.1, 6.2, 6.4 y de las áreas 5.x (las relevantes para la FFyH); confirmar si los topes (4 áreas, 3 líneas, 1100 caracteres) los valida el sistema o son solo indicación; ver si Experticia entra en "Compartir formularios" / Importar y en la impresión del CV.

---

## 2. Cargos

### 2.1 Docencia

**Nivel superior universitario y/o posgrado**
- Fecha inicio `*` · Fecha fin (solo si ya no se desarrolla la actividad)
- Buscador de institución `*`
- Cargo `*` (desplegable; aparece vacío hasta elegir institución — a confirmar) · existe un campo interno "otro cargo"
- Tipo de cargo `*` → Rentado · Ad Honorem
- Dedicación `*` → Exclusiva · Completa · Semi-exclusiva · Simple · Parcial · Otra
- Otra dedicación (solo si se eligió "Otra")
- Dedicación horaria semanal del cargo docente `*` → 40 horas o más · De 20 hasta 39 horas · De 0 hasta 19 horas
- Condición `*` → Regular o por concurso · Interino · Por contrato
- ¿Realiza actividades de investigación y desarrollo con este cargo docente? `*` Sí / No
- Nivel educativo de las actividades curriculares dictadas `*` (casillas): posgrado/doctorado · posgrado/maestría · posgrado/especialización · grado · posdoctorado
- **Actividades curriculares dictadas** `*`: tabla con Nuevo / Borrar; por fila, Nombre de la actividad curricular (obligatorio, máx. 150) y Profesor titular o responsable (opcional, máx. 150)
- Botones: Guardar / Volver

**Nivel terciario no universitario**
- Fecha inicio `*` · Fecha fin · Buscador de institución `*` · Cargo `*`
- Dedicación horaria semanal `*` (mismas tres franjas)
- Denominación de la carrera/tecnicatura `*`
- Tipo de formación `*` → Docente · Técnico-profesional

**Nivel básico y/o medio**
- Fecha inicio `*` · Fecha fin · Buscador de institución `*` · Cargo `*`
- Dedicación horaria semanal `*`
- Tipo de sistema de educación básica/media `*` → Educación general básica (E.G.B.) · Otro de nivel básico o medio · Polimodal · Primario · Secundario
- Otro tipo de sistema (solo si se eligió "Otro")

**Cursos de posgrado y capacitaciones extracurriculares**
- Fecha inicio `*` · Fecha fin · Buscador de institución `*`
- Cargo (no obligatorio) · Dedicación horaria semanal del cargo docente (no obligatorio)
- Nombre o temática del curso `*`
- Tipo de curso `*` → Curso · Otro · Seminario · Taller
- Carga horaria total del curso `*`

### 2.2 Cargos I+D

**Cargos en organismos científico-tecnológicos**
- Fecha inicio `*` · Fecha fin (solo cargos no vigentes o con fin conocido)
- Carrera `*` → Carrera de investigador científico y tecnológico (CONICET) · Carrera de investigador científico y tecnológico (CIC pcia. Bs. As.) · Otra
- Categoría `*` · Otro cargo/función `*` (presumiblemente según la carrera elegida — a confirmar)
- Buscador de institución `*`
- Dedicación horaria semanal `*`

**Categorización del programa de incentivos**
- Fecha inicio `*` · Fecha fin
- Año de categorización `*`
- Categoría en el Programa de Incentivos `*` → Categoría I a V
- Institución de categorización en el Programa: buscador de institución `*`

**Cargos de I+D en otro tipo de instituciones**
- Fecha inicio `*` · Fecha fin · Buscador de institución `*`
- Cargo para realizar I+D `*` · Dedicación horaria semanal `*`

### 2.3 Cargos en gestión institucional
- Fecha inicio `*` · Fecha fin · Buscador de institución `*`
- Cargo `*` → lista cerrada de 38 opciones (Asesor, Consejero, Coordinador, Decano, Director, Jefe de área, Jefe de departamento, Prosecretario, Rector, Secretario, Subsecretario, Vicedecano, Vicedirector, Vicerrector, varias categorías de técnico, Otro, etc.)
- Otro cargo (solo si se eligió "Otro")
- Tipo de función desempeñada `*` → Ejecutiva/Directiva · De coordinación · De asesoramiento especializado · De apoyatura técnica · Administrativa
- Dedicación horaria semanal `*`

### 2.4 Otros cargos
- Fecha inicio `*` · Fecha fin · Buscador de institución `*`
- Cargo `*` · Dedicación horaria semanal `*` · Categoría (no obligatorio)

---

## 3. Formación

### 3.2 Formación complementaria

**Especialidad certificada por organismo/s de salud**
- Situación de la formación `*` Completo / Incompleto
- Fecha de inicio `*` · Fecha de finalización (si "Completo")
- Tipo de formación incluida `*` → Residencia · Concurrencia · Acreditación de antigüedad en el ejercicio de la especialidad · Otro (+ campo "Otra")
- Especialidad `*` → lista de unas 45 especialidades médicas (+ "Otra")
- Certificado de especialidad Sí / No · Institución otorgante (buscador; si "Sí")
- Año de obtención de la última certificación `*`
- Institución en que realiza la formación: buscador de institución `*`
- Beca: ¿Realizó la especialidad con una beca de residencia? `*` Sí / No · institución financiadora (buscador)
- Informaciones adicionales (máx. 1000 caracteres)

**Posdoctorado**
- Fecha de inicio `*` · Fecha de finalización `*`
- Título del trabajo o proyecto de investigación
- Apellido y nombre del investigador anfitrión · Apellido y nombre del co-anfitrión
- Institución en que realiza o realizó el posdoctorado: buscador `*`
- Beca: ¿Realizó su posdoctorado con una beca? `*` Sí / No · institución financiadora (buscador)
- Áreas de conocimiento `*` · Especialidad `*`
- Informaciones adicionales (máx. 1000)

**Cursos de posgrado y/o capacitaciones extracurriculares**
- Situación del curso `*` Completo / Incompleto
- Fecha de inicio `*` · Fecha de finalización (si "Completo")
- Tipo de curso → Curso · Seminario · Taller · Otro (+ campo "Otro"). Una nota al pie lo condiciona a haber elegido el INTI como institución (revisar: parece una nota heredada)
- Denominación del curso `*`
- Carga horaria `*` → Hasta 24 horas · Entre 25 y 50 · Entre 51 y 100 · Entre 101 y 200 · Entre 201 y 359 · 360 horas o más
- Tipo de certificación final (si "Completo") → Certificado de asistencia · Certificado de aprobación
- Institución en que realiza o realizó el curso: buscador `*`
- Áreas de conocimiento `*` · Especialidad `*`
- Informaciones adicionales (máx. 1000)

**Idiomas**
- Idioma `*` → Español · Inglés · Portugués · Francés · Alemán · Italiano · Japonés · Chino · Ruso · Latín · Griego (moderno) · Otro (+ campo "Otro")
- Nivel de dominio del idioma `*` → Básico · Intermedio · Avanzado
- Certificado/s obtenido/s · Institución emisora del certificado · Año de obtención (texto libre, no obligatorios)
- Informaciones adicionales (máx. 1000)

**Estancias y pasantías**
- Fecha inicio `*` · Fin
- Tipo de tareas `*` → Tareas de investigación y desarrollo · Formación académica · Formación académica incluyendo tareas de I+D · Capacitación pre-profesional y/o profesional · Otro
- Tema del plan de trabajo `*` (no obligatorio para "Capacitación pre-profesional y/o profesional" u "Otro")
- Actividades realizadas y/o logros alcanzados `*` (casillas, se puede marcar más de una; 14 opciones: docencia, formación teórica, habilidades para conducir investigación, contactos con otros grupos, capacidades experimentales, acceso a fuentes especializadas, bases de datos, eventos científicos, publicaciones, redes, actividades de investigación, capacitación, otra…)
- Descripción de la actividad `*` (máx. 2000 caracteres)
- Instituciones ejecutoras/financiadoras `*`: tabla con buscador de institución y columnas Ejecuta / % Financia
- Director: nombre y apellido del director/tutor · institución (buscador) `*`
- Áreas del conocimiento `*` (máximo tres)

### 3.1 Formación académica

Las siete tablas (doctorado, maestría, especialización, grado, terciario, medio, básico) abren el mismo formulario con variantes según el nivel. Se abrieron tres: doctorado, grado y medio.

**Universitaria de posgrado/doctorado**
- Situación del nivel `*` Completo / Incompleto
- Fecha inicio `*` · Fecha de egreso (si "Completo")
- Denominación de la carrera `*` · Título `*`
- Número de resolución de acreditación del posgrado por CONEAU (no obligatorio)
- Instituciones otorgantes del título `*` (tabla con buscador: admite más de una)
- Tesis: título · porcentaje de avance (0 a 100, si "Incompleto") · apellido, nombre e institución del director/tutor · ídem codirector/co-tutor
- Beca: ¿Realizó su posgrado con una beca? `*` Sí / No · institución financiadora (buscador)
- Áreas de conocimiento `*` · Especialidad `*`
- Informaciones adicionales (máx. 1000)

**Universitaria de grado**
- Situación del nivel `*` · Fecha inicio `*` · Fecha de egreso (si "Completo")
- Denominación de la carrera `*`
- Obtención de título intermedio `*` Sí / No · Denominación del título intermedio (si "Sí")
- Título `*`
- Instituciones otorgantes del título `*`
- Tesina: título · porcentaje de avance (si "Incompleto") · apellido y nombre del director/tutor
- Áreas de conocimiento `*` · Especialidad `*`
- Informaciones adicionales (máx. 1000)

**Media**
- Situación del nivel `*` · Formación técnica `*` Sí / No
- Fecha inicio `*` · Fecha de egreso (si "Completo") · Título `*`
- Buscador de institución `*`
- Informaciones adicionales (máx. 1000)

Pendiente: variantes de maestría, especialización, terciario y básico (presumiblemente análogas).

---
## 4. Antecedentes

### 4.1 Formación de recursos humanos en CyT

En los cinco formularios, **Función desempeñada** `*` → Director o tutor · Co-director o co-tutor.

**Becarios**
- Año inicio `*` · Fin `*` (si la actividad sigue en curso, fecha estimada de finalización)
- Nombre becario `*` · Apellido becario `*`
- Institución de trabajo del becario: buscador `*` · Institución financiadora de la beca: buscador `*`
- Tipo de tareas `*` → Tareas de investigación y desarrollo · Formación académica · Formación académica incluyendo tareas de I+D · Capacitación pre-profesional y/o profesional
- Tipo de beca `*` → Posdoctorado · Postgrado/Doctorado · Postgrado/Maestría · Postgrado/Especialización · Formación de grado · Iniciación a la Investigación · Perfeccionamiento en la Investigación · Especialización · Práctica profesional · Otro tipo de beca de Investigación · Otro tipo de beca

**Tesistas**
- Año inicio `*` · Año defensa tesis `*` (si sigue en curso, fecha estimada)
- Nombre tesista `*` · Apellido tesista `*`
- Institución otorgante del título: buscador `*`
- Tipo de trabajo dirigido `*` → Tesis de Doctorado · Trabajo final, proyecto, obra o tesis de Maestría · Trabajo final de Especialización · Tesina o trabajo final de Grado
- Calificación obtenida (no obligatorio)

**Investigadores**
- Año inicio `*` · Fin · Nombre `*` · Apellido `*` · Institución de trabajo: buscador `*`
- Carrera `*` → CONICET · CIC pcia. Bs. As. · Otra
- Categoría `*` (nota en pantalla: si la carrera es CONICET y el año de inicio es posterior a 2008, no puede ser Adjunto) · Otro cargo/función

**Pasantes de I+D y/o formación académica**
- Año inicio `*` · Fin · Institución de trabajo del pasante: buscador `*`
- Nombre `*` · Apellido `*`
- Tipo de tareas `*` (mismas cuatro opciones que Becarios)
- Ámbito institucional `*` (solo para "Capacitación pre-profesional y/o profesional") → Organismo gubernamental de CyT · Entidad administrativa de gobierno · Universidad o instituto universitario estatal · ídem privado · Otra institución educativa no universitaria · Empresa · Entidad sin fines de lucro · Establecimiento asistencial de salud · Entidad internacional · Otro
- Tema del plan de trabajo `*`
- Nivel educativo del pasante `*` → grado · especialización · maestría · doctorado · posdoctorado

**Personal técnico y de apoyo a la I+D**
- Año inicio `*` · Fin · Institución de trabajo: buscador `*` · Nombre `*` · Apellido `*`
- Carrera `*` → Carrera del personal de apoyo (CONICET) · (CIC pcia. Bs. As.) · Otra
- Categoría `*` · Otro cargo/función (si "Otra")

### 4.2 Evaluación

Campos comunes: Año inicio `*` · Fin (solo si ya no se desarrolla) · Institución convocante: buscador `*` · **Rol evaluador** (solo si la institución convocante es CONICET) → Par consultor · Miembro de comisión asesora · Coordinador de comisión asesora · Coordinador alterno · Miembro de comité evaluación · País (lista de países) · Ciudad.

**Evaluación de personal CyT y jurado de tesis y/o premios**
- Tipo de personal evaluado `*` → Categorización docentes investigadores (Incentivos) · Evaluación de becarios · Evaluación de investigadores · Evaluación de personal de apoyo a la I+D · **Jurado de concursos docentes** · Jurado de premios · Jurado de tesinas, trabajos finales y/o tesis
- Descripción `*` (máx. 500; la ayuda sugiere detallar, por ejemplo para concurso docente, carrera, cargo, cátedra)

**Evaluación de programas/proyectos de I+D y/o extensión**
- Tipo de programas/proyectos evaluados (casillas, más de una): investigación básica · aplicada · desarrollo experimental o tecnológico · divulgación de información CyT · producción y/o divulgación artística o cultural · servicios sociales y/o comunitarios · extensionismo rural o industrial · programas de CTI · programas de extensión · otro
- Observaciones (máx. 500)

**Evaluación de trabajos en revistas CyT** (título en pantalla: "Gestión editorial y evaluación de trabajos en revistas CyT"; es el mismo formulario que abre "Gestión editorial" en Otros antecedentes)
- **Buscador de revista**: por ISSN / e-ISSN o por parte del nombre → Revista seleccionada `*`
- País `*` · Ciudad · URL · Año inicio `*` · Fin · Observaciones (máx. 500)

**Evaluación institucional**
- Tipo de evaluación institucional `*` → Actividades curriculares para instituciones universitarias · Evaluación de planes y/o políticas · Evaluación y/o acreditación de carreras de grado y postgrado · Proyectos institucionales o evaluación institucional externa
- Observaciones (máx. 500)
- Solo para "Evaluación de planes y/o políticas": ámbito del plan o política evaluado (casillas; mismos ámbitos institucionales que Pasantes) + "Otro ámbito"
- Solo para "Evaluación institucional externa": institución evaluada (buscador)

**Otro tipo de evaluación**
- Tipo evaluación `*` (texto libre) · Observaciones `*` (máx. 500); sin rol evaluador

### 4.3 Financiamiento CyT

**Proyecto de I+D** (las tablas Proyectos de I+D, de extensión/vinculación/transferencia y de comunicación pública abren el mismo formulario con otro tipo; solo se abrió el primero)
- Tipo de actividad de I+D `*` → Investigación básica · Investigación aplicada · Desarrollo experimental o tecnológico
- Denominación del proyecto `*` · Tipo de proyecto · Código de identificación (si corresponde)
- Fecha desde `*` · Hasta `*`
- Breve descripción del proyecto `*`
- Campo de aplicación `*` (lista de unas 280 opciones)
- Áreas de conocimiento `*` · Especialidad `*`
- Palabras clave `*` (la ayuda indica: en mayúscula y una por renglón)
- Moneda `*` → Dólares · Euros · Libras · Pesos · Monto total `*`
- **Entidades participantes** `*`: tabla con buscador y columnas Ejecuta · Evalúa · Adopta · Demanda · Promueve · % Financia. La ayuda en pantalla define cada rol; los porcentajes de financiamiento deben sumar 100 %.
- Director del proyecto `*` · Co-director del proyecto
- Función desempeñada `*` → Becario de I+D · Co-director · Director · Estudiante · Investigador · Personal técnico de apoyo
- Fecha de inicio de participación en el proyecto `*` · Fin `*`
- **Documentación de otorgamiento del proyecto** `*`: archivo adjunto, hasta 35 MB, preferentemente PDF (también .doc o .rtf; varios archivos en un .zip). La ayuda pide resoluciones, disposiciones, dictámenes o avales que contengan la aprobación.

**Subsidio para eventos CyT** (la tabla de infraestructura y equipamiento abre el mismo formulario con otro grupo; no se abrió)
- Tipo de subsidio `*` → para organización de eventos CyT · para asistencia a eventos CyT
- Actividad objeto del financiamiento `*` · Fecha desde `*` · Hasta `*` · Breve descripción `*`
- Moneda `*` · Monto total `*`
- Instituciones `*`: tabla con columnas Ejecuta · Evalúa · % Financia

### 4.4 Otras actividades CyT

**Operación y mantenimiento de sistemas de alta complejidad**
- Fecha inicio `*` · Fin
- Función desempeñada `*` (el desplegable muestra las mismas opciones que "Tipo de tareas": I+D · Formación académica · … · Otro) + "Otra"
- Tipo de sistema operado y/o mantenido `*` (casillas): máquinas y equipos productivos · equipos e instalaciones receptores, registradores y/o procesadores de información · Otro (+ campo)
- Denominación de la actividad · Descripción de las principales tareas (máx. 2000)
- Institución `*` (tabla con buscador)
- ¿Está vinculada con una red o sistema de información? `*` Sí / No → denominación de la red y alcance geográfico (Nacional / Internacional)

**Normalización**
- Fecha inicio `*` · Fin · Función desempeñada `*` (ídem) + "Otra"
- Tipo de tareas realizadas `*` (casillas; la misma lista de 14 actividades que Estancias y pasantías) + "Otro"
- Descripción de las principales actividades (máx. 2000) · Buscador de institución `*`

**Ejercicio de la profesión en el ámbito no académico**
- Fecha inicio `*` · Fin
- Área de ejercicio de la profesión `*` → 15 opciones (Física, química y afines · Matemática, estadística y afines · Informática · Arquitectura, ingeniería y afines · Ciencias biológicas… · Medicina y profesiones afines · Enfermería… · Organización y administración de empresas · Derecho · Bibliotecología y afines · **Ciencias sociales y humanas** · Artes · Técnicos y profesiones de nivel medio · Agricultura… · Fuerzas armadas)
- Función/Cargo `*` (ídem lista de tareas) + "Otra"
- Tareas realizadas `*` (casillas; según nota, solo para "Medicina y profesiones afines") + "Otras tareas realizadas"
- Descripción de la actividad (máx. 1000)
- Ámbito de desempeño `*` → Institucional · Trabajador independiente; buscador de institución `*`; País `*` y Provincia `*` solo para trabajador independiente

**Otra actividad CyT** (rareza: el título de la pantalla dice "Producción de bienes")
- Fecha inicio `*` · Fin · Tipo de actividad `*` (texto) · Función desempeñada · Descripción de la actividad (máx. 2000) · Buscador de institución `*`

**Beca recibida** (tabla "Becas recibidas", dentro de Financiamiento CyT)
- Fecha inicio `*` · Fin `*` (si sigue en curso, fecha estimada)
- Tipo de beca `*` (mismas 11 opciones que en Becarios) · Denominación de la beca `*`
- Tipo de tareas `*` (cuatro opciones)
- Institución de trabajo del becario: buscador `*` · Institución financiadora: buscador `*`
- Nombre y apellido del director `*` · Nombre y apellido del codirector
- Descripción (tema, plan de trabajo, tareas…) (máx. 2000)
- ¿Financia o financió un posgrado con esta beca? `*` No / Sí → Porcentaje de financiamiento `*` 25 % · 50 % · 75 % · 100 %

### 4.5 Extensión

**Comunicación pública de la ciencia y la tecnología**
- Denominación de la actividad `*` · Fecha inicio `*` · Fin
- Función desempeñada `*` → Co-organizador o co-coordinador · Conferencista/expositor/entrevistado individual · Integrante de equipo · Organizador o coordinador · Otra (+ campo)
- Descripción de la actividad `*` (máx. 2500)
- **Medios de divulgación** `*`: tabla (tres filas visibles) con Tipo de medio → Conferencia/debate público · Exposición · Prensa escrita · Radio · Televisión · Internet · Libro · CD · DVD · Videos · Centros, ferias y/o museos · Exhibiciones interactivas de CyT · Jardines zoológicos y botánicos · Granjas educativas · Encuentros · Otro; Nombre del medio; Lugar de realización; casilla "Part. periódica"
- Tipo de destinatario `*` (casillas): Público en general · Comunidad científica · Organizaciones sociales · Comunidad educativa · Sector productivo · Otros
- Fuente de financiamiento `*` (casillas): Ninguna · Fondos de la propia institución · Beneficiarios/destinatarios · Fondos externos · Otra (+ campo)
- Adjuntar archivo (hasta 35 MB, preferentemente PDF)

**Extensión rural o industrial**
- Denominación del proyecto o actividad `*` · Fecha inicio `*` · Fin
- Tipo de extensión `*` (Rural / Industrial) · Ámbito de extensión `*` (Rural / Periurbano / Urbano)
- Función desempeñada `*` → Director o coordinador · Co-director o co-coordinador · Integrante de equipo extensionista · Extensionista individual · Promotor · Otra
- Descripción `*` (máx. 2500) · Institución de trabajo: buscador `*`
- Tipo de acciones comprendidas `*`: tabla con 11 tipos de acción, lugar de realización y casilla "Part. periódica"
- Tipo de destinatario `*` (14 casillas) · Fuente de financiamiento `*`

**Prestación de servicios sociales y/o comunitarios**
- Fecha inicio `*` · Fin · Denominación de la actividad `*`
- Función desempeñada `*` → Organizador o coordinador · Co-organizador o co-coordinador · Integrante de equipo · Prestador individual del servicio · Otra
- Descripción `*` (máx. 1000) · Institución de trabajo: buscador `*` · Fuente de financiamiento `*`

**Producción y/o divulgación artística o cultural**
- Fecha inicio `*` · Fin · Denominación de la actividad `*`
- Función desempeñada `*` → Organizador o coordinador · Co-organizador o co-coordinador · Integrante de equipo · Actor/expositor individual · Otra
- Descripción `*` (máx. 1000) · Institución de trabajo: buscador `*`

**Otro tipo de actividad de extensión**
- Igual al anterior, con Función desempeñada `*` → Organizador o coordinador · Co-organizador o co-coordinador · Integrante de equipo · Otra

---

## 5. Producciones y servicios

Bloques que se repiten en esta solapa:
- **Autores** `*`: tabla con columnas Autores · Instituciones · Orden (cuatro filas visibles). La ayuda indica cargarlos en el orden en que figuran en la publicación. Falta relevar cómo se agregan filas, cómo se asocia la institución y cómo se marca el propio nombre.
- **Áreas del conocimiento y palabras clave** `*`: hasta tres áreas; palabras clave en mayúscula, una por renglón, en el orden e idioma de la publicación.
- **Resumen (o abstract)** `*`.
- **Full text o texto completo**: archivo de hasta 35 MB, preferentemente PDF (también .doc o .rtf). Si la publicación está en prensa, la nota pide un .zip con el trabajo y la constancia de que está en prensa.
- **Derecho de exclusión (OPT-OUT)**: desplegable con motivos (Confidencialidad · En vías de obtener un derecho de propiedad industrial · Acuerdos previos con terceros). La pantalla cita la Ley 26.899 y la Res. 753/16 del MinCyT: sirve para indicar que el texto completo no esté disponible en el Repositorio Institucional. **Importante para el manual**: implica que lo cargado puede ir al repositorio institucional (confirmar con la UNC cómo opera).
- Idioma → Español · Inglés · Portugués · Francés · Alemán · Italiano · Japonés · Chino · Ruso · Latín · Griego (moderno) · Otro.
- Soporte y/o medio de difusión `*` (Impreso / Electrónico y/o Digital; si es digital pide URL).

### 5.1 Publicaciones

**Artículos publicados en revistas** — "Nuevo" abre primero la pantalla **Precarga de Artículos**:
- Campo DOI / ISSN, botones **Precargar** y **Omitir**.
- Según el texto de la pantalla: con DOI, los metadatos se importan desde aplicaciones de Elsevier o Crossref; si el DOI no está indexado allí, el sistema intenta ubicar el mismo ítem ya autoarchivado en SIGEVA por un coautor. Con ISSN solo se completan los datos de revista y editorial. Lo precargado se puede editar (y al editar se pierde la carga estandarizada).
- Formulario de artículo (tras "Omitir"):
  - **Buscador de revista** por ISSN / e-ISSN o por parte del nombre → Revista seleccionada `*`
  - Editorial `*` · País de edición `*` · Ciudad de la editorial
  - Título del artículo `*` · Idioma `*` · Volumen · Tomo · Número · Página inicial · Página final
  - Fecha de publicación `*` (si está en prensa, año/mes en que entró en prensa)
  - URL · DOI (uno de los dos si el soporte es electrónico)
  - Referato `*` Sin referato / Con referato · Estado de publicación `*` Publicado / En prensa · Soporte `*`
  - Autores `*`: tabla con columnas Sel. · Autores · Instituciones · Orden · Mover; hay que seleccionar el propio nombre en la lista
  - Resumen `*` · Áreas y palabras clave `*`
  - Full text `*` + **Tipo de archivo** `*` → Post print · Versión final. La pantalla indica como preferente el post-print (versión aceptada, ya evaluada, sin logo comercial ni diagramación editorial)
  - OPT-OUT

**Libro**
- Título del libro `*` · ISBN `*` · Idioma `*` · Cantidad de volúmenes o tomos · Cantidad de páginas `*`
- Estado de publicación `*` Publicado / En prensa · Comité editorial/referato `*` No / Sí
- País de edición `*` · Ciudad de la editorial · Editorial `*` · Año de publicación `*` (si está en prensa, año en que entró en prensa)
- Soporte `*` · URL · Rol en la publicación `*` Autor / Editor-Compilador / Revisor
- Autores `*` · Áreas y palabras clave `*` · Resumen `*` · Full text (no marcado como obligatorio) · OPT-OUT

**Parte de libro**
- Tipo de parte de libro `*` → Capítulo de libro · Artículo de enciclopedia o anuario · Entrada de diccionario, glosario o repertorio biográfico · Prólogo o prefacio · Introducción · Epílogo o conclusión · Índice analítico · Nota al pie
- Título del libro `*` · Título de la parte `*` · ISBN `*` · Idioma `*` · Volumen · Tomo · Número
- Cantidad de páginas de libro `*` · Página inicial `*` · Página final `*` (obligatorias solo si está publicado)
- Estado `*` · Referato `*` · País de edición `*` · Ciudad · Editorial `*` · Año `*` · Soporte `*` · URL · Rol `*`
- Autores `*` · **Compiladores, editores u organizadores del libro** `*` (segunda tabla de personas) · Áreas y palabras clave `*` · Resumen `*` · Full text `*` · OPT-OUT

**Trabajo en eventos científico-tecnológicos publicados**
- Tipo de trabajo `*` → Artículo completo · Artículo breve · Resumen · Otro
- Título `*` · Idioma `*` · Tipo de publicación `*` (Libro / Revista) · Título de la revista/libro `*` · ISSN/ISBN
- País de edición `*` · Ciudad de la editorial `*` · Editorial `*` · Año `*` · Soporte `*` · URL
- Datos del evento: Nombre `*` · Tipo de evento `*` → Conferencia · Congreso · Simposio · Workshop · Taller · Jornada · Exposición · Feria · Mesa redonda · Seminario · Encuentro · Ronda de negocios · Otro · Alcance geográfico `*` Nacional / Internacional · País `*` · Ciudad · Fecha `*` · Institución organizadora
- Autores `*` · Áreas y palabras clave `*` · Resumen `*` · Full text `*` · OPT-OUT

**Tesis**
- Título `*` · Nivel educativo `*` (doctorado · maestría · especialización · grado · posdoctorado) · Buscador de institución `*`
- Título obtenido `*` · Fecha de defensa/aprobación `*` · Idioma `*` · Soporte `*` · URL
- Director de tesis `*` · Co-director de tesis
- Áreas y palabras clave `*` · Resumen `*` · Full text `*` · OPT-OUT

**Demás tipos de producción C-T publicada**
- Tipo de producción `*` → Traducciones publicadas como artículos en revistas · Traducciones publicadas como libros o partes de libros · **Reseñas bibliográficas** · Material didáctico sistematizado · Innovación pedagógica · Otro (+ campo)
- Título `*` · Idioma `*` · Año `*` · ISBN · ISSN · País `*` · Ciudad · Cantidad de páginas · Soporte `*` · URL
- Autores `*` · Áreas y palabras clave `*` · Resumen `*` · Full text `*` · OPT-OUT

**Informe técnico**
- Tipo del informe o memoria `*` · Características de la producción tecnológica referida `*`
- Tipo de producción tecnológica `*` (6 opciones + Otro) · Naturaleza `*` (Informática, Mecánica, Electrónica, Biológica, Psicológica, Organizacional, Social, Lingüística, Química, Otra)
- Soporte `*` · URL · Autores `*`
- Disciplina `*` (21 opciones; incluye "Filosofía, Psicología y Ciencias de la Educación", "Filología, Lingüística y Literatura", "Historia, Antropología y Geografía")
- Páginas · Porcentaje de participación en la autoría `*` · Moneda `*` · Monto percibido `*` · Fecha inicio `*` · Fecha finalización `*`
- Contacto si es confidencial · Destinatario · Tipo de institución financiadora `*` · % de participación en el financiamiento · Campo de aplicación `*`
- Archivo del informe técnico · OPT-OUT

### 5.2 Desarrollos tecnológicos, organizacionales y socio-comunitarios

Las cuatro tablas abren el mismo formulario con distinto tipo. Se abrió **Desarrollo de procesos socio-comunitarios** (en este formulario los obligatorios no aparecieron marcados en el texto extraído; revisar en pantalla):
- Tipo de desarrollo → Normas y regulaciones · Instrumentos de planificación, gestión y participación común · Sistemas de información · Planes de desarrollo · Modelo de gestión · Modelo de organización
- Denominación · Breve descripción (máx. 2000) · Año de referencia
- Descripción completa: archivo adjunto (PDF o .zip; admite planos, imágenes, etc.) · URL
- Área del conocimiento · Campo de aplicación · Especialidad · Palabras clave
- Autores (tabla con columnas Sel. · Autores · Instituciones · Orden · Mover; la ayuda pide seleccionar el propio nombre en la lista)
- Función desempeñada en el equipo → Director o responsable · Co-director o co-coordinador · Asesor o consultor individual · Investigador integrante · Técnico integrante · Organizador o coordinador · Becario
- Porcentaje de participación · Desarrollo con financiamiento Sí/No · Posee título con propiedad intelectual Sí/No · Transferencia de la producción Sí/No (cada "Sí" despliega más datos)
- OPT-OUT

### 5.3 Producción artística

Nueve tablas (la pantalla principal lista ocho; en la lista aparece además "otra"). Bloques comunes: Autores `*`; **críticas en medios** (¿Obtuvo críticas? `*` → medio, autor, año, país, cita); Áreas y palabras clave `*`.

**Musical-sonora**
- Tipo de producción `*` → Sonorización · Arreglo musical original · Composición musical original · Interpretación musical
- Tipo de sonorización `*` → Cine · TV · Video · Radio · Teatro · Danza · Instalación multimedia · Otro
- Medio `*` → vocales · electroacústicos · instrumentales · mixtos
- Título `*` · Año `*` · Soporte `*` · URL
- **Presentaciones**: Cantidad `*` (única / más de una) · Primera presentación `*` y Presentación más importante: Tipo de evento (Concierto o recital · Concurso · Creación · Exposición · Festival · Instalación · Muestra · Obra de teatro · Otro) · País · Año · Tipo de presentación (Colectiva / Individual) · Institución o establecimiento

**Visual**
- Tipo de producción visual `*` (casillas): Dibujo · Cerámica · Escultura · Fotografía · Escenografía · Instalación · Grabado · Dibujo de historieta · Pintura · Otro
- Título `*` · Año `*` · Presentaciones (igual que Musical-sonora)

**Género literario narrativo** (los cuatro géneros literarios comparten formulario)
- Tipo de género narrativo `*` → Cuento · Novela · Biografía · Otro
- Título `*` · Año `*` · Modo de divulgación `*` (Publicación / Representación)
- Datos de la publicación (si "Publicación"): Tipo `*` (Artículos de revistas · Libros · Partes de libros) · Título `*` · País `*` · ISBN/ISSN · Idioma `*` · páginas
- Representación (si corresponde): País · Ciudad · Año · Institución o establecimiento

No se abrieron: Audiovisual multimedial, Corporal teatral, los otros tres géneros literarios, "otra".

### 5.4 Servicios

**Servicio**
- Denominación `*` · Tipo de servicio `*` (12 opciones: asesoramientos, consultorías y asistencias técnicas · diagnósticos · ensayos · estudios de factibilidad · servicios bibliográficos y de bases de datos · … · Otro)
- Finalidad principal `*` (16 opciones) · Fecha de inicio `*` · Fin `*` · Modalidad `*` (eventual / permanente) · Descripción `*` (máx. 2000)
- Área del conocimiento `*` · Campo de aplicación `*` · Especialidad `*` · Palabras clave `*`
- Financiamiento `*` No / Sí → Moneda y Monto total
- Entidades participantes `*` (Ejecuta · Evalúa · % Financia) · Prestador/es del servicio `*` (tabla tipo autores)
- Función desempeñada `*` · Porcentaje de participación `*` · Modalidad de vinculación `*` → Asesoría técnica · Convenio de cooperación técnica · Convenio I+D · Servicios a terceros · STAN · Otro
- Destinatarios `*` (persona física / jurídica) · Certificado de calidad
- Documentación de prestación de servicio `*` (archivo: convenio, contrato o acuerdo; carta aval si es ad honorem)

### 5.5 Producción de bienes intensivos en conocimiento
- Fecha inicio `*` · Fin · Función desempeñada `*` (+ Otra) · Tipo de producto `*` (8 opciones + Otro)
- Denominación del producto · Denominación de la actividad · Descripción de las tareas (máx. 2000)
- Instituciones ejecutoras/financiadoras `*` · Destinatarios `*` (tipo, país, destinatario) · Áreas del conocimiento `*` (máx. tres)

---

## 6. Otros antecedentes

### 6.1 Redes, gestión editorial y eventos

**Participación u organización de eventos CyT**
- Nombre del evento `*` · Tipo de evento `*` (13 opciones, las mismas que en trabajos en eventos; + "Otro tipo de evento")
- Alcance geográfico `*` Nacional / Internacional · País `*` · Ciudad · Año `*`
- Modo de participación `*` (casillas): Asistente · Presentador de póster · Panelista · Conferencista · Organizador general · Miembro del comité organizador · Miembro del comité científico-tecnológico · Coordinador/moderador · Relator · Otro (+ campo)
- Institución organizadora `*` (tabla con buscador) · Informaciones adicionales

**Trabajo en eventos científico-tecnológicos no publicados**
- Título de trabajo `*` · Idioma `*`
- Datos del evento: Nombre `*` · Tipo `*` · Alcance geográfico · País `*` · Ciudad · Fecha `*` · Institución organizadora
- Autores `*` · Áreas y palabras clave `*` · Resumen `*` · Full text (no obligatorio) · OPT-OUT

**Participación en redes temáticas o institucionales**
- Año de inicio `*` · Año de finalización · Denominación de la red `*` · Alcance geográfico `*`
- Objetivo de la red `*` (9 casillas + "Otro") · Descripción de la actividad (máx. 1000) · Informaciones adicionales (máx. 1000)

**Membresías en asociaciones C-T y/o profesionales**
- Año de inicio `*` · Año de finalización · Denominación de la asociación `*` · Alcance geográfico `*`
- Modalidad de admisión → Invitación · Selección · Suscripción/inscripción · Otra (+ campo) · Informaciones adicionales (máx. 1000)

**Coordinación de proyectos de cooperación académica o C-T**
- Año de inicio `*` · Año de finalización · Denominación del proyecto y/o programa `*` · Alcance geográfico `*`
- Tipo de actividades `*` (mismas 9 casillas que "Objetivo de la red")
- Institución/es participante/s `*` (tabla con buscador y % Financia) · Áreas de conocimiento `*` (máx. tres) · Informaciones adicionales

**Gestión editorial**: abre el mismo formulario que "Evaluación de trabajos en revistas CyT" (ver 4.2).

### 6.2 Premios y/o distinciones
- Denominación del premio o distinción honorífica `*` · Categoría
- Tipo `*` → Individual (titular del CV) · Colectivo (grupo de I+D, empresa innovadora, grupo de productores/emprendedores, etc.)
- Alcance geográfico `*` · Año `*` · Institución otorgante: buscador `*` · Áreas de conocimiento `*` · Informaciones adicionales

### 6.3 Currículum (adjuntar archivos)
Pantalla "Adjuntar archivos": tabla "Tipos de archivos a adjuntar" con columnas Archivo adjunto y Fecha de alta; botones Importar, Limpiar y Salir. No se relevó en detalle (contiene el archivo del usuario).

---

## 7. Datos personales (resto)

**Dirección residencial** (formulario único; Guardar / Salir)
- Calle `*` · Número `*` · Piso · Oficina/Departamento
- País `*` · Provincia `*` · Partido/Departamento `*` (+ "Otro") · Localidad (+ "Otro") · Código postal `*` · Casilla postal
- Un grupo de cinco campos obligatorios sin rótulo propio en la fila (presumiblemente teléfono con prefijos — mirar en pantalla) · Teléfono celular · Fax
- E-mail `*` · URL · Informaciones adicionales

**Lugar de trabajo**: los mismos campos, precedidos por un buscador de institución `*`.

**Identificación**: ver `relevamiento-sistema.md`, sección 4.

---

## 8. Imprimir currículum

- Campos **Fecha desde** y **Fecha hasta** (opcionales).
- Árbol de casillas con todos los formularios del banco de datos, agrupados igual que en la pantalla principal, con enlaces Seleccionar todos · Deseleccionar todos · Expandir todos · Agrupar todos. **Incluye Experticia en CyT.**
- Botones: **Imprimir CV (pdf)** · **Imprimir CV (doc)** · Volver.
- La ayuda indica que, para obtener todo lo cargado, hay que dejar las fechas vacías y todos los formularios seleccionados.
- No se generó ningún CV.

## 9. Instructivos enlazados desde el sistema

| Enlace en pantalla | Destino |
|---|---|
| Manual del Banco de Datos de Actividades CyT | PDF en `convocatorias.conicet.gov.ar` (`Manual-Banco-de-Datos-CyT_v2.pdf`) — es decir, **el sistema de la UNC enlaza a un manual de CONICET (v2), no al manual UNC 2011** |
| Instructivo Navegación | página interna del sistema (`instructivoBancoDeDatoNavOper.do`) |
| Instructivo de sincronización | PDF en `web.conicet.gov.ar` (`SIGEVA-Guia-de-Sincronizacion_v2.pdf`) |

Ninguno de los tres se abrió ni se leyó en esta pasada.

## 10. Rarezas y posibles errores del sistema (para la FAQ o para reportar)

- "Otra actividad CyT" abre un formulario cuyo título dice "Producción de bienes".
- En Sistemas de alta complejidad, Normalización y Ejercicio de la profesión, el desplegable "Función desempeñada" / "Función/Cargo" muestra la lista de "Tipo de tareas" (I+D, formación académica…), y Normalización reutiliza la lista de actividades de Estancias y pasantías.
- En Cursos (formación complementaria) una nota condiciona "Tipo de curso" a haber elegido el INTI como institución.
- Erratas en pantalla: "Posdoctorardo", "Indentificación", "comisón", "Otras Filosofía, Étnica y Religión".
- Entrar a un formulario escribiendo la dirección a mano (sin pasar por el enlace "Nuevo") devuelve en varios casos una "Página de errores"; no tiene efecto sobre los datos.

## 11. Pendiente

1. **Importar**: no se pulsó el botón (regla de solo lectura); falta saber qué pantalla abre y qué pide.
2. **Buscador de autores**: no se probó (ver sección 12 para institución y revista).
3. Formularios no abiertos por ser variantes de uno ya visto: maestría, especialización, terciario y básico (formación académica); proyectos de extensión y de comunicación pública, subsidios de infraestructura (financiamiento); los otros tres desarrollos; audiovisual, corporal-teatral, tres géneros literarios y "otra" (producción artística).
4. Subáreas (tercer nivel) de la clasificación de áreas para Humanidades y Ciencias Sociales.
5. Qué campos condicionales se habilitan o bloquean al elegir cada opción, y qué valida el sistema al guardar (no se puede ver sin guardar; habría que usar un registro de prueba con autorización expresa).
6. "Más ..." de la segunda barra; "Instructivo Navegación"; selección de rol al ingresar; pantallas previas al login.
7. Formularios de edición de registros existentes (Editar): se supone que son iguales a los de alta.

## 12. Buscadores (búsqueda de prueba, 2026-09-30)

Se ejecutó una búsqueda en cada uno desde un formulario "Nuevo" vacío y se salió sin seleccionar ni guardar.

### 12.1 Buscador de instituciones

Probado desde Otros cargos, con el texto "filosofia y humanidades".

- Al pulsar **Buscar** el sistema sale del formulario y abre la pantalla **Búsqueda de instituciones**, con el texto ya cargado.
- **Filtro**: País · Provincia · Tipo de institución (Organismo gubernamental de CyT · Entidad administrativa de gobierno · Universidad o instituto universitario estatal · ídem privado · Otra institución educativa no universitaria · Empresa · Entidad sin fines de lucro · Establecimiento asistencial de salud · Entidad internacional) · Institución (texto). Botones Buscar y Volver.
- **Resultados**: lista paginada de a 20 (la búsqueda de prueba dio 96 registros; la ayuda dice que se muestran hasta 300). Cada resultado es una ruta jerárquica con los niveles separados por `\`, por ejemplo universidad \ facultad \ unidad. La búsqueda encontró el texto sin tildes y devolvió instituciones de varias universidades y países.
- **Navegación por niveles**: al hacer clic en un resultado, ese nivel pasa a "Institución seleccionada", aparece el botón **Seleccionar** y debajo se listan sus dependencias (nivel siguiente), que a su vez se pueden abrir. La ayuda indica: ubicar el nivel que corresponde, hacer clic en él y pulsar Seleccionar.
- **Si la institución no está**: al pie hay un bloque "Solo en caso de no encontrar la institución en la búsqueda, ingrese otra", con País `*`, Provincia `*` (obligatoria solo para Argentina), Tipo de institución `*` (cuando no hay nivel elegido) y un campo de texto para el nivel nuevo; botón **Ingresar otra**. Si ya se eligió un nivel, los niveles superiores quedan fijos y se escribe solo el siguiente. No se usó.
- La ayuda en pantalla da además un correo de la UNC para pedir la incorporación de un nivel faltante (`lugardetrabajo@sigeva.unc.edu.ar`, asunto "Lugar de Trabajo", con los datos completos de la unidad). Verificar que siga vigente antes de publicarlo en el manual.
- **Dato relevante para la FFyH**: bajo UNIVERSIDAD NACIONAL DE CORDOBA \ FACULTAD DE FILOSOFIA Y HUMANIDADES el sistema lista 17 dependencias (áreas, cátedras, centros, departamentos, escuelas, institutos, biblioteca). La lista parece desactualizada respecto de la estructura actual de la Facultad (por ejemplo, incluye una Escuela de Psicología). Conviene que la SeICyT la revise y defina qué nivel recomendar a quienes cargan, y si corresponde pedir altas o correcciones.

### 12.2 Buscador de revistas

Probado desde "Evaluación de trabajos en revistas CyT", por nombre, con el texto "filosofia". Es el mismo buscador del formulario de artículos.

- Dos criterios, cada uno con su botón: **Buscar por ISSN / e-ISSN** y **Buscar por Nombre** (alcanza una parte del nombre).
- Abre la pantalla "Seleccione la revista…" con una tabla ordenable: Nombre · Editorial · ISSN · e-ISSN · Sel. (botón de opción). La búsqueda de prueba dio 36 registros en una sola página. Varias filas no tienen editorial y algunas no tienen ISSN; hay títulos repetidos con distinto ISSN, así que conviene identificar la revista por ISSN.
- Se marca la fila y se pulsa **Seleccionar**; **Volver** regresa al formulario.
- **Si la revista no está**: al pie, "Solo en caso que no haya podido seleccionar una revista, ingrese otra", con Nombre revista `*`, ISSN y e-ISSN para cargarla a mano. No se usó.

## 13. Agregados del 2026-10-01 (al tomar capturas)

- **Trámite**: la nota 2 de la pantalla dice que, al incorporarse al trámite, el sistema saca una foto de los datos y que las actualizaciones posteriores no se reflejan en el trámite actual. El efecto "foto" queda así **confirmado en el texto de SIGEVA-UNC** (antes solo documentado por la UBA). Sigue sin probarse con un código real.
- **Tabla de autores (artículos)**: columnas Nuevo/Borrar · Sel. (botón de opción) · Autores · Instituciones (con botón Buscar) · Orden · Mover (flechas). Empieza con una fila.
- **Resumen (artículos)**: hay un botón "Limpiar resumen o abstract".
- **Proyecto de I+D**: Director y Co-Director se cargan con Apellido · Nombre · CUIT/CUIL/PAS; el monto tiene parte entera y decimales separadas; el adjunto se sube con un botón "Adjuntar".
- **Capturas**: guardadas en `docs/assets/`, recortadas para excluir el encabezado (nombre de usuario y fecha). Al desplazarse, el sistema muestra un encabezado compacto fijo que también lleva el nombre; quedó fuera del recorte.
