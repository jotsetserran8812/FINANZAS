# Plata

Presupuesto semanal por sobres, vencimientos de tarjetas y movimientos. PWA instalable en el móvil, sin build step: todo vive en `index.html`.

- **Inicio** — disponible de la semana (presupuesto − gastado desde el día de pago), próximos vencimientos y últimos movimientos.
- **Agregar** — gastos e ingresos con sobre, método y fecha.
- **Sobres** — límite semanal por categoría.
- **Tarjetas** — tarjetas, cuotas y servicios; "Pagar" registra el gasto y pasa al mes siguiente.

Los datos se guardan en el navegador (`localStorage`, clave `pl_data`). Ajustes permite exportar/importar una copia en JSON.

## Correr en local

```bash
npx serve -l 4340 .
```

Al cambiar archivos, sube la versión de `CACHE` en `sw.js` (`plata-vN`) para que el móvil reciba la actualización.
