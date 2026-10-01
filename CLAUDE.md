# CLAUDE.md — Manual de SIGEVA para investigadores de la UNC

Proyecto de la Secretaría de Investigación, Ciencia y Técnica (SeICyT) de la Facultad de Filosofía y Humanidades (FFyH), UNC.

## Objetivo del proyecto
Producir un manual de uso de SIGEVA (instalación de la Universidad Nacional de Córdoba) más amigable que el vigente, en formato de documentación versionable (MkDocs / Material for MkDocs o similar). El punto de partida es actualizar el *Manual del Usuario del Banco de Datos* de la UNC (2011) al menos al nivel de cobertura del *Manual del Investigador* de la UBA (7.ª edición), e ir agregando sugerencias propias a lo largo del proyecto.

Contexto completo, hallazgos y plan: ver `HANDOFF.md`. Comparación de los tres manuales base: `investigacion/comparacion-manuales.md`. Fuentes y estado de verificación: `investigacion/fuentes.md`.

## Alcance de la versión 1
Banco de datos (CV), sincronización con SIGEVA-CONICET y CVar, y los trámites que la FFyH canaliza por SIGEVA (a confirmar cuáles contra el sistema real y los instructivos de la Facultad). La postulación completa de proyectos como director queda fuera de la v1.

## Audiencia
Docentes-investigadores y becarios de la UNC que cargan su CV en SIGEVA-UNC (https://sigeva.unc.edu.ar). Nivel técnico variable; el manual debe poder usarse sin conocer el sistema.

## Reglas de trabajo (importantes)
1. **No afirmar nada sobre el sistema que no esté verificado.** Cada página del manual debe indicar en su front matter: `fuente`, `verificado_contra` (manual / sistema real / ambos) y `fecha_verificacion`. Lo que solo proviene de un manual viejo se marca como `pendiente_verificar`.
2. **No copiar texto ni capturas de los manuales fuente.** Redactar texto propio. Las capturas deben ser propias, tomadas del sistema real, sin datos personales. Motivo: licencias (ver "Licencias" abajo) y calidad.
3. **Citar fuentes** cuando se tome una estructura o un dato de un manual (referencia a la sección, no transcripción).
4. **Separar hechos de sugerencias.** Las sugerencias propias del proyecto (buenas prácticas, advertencias, flujos recomendados) van marcadas como tales y no se presentan como comportamiento oficial del sistema.
5. **Idioma:** español rioplatense. Tratamiento: **vos** (decidido el 2026-09-30).
6. **Aviso de honestidad heredado:** un relevamiento previo de manuales de ~30 universidades quedó **descartado** por no estar respaldado (ver `HANDOFF.md`, sección 2). No usarlo como fuente. Todo relevamiento nuevo debe abrir y leer cada documento citado. `investigacion/pistas-relevamiento-no-verificado.md` es solo una lista de enlaces a comprobar: nada de su contenido se cita sin abrir el documento original.
7. **Verificación contra el sistema real:** se navega https://sigeva.unc.edu.ar con la sesión del usuario en **solo lectura** (no guardar, modificar, borrar, compartir ni importar). No se registran datos personales en notas ni capturas.

## Estructura del repo
```
.
├── CLAUDE.md
├── HANDOFF.md
├── mkdocs.yml
├── docs/
│   ├── index.md
│   ├── primeros-pasos/
│   ├── cv/                 # carga del banco de datos, una página por sección
│   ├── sincronizacion/
│   ├── proyectos-y-tramites/
│   ├── assets/             # capturas propias
│   ├── faq.md
│   ├── glosario.md
│   └── cambios.md          # registro de versiones del manual
└── investigacion/          # material de trabajo, no se publica
    ├── comparacion-manuales.md
    ├── fuentes.md
    ├── pistas-relevamiento-no-verificado.md
    └── fuentes-pdf/        # PDF de terceros, fuera de git
```

## Convenciones de versionado
- Versión del manual con SemVer adaptado: `MAYOR.MENOR` (mayor = cambia estructura; menor = correcciones/ampliaciones).
- Cada release registra en `docs/cambios.md` qué se verificó contra el sistema y cuándo.
- Ramas: `main` (publicable), `borrador/*` (secciones en redacción).

## Licencias (a resolver antes de publicar)
- La guía CONICET v4 declara en su portada que no admite uso comercial de la obra ni de derivadas, y que su distribución debe hacerse con licencia igual. El pie del portal SIGEVA del CONICET dice contenidos bajo CC Reconocimiento 2.5 Argentina. Hay una discrepancia a aclarar.
- No se conoce la licencia del manual de la UBA ni del de la UNC.
- Recomendación: texto original, licencia abierta para el nuevo manual (por ejemplo CC BY-SA 4.0) tras confirmar compatibilidad, y declarar las fuentes consultadas.
