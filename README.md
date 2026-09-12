# Cuentas Claras

App web para registrar ingresos, gastos y ahorro, pensada para crear el hábito de ahorrar
con metas concretas. Funciona en el celular y en el computador, y se puede instalar como app.

**Abrir la app:** https://cvargas-bubba.github.io/cuentas-claras/

## Qué hace

- **Registro rápido** de gastos, ingresos y ahorro, con categoría sugerida según el comercio.
- **Metas de ahorro** con monto, fecha opcional y barra de avance. Calcula cuánto apartar
  por semana para llegar a tiempo.
- **Ahorra primero**: al registrar un ingreso, propone apartar un porcentaje para la meta
  principal antes de gastar.
- **Logros y rachas**: semanas seguidas ahorrando e hitos al 25 %, 50 % y 100 % de una meta.
- **Resumen del mes**: cuánto recibiste, gastaste, apartaste y te queda libre; presupuesto
  por categoría y gráfico de los últimos 6 meses.
- **Importar Excel o CSV** (cartolas bancarias o la plantilla de la app), con detección de
  columnas y de movimientos duplicados.
- **Exportar a Excel** y **respaldo completo** en un archivo `.json` que se puede restaurar.

## Privacidad

Los datos se guardan **solo en el navegador del dispositivo** (`localStorage`). No se envían
a ningún servidor y este repositorio no contiene datos personales. Por eso conviene descargar
un respaldo de vez en cuando desde **Ajustes → Descargar respaldo**.

## Instalar en el celular

- **Android (Chrome):** menú ⋮ → *Agregar a la pantalla principal*.
- **iPhone (Safari):** botón Compartir → *Agregar a inicio*.

Instalada, se abre como una app y funciona sin conexión.

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La app completa (HTML, CSS y JavaScript en un solo archivo) |
| `manifest.webmanifest` | Nombre, colores e íconos para instalarla |
| `sw.js` | Service worker: uso sin conexión |
| `icon-*.png`, `apple-touch-icon.png` | Íconos |

No requiere compilación: basta con servir la carpeta (GitHub Pages lo hace).
Usa [SheetJS](https://sheetjs.com/) desde cdnjs para leer y crear archivos Excel.
