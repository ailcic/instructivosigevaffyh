# Armonización de instructivos (UBA, UNC 2011, CONICET e instructivos UNC 2019–2026)

Fecha: 2026-11-06. Material de trabajo: no se publica. Registra, tema por tema, qué dice cada fuente, dónde no coinciden y qué criterio adopta el manual. Las claves de fuente están definidas en `fuentes.md`.

## Reglas de armonización

1. **Lo más reciente sobre la UNC manda sobre lo viejo.** Si un instructivo UNC 2024–2026 o un taller con demostración en pantalla (2026) contradice al manual UNC 2011 o al UBA, el manual sigue a la fuente reciente y deja la discrepancia anotada.
2. **Dos fuentes recientes independientes que coinciden** cuentan como «documentado». Una sola fuente reciente cuenta como «documentado, una fuente». Nada de esto equivale a «verificado contra el sistema»: todas las páginas siguen en `pendiente_verificar` hasta la verificación en SIGEVA-UNC.
3. **Criterio de carga ≠ comportamiento del sistema.** Lo que recomiendan las bibliotecas o los talleres (dónde conviene cargar algo, cómo escribir un título) se presenta como criterio de esas áreas, no como regla del sistema.
4. **Cuando dos criterios chocan**, el manual muestra ambos, indica cuál adopta y por qué, y lo marca para consultar a soporte o a la SeICyT.
5. **Nada de los talleres que identifique a participantes** pasa al manual.

## 1. Estructura actual del banco de datos

El sistema actual **no tiene la estructura del manual UNC 2011**. Coinciden en la estructura nueva FAUD-2025, FCE-2024, Taller-1 y Taller-2 (con demostración en pantalla).

| Solapa (nombre actual) | Contenido según fuentes recientes | Diferencia con UBA 7.ª ed. |
|---|---|---|
| Principal | Lista de todas las secciones con columnas «Estado» (con datos / sin datos) y «Cant.»; acceso a «Compartir formularios» e «Imprimir CV» (FAUD-2025, Taller-2) | UBA: igual (3.2.1) |
| Datos personales | Identificación, lugar de trabajo, experticia en CyT (resumen, áreas, palabras clave en español e inglés) (Taller-1). Dirección residencial: no se menciona; se asume que sigue | UBA no tiene experticia |
| Formación | Académica (niveles de básico a doctorado) y complementaria (posdoctorado, cursos de posgrado y/o capacitaciones extracurriculares, idiomas) (FAUD-2025, Taller-2) | UBA suma «especialidad certificada por organismos de salud»: no confirmada en UNC |
| Cargos | Docencia (por nivel), I+D, gestión institucional, otros cargos (Taller-1, Taller-2, FAUD-2025) | Igual |
| Antecedentes | Formación de RRHH en CyT, Financiamiento CyT (con becas adentro), Extensión, Evaluación, Otras actividades (FAUD-2025, Taller-1, Taller-2) | UBA tiene «Becas» y «Áreas de actuación» como ítems aparte |
| Producción y servicios | Publicaciones; Desarrollo tecnológico, organizacional y sociocomunitario; Producción artística; Servicios; Producción de bienes intensivos en conocimiento (FAUD-2025) | UBA: «Producción» con científica / tecnológica / artística |
| Publicaciones (dentro de Producción y servicios) | Artículos publicados en revistas; Libros; Partes de libros; Trabajos en eventos C-T publicados; Tesis; Demás tipos de producción C-T publicada; Informes técnicos (FCE-2024, Taller-2) | En UBA «Trabajos en eventos no publicados» está en Producción científica e «Informes técnicos» en Producción tecnológica |
| Otros antecedentes | Participación u organización de eventos C-T; Trabajos en eventos C-T no publicados; Redes temáticas o institucionales; Membresías; Coordinación de proyectos de cooperación; Gestión editorial; Premios y distinciones (Taller-1, Taller-2, FCE-2024 p. 65, FO) | UBA: premios, eventos, membresías (con redes y coordinación adentro), archivos adjuntos |
| CV adjunto | Existe un lugar para subir un CV en archivo (Taller-1, Taller-2). Ubicación exacta: no documentada | UBA: Otros antecedentes > Archivos adjuntos |

**Decisión:** la navegación del manual sigue la estructura actual. Los nombres exactos de solapas y subsolapas quedan para verificar en pantalla.

## 2. Temas con acuerdo entre fuentes

| Tema | Criterio adoptado | Fuentes |
|---|---|---|
| Un único usuario por persona (CUIL) | No crear un segundo usuario; recuperar el viejo y cambiar el correo | Taller-1, Taller-2 |
| Correo | Recomendado el institucional; algunas unidades lo exigen (IdUNC) | Taller-1, UNC-concursos-2022 |
| Roles | Banco de datos (CV), Presentación/solicitud (trámites), Miembro comisión (solo si te designan) | Encuentro I diap. 5, Taller-1, FAUD-2025 |
| Presentación toma los datos del banco | Cargar primero el banco; la presentación los levanta | Taller-1, Taller-2, UBA 4.2 |
| Efecto «foto» | Al presentar o asociarte se copia el banco; cambios posteriores no se reflejan | UBA 3.14 y 4.2, CONICET evaluación docente 2012 |
| Campos obligatorios | Asterisco rojo; sin ellos no guarda | UBA 3.4, Taller-2 |
| Nuevo / Editar / Borrar / Guardar / Volver | Mecánica de tablas | UBA 3.4, FAUD-2025 |
| Sesión que expira | Guardar seguido | FAUD-2025, Taller-1 |
| Autores | Todos, en el orden de la publicación, uno por fila, «Apellido, Nombre» | UBA 3.5, FCE-2024, FCE-pautas, FO |
| Precarga de artículos por DOI/ISSN, botón «Omitir» | Existe en SIGEVA-UNC | FCE-2024 pp. 16–17, Taller-1, Taller-2 (demostración) |
| Revista o institución que no aparece | Carga manual en el pie de la ventana de búsqueda («Ingresar otra») | FCE-2024, Taller-1, Taller-2, UBA 3.7 |
| Lo cargado a mano no se acumula | Cada vez hay que volver a ingresar la revista o institución manual | Taller-2 |
| Texto completo | PDF, máximo 35 MB | FCE-2024, Taller-2 |
| En prensa | Un .zip con el texto y la constancia de aceptación de la editorial | FCE-2024, Encuentro I diap. 16, Taller-1, Taller-2 |
| Envío sin evaluar | No se carga hasta que sea aceptado | Taller-2 |
| Ponencia publicada | Publicaciones > Trabajos en eventos C-T publicados | FCE-2024, FO, Taller-2 diap. 3 |
| Ponencia no publicada | Otros antecedentes > Trabajos en eventos C-T no publicados | FCE-2024 p. 65, Taller-2 diap. 4 |
| Un evento, varios roles | Un solo registro y se marcan todos los roles | Taller-1, Taller-2 diap. 5, UBA 3.13.2 |
| Reseñas | Demás tipos de producción C-T publicada; nunca como artículo | FO diap. 8, 15 |
| Material didáctico | Demás tipos de producción C-T publicada (notas de cátedra; no presentaciones de clase) | Taller-2 diap. 4 y grabación, FO diap. 11 |
| Agradecimientos | No se cargan | Taller-2 diap. 4 |
| Un cargo docente = un registro | Varias asignaturas del mismo cargo van en «actividades curriculares dictadas» | Taller-2 diap. 6 |
| Interinatos | Fecha de inicio y fin vacía mientras siga; si cambia la situación de revista, registro nuevo | Taller-1, Taller-2 diap. 7 |
| Ascenso de cargo | Registro nuevo por cada cargo | Taller-2 |
| Carrera docente | No tiene formulario | Taller-2 diap. 7 |
| Formación en curso | Se carga incompleta con grado de avance; no se cargan aparte los cursos que forman parte de la carrera | Taller-1 |
| FRRHH | Solo si vos sos responsable (director/a de tesis, beca, adscripción, integrante de equipo) | Taller-2 |
| Financiamiento | Solo actividades con financiamiento competitivo; no honorarios | Taller-1 |
| Becas | Dentro de Financiamiento CyT | Taller-1, Taller-2, FAUD-2025 |
| Evaluación como jurado de concurso o selección docente | Antecedentes > Evaluación > Otro tipo de evaluación | Taller-2 |
| Gestión institucional | Secretarías, direcciones, consejos, coordinaciones, representaciones | Taller-2 |
| Sincronización | UNC → CONICET → CVar → CONEAU Global; compartir en origen, importar ítem por ítem en destino; contraseña propia de la operación; entre universidades se pasa por CONICET | Taller-2 diap. 13 y grabación, Taller-1, CONICET-sinc-v2, FCM-2022, UBA 3.3 |
| Cada plataforma tiene su usuario | SIGEVA-UNC, SIGEVA-CONICET, CVar y CONEAU Global piden cuentas distintas | Taller-2 |
| Control tras importar | Comparar la columna «Cant.» de origen y destino | Taller-2 |
| Caracteres especiales | Las comillas se convierten en signos de pregunta; pegar desde texto plano | Taller-1, Taller-2 (se vio en pantalla), Encuentro I diap. 17, FO diap. 14 |
| Legajo | No hay campo | Taller-2 |
| Antigüedad de la carga | No caduca; se puede cargar antes de tener cargo y después de jubilarse | Taller-2 diap. 14 |
| Derecho de exclusión del repositorio | Ley 26.899 y Res. MinCyT 753/16; dejar en blanco si no corresponde | FCE-2024, FO diap. 16 |

## 3. Discrepancias y criterio adoptado

| # | Tema | Qué dice cada fuente | Criterio del manual |
|---|---|---|---|
| D1 | Tipo de archivo del texto completo | FCE-2024: publicado → «PostPrint»; en prensa → «Versión final». FCE-pautas: subir la versión final y la posprint solo si hay acuerdo con terceros. FO: PDF y versión posprint aceptada | Se describen los valores que muestra FCE-2024 y se marca para verificar qué opciones ofrece hoy el campo. No se fija una regla propia |
| D2 | Publicación sin ISSN/ISBN | Taller-2 (grabación): poner un número ficticio (todos ceros o unos) y aclararlo. Encuentro I diap. 16: sin ISBN «no se puede subir» un artículo en prensa. FO diap. 11 y Taller-2: en «Demás tipos de producción» no es obligatorio | El manual **no recomienda** números ficticios (un CV es declaración jurada y el dato sería falso). Primero, ver si corresponde «Demás tipos de producción»; si el formulario lo exige igual, consultar a soporte. El número ficticio se menciona como práctica que circula, no como recomendación |
| D3 | Mayúsculas en palabras clave | FCE-2024: palabras clave en mayúsculas sostenidas. FO: autores sin mayúsculas. Nada en el sistema lo exige | Se presenta como criterio de la Biblioteca FCE. El manual recomienda copiar las palabras clave como figuran en la publicación (orden e idioma), que es lo que comparten todas las fuentes |
| D4 | Adscripciones | Taller-1 (FCE): la adscripción estudiantil se carga como ayudantía. Taller-2: depende de la unidad académica; en FFyH y Sociales las adscripciones son de egresados, no dan antigüedad y van en Cargos > Otros cargos; las ayudantías van en Docencia (ayudante alumno) | Para la FFyH: adscripción → Otros cargos; ayudantía alumno → Docencia. Confirmar con la SeICyT |
| D5 | Trayecto pedagógico / profesorado / diplomaturas | Taller-2 (grabación): primero «formación complementaria», luego «formación académica»; diplomaturas a la vez «posgrado» y «capacitaciones extracurriculares» | Si otorga título (profesorado), Formación académica en su nivel. Si es un trayecto o curso sin título, Formación complementaria con carga horaria. Diplomaturas: según tengan o no título de posgrado acreditado; marcado para consultar |
| D6 | Carrera docente | Taller-2 diap. 7: «no se carga; se adjunta la resolución como antecedente». Grabación: «no se carga» | No hay formulario. Dónde adjuntar la resolución no está documentado: pendiente |
| D7 | Extensión con o sin financiamiento | Encuentro I diap. 13: en la solapa Extensión solo van actividades sin financiamiento. Taller-2 (pantalla): el formulario pregunta si tuvo financiamiento. UBA 3.11.5: fuente de financiamiento obligatoria («Ninguna» si no tiene) | Proyectos de extensión con subsidio competitivo: Financiamiento CyT. La actividad en sí puede ir en Extensión indicando la fuente. Marcado para verificar |
| D8 | Beca de extensión (SEU) | Taller-2: va en Financiamiento > Becas, aclarando que es de extensión (el sistema solo prevé becas de investigación) | Se adopta, como limitación conocida del sistema |
| D9 | Lugar de trabajo | Encuentro I diap. 6: becas → lugar de radicación; elegir el más abarcativo (p. ej., Escuela de Historia, FFyH). Taller-1: concurso en otra unidad → esa unidad. Taller-2 diap. 14: el de mayor carga horaria o el que origina el llamado | Regla general: el de mayor dedicación. Para cada trámite, lo que pidan las bases (radicación de la beca, unidad del concurso). Revisarlo antes de cada presentación |
| D10 | ¿Lo que no está en SIGEVA no cuenta? | Taller-1: en concursos por SIGEVA, lo no cargado no se considera (declaración jurada). Taller-2: algunas unidades evalúan también con el CV adjunto | Depende del reglamento de cada convocatoria. El manual recomienda cargar todo lo pertinente en el banco y no confiar en el CV adjunto |
| D11 | Qué cargar | Taller-1: «solo lo pertinente al perfil»; también «mejor que sobre a que falte». Taller-2: idealmente todo, de lo más nuevo y relevante a lo más antiguo | Cargar toda la trayectoria académica pertinente, empezando por lo más reciente y relevante. No cargar actividades ajenas a la vida académica |
| D12 | Quitar antecedentes para una convocatoria | Taller-1 lo menciona como estrategia avanzada | El manual no lo recomienda (riesgo de pérdida y de inconsistencia); si se hace, es decisión personal |
| D13 | Traducciones | FO diap. 8: «Demás tipos» o parte de libro. FO diap. 16: «Demás tipos» | «Demás tipos de producción C-T publicada», salvo que la traducción sea un capítulo dentro de un libro (parte de libro). Marcado |
| D14 | «Ingresar otra» institución: qué nivel | FCE-2024 p. 26: «nivel 3»; pp. 39, 50, 53, 69: «nivel 1» (55 caracteres) | Se documenta «nivel 1» (mayoría de casos y Taller-2) y se marca para verificar |
| D15 | Reimportar tras cambios | CONICET-sinc-v2: no duplica registros iguales y deja el último modificado. Taller-2: si cambiaste mucho, lo distinto queda duplicado; se puede borrar el destino y reimportar | Se describen ambas cosas; se sugiere comparar «Cant.» y depurar duplicados en destino |
| D16 | Uso de IA | Taller-1 y Encuentro I diap. 24 proponen usar asistentes de IA para extraer datos, buscar duplicados, clasificar | Se incluye como sugerencia de los talleres con advertencia propia: no subir a servicios externos documentos con datos personales (CUIL, domicilio) ni CV completos sin revisar condiciones de uso; verificar todo lo que devuelva |
| D17 | Notas en medios no científicos | Taller-2 diap. 8: artículos de divulgación en diarios o portales → Extensión › Comunicación pública de la ciencia. Taller-2 (grabación): notas en medios como *La Tinta*, si forman parte de una investigación → Demás tipos de producción C-T publicada | Por defecto, Extensión › Comunicación pública. Se menciona la alternativa; nunca en los dos lugares |

## 4. Pendientes que solo resuelve el sistema real

- Nombres exactos de solapas, subsolapas y botones (sección 1).
- Lista de subformularios de Datos personales y si existe «Dirección residencial».
- Dónde está el CV adjunto; formatos aceptados hoy (UBA: .pdf preferido, .doc, .rtf).
- Opciones del campo «tipo de archivo» del texto completo (D1).
- Si existen «Asignar colaborador» y «Trámite» en la instalación UNC.
- Qué secciones admite hoy «Compartir formularios» (UNC 2011 listaba 8; UBA excluye identificación, domicilio y lugar de trabajo) y si mantiene el filtro de años.
- Subtipos de Producción artística y de Desarrollo tecnológico en la versión actual.
- Reglas de contraseña actuales.
- Tope de caracteres del resumen de experticia (Taller-1 dijo «algo así como 1.100»).
