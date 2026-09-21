# Plugins de la empresa para Claude

Catálogo de plugins aprobados por IT. Solo se agrega lo que está en este repo.

## Cómo instalarlo (una sola vez por usuario, en Claude Desktop)

1. Abrir **Customize** (barra lateral izquierda) → pestaña **Plugins**.
2. En **Personal plugins**, tocar **+** → **Add marketplace** → **Add from a repository**.
3. Pegar la dirección de este repositorio.
4. En **Browse plugins**, instalar los que necesites.
5. La primera vez que uses Gmail, Calendar o ProjectCor, Claude te va a pedir
   que autorices tu propia cuenta. Eso es individual de cada persona.

## Plugins incluidos

| Plugin | Qué hace |
|---|---|
| Gmail | Buscar, leer y redactar correos de tu casilla |
| Google Calendar | Consultar agenda y coordinar reuniones |
| ProjectCor | Consultar proyectos, tareas y horas |

## Para IT: cómo agregar un plugin nuevo

1. Crear la carpeta `plugins/<nombre>/` con `.claude-plugin/plugin.json` y, si
   usa un conector, un `.mcp.json`.
2. Agregar la entrada correspondiente en `.claude-plugin/marketplace.json`.
3. Nombres en minúscula y con guiones (`mi-plugin`), sin espacios.
4. No poner credenciales, tokens ni datos internos: el repo es público.
5. No se declara `version` a propósito: así cada commit cuenta como versión
   nueva y los usuarios reciben el cambio al sincronizar.
