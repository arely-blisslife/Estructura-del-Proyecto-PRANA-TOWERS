# Prana Towers — Datos del Proyecto

Carpeta lista para copiar dentro de tu proyecto en VS Code. Contiene todo el material que hemos generado hasta ahora: brief ejecutivo, estudio de mercado completo y datos estructurados en JSON.

## Estructura

```
prana-towers-project/
├── data/
│   ├── 01-brief-ejecutivo.md       → Brief original del cliente (Markdown)
│   ├── 02-estudio-mercado.md       → Estudio de mercado completo (Markdown)
│   └── prana-towers-data.json      → Todos los datos en JSON estructurado
└── README.md                       → Este archivo
```

## Cómo usar cada archivo

### `01-brief-ejecutivo.md` y `02-estudio-mercado.md`

Documentación en Markdown. Puedes:

- Verlos directamente en VS Code con la extensión **Markdown Preview** (`Ctrl+Shift+V` / `Cmd+Shift+V`).
- Usarlos como fuente de verdad para copy de landing pages, presentaciones o reportes.
- Convertirlos a PDF/HTML con herramientas como `pandoc` si los necesitas en otro formato.

### `prana-towers-data.json`

Datos estructurados listos para consumir en código. Ideal para:

- Alimentar una **calculadora de ROI** interactiva (los datos de `proyeccion_roi` ya están listos).
- Poblar una **landing page** (React, HTML, etc.) sin tener que volver a escribir los números.
- Construir un **dashboard** con los KPIs y benchmarks de competencia.

Ejemplo de import en JavaScript/React:

```
import pranaData from './data/prana-towers-data.json';

console.log(pranaData.proyecto.precio_desde_mxn); // 3200000
console.log(pranaData.proyeccion_roi); // array de escenarios ROI
```

Ejemplo en Python:

```
import json

with open('data/prana-towers-data.json', encoding='utf-8') as f:
    data = json.load(f)

print(data['perfiles_comprador'])
```

## Próximos pasos sugeridos

- [ ] Landing page del proyecto (HTML/React) usando estos datos
- [ ] Calculadora de ROI interactiva (lead magnet mencionado en recomendación #4)
- [ ] Dashboard de KPIs de campaña conectado a Meta Ads / CRM
- [ ] Presentación PPTX para brokers con los datos de competencia

---

*Datos generados por Bliss Strategy — Junio 2026*
Prana Towers es un desarrollo residencial boutique en Playa del Carmen conformado por solo 10 departamentos de 2 y 3 recámaras. Diseñado para inversionistas y compradores de segunda residencia, ofrece una ubicación estratégica, alta plusvalía y excelente potencial de rentas. Actualmente se encuentra en construcción se entrega en diciembre 2026
