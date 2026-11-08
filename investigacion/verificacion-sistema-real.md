# Verificación contra SIGEVA-UNC (sistema real)

Registro de lo observado navegando https://sigeva.unc.edu.ar con la sesión del usuario, en **solo lectura**. Sin datos personales ni cantidades de registros de la cuenta.

## Sesión 2026-11-08

### Pantalla de ingreso (`/auth/`)
- Izquierda: «Identificación de Usuario», campos **Usuario** y **Contraseña**, botón **Ingresar**. Debajo: enlace «Si olvidó su contraseña presione aquí» y contador de usuarios conectados.
- Derecha: «Recomendaciones». Incluye: servicio exclusivo para usuarios registrados; enlace para no registrados («Si usted no es un usuario registrado, haga click aquí»); el nombre de usuario es el elegido al registrarse; evitar que otros vean el teclado; acceder desde una PC conocida.
- **Bloqueo:** al 5.º intento fallido el usuario queda bloqueado automáticamente; hay un enlace para obtener una nueva contraseña; si persiste, escribir a `consultas@sigeva.unc.edu.ar`.
- Pie: «Desarrollado por CONICET».
- Captura propia: **pendiente** (requiere sesión cerrada o ventana privada).

### Pantalla de roles (`/auth/menu.jsp`)
- Mensaje de bienvenida con fecha y hora del último acceso, y aviso: si no fuiste vos, cambiar la contraseña y avisar a `consultas@sigeva.unc.edu.ar`.
- Tabla «Seleccione para operar»: columnas SISTEMA / ROL. Sistema: «Sistema Integral de Gestión y Evaluación». Roles vistos en esta cuenta: Usuario banco de datos de actividades de CyT; Usuario presentación/solicitud; Colaborador banco de datos de actividades CyT; además un rol administrativo propio de esta cuenta (no generalizable).
- No se revisaron todavía las opciones «Cambio de Contraseña» / «Cambio de Datos».

### Banco de datos — Principal (`/eva/indexBancoDatos.do`)
- Encabezado: nombre de la persona y fecha arriba a la derecha.
- Menú superior: **PRINCIPAL · DATOS PERSONALES · FORMACIÓN · CARGOS · ANTECEDENTES · PRODUCCIONES Y SERVICIOS · OTROS ANTECED. · TRÁMITE** y botón **CERRAR SESIÓN**.
- Submenú de la Principal: **INSTRUCTIVOS · COMPARTIR FORMS. · ASIGNAR COLABORADOR**.
- Columnas: **Estado** («Con datos»/«Sin datos») en ítems de registro único; **Cant.** en ítems con varios registros.
- Estructura completa (agrupada como en pantalla):
  - **Datos personales:** Identificación; Dirección residencial; Lugar de trabajo; Experticia en CyT.
  - **Formación** — *Formación académica:* Nivel universitario de posgrado/doctorado; …/maestría; …/especialización; Nivel universitario de grado; Nivel terciario no universitario; Nivel medio; Nivel básico. *Formación complementaria:* Especialidad certificada por organismo/s de salud; Posdoctorado; Cursos de posgrado y/o capacitaciones extracurriculares; Idiomas; Estancias y pasantías.
  - **Cargos** — *Docencia:* Nivel superior universitario y/o posgrado; Nivel terciario no universitario; Nivel básico y/o medio; Cursos de posgrado y capacitaciones extracurriculares. *Cargos I+D:* Cargos en organismos científico-tecnológicos; Categorización del programa de incentivos; Cargos de I+D en otro tipo de instituciones. *Cargos en gestión institucional.* *Otros cargos.*
  - **Antecedentes** — *Formación de recursos humanos en CyT:* Becarios; Tesistas; Investigadores; Pasantes de I+D y/o formación académica; Personal técnico y de apoyo a la I+D. *Evaluación:* Evaluación de personal CyT y jurado de tesis y/o premios; Evaluación de programas/proyectos de I+D y/o extensión; Evaluación de trabajos en revistas CyT; Evaluación institucional; Otro tipo de evaluación. *Financiamiento CyT:* Proyectos de I+D; Proyectos de extensión, vinculación y transferencia; Proyectos de comunicación pública de CyT; Subsidios para eventos CyT; Subsidios para infraestructura y equipamiento; Becas recibidas. *Otras actividades CyT:* Operación y mantenimiento de sistemas de alta complejidad; Normalización; Ejercicio de la profesión en el ámbito no académico; Otra actividad CyT. *Extensión:* Comunicación pública de la ciencia y la tecnología; Extensión rural o industrial; Prestación de servicios sociales y/o comunitarios; Producción y/o divulgación artística o cultural; Otro tipo de actividad de extensión.
  - **Producciones y Servicios** — *Publicaciones:* Artículos publicados en revistas; Libros; Partes de libros; Trabajos en eventos C-T publicados; Tesis; Demás producciones C-T publicados; Informes técnicos. *Producción artística:* Musical-sonora; Visual; Audiovisual multimedial; Corporal teatral; Género literario narrativo; Género literario dramático, poético o ensayo; Género literario guión; Otro tipo de género literario. *Desarrollos tecnológicos, organizacionales y socio-comunitarios:* Desarrollo de productos, procesos productivos y sistemas tecnológicos; Desarrollo de procesos socio-comunitarios; Desarrollo de procesos de gestión empresarial; Desarrollo de procesos de gestión pública. *Servicios.* *Producción de bienes intensivos en conocimiento.*
  - **Otros antecedentes** — *Redes, gestión editorial y eventos:* Participación u organización de eventos CyT; Trabajos en eventos C-T no publicados; Participación en redes temáticas o institucionales; Membresías en asociaciones C-T y/o profesionales; Coordinación de proyectos de cooperación académica o C-T; Gestión editorial. *Premios y/o distinciones.* *Otros antecedentes:* **Curriculum vitae** (con Estado).
  - Al pie de la Principal: **Compartir formularios** e **Imprimir currículum / Imprimir CV**.

### Tablas (ejemplo: Formación complementaria, `bcoFormacionComplementariaLista.do`)
- Una pantalla por subsolapa, con una tabla por ítem. Cada ítem tiene un **texto explicativo** arriba de la tabla.
- **Importar**: botón arriba a la derecha de cada ítem (lleva a `bcoImportarFormulario.do`).
- **Nuevo**: en la primera celda del encabezado de la tabla.
- **Editar | Borrar**: enlaces a la izquierda de cada registro.
- Columnas ordenables (flechas en el encabezado). Pie: «N registros, mostrando todos los registros» o «No se encontraron registros».
- Botón **Salir** al pie de la pantalla.

### Formulario nuevo (ejemplo: Cursos de posgrado y/o capacitaciones extracurriculares)
- Obligatorios con **asterisco rojo**.
- Campos condicionales con llamadas numeradas «(1)», «(2)»… explicadas en un recuadro debajo del bloque.
- Institución: campo de búsqueda con botón **Buscar**, «Institución seleccionada» con botón **Limpiar**.
- Áreas del conocimiento: dos selectores encadenados, con enlace **Borrar** a la izquierda.
- «Informaciones adicionales»: máximo 1000 caracteres.
- Botones al pie, a la derecha: **Guardar** y **Volver**.
- **Editar** (abierto, no enviado): botones **Modificar** y **Volver**.
- **Borrar**: no se cliqueó. El flujo (formulario de confirmación con **Eliminar** y **Volver**) se tomó del *Instructivo Navegación* interno del sistema (ver abajo).

### Instructivos (`instructivoConvocatoriaGral.do`)
- Tres enlaces: «Manual del Banco de Datos de Actividades CyT» (PDF en convocatorias.conicet.gov.ar), «Instructivo Navegación» (interno: `instructivoBancoDeDatoNavOper.do`) e «Instructivo de sincronización» (PDF en web.conicet.gov.ar). No hay instructivos propios de la UNC.

### Instructivo Navegación (interno del sistema; capturas de 2011)
- Secciones: Menú; Pantalla Principal; Guardar; Operatividad de formularios; Validación; Autores; Sesión.
- Guardar: si se pasa de una pantalla a otra sin Guardar, se pierden los cambios; **Salir** vuelve a la Principal.
- Alta/edición/baja: Nuevo → Guardar/Volver; Editar → Modificar/Volver; Borrar → formulario de confirmación con **Eliminar**/Volver.
- Validación: obligatorios con asterisco rojo; si faltan, «Error de validación: debe corregir el/los siguiente/s error/es antes de seguir:» en rojo arriba del formulario. Si el registro no pasa la validación, el archivo adjunto hay que volver a seleccionarlo.
- Autores: hay instrucciones para el ingreso de autores (búsqueda con más de 3 caracteres). Pendiente de leer completo para `campos-comunes.md`.
- **Sesión:** se cierra tras **4 horas de inactividad**; puede cerrarse por error grave o si se supera el **límite de 20 MB** de archivos enviados.

### Técnica de capturas
- Zoom de página 0,76 (solo en el navegador) para que el formulario entre en una pantalla; ventana de 1080×794.
- Enmascarado solo en el DOM: nombre del encabezado (`div#persona`, que un script de la página reescribe: hace falta un `MutationObserver`), cantidades de la Principal a 0 y celdas de registros reemplazadas por «Ejemplo».
- Recorte con `PIL`, PNG sin cuantizar (la cuantización borra el naranja de la subsolapa activa).
- Capturas en `docs/assets/`: `cv-principal-arriba.png`, `cv-principal-abajo.png`, `cv-tabla-registros.png`, `cv-formulario-nuevo.png`.

### Datos personales (relevado solo por etiquetas; ningún valor registrado)
- Cuatro formularios únicos, botones **Guardar** y **Salir**. Barra negra: IDENTIFICACIÓN · DIRECCIÓN RESIDENCIAL · LUGAR DE TRABAJO · EXPERTICIA EN CYT.
- **Identificación**: *Datos básicos* (Nombre/s*, Apellido/s*, Apellido/s de casada, Sexo* [Masculino / Femenino / No binario/Indeterminado], Estado civil*, Cantidad hijos, Nacionalidad*, (1) Condición nacionalidad* [Nativo / Naturalizado / Por opción]); *Documento de identidad* (Tipo*, (2) País emisión pasaporte, Número*, (3)(4) CUIT/CUIL*); *Datos de nacimiento* (Fecha*, País*, Provincia*, Partido/Departamento, (5) Otro); *Información adicional* (máx. 500). Notas: (1) solo si nacionalidad argentina; (2) solo si pasaporte; (3) con pasaporte el CUIT/CUIL puede omitirse; (4) CUIT/CUIL con guiones, ej. 20-12345678-0; (5) solo si «Otro» partido. **No hay campo de legajo.** No hay campos de correo ni usuario.
- **Dirección residencial**: Calle*, Número*, Piso, Oficina/Departamento, País*, Provincia*, (1) Partido/Departamento* (obligatorio solo si Argentina), (2) Otro, Localidad, (3) Otro, Código postal*, Casilla postal, Teléfono* (país, área, característica, número, interno), Teléfono celular, Fax, E-mail*, URL; Informaciones adicionales (máx. 500).
- **Lugar de trabajo**: Institución (Buscar) + Institución seleccionada* (Limpiar); aviso: si no se encuentra, escribir a `lugardetrabajo@sigeva.unc.edu.ar`, asunto «Solicito nuevo lugar de trabajo», cuerpo con Organismo / Dependencia / Departamento / Área. *Detalles* idénticos a la dirección residencial (E-mail*, URL optativa).
- **Experticia en CyT**: Resumen* (textarea sin tope técnico ni contador; leyenda «Hasta 1100 caracteres»); Áreas de actuación y líneas de investigación* (filas con Nuevo/Borrar: dos selectores encadenados —gran área/disciplina, p. ej. «1 CIENCIAS NATURALES Y EXACTAS», «6.5 Otras Humanidades», y subdisciplina, p. ej. «6.3.1 …»— y campo Línea de 150 caracteres; leyenda: hasta 4 áreas en orden de relevancia y hasta 3 líneas por área → **DECIDIR**); Palabras clave* en español y en inglés (filas con Nuevo/Borrar, sin límite indicado).
- Capturas: `cv-lugar-de-trabajo.png`, `cv-experticia.png` (campos vaciados en el DOM).

### Producciones › Publicaciones: lista y formulario Nuevo de Libro
- Enlaces **Nuevo** de la lista: Artículos → `bcoPrecargarArticulo.do` (pantalla de **precarga**, por revisar para `produccion-cientifica.md`); Libro, Parte de libro, Tesis, Demás producciones e Informe técnico → formularios directos.
- **Libro (Nuevo)** — *Datos básicos:* Título*, ISBN* («Acerca de ISBN»), Idioma*, Cantidad de volúmenes, Cantidad de páginas*, Publicado/En prensa*, (radio No/Sí sin etiqueta legible)*, País de edición*, Ciudad de la editorial, Editorial*, (1) Año de publicación*; *Soporte:* Impreso / Electrónico y/o Digital, (2) URL; rol* Autor / Editor-Compilador / Revisor (casillas).
- **Autores:** tabla Nuevo | Autores | Instituciones (+ Buscar) | Orden; 4 filas con Borrar; **sin flechas para mover**; leyenda «Deberán ingresarse en el orden en el que figura en publicación». Un único campo de institución por fila.
- **Áreas del conocimiento (Máximo tres)***: filas con dos selectores encadenados.
- **Palabra clave***: leyenda «(En mayúscula y una por renglón. En el orden e idioma de la publicación).»; 4 filas, Nuevo/Borrar. → **DECIDIR**.
- **Resumen (o abstract)***: editor enriquecido, botón «Limpiar resumen o abstract»; leyenda: puede ser copia del enviado a la editorial, en el idioma de la publicación; con caracteres especiales (∑ ξ ∫) se recomienda copiar del editor original (p. ej. Word). → **DECIDIR** (contradice el consejo de pegar texto plano).
- **Full text:** «Tamaño máximo del archivo 35 (treinta y cinco) MegaBytes», «Preferentemente con formato .pdf, eventualmente se aceptan .doc o .rtf», botón Adjuntar. Nota EN PRENSA: adjuntar un .zip con la publicación y la constancia de que está en prensa, en el mismo campo. → contradice los **20 MB** del Instructivo Navegación: **DECIDIR** en `mecanica.md`.
- **Derecho de exclusión (OPT-OUT):** Confidencialidad / En vías de obtener un derecho de propiedad industrial / Acuerdos previos con terceros.
- Botones Guardar / Volver. El formulario se abandonó sin guardar.

### Búsqueda de instituciones (`bcoBuscarOrganizacion…`; búsqueda de prueba «Filosofia y Humanidades»)
- Es una pantalla completa (no una ventana emergente). *Filtro de búsqueda de institución:* País, Provincia, Tipo de institución [Organismo gubernamental de CyT / Entidad administrativa de gobierno / Universidad o instituto universitario estatal / … privado / Otra institución educativa no universitaria / Empresa / Entidad sin fines de lucro / Establecimiento asistencial de salud / Entidad internacional], (1) Institución (500 caracteres), Buscar; Volver.
- Nota (1): hasta 300 resultados; se navegan los niveles jerárquicos con clic; al llegar al nivel, clic y **Seleccionar**. Si no está el nivel: correo a `lugardetrabajo@sigeva.unc.edu.ar`, asunto «Lugar de Trabajo», con universidad, facultad, departamento o instituto, domicilio, correo institucional, fax y teléfono. (El formulario de Lugar de trabajo da otro asunto: «Solicito nuevo lugar de trabajo». Discrepancia menor, documentada en cada página según su pantalla.)
- Resultados de a 20, con la ruta completa («UNIVERSIDAD NACIONAL DE CORDOBA \ FACULTAD DE FILOSOFIA Y HUMANIDADES»). Al hacer clic: «Institución seleccionada», botón **Seleccionar** y lista de niveles inferiores (17 para FFyH: áreas, cátedras, centros, departamentos, escuelas, institutos).
- Carga manual: «Solo en caso de no encontrar la institución en la búsqueda, ingrese otra»: País*, (2) Provincia* (solo si Argentina), Tipo de institución* [Entidad administrativa de gobierno / Otra institución educativa no universitaria / Empresa / Entidad sin fines de lucro / Establecimiento asistencial de salud / Entidad internacional], **Nivel 1*** (55 caracteres); botón **Ingresar otra**. Resuelve el «nivel 3» de FCE: es **Nivel 1**.
- Capturas: `cv-autores-palabras-clave.png`, `cv-busqueda-institucion.png`, `cv-institucion-niveles.png`.

### Otros anteced. › Currículum
- Barra negra de Otros anteced.: REDES, GESTIÓN EDITORIAL Y EVENTOS · PREMIOS · CURRÍCULUM.
- **Adjuntar archivos** (`bcoCArchivosAdjuntos.do`): «Seleccione los archivos para adjuntar»; tabla Tipos de archivos a adjuntar | Archivo adjunto | Fecha de alta; fila «Curriculum vitae» con botón **Limpiar** (submit; **no se cliqueó**). Botones **Importar** y **Salir**. Con un archivo ya cargado no hay campo para elegir uno nuevo: el alta y los formatos quedan **pendientes**.
- **Imprimir currículum** (`filtroImprimirCurriculum.do`): Fecha desde / Fecha hasta; «Imprimir los formularios seleccionados» con árbol de 6 secciones (179 casillas, todas marcadas por defecto); enlaces Seleccionar todos | Deseleccionar todos | Expandir todos | Agrupar todos; leyenda: para imprimir todo, fechas vacías y todos los formularios seleccionados. Botones **Imprimir CV (pdf)**, **Imprimir CV (doc)** y **Volver**. No se generó ningún CV. (Errata del sistema: «Indentificación».)
- Capturas: `cv-adjunto.png` (nombre de archivo y fecha reemplazados), `cv-imprimir.png`.
