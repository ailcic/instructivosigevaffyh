# Fuentes y estado de verificación

Fecha: 2026-09-30.

Leyenda de verificación:
- **Leído completo**: se abrió el documento y se leyó el texto extraído completo.
- **Leído parcial**: se abrió, pero el texto se cortó o faltan partes.
- **Solo fragmento**: se vio únicamente un extracto en resultados de búsqueda. No usar como fuente sin abrirlo.

## Manuales base del proyecto
| Fuente | URL | Estado |
|---|---|---|
| CONICET — Banco de Datos de Actividades CyT, v4 (ene. 2017) | https://sigeva.conicet.gov.ar/wp-content/uploads/2017/01/Manual-Banco-de-Datos-C-y-T_v4.pdf | Leído completo (texto, 26 pp. de PDF); imágenes no extraídas |
| UBA — Manual del Investigador SIGEVA, 7.ª ed. | https://cyt.rec.uba.ar/wp-content/uploads/Manual-del-investigador-SIGEVA.pdf | Índice y pp. 246–257 releídos del PDF local el 2026-09-30; el resto, según la lectura del chat previo (hasta p. 248). Releer cada sección al redactar |
| UNC — Manual del Usuario del Banco de Datos (2011) | https://www.unc.edu.ar/sites/default/files/manual-banco-datos.pdf | Leído completo |

## Páginas oficiales de CONICET
| Fuente | URL | Estado |
|---|---|---|
| Portal SIGEVA CONICET (módulos y formularios del CV) | https://sigeva.conicet.gov.ar/ | Leído |
| Documentación SIGEVA CONICET | https://sigeva.conicet.gov.ar/documentacion/ | Leído (inventario más abajo) |

### Inventario de la página de documentación de CONICET (guías listadas)
Guías de usuario: Sincronización de Datos del CV v2 (`.../2012/10/SIGEVA-Guia-de-Sincronizacion_v2.pdf`), Banco de Datos v4, Presentación de informe genérico v2, y manuales de evaluación (secretario, coordinador y miembro de comisión, par especialista, junta). Guías funcionales: Módulo de Memoria v1, Evaluación de Convocatorias v2, Gestión de Convocatorias v7, **Evaluación Docente** (`.../2012/10/SIGEVA-Modulo-Evaluacion-Docente-jun2012.pdf`), **Informe de Proyectos de Incentivos** (`.../2012/10/SIGEVA-Modulo-Informe-Incentivos.pdf`). Guías técnicas: requerimientos, actualización de versiones, batchs, migración de bases. Esta página también lista el módulo "Carrera docente" entre los objetos de evaluación soportados por SIGEVA. Útiles para el proyecto: la guía de sincronización v2 y la de Evaluación Docente (leídas el 2026-09-30, ver abajo) y la de Informe de Incentivos (no leída aún). Los PDF están bajo `https://sigeva.conicet.gov.ar/wp-content/uploads/`.

## Documentos abiertos y leídos el 2026-09-30 (Claude Code)
Descargados a `investigacion/fuentes-pdf/` y leídos completos (texto extraído con `pdftotext`; las capturas no se leen).

| Fuente | URL | Estado |
|---|---|---|
| UNC, Prosecretaría de Informática — Instructivo para creación de usuario y postulación en SIGEVA (concursos docentes; alojado en el sitio de Concursos de la FFyH), 8 pp. | https://sitio.ffyh.unc.edu.ar/concursos/wp-content/blogs.dir/148/files/sites/13/2022/05/SIGEVA-Instructivo-Postulacion.pdf | Leído completo |
| CONICET — Sincronización de datos del CV, Guía Usuario v2 (01/07/2015), 8 pp. | https://sigeva.conicet.gov.ar/wp-content/uploads/2012/10/SIGEVA-Guia-de-Sincronizacion_v2.pdf | Leído completo |
| CONICET — Instructivo para la Sincronización de Datos entre Instituciones Universidad–CONICET–CVAR, v1.0 (12/08/2013), 4 pp. | https://www.conicet.gov.ar/wp-content/uploads/InstructivoSincronizaci%C3%B3nUniv-Sigeva-CVar.pdf | Leído completo |
| FCM-UNC — Instructivo para generar Ficha Docente (2022), 5 pp. | https://fcm.unc.edu.ar/wp-content/uploads/2022/04/INSTRUCTIVO-PARA-GENERAR-FICHA-DOCENTE-1.pdf | Leído completo |
| CONICET — SIGEVA, Módulo Evaluación Docente (jun. 2012), 7 pp. Guía funcional; menciona a la UNC y la convocatoria "EV DOC 2012 CS ECONOMICAS" | https://sigeva.conicet.gov.ar/wp-content/uploads/2012/10/SIGEVA-Modulo-Evaluacion-Docente-jun2012.pdf | Leído completo |
| FCC-UNC — Instructivo Postulación SIGEVA (convocatoria 2025) | https://fcc.unc.edu.ar/wp-content/uploads/sites/9/2024/11/2.-Instructivo-Postulacion-SIGEVA-FCC-UNC-CD-2025.pdf | **No leído** (verificación anti-bots). Fuera de consideración en esta etapa por decisión del 2026-09-30 |
| FAUD-UNC — Instructivo CV en SIGEVA | https://faud.unc.edu.ar/files/INSTRUCTIVO-C-CV-en-Sigeva.pdf | **No leído** (verificación anti-bots). Fuera de consideración en esta etapa por decisión del 2026-09-30 |

### Qué aportan (datos de documento, aún no verificados contra el sistema)
- **Concursos docentes (instructivo UNC/FFyH):** autorregistro con datos como figuran en el DNI; el correo registrado funciona como domicilio electrónico y se cambia desde la solapa "Cambio de Datos" antes del cierre; a integrantes de la UNC se les pide correo IdUNC (@unc / @mi.unc); el CV se carga con el rol de banco de datos y la inscripción se hace con el rol "Usuario presentación/solicitud" (botón "Postular", "Lugar de Trabajo Propuesto", "Datos Académicos", archivos adjuntos, "Enviar Presentación"); una vez enviada no se puede corregir; cita la Resolución RHCS-2021-59-E-UNC-REC sobre el carácter de declaración jurada. Remite a un "Manual Banco de Datos CyT" por enlace (URL no recuperada del PDF).
- **Sincronización (CONICET v2, 2015):** dos etapas (compartir en origen, importar formulario por formulario en destino); "Compartir Formularios" está en la solapa "Principal"; la contraseña de sincronización es independiente de la de ingreso; entre dos instituciones que no son CONICET hay que pasar por SIGEVA-CONICET; lo importado se agrega sin duplicar registros iguales y, ante un registro modificado, queda el último modificado; CVar no admite archivos adjuntos; un colaborador designado también puede sincronizar; no hay migración masiva.
- **Ficha docente CONEAU (FCM):** cadena SIGEVA UNC → SIGEVA CONICET → CVar → CONEAU Global, tildando "Tengo una ficha creada en CVar" al crear la cuenta.
- **Evaluación docente (guía funcional CONICET, 2012):** el docente usa el rol de banco de datos (al CV se le "saca una foto" al presentar) y el rol de presentación/solicitud; una convocatoria por unidad académica; "Dato académico" con cargo, materia/área, legajo, resolución de designación, vencimiento, especialidad y comisión; adjuntos: plan de trabajo (obligatorio), informe y otros. Es de 2012: verificar vigencia en la UNC y si la FFyH lo usa.

## Sistema real
| Fuente | URL | Estado |
|---|---|---|
| SIGEVA-UNC, versión 13.2.16.2, rol de banco de datos | https://sigeva.unc.edu.ar | Relevado el 2026-09-30 y el 2026-10-01 en solo lectura. Notas en `relevamiento-sistema.md` y `relevamiento-formularios.md`; método en `metodo-relevamiento.md` |

### Documentos que el propio sistema enlaza (Principal → Instructivos)
Identificados por su dirección; **no abiertos ni leídos**.
- Manual del Banco de Datos de Actividades CyT, v2 (CONICET): `convocatorias.conicet.gov.ar/wp-content/uploads/sites/3/Manual-Banco-de-Datos-CyT_v2.pdf`. Es una versión anterior a la v4 ya leída.
- Guía de sincronización v2 (CONICET): `web.conicet.gov.ar/documents/16254/3597638/SIGEVA-Guia-de-Sincronizacion_v2.pdf`. Presumiblemente el mismo documento ya leído desde otra dirección.
- Instructivo de navegación: página interna del sistema (`instructivoBancoDeDatoNavOper.do`).

## Otros documentos abiertos
| Fuente | URL | Estado |
|---|---|---|
| Manual genérico CONICET antiguo (era SICyTAR), espejo en FAUD-UNMdP | https://faud.mdp.edu.ar/wp-content/uploads/2022/04/manual_banco_de_datos_10.pdf | Leído; no usado como base |
| Manual UNSAM (CONICET v. 2014) | https://noticias.unsam.edu.ar/wp-content/uploads/2014/02/Manual-Banco-de-Datos-C-y-T.pdf | Error 402 al abrir; no leído |

## Pistas de otras instalaciones (solo fragmento de búsqueda; NO verificadas)
Vistas en resultados de búsqueda del 2026-09-30. Abrir antes de citar.
- UNCuyo, manuales de postulación SIIP y becas (varias URLs bajo `uncuyo.edu.ar/ciencia_tecnica_y_posgrado/upload/`).
- UNL, instructivo para docentes de acreditación: https://www.fcv.unl.edu.ar/institucional/wp-content/uploads/sites/3/2018/11/ACREDITACIÓN_-INSTRUCTIVO-PARA-DOCENTES-.pdf
- UNMdP, guía de usuario del Banco de Datos: https://fca.mdp.edu.ar/wp-content/uploads/2025/06/05-Proyectos-UNMdP-2026-27-Manual-del-Usuario-SIGEVA.pdf
- UNICEN, instructivo de módulo de informe de Incentivos: https://secat.unicen.edu.ar/wp-content/uploads/2017/04/Instructivo-Sigeva-Modulo-Informe-Proyecto-de-Incentivos-1.pdf
- UNLP (Exactas), procedimiento SIGEVA-UNLP ↔ CONICET ↔ CVar: https://www.exactas.unlp.edu.ar/uploads/docs/manual_procedimientos_sigevaunlp_cvar.pdf
- Universidad Barceló, manual de usuario n.º 2 (carga de datos, 2025): https://www.barcelo.edu.ar/archivos/investigacion/Instructivo 2 - Carga datos 2025.pdf

## Copias locales
Los tres PDF base están en `investigacion/fuentes-pdf/` (fuera de git por licencias sin resolver). Texto extraíble con `pdftotext`.

## Descartado
El informe de la primera respuesta (relevamiento de ~30 universidades nacionales, con la afirmación de haber verificado enlaces) no estaba respaldado por documentos leídos. No usar ningún dato de ese informe. Las pistas de arriba son las únicas del relevamiento que tienen algún respaldo en esta conversación y solo como fragmentos.

`pistas-relevamiento-no-verificado.md` (informe de investigación automática guardado el 2026-09-30) se conserva únicamente como lista de enlaces a comprobar; sus propias advertencias indican que solo se abrieron tres de las fuentes.
