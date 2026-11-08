# SIGEVA-UNC: guía para investigadores

Manual de uso de [SIGEVA-UNC](https://sigeva.unc.edu.ar) para docentes-investigadores y becarios de la Universidad Nacional de Córdoba. Lo elabora la Secretaría de Investigación, Ciencia y Técnica (SeICyT) de la Facultad de Filosofía y Humanidades.

**Sitio publicado:** <https://ailcic.github.io/instructivosigevaffyh/>

## Estado

Versión 0.3, verificada contra el sistema real el 8 de noviembre de 2026 (en solo lectura). Lo que no se pudo comprobar está marcado como pendiente en cada página. Detalle en [`docs/cambios.md`](docs/cambios.md).

Las ambigüedades que el sistema no resuelve están marcadas con recuadros **DECIDIR**, para revisión del Consejo Asesor de Ciencia Abierta de la UNC:

```sh
grep -rn 'DECIDIR' docs
```

## Estructura

- `docs/`: el manual (Markdown, [MkDocs](https://www.mkdocs.org/) con [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)).
- `docs/assets/`: capturas propias del sistema, sin datos personales.
- `investigacion/`: material de trabajo (comparación de manuales, fuentes, registro de la verificación). No se publica en el sitio.
- `CLAUDE.md` y `HANDOFF.md`: reglas de trabajo y contexto del proyecto.

## Ver el sitio en tu computadora

```sh
python3 -m venv .venv
.venv/bin/pip install -r requirements.txt
.venv/bin/mkdocs serve
```

Y abrí <http://127.0.0.1:8000>.

## Publicación

Cada cambio que llega a `main` se publica solo en GitHub Pages (ver [`.github/workflows/publicar.yml`](.github/workflows/publicar.yml)). Las secciones en redacción se trabajan en ramas `borrador/*` y se integran con un pull request.

## Licencia

El manual (texto y capturas) se publica bajo [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.es). Ver [`LICENSE`](LICENSE). Los nombres, marcas y logotipos de la UNC y del CONICET que aparecen en las capturas no quedan alcanzados por esta licencia.

## Correcciones

Si algo del manual no coincide con lo que ves en SIGEVA-UNC, vale la pantalla: abrí un *issue* en este repositorio o escribí a la SeICyT de la FFyH.
