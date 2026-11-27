# Pequeñas creaciones

Galería de bocetos, simulaciones y experimentos interactivos.
**Sitio:** https://avel1956.github.io/creaciones/

La página se arma sola: lee la carpeta `creaciones/` y muestra una tarjeta por cada creación. No hay que tocar `index.html` nunca.

## Cómo subir una creación nueva (desde el navegador)

1. Prepara en tu computador una carpeta con un nombre corto, sin espacios ni tildes (ej. `pandeo-euler`). Adentro debe ir un `index.html` y todo lo que use (scripts, imágenes…).
2. En GitHub entra a la carpeta **`creaciones/`** de este repositorio.
3. **Add file → Upload files** y arrastra la carpeta completa.
4. Escribe un mensaje corto y pulsa **Commit changes**.
5. En 1–2 minutos aparece en el sitio.

¿Es un solo archivo? También puedes subir un `.html` suelto directamente dentro de `creaciones/`.

## Ficha opcional: `info.json`

Pon un `info.json` dentro de la carpeta para darle título, descripción, fecha y etiquetas (copia el de `creaciones/_plantilla/`):

```json
{
  "titulo": "Pandeo de Euler",
  "descripcion": "Columna interactiva: cambia la longitud y mira la carga crítica.",
  "fecha": "2026-11-27",
  "etiquetas": ["mecánica", "p5.js"],
  "portada": "portada.png"
}
```

| Campo | Para qué | Si no lo pones |
|---|---|---|
| `titulo` | Nombre en la tarjeta | Se usa el nombre de la carpeta |
| `descripcion` | Una o dos líneas | Sin descripción |
| `fecha` | `AAAA-MM-DD`, ordena la galería (más reciente primero) | Va al final, por orden alfabético |
| `etiquetas` | Filtros de la galería | Sin filtro |
| `portada` | Imagen de la tarjeta | Se muestra la creación en vivo, en miniatura |
| `abrir` | Archivo a abrir si no es `index.html` | `index.html` |
| `vista_viva` | `false` para no cargar la miniatura en vivo (piezas pesadas) | `true` |

## Reglas pequeñas

- Las carpetas que empiezan con `_` (como `_plantilla`) no aparecen en la galería.
- Para quitar una creación, borra su carpeta.
- Nada de claves de API ni datos personales dentro de las creaciones: el repositorio es público.
