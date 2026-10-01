# Método de relevamiento del sistema y de capturas

Cómo se hizo el relevamiento de SIGEVA-UNC con Claude Code y la extensión de Chrome, para poder repetirlo o continuarlo (por ejemplo, con el rol de presentación para becas). Complementa las reglas de `CLAUDE.md` y las autorizaciones listadas en `bitacora.md`.

## Condiciones

- El usuario inicia sesión en SIGEVA-UNC en Chrome y habilita la extensión (`/chrome`). Claude trabaja en una pestaña propia y la cierra al terminar.
- Rol usado hasta ahora: «Usuario banco de datos de actividades de CyT».
- La sesión siguió activa de un día al siguiente sin pedir reingreso.

## Direcciones útiles

Todas bajo `https://sigeva.unc.edu.ar/eva/`.

| Pantalla | Dirección |
|---|---|
| Principal | `indexBancoDatos.do` |
| Listas (una por apartado) | `bcoFormacionAcademica.do`, `bcoFormacionComplementariaLista.do`, `bcoCargoDocenteLista.do`, `bcoCargoIDLista.do`, `bcoCargoGestionLista.do`, `bcoCargoOtroLista.do`, `bcoFormacionRRHH.do`, `bcoActividadEvaluacionLista.do`, `bcoFinanciamientoCyTLista.do`, `bcoOtrasActividadesCYTLista.do`, `bcoExtensionLista.do`, `bcoProduccionListaPublicacion.do`, `bcoProduccionArtisticaLista.do`, `bcoProduccionListaDesarrollo.do`, `bcoProduccionListaServicios.do`, `bcoProduccionListaBienes.do`, `bcoRedesLista.do`, `bcoPremioLista.do` |
| Formularios únicos | `bcoDatoPersonalIdentificacion.do`, `bcoDatoPersonalDireccion.do?tipoDir=residencial` (o `laboral`), `bcoExperticia.do` |
| Otras | `bcoCompartirFormulario.do`, `bcoRoles.do` (asignar colaborador), `instructivoConvocatoriaGral.do`, `bcoIncorporarParticipanteTramite.do`, `bcoCArchivosAdjuntos.do`, `filtroImprimirCurriculum.do` |

Las listas se abren sin parámetros. Los parámetros `idModulo`, `idGrupo` e `idMenu` solo cambian qué solapa queda resaltada.

## Abrir un formulario de alta

- **Vía segura:** ir a la lista y activar el enlace **Nuevo** de la tabla que corresponde (el enésimo enlace con texto «Nuevo» de la página).
- Algunos formularios se abren también con `…?accion=Nuevo` directo, pero varios necesitan parámetros extra (`tipoActividad`, `tipoExtension`, `nivel`, `grupoArtistica`, `tipo`, etc.) y sin ellos devuelven una «Página de errores». Ese error no afecta datos.
- **Artículos:** «Nuevo» abre la precarga; el formulario aparece al pulsar **Omitir**.
- Para salir, navegar a otra pantalla. Nunca **Guardar**.

## Leer la estructura de un formulario

- La extracción de texto de la página devuelve rótulos, asteriscos, opciones de listas y notas. Conviene vaciar antes, **solo en pantalla**, las listas largas (países, áreas, campo de aplicación) para no llenar la salida.
- Los asteriscos de obligatoriedad salen en el texto, pero en formularios con tablas complejas no siempre queda claro a qué campo pertenecen: confirmar con una captura.
- La herramienta de JavaScript de la extensión bloquea salidas que contengan cadenas de consulta o que parezcan datos codificados, y trunca las salidas largas. Devolver solo nombres o rutas, en tramos cortos.
- Las segundas listas encadenadas (subáreas) se cargan según la primera: no se pueden enumerar sin cambiar la selección en pantalla.

## Ejecutar una búsqueda de prueba

- El clic con el ratón sobre el campo y el botón no siempre respondió. Lo que funcionó de forma fiable fue asignar el valor al campo y activar el botón **Buscar** desde JavaScript.
- No pulsar **Seleccionar** ni **Ingresar otra**.

## Capturas

- La opción de escala de la captura también reduce el archivo guardado: para capturas publicables hay que tomarlas a escala completa.
- Ventana usada: 1364 × 896 px.
- **Datos personales en pantalla:** el encabezado muestra nombre y fecha arriba a la derecha; al desplazarse aparece un encabezado compacto fijo (unos 34 px) que también muestra el nombre. La pantalla principal y las listas muestran registros del usuario.
- **Recorte aplicado** (con PIL, desde las capturas completas): columna de contenido `x = 236–1114`; desde `y = 150` en pantallas sin desplazar y desde `y = 36` en pantallas desplazadas. La barra de solapas se recortó aparte (`196, 68, 1160, 145`).
- **Formularios con datos del usuario** (Experticia en CyT): se pusieron en blanco los campos en pantalla mediante JavaScript, se capturó y se salió sin guardar.
- Para una tabla sin registros se usó **Otros cargos**, que estaba vacía.
- Los archivos originales quedan en un directorio temporal del sistema y no se versionan.

## Qué no se pudo ver sin modificar datos

Para relevar lo siguiente hace falta autorización expresa o un usuario de prueba:

- Mensajes de validación al guardar; formularios de edición y de borrado.
- Pantalla de **Importar** y efecto de **Compartir**.
- Confirmación al ingresar un código en **Trámite**.
- Campos que se habilitan al elegir una opción (subformularios de financiamiento, propiedad intelectual y transferencia en Desarrollos; cargos disponibles según la institución en Docencia).
- Documento que genera **Imprimir CV** (no modifica datos, pero expone el CV completo: decidir si se revisa).
- Pantallas previas al ingreso (registro, recuperación de contraseña) y selección de rol.
