---
fuente:
  - "SIGEVA-UNC, Datos personales: Identificación, Dirección residencial, Lugar de trabajo"
  - "Estructura: Manual del Investigador, UBA (7.ª ed.), 3.8; Manual del Usuario del Banco de Datos, UNC (2011), Datos personales y laborales"
verificado_contra: sistema real
fecha_verificacion: 2026-09-30
estado: pendiente_verificar
---

# Datos personales

La solapa **Datos personales** tiene cuatro apartados. Los tres primeros se explican acá; el cuarto, [Experticia en CyT](experticia.md), tiene página propia.

Los cuatro son formularios únicos: no hay tabla ni enlace **Nuevo**. Completás, presionás **Guardar** y la pantalla principal pasa a mostrar **Con datos**. **Salir** vuelve sin guardar.

!!! note "Pendiente de verificar"
    Estas tres pantallas se relevaron leyendo su estructura, sin capturas y sin modificar nada. No se comprobó cuáles campos vienen bloqueados (por ejemplo, los que se cargaron al crear el usuario).

## Identificación

Reúne tus datos de identidad:

| Campo | Observaciones |
|---|---|
| Nombre y apellido | Hay además un campo para apellido de casada |
| Sexo | Tres opciones |
| Estado civil · Cantidad de hijos | |
| País de nacionalidad · Condición de nacionalidad | Listas |
| Tipo y número de documento | Si el documento es pasaporte, también país de emisión |
| CUIT/CUIL | |
| País, provincia y partido de nacimiento | Con un campo «otro» por si el partido no figura |
| Fecha de nacimiento | |
| Información adicional | Texto libre |

!!! tip "Sugerencia de la SeICyT"
    Controlá que nombre, apellido y CUIL estén escritos igual que en tu documento. Son los datos que identifican tu registro cuando sincronizás con otras instalaciones de SIGEVA.

## Dirección residencial

| Campo | Obligatorio |
|---|---|
| Calle · Número | Sí |
| Piso · Oficina/Departamento | No |
| País · Provincia · Partido/Departamento | Sí |
| Localidad | No |
| Código postal | Sí |
| Casilla postal | No |
| Teléfono | Sí (grupo de varios campos) |
| Teléfono celular · Fax | No |
| E-mail | Sí |
| URL · Informaciones adicionales | No |

Si tu partido o tu localidad no están en la lista, hay campos **Otro** para escribirlos.

## Lugar de trabajo

Tiene los mismos campos de dirección y contacto, precedidos por el bloque de [búsqueda de institución](campos-comunes.md#instituciones): primero elegís la institución donde trabajás y después completás su domicilio.

!!! tip "Sugerencia de la SeICyT"
    El lugar de trabajo es el dato institucional más visible de tu currículum. Elegí el nivel del catálogo que mejor represente tu radicación real (facultad, centro o instituto) y usá el mismo criterio en los cargos.

## Qué no se comparte

El manual de la UBA indica que los datos de identificación, domicilio y lugar de trabajo no viajan al sincronizar con otra instalación: hay que cargarlos en cada sistema. Ver [Compartir e importar datos](../sincronizacion/index.md).

## Fuentes

- SIGEVA-UNC, **Datos personales**, relevada el 2026-09-30.
- Manual UBA (7.ª ed.), 3.8 y 3.3; manual UNC (2011), «Datos personales y laborales».
