# Esquema Excel VIEX

`PROSPECTOS` contiene una fila por contacto. `LISTA_PROSPECTOS` contiene una fila por prospecto y es la lista maestra. Los encabezados deben coincidir exactamente con `SKILL.md`.

## Integridad

- Todos los IDs de `LISTA_PROSPECTOS` son únicos.
- Todo ID de `PROSPECTOS` existe en `LISTA_PROSPECTOS`.
- `Cantidad de contactos` equivale al número de filas de contacto asociadas.
- `Score` es entero entre 0 y 100.
- `Prioridad` es `A`, `B`, `C` o `D`.
- `Estado` pertenece al conjunto definido en `SKILL.md`.
- Las fuentes son URLs separadas por salto de línea o ` | `.
- Los campos ausentes conservan exactamente `No encontrado`.

El generador no debe crear hojas adicionales. Debe congelar `A2`, activar autofiltro, usar tablas con filas, ajustar anchos y crear hipervínculos para URLs válidas.

