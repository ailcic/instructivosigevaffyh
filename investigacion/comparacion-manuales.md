# Comparación sistemática: CONICET genérico vs UBA vs UNC

Fecha: 2026-09-30. Basada en la lectura directa del texto de los tres PDF (ver `fuentes.md`).

## Límites de la lectura
- UBA: en la lectura original el texto se cortó en la p. 248 de 257. Las pp. 246–257 (4.3.5 Presentación, 4.3.6 Seguimiento, 5 Otros integrantes, 6 Material de referencia) se leyeron del PDF local el 2026-09-30: confirman el efecto "foto" tanto al enviar la presentación (director) como al asociarse (integrante), y que para asociarse se piden como mínimo datos personales, lugar de trabajo, formación académica y CV adjunto.
- Las capturas de pantalla no se extraen. La lista de campos por solapa de CONICET v4 está en una imagen; la estructura de CONICET se tomó de la descripción del módulo en https://sigeva.conicet.gov.ar/.
- Hay otro manual genérico más antiguo (era SICyTAR), espejado en https://faud.mdp.edu.ar/wp-content/uploads/2022/04/manual_banco_de_datos_10.pdf. Se abrió, pero no se usó como base.

## 1. Ficha
| | CONICET v4 | UBA 7.ª ed. | UNC 2011 |
|---|---|---|---|
| Emisor | Dirección de Informática, CONICET | UBA | UNC (Prosecretaría de Informática) |
| Extensión | 26 pp. de PDF (23 numeradas) | 257 pp. | 65 pp. |
| Alcance | Banco de Datos | Banco de Datos + postulación de proyectos | Banco de Datos |
| Nivel de detalle | Funcional, sin campos obligatorios por formulario | Formulario por formulario con campos mínimos | Formulario por formulario con campos mínimos |
| FAQ | Sí (3 casos) | No | No |
| Licencia declarada | Portada: sin uso comercial, derivadas con licencia igual | No consta en el texto leído | No consta |

## 2. Genealogía
El manual UNC declara en su cierre que fue desarrollado por la Coordinación General de TIC de la UBA, adaptado por la Prosecretaría de Informática de la UNC, con aporte del área de desarrollo de CONICET. Evidencia en el texto: introducción casi idéntica, mismas reglas de contraseña (6 a 20 caracteres, alfanumérica, sin el nombre de usuario), misma mecánica de compartir/importar y referencias cruzadas con numeración UBA ("sección 3.6", "punto 3.8.2", "punto 3.4.1") inexistentes en el UNC. El manual UBA tiene a su vez referencias desfasadas: "3.6" para autores (está en 3.5), "3.8" para instituciones (está en 3.7), "3.9.4" para financiamiento (está en 3.11.1).

## 3. Cobertura del CV
| Sección | CONICET (portal) | UBA | UNC |
|---|---|---|---|
| Datos personales | Identificación, domicilio, lugar de trabajo, experticia en CyT | Identificación, domicilio, lugar de trabajo (experticia no figura en el índice) | Datos personales y lugar de trabajo |
| Formación | Académica y complementaria | Académica (7 niveles) y complementaria (especialidad de salud, posdoctorado, cursos, idiomas) | Solo académica: grado o inferior y posgrado |
| Cargos | Docencia, I+D, gestión, otros | Los cuatro | Cargos docentes, otros cargos y "Carrera de investigador" |
| Antecedentes | Financiamiento, RRHH, extensión, evaluación, becas, otras | Esas seis más áreas de actuación | Financiamiento, formación de RRHH, divulgación |
| Producción científica | 6 formularios | 7 ítems | 4 ítems: artículos, capítulos, libros, congresos |
| Producción tecnológica | Con título de PI, servicios, informes | 4 ítems | 5 ítems: convenios, marcas, modelos y diseños, patentes, informes |
| Producción artística | Sí | Sí, 9 subtipos | No |
| Otros antecedentes | Eventos, premios, membresías | Premios, eventos, membresías, archivos adjuntos | Solo archivos adjuntos |
| Categoría de Incentivos | No figura en el portal | Sí, en Cargos I+D (año, categoría, institución) | No |

## 4. Funcionalidades y comportamiento
| | CONICET v4 | UBA | UNC |
|---|---|---|---|
| Precarga por DOI/ISSN | Sí (Crossref/Elsevier; con ISSN solo revista y editorial) | No documentada | No documentada |
| Asignar colaborador | Sí; debe estar registrado en la misma institución | Aparece como solapa, sin sección en el manual | No |
| Compartir/importar | Remite a guía de sincronización aparte (v2) | Paso a paso; no se comparten identificación, domicilio ni lugar de trabajo | Paso a paso; 8 secciones habilitadas, sin Formación académica ni Carrera de investigador |
| Imprimir CV | Selección de secciones y rango de fechas; PDF o DOC | PDF o Word | PDF o Word |
| CV adjunto | No lo trata | .pdf preferido, .doc o .rtf; para cambiarlo, "Limpiar" y subir otro | Igual que UBA |
| Vincularse a un trámite | Código y "Confirmar" | Igual, más el efecto "foto" del banco de datos | Fuera de alcance |
| Carga de autores | Debe coincidir con el nombre registrado ("Garcia, Juan Pedro"; no reconoce "JP Garcia") | Nombre y apellido en el orden de publicación | Igual que UBA |
| Elegir institución | Búsqueda o "ingresar otra" (país, provincia, tipo, nivel 1) | Búsqueda con filtros y navegación jerárquica | Tipo de lugar de trabajo y "Más detalle" |
| Navegador | Recomienda Chrome; no usar atrás/adelante del navegador | No menciona | No menciona |

### Campos mínimos de un artículo (ejemplo)
UBA y UNC piden casi lo mismo: revista (ISSN o nombre), título, idioma, referato, páginas inicial y final si está publicado, publicado o en prensa, editorial, mes y año, autores, al menos una palabra clave, resumen y archivo de texto completo. Diferencias: UBA agrega país de edición y pide hasta 3 áreas y subáreas de conocimiento; UNC pide campo disciplinar y campo disciplinar desagregado.

## 5. Lectura para docentes
- Ninguno es un manual para docentes.
- Docencia en UBA: distingue universitario/posgrado, terciario, medio o básico y cursos; en nivel universitario exige al menos una actividad curricular dictada. UNC: un único formulario (nivel, cargo, condición, tipo, dedicación horaria semanal, fecha, lugar de trabajo) sin actividades curriculares.
- Ninguno cubre evaluación o carrera docente.
- El manual UNC tiene unos 15 años; no se sabe qué formularios tiene hoy el sistema de la UNC sin acceder a él.
